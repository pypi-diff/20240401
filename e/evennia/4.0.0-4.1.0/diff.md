# Comparing `tmp/evennia-4.0.0.tar.gz` & `tmp/evennia-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evennia-4.0.0.tar", last modified: Sun Mar 17 13:43:07 2024, max compression
+gzip compressed data, was "evennia-4.1.0.tar", last modified: Mon Apr  1 18:37:21 2024, max compression
```

## Comparing `evennia-4.0.0.tar` & `evennia-4.1.0.tar`

### file list

```diff
@@ -1,988 +1,988 @@
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.415913 evennia-4.0.0/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2024-03-17 13:16:36.000000 evennia-4.0.0/LICENSE.txt
--rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-03-17 13:43:07.415913 evennia-4.0.0/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3034 2024-03-17 13:16:36.000000 evennia-4.0.0/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.315913 evennia-4.0.0/bin/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/bin/unix/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2024-03-17 13:16:36.000000 evennia-4.0.0/bin/unix/evennia
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/evennia/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/VERSION.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      437 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/VERSION_REQS.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15075 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/__main__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.331913 evennia-4.0.0/evennia/accounts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    74097 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26930 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/bots.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.331913 evennia-4.0.0/evennia/accounts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0002_move_defaults.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0007_copy_player_to_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17496 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/accounts/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.331913 evennia-4.0.0/evennia/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.331913 evennia-4.0.0/evennia/commands/_trial_temp/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/_trial_temp/_trial_marker
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31495 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/cmdhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27312 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/cmdset.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26151 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/cmdsethandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29275 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/command.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.335913 evennia-4.0.0/evennia/commands/default/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35295 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19512 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/admin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22982 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/batchprocess.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   171758 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/building.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/cmdset_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/cmdset_character.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/cmdset_session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/cmdset_unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    76280 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22486 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/general.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39812 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12774 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/muxcommand.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/syscommands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42142 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/system.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    82640 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15023 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/default/unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    47839 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/commands/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.335913 evennia-4.0.0/evennia/comms/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32602 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16864 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.335913 evennia-4.0.0/evennia/comms/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0003_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0004_auto_20150118_1631.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0005_auto_20150223_1517.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0007_msg_db_tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0008_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0009_auto_20160921_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0010_auto_20161206_1912.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0011_auto_20170217_2039.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0011_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0012_merge_20170617_2017.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0013_auto_20170705_1726.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0014_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0015_auto_20170706_2041.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0016_auto_20180925_1735.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0017_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0018_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0019_auto_20210514_2032.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0020_auto_20210514_2210.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0021_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22646 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/comms/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/awsstorage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/awsstorage/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/awsstorage/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/awsstorage/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/building_menu/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/building_menu/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/building_menu/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42691 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/building_menu/building_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6879 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/building_menu/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/color_markups/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/color_markups/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/color_markups/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/color_markups/color_markups.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/color_markups/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/components/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6914 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      513 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4638 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/component.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5161 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/dbfield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      157 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/exceptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10305 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/holder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/listing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7516 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/signals.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17207 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/components/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.339913 evennia-4.0.0/evennia/contrib/base_systems/email_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/email_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/email_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/email_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/email_login/email_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/email_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6041 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3186 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/test_webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2682 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/ingame_python/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/base_systems/menu_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/menu_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/menu_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/menu_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8933 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/menu_login/menu_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/menu_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/base_systems/unixcommand/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/unixcommand/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/unixcommand/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/unixcommand/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/full_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22694 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10560 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34344 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      751 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/state.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.343913 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/states/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/states/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10420 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/barter/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/barter/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/barter/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/barter/barter.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/barter/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/clothing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4256 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/clothing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/clothing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24854 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/clothing/clothing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6344 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/clothing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/containers/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/containers/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/containers/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10015 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/containers/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2851 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/containers/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/cooldowns/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/cooldowns/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/cooldowns/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/cooldowns/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/crafting/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/crafting/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/crafting/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41643 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/crafting/crafting.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17891 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/crafting/example_recipes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/crafting/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/gendersub/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/gendersub/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/gendersub/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/gendersub/gendersub.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2352 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/gendersub/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/mail/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/mail/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/mail/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/mail/mail.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/mail/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.347913 evennia-4.0.0/evennia/contrib/game_systems/multidescer/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3228 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/multidescer/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/multidescer/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/multidescer/multidescer.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/multidescer/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/game_systems/puzzles/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/puzzles/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/puzzles/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27836 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/puzzles/puzzles.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41327 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/puzzles/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37445 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_items.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_range.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29680 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/extended_room/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6358 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/extended_room/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/extended_room/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34234 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/extended_room/extended_room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12948 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/extended_room/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/ingame_map_display/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/ingame_map_display/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/ingame_map_display/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/ingame_map_display/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/mapbuilder/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/mapbuilder/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/mapbuilder/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/mapbuilder/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/simpledoor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/simpledoor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/simpledoor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/simpledoor/simpledoor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/simpledoor/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/slow_exit/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/slow_exit/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/slow_exit/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/slow_exit/slow_exit.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/slow_exit/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.351913 evennia-4.0.0/evennia/contrib/grid/wilderness/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/wilderness/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/wilderness/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6226 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/wilderness/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27385 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/wilderness/wilderness.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/grid/xyzgrid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54837 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      243 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20845 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7823 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13700 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/launchcmd.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42118 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40427 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/xymap.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    52079 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10483 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24732 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/grid/xyzgrid/xyzroom.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/rpg/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/rpg/buffs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/buffs/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/buffs/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    45718 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/buffs/buff.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/buffs/samplebuffs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/buffs/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/rpg/character_creator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3922 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/character_creator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/character_creator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7447 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/character_creator/character_creator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/character_creator/example_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1809 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/character_creator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/rpg/dice/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3812 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/dice/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/dice/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12729 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/dice/dice.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/dice/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/rpg/health_bar/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/health_bar/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/health_bar/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/health_bar/health_bar.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/health_bar/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.355913 evennia-4.0.0/evennia/contrib/rpg/llm/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15039 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/llm/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       74 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/llm/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5986 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/llm/llm_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7444 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/llm/llm_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/llm/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.359913 evennia-4.0.0/evennia/contrib/rpg/rpsystem/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10331 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/rpsystem/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/rpsystem/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/rpsystem/rplanguage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    59464 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/rpsystem/rpsystem.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16899 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/rpsystem/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.359913 evennia-4.0.0/evennia/contrib/rpg/traits/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14247 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/traits/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/traits/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/traits/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54515 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/rpg/traits/traits.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.359913 evennia-4.0.0/evennia/contrib/tutorials/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.359913 evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.359913 evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/evadventure/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6817 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/ai.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/evadventure/batchscripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/build_world.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11180 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16990 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/combat_base.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27710 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18204 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/combat_twitch.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17918 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1742 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/enums.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14537 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11354 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/random_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12129 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/shops.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1671 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_ai.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2150 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28160 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3742 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/evadventure/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/mirror/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/mirror/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/mirror/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/mirror/mirror.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/red_button/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/red_button/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/red_button/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/red_button/red_button.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/talking_npc/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/talking_npc/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/talking_npc/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/talking_npc/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.363913 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/build.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25399 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/mob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7522 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/auditing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/auditing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/auditing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/auditing/outputs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/auditing/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/auditing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/fieldfill/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/fieldfill/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/fieldfill/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26382 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/fieldfill/fieldfill.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/git_integration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/git_integration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/git_integration/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/git_integration/git_integration.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/git_integration/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/name_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/name_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/name_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/name_generator/btn_givennames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/name_generator/btn_surnames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/name_generator/namegen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/name_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/random_string_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/random_string_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/random_string_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/random_string_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/contrib/utils/tree_select/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/tree_select/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/tree_select/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/tree_select/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/contrib/utils/tree_select/tree_select.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/game_template/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.367913 evennia-4.0.0/evennia/game_template/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/commands/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/commands/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/commands/command.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/commands/default_cmdsets.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      576 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/gitignore
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/server/conf/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/at_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/at_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/at_server_startstop.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/inlinefuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/portal_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/secret_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/server_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1545 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/conf/web_plugins.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/server/logs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/server/logs/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1523 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/exits.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/typeclasses/scripts.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/admin/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/admin/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/api/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/game_template/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/rest_framework/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/rest_framework/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/game_template/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/webclient/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/webclient/js/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/game_template/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/website/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.371913 evennia-4.0.0/evennia/game_template/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/static/website/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/templates/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/templates/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/templates/rest_framework/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/templates/webclient/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/templates/website/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/templates/website/flatpages/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/templates/website/registration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/webclient/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/webclient/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/website/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/web/website/views/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/game_template/world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/world/batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/world/help_entries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/game_template/world/prototypes.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/help/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/filehelp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/help/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/0002_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/0003_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/0004_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/0005_auto_20210530_1818.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/0006_alter_helpentry_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7685 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/help/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/locale/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/README
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/de/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/locale/de/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/es/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/locale/es/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/fr/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/it/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/locale/it/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/ko/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.375913 evennia-4.0.0/evennia/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/la/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locale/la/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/la/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/la/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/pl/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/pt/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/ru/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/sv/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.323913 evennia-4.0.0/evennia/locale/zh/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locale/zh/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/zh/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locale/zh/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/locks/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locks/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22156 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locks/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27271 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locks/lockhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/locks/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/objects/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29651 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.379913 evennia-4.0.0/evennia/objects/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0002_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0004_auto_20150118_1622.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0005_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0007_objectdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0008_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0010_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0011_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13398 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   130580 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21597 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/objects/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.383913 evennia-4.0.0/evennia/prototypes/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    92096 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/menus.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/protfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46538 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42852 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/spawner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39629 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/prototypes/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.383913 evennia-4.0.0/evennia/scripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.383913 evennia-4.0.0/evennia/scripts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8761 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/monitorhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27363 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/ondemandhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/scripthandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27674 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20795 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/taskhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26184 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24661 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/scripts/tickerhandler.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.387913 evennia-4.0.0/evennia/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8753 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/amp_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16627 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/connection_wizard.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8128 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/deprecations.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    79791 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/evennia_launcher.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.387913 evennia-4.0.0/evennia/server/game_index_client/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/game_index_client/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/game_index_client/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6181 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/game_index_client/client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1987 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/game_index_client/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7407 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20403 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1845 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.387913 evennia-4.0.0/evennia/server/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/migrations/0002_auto_20190128_2311.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/migrations/0003_alter_serverconfig_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/models.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.391913 evennia-4.0.0/evennia/server/portal/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/amp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17650 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/amp_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19119 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/discord.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11344 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/grapevine.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/irc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/mccp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/mxp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/naws.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1167 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/portal.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17380 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/portalsessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/rss.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14930 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/ssh.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/suppress_ga.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17380 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/telnet.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/telnet_oob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4750 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/telnet_ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15494 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/ttype.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11521 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16165 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/portal/webclient_ajax.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.391913 evennia-4.0.0/evennia/server/profiling/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20880 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/dummyrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/dummyrunner_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3923 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/memplot.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/settings_mixin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1094 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/test_queries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/profiling/timetrace.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16592 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26992 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30266 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/sessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5390 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/signals.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.391913 evennia-4.0.0/evennia/server/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5193 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/test_amp_connection.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/test_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/test_launcher.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3814 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/test_misc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8694 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/test_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      984 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/tests/testrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/throttle.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1216 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/validators.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/server/webserver.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    62335 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/settings_default.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.391913 evennia-4.0.0/evennia/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    64399 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.395913 evennia-4.0.0/evennia/typeclasses/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37170 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30233 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17814 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/typeclasses/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.395913 evennia-4.0.0/evennia/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    51449 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7756 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/create.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32814 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/evennia-mode.el
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21381 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    80600 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18832 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/evmore.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65172 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    55429 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/gametime.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.395913 evennia-4.0.0/evennia/utils/idmapper/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/LICENSE.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/README_evennia.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/README_orig.rst
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/manager.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2875 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/idmapper/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18789 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/logger.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10324 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/optionclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6519 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/optionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/picklefield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25802 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/test_resources.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.399913 evennia-4.0.0/evennia/utils/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.399913 evennia-4.0.0/evennia/utils/tests/data/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/data/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/data/broken_script.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/data/evform_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/data/evmenu_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/data/prototypes_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7030 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_create_functions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12170 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11764 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12705 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31687 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_tagparsing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31842 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6370 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/tests/test_validatorfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   100943 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/validatorfuncs.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.399913 evennia-4.0.0/evennia/utils/verb_conjugation/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/verb_conjugation/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/verb_conjugation/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9944 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/verb_conjugation/conjugate.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/verb_conjugation/pronouns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/verb_conjugation/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/utils/verb_conjugation/verbs.txt
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.399913 evennia-4.0.0/evennia/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/frontpage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11705 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4498 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      877 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/admin/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/filters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/permissions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/root.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/serializers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8146 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/api/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/evennia/web/static/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/evennia/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/rest_framework/css/api.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/rest_framework/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/evennia/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/css/goldenlayout.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/css/webclient.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/static/webclient/fonts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.403913 evennia-4.0.0/evennia/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18677 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/evennia.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/static/webclient/js/plugins/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/clienthelp.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/default_in.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1967 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/default_out.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/default_unload.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/font.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30344 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/history.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/iframe.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/message_routing.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/multimedia.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/notifications.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/oob.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/options2.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/popups.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/plugins/text2html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9615 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/js/webclient_gui.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/static/webclient/media/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/webclient/media/notification.wav
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/evennia/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/website/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/website/css/website.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/website/images/LICENCE
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/website/images/evennia_logo.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/website/images/evennia_logo_festive.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/static/website/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.327913 evennia-4.0.0/evennia/web/templates/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/templates/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/admin/app_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/admin/frontpage.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/rest_framework/api.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/rest_framework/redoc.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8353 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/webclient/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/webclient/webclient.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/404.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/500.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4059 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/_menu.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/channel_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/channel_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/character_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/character_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/character_manage_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.407913 evennia-4.0.0/evennia/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/flatpages/default.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/generic_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/help_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/help_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.411913 evennia-4.0.0/evennia/web/templates/website/homepage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/homepage/accounts-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      574 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/homepage/database-stats-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/homepage/evennia-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1980 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/homepage/main-content.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      387 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/homepage/recently-connected-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/index.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/messages.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/object_confirm_delete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/object_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/object_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/pagination.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.411913 evennia-4.0.0/evennia/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/logged_out.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/login.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_change_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_change_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_reset_complete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_reset_confirm.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_reset_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_reset_email.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/password_reset_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/registration/register.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templates/website/tbi.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.411913 evennia-4.0.0/evennia/web/templatetags/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templatetags/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templatetags/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/templatetags/addclass.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.411913 evennia-4.0.0/evennia/web/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1353 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/adminsite.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/apache_wsgi.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/backends.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/evennia_modpy_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/evennia_wsgi_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4130 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/general_context.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3144 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/middleware.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2444 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/utils/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.411913 evennia-4.0.0/evennia/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/webclient/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/webclient/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.411913 evennia-4.0.0/evennia/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5737 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/forms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12375 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.415913 evennia-4.0.0/evennia/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2121 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8852 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/errors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11789 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/index.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2024-03-17 13:16:37.000000 evennia-4.0.0/evennia/web/website/views/objects.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:43:07.415913 evennia-4.0.0/evennia.egg-info/
--rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-03-17 13:43:06.000000 evennia-4.0.0/evennia.egg-info/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35956 2024-03-17 13:43:07.000000 evennia-4.0.0/evennia.egg-info/SOURCES.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2024-03-17 13:43:06.000000 evennia-4.0.0/evennia.egg-info/dependency_links.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-03-17 13:43:06.000000 evennia-4.0.0/evennia.egg-info/requires.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2024-03-17 13:43:06.000000 evennia-4.0.0/evennia.egg-info/top_level.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-03-17 13:16:37.000000 evennia-4.0.0/pyproject.toml
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2024-03-17 13:43:07.415913 evennia-4.0.0/setup.cfg
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2024-03-17 13:16:37.000000 evennia-4.0.0/setup.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.223504 evennia-4.1.0/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2024-03-17 13:16:36.000000 evennia-4.1.0/LICENSE.txt
+-rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-04-01 18:37:21.223504 evennia-4.1.0/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3034 2024-03-17 13:16:36.000000 evennia-4.1.0/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.175504 evennia-4.1.0/bin/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/bin/unix/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2024-03-17 13:16:36.000000 evennia-4.1.0/bin/unix/evennia
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2024-04-01 18:25:42.000000 evennia-4.1.0/evennia/VERSION.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      437 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/VERSION_REQS.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15076 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/__main__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/accounts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    74120 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/accounts/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26930 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/bots.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/accounts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/accounts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0002_move_defaults.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0007_copy_player_to_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5741 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/accounts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17496 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/commands/_trial_temp/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/_trial_temp/_trial_marker
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31495 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/cmdhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8286 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27313 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/cmdset.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26152 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/cmdsethandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29047 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/command.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/commands/default/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35296 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19512 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/admin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22983 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/batchprocess.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   172644 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/default/building.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/cmdset_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3033 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/cmdset_character.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      372 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/cmdset_session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      873 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/cmdset_unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    77528 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/default/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25743 2024-04-01 18:23:38.000000 evennia-4.1.0/evennia/commands/default/general.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40503 2024-03-30 15:40:53.000000 evennia-4.1.0/evennia/commands/default/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12774 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/muxcommand.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/syscommands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42139 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/system.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    84255 2024-04-01 18:13:45.000000 evennia-4.1.0/evennia/commands/default/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15024 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    47839 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/comms/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32603 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/comms/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/comms/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/comms/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0003_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0004_auto_20150118_1631.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0005_auto_20150223_1517.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0007_msg_db_tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0008_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0009_auto_20160921_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0010_auto_20161206_1912.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0011_auto_20170217_2039.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0011_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0012_merge_20170617_2017.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0013_auto_20170705_1726.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0014_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0015_auto_20170706_2041.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0016_auto_20180925_1735.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0017_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0018_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0019_auto_20210514_2032.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0020_auto_20210514_2210.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0021_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22647 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/comms/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32479 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/building_menu/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      149 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42684 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/building_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6879 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/color_markups/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/color_markups.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/components/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6914 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      514 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/components/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4638 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/component.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5162 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/components/dbfield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      157 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/exceptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10305 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/holder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/listing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7516 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/signals.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17207 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10389 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/email_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/email_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6041 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      704 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3186 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27603 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2683 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6776 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21871 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23988 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21615 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34959 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8150 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/menu_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8937 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/menu_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16013 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1653 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9986 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/full_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22694 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10561 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34345 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      751 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/state.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10421 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/barter/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/barter.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/clothing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4256 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24856 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/clothing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/containers/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10016 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2851 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/crafting/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41698 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/crafting.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17891 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/example_recipes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25314 2024-03-30 22:45:30.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/gendersub/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/gendersub.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2351 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/mail/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/mail.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/multidescer/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3228 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9952 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/multidescer.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/puzzles/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27836 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/puzzles.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41327 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37445 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_items.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_range.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29680 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/extended_room/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6358 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34233 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/extended_room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12949 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1403 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/mapbuilder/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/simpledoor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/simpledoor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1078 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/slow_exit/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/slow_exit.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/wilderness/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6226 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27385 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/wilderness.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/grid/xyzgrid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54837 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      244 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20845 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7823 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13700 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/launchcmd.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1146 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42076 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40422 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    52059 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24732 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzroom.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/buffs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      210 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    45719 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/buff.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/samplebuffs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16471 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/character_creator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3922 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7448 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/character_creator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/example_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1809 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/dice/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3812 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/dice/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/dice/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12730 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/dice/dice.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/dice/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/health_bar/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/health_bar.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/llm/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15039 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       90 2024-03-24 16:21:41.000000 evennia-4.1.0/evennia/contrib/rpg/llm/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5986 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/llm_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7444 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/llm_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/rpsystem/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10331 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24723 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/rplanguage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    59481 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/rpsystem.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17394 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/traits/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14247 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/traits/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/traits/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/traits/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54514 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/traits/traits.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2312 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3325 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/evadventure/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3758 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/ai.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/build_world.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2024-03-30 20:22:07.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11181 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16990 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_base.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27740 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18271 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_twitch.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17570 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1743 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/enums.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14537 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12402 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11184 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/random_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12130 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/shops.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1664 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_ai.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2150 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28160 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3742 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3322 2024-03-24 14:40:20.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7810 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4159 2024-03-30 22:04:09.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/mirror/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/mirror/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/mirror/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/mirror/mirror.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/red_button/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/red_button/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/red_button/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18610 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/red_button/red_button.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      450 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/build.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25399 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/mob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42921 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7522 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/auditing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/auditing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/auditing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2066 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/auditing/outputs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8516 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/auditing/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/auditing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/fieldfill/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/fieldfill/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/fieldfill/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26383 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/fieldfill/fieldfill.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/git_integration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/git_integration.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/name_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/btn_givennames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/btn_surnames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/namegen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/random_string_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12591 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/tree_select/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/tree_select.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/command.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/default_cmdsets.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      576 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/gitignore
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/server/conf/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/at_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/at_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/at_server_startstop.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/inlinefuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/portal_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/secret_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/server_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1545 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/web_plugins.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/server/logs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/logs/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1524 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/typeclasses/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2045 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/typeclasses/exits.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8848 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/typeclasses/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/scripts.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/admin/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      519 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/web/admin/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/api/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/game_template/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/rest_framework/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/rest_framework/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/game_template/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/webclient/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/webclient/js/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/game_template/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/website/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/website/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/rest_framework/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/webclient/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/website/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/website/flatpages/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/website/registration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1100 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/webclient/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/webclient/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/views/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/help_entries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/prototypes.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/help/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8021 2024-03-30 14:56:23.000000 evennia-4.1.0/evennia/help/filehelp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6230 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/help/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/help/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0002_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0003_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0004_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0005_auto_20210530_1818.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0006_alter_helpentry_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9730 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/help/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3744 2024-03-30 14:56:23.000000 evennia-4.1.0/evennia/help/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7686 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/help/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/README
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/de/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/es/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/fr/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/it/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/ko/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/la/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/la/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/pl/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/pt/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/ru/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/sv/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/zh/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locks/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locks/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22155 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/locks/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27271 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locks/lockhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locks/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/objects/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29653 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/objects/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/objects/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0002_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0004_auto_20150118_1622.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0005_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0007_objectdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0008_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0010_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0011_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13400 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/objects/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   131813 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/objects/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21877 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/objects/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/prototypes/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    92096 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/menus.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/protfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46538 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42851 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/prototypes/spawner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39629 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/scripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/scripts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6312 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8762 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/monitorhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27363 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/ondemandhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5510 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/scripthandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27674 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20794 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/taskhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26185 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/scripts/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24662 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/scripts/tickerhandler.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8753 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/amp_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16628 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/connection_wizard.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8129 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/deprecations.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    79791 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/evennia_launcher.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/server/game_index_client/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/game_index_client/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/game_index_client/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6182 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/game_index_client/client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1988 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/game_index_client/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7406 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20403 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1846 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/server/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/0002_auto_20190128_2311.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/0003_alter_serverconfig_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3819 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/models.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/server/portal/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/amp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17650 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/amp_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19120 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/discord.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/grapevine.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/irc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2572 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/mccp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3883 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2342 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/mxp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2360 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/naws.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1168 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/portal.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/portalsessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4451 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/rss.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14930 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15898 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/server/portal/ssh.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3320 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1787 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/suppress_ga.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17380 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/telnet.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15610 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/telnet_oob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4751 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/telnet_ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15494 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/ttype.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11522 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16166 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/webclient_ajax.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/server/profiling/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20879 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/profiling/dummyrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9428 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/profiling/dummyrunner_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3923 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/memplot.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/settings_mixin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1094 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/test_queries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/timetrace.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1167 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16593 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27031 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5617 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30267 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/sessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5391 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/signals.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/server/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5193 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_amp_connection.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_launcher.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3814 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_misc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8859 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/tests/test_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      985 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/tests/testrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/throttle.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1216 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/validators.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8654 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/webserver.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    62336 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/settings_default.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    64400 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/typeclasses/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31305 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/typeclasses/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/typeclasses/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37171 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/typeclasses/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30234 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/typeclasses/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17814 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    51450 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/utils/ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15393 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7755 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/create.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32815 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41555 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evennia-mode.el
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21381 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    80600 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18832 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evmore.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65172 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    55430 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/utils/funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/gametime.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/utils/idmapper/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/LICENSE.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/README_evennia.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/README_orig.rst
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1182 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/idmapper/manager.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2875 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18788 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/logger.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10324 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/optionclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6519 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/optionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/picklefield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2024-03-31 10:02:22.000000 evennia-4.1.0/evennia/utils/search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25825 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/test_resources.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/utils/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/utils/tests/data/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/broken_script.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/evform_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/evmenu_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/prototypes_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7030 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_create_functions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14444 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/tests/test_eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12171 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/tests/test_evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11764 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31687 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13565 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/tests/test_tagparsing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    33293 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6370 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_validatorfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   102284 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/validatorfuncs.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/utils/verb_conjugation/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9944 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/conjugate.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11299 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/verb_conjugation/pronouns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/verbs.txt
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/frontpage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1890 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/admin/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4498 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8954 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/admin/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/admin/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/filters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3948 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/permissions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/root.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/serializers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8147 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5829 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/rest_framework/css/api.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/rest_framework/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/css/goldenlayout.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/css/webclient.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/fonts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18677 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/evennia.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/js/plugins/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/clienthelp.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_in.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1967 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_out.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_unload.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/font.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/history.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/iframe.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/message_routing.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/multimedia.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/notifications.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/oob.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/options2.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/popups.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/text2html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9615 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/webclient_gui.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/media/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/media/notification.wav
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/css/website.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/LICENCE
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/evennia_logo.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/evennia_logo_festive.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/templates/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/admin/app_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/admin/frontpage.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/rest_framework/api.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/rest_framework/redoc.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8353 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/webclient/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/webclient/webclient.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/404.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/500.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4059 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/_menu.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/channel_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/channel_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/character_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/character_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/character_manage_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/flatpages/default.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/generic_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/help_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/help_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/homepage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/accounts-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      574 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/database-stats-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/evennia-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1980 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/main-content.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      387 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/recently-connected-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/index.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/messages.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/object_confirm_delete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/object_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/object_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/pagination.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/logged_out.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/login.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_change_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_change_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_complete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_confirm.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_email.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/register.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/tbi.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templatetags/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templatetags/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templatetags/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templatetags/addclass.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1353 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/adminsite.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/apache_wsgi.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/backends.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/evennia_modpy_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/evennia_wsgi_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4130 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/web/utils/general_context.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3144 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/middleware.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2444 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      210 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/webclient/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/webclient/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5737 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/forms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12375 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2576 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/views/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8802 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/web/website/views/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/errors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11790 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/views/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/index.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2354 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/views/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/objects.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia.egg-info/
+-rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35956 2024-04-01 18:37:21.000000 evennia-4.1.0/evennia.egg-info/SOURCES.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/dependency_links.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/requires.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/top_level.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-04-01 18:25:49.000000 evennia-4.1.0/pyproject.toml
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2024-04-01 18:37:21.223504 evennia-4.1.0/setup.cfg
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2024-03-17 13:16:37.000000 evennia-4.1.0/setup.py
```

### Comparing `evennia-4.0.0/LICENSE.txt` & `evennia-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/PKG-INFO` & `evennia-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 4.0.0
+Version: 4.1.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-4.0.0/README.md` & `evennia-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/__init__.py` & `evennia-4.1.0/evennia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
    evennia shell
 
 to launch such a shell (using python or ipython depending on your install).
 See www.evennia.com for full documentation.
 
 """
+
 import evennia
 
 # docstring header
 
 DOCSTRING = """
 Evennia MU* creation system.
```

### Comparing `evennia-4.0.0/evennia/__main__.py` & `evennia-4.1.0/evennia/__main__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/accounts.py` & `evennia-4.1.0/evennia/accounts/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 object represents the actual user (not their
 character) and has NO actual presence in the
 game world (this is handled by the associated
 character object, so you should customize that
 instead for most things).
 
 """
+
 import re
 import time
 import typing
 from random import getrandbits
 
 from django.conf import settings
 from django.contrib.auth import authenticate, password_validation
@@ -1330,15 +1331,16 @@
             objects.objects.DefaultObject.search.
 
         """
         # handle me, self and *me, *self
         if isinstance(searchdata, str):
             # handle wrapping of common terms
             if searchdata.lower() in ("me", "*me", "self", "*self"):
-                return self
+                return [self] if quiet else self
+
         searchdata = self.nicks.nickreplace(
             searchdata, categories=("account",), include_account=False
         )
         if search_object:
             matches = ObjectDB.objects.object_search(searchdata, typeclass=typeclass)
         else:
             matches = AccountDB.objects.account_search(searchdata, typeclass=typeclass)
```

### Comparing `evennia-4.0.0/evennia/accounts/bots.py` & `evennia-4.1.0/evennia/accounts/bots.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/manager.py` & `evennia-4.1.0/evennia/accounts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0001_initial.py` & `evennia-4.1.0/evennia/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0003_auto_20150209_2234.py` & `evennia-4.1.0/evennia/accounts/migrations/0003_auto_20150209_2234.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0004_auto_20150403_2339.py` & `evennia-4.1.0/evennia/accounts/migrations/0004_auto_20150403_2339.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0005_auto_20160905_0902.py` & `evennia-4.1.0/evennia/accounts/migrations/0005_auto_20160905_0902.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0006_auto_20170606_1731.py` & `evennia-4.1.0/evennia/accounts/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0007_copy_player_to_account.py` & `evennia-4.1.0/evennia/accounts/migrations/0007_copy_player_to_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0008_auto_20190128_1820.py` & `evennia-4.1.0/evennia/accounts/migrations/0008_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0009_auto_20191025_0831.py` & `evennia-4.1.0/evennia/accounts/migrations/0009_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py` & `evennia-4.1.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/accounts/models.py` & `evennia-4.1.0/evennia/accounts/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 correctly.
 
 To make the Account model more flexible for your own game, it can also
 persistently store attributes of its own. This is ideal for extra
 account info and OOC account configuration variables etc.
 
 """
+
 from django.conf import settings
 from django.contrib.auth.models import AbstractUser
 from django.db import models
 from django.utils.encoding import smart_str
 
 from evennia.accounts.manager import AccountDBManager
 from evennia.server.signals import SIGNAL_ACCOUNT_POST_RENAME
```

### Comparing `evennia-4.0.0/evennia/accounts/tests.py` & `evennia-4.1.0/evennia/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/commands/cmdhandler.py` & `evennia-4.1.0/evennia/commands/cmdhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/commands/cmdparser.py` & `evennia-4.1.0/evennia/commands/cmdparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 The default command parser. Use your own by assigning
 `settings.COMMAND_PARSER` to a Python path to a module containing the
 replacing cmdparser function. The replacement parser must accept the
 same inputs as the default one.
 
 """
 
-
 import re
 
 from django.conf import settings
 
 from evennia.utils.logger import log_trace
 
 _MULTIMATCH_REGEX = re.compile(settings.SEARCH_MULTIMATCH_REGEX, re.I + re.U)
```

### Comparing `evennia-4.0.0/evennia/commands/cmdset.py` & `evennia-4.1.0/evennia/commands/cmdset.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     exist. Ex: A1,A3 + B1,B2,B4,B5 = A1,A3
 * Remove -    This removes the relevant commands from the
     lower-priority cmdset completely.  They are not replaced with
     anything, so this in effects uses the high-priority cmdset as a filter
     to affect the low-priority cmdset.  Ex: A1,A3 + B1,B2,B4,B5 = B2,B4,B5
 
 """
+
 from weakref import WeakKeyDictionary
 
 from django.utils.translation import gettext as _
 
 from evennia.utils.utils import inherits_from, is_iter
 
 __all__ = ("CmdSet",)
```

### Comparing `evennia-4.0.0/evennia/commands/cmdsethandler.py` & `evennia-4.1.0/evennia/commands/cmdsethandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 Since any number of CommandSets can be piled on top of each other, you
 can then implement separate sets for different situations. For
 example, you can have a 'On a boat' set, onto which you then tack on
 the 'Fishing' set. Fishing from a boat? No problem!
 
 """
+
 import sys
 from importlib import import_module
 from inspect import trace
 from traceback import format_exc
 
 from django.conf import settings
 from django.utils.translation import gettext as _
```

### Comparing `evennia-4.0.0/evennia/commands/command.py` & `evennia-4.1.0/evennia/commands/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The base Command class.
 
 All commands in Evennia inherit from the 'Command' class in this module.
 
 """
+
 import inspect
 import math
 import re
 
 from django.conf import settings
 from django.urls import reverse
 from django.utils.text import slugify
@@ -17,15 +18,14 @@
 from evennia.utils.evtable import EvTable
 from evennia.utils.utils import fill, is_iter, lazy_property, make_iter
 
 CMD_IGNORE_PREFIXES = settings.CMD_IGNORE_PREFIXES
 
 
 class InterruptCommand(Exception):
-
     """Cleanly interrupt a command."""
 
     pass
 
 
 def _init_command(cls, **kwargs):
     """
@@ -483,39 +483,37 @@
     def get_command_info(self):
         """
         This is the default output of func() if no func() overload is done.
         Provided here as a separate method so that it can be called for debugging
         purposes when making commands.
 
         """
-        variables = "\n".join(
-            " |w{}|n ({}): {}".format(key, type(val), val) for key, val in self.__dict__.items()
-        )
-        string = f"""
-Command {self} has no defined `func()` - showing on-command variables:
-{variables}
-        """
-        # a simple test command to show the available properties
-        string += "-" * 50
-        string += "\n|w%s|n - Command variables from evennia:\n" % self.key
-        string += "-" * 50
-        string += "\nname of cmd (self.key): |w%s|n\n" % self.key
-        string += "cmd aliases (self.aliases): |w%s|n\n" % self.aliases
-        string += "cmd locks (self.locks): |w%s|n\n" % self.locks
-        string += "help category (self.help_category): |w%s|n\n" % self.help_category.capitalize()
-        string += "object calling (self.caller): |w%s|n\n" % self.caller
-        string += "object storing cmdset (self.obj): |w%s|n\n" % self.obj
-        string += "command string given (self.cmdstring): |w%s|n\n" % self.cmdstring
-        # show cmdset.key instead of cmdset to shorten output
-        string += fill(
-            "current cmdset (self.cmdset): |w%s|n\n"
-            % (self.cmdset.key if self.cmdset.key else self.cmdset.__class__)
-        )
+        output_string = """
+Command \"{cmdname}\" has no defined `func()` method. Available properties on this command are:
 
-        self.msg(string)
+    {variables}"""
+        variables = [
+            " |w{}|n ({}): {}".format(key, type(val), f'"{val}"' if isinstance(val, str) else val)
+            for key, val in (
+                ("self.key", self.key),
+                ("self.cmdname", self.cmdstring),
+                ("self.raw_cmdname", self.raw_cmdname),
+                ("self.raw_string", self.raw_string),
+                ("self.aliases", self.aliases),
+                ("self.args", self.args),
+                ("self.caller", self.caller),
+                ("self.obj", self.obj),
+                ("self.session", self.session),
+                ("self.locks", self.locks),
+                ("self.help_category", self.help_category),
+                ("self.cmdset", self.cmdset),
+            )
+        ]
+        output = output_string.format(cmdname=self.key, variables="\n    ".join(variables))
+        self.msg(output)
 
     def func(self):
         """
         This is the actual executing part of the command.  It is
         called directly after self.parse(). See the docstring of this
         module for which object properties are available (beyond those
         set in self.parse())
```

### Comparing `evennia-4.0.0/evennia/commands/default/account.py` & `evennia-4.1.0/evennia/commands/default/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 case of the `ooc` command), it is None if we are OOC.
 
 Note that under MULTISESSION_MODE > 2, Account commands should use
 self.msg() and similar methods to reroute returns to the correct
 method. Otherwise all text will be returned to all connected sessions.
 
 """
+
 import time
 from codecs import lookup as codecs_lookup
 
 from django.conf import settings
 
 import evennia
 from evennia.utils import create, logger, search, utils
```

### Comparing `evennia-4.0.0/evennia/commands/default/admin.py` & `evennia-4.1.0/evennia/commands/default/admin.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/commands/default/batchprocess.py` & `evennia-4.1.0/evennia/commands/default/batchprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Batch-code is a full-fledged python code interpreter that reads blocks
 of python code (*.py) and executes them in sequence. This allows for
 much more power than Batch-command, but requires knowing Python and
 the Evennia API.  It is also a severe security risk and should
 therefore always be limited to superusers only.
 
 """
+
 import re
 
 from django.conf import settings
 
 from evennia.commands.cmdset import CmdSet
 from evennia.utils import logger, utils
 from evennia.utils.batchprocessors import BATCHCMD, BATCHCODE
```

### Comparing `evennia-4.0.0/evennia/commands/default/building.py` & `evennia-4.1.0/evennia/commands/default/building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """
 Building and world design commands
 """
+
 import re
 import typing
 
-import evennia
 from django.conf import settings
 from django.core.paginator import Paginator
 from django.db.models import Max, Min, Q
+
+import evennia
 from evennia import InterruptCommand
-from evennia.commands.cmdhandler import (generate_cmdset_providers,
-                                         get_and_merge_cmdsets)
+from evennia.commands.cmdhandler import generate_cmdset_providers, get_and_merge_cmdsets
 from evennia.locks.lockhandler import LockException
 from evennia.objects.models import ObjectDB
 from evennia.prototypes import menus as olc_menus
 from evennia.prototypes import prototypes as protlib
 from evennia.prototypes import spawner
 from evennia.scripts.models import ScriptDB
 from evennia.utils import create, funcparser, logger, search, utils
 from evennia.utils.ansi import raw as ansi_raw
 from evennia.utils.dbserialize import deserialize
 from evennia.utils.eveditor import EvEditor
 from evennia.utils.evmore import EvMore
 from evennia.utils.evtable import EvTable
-from evennia.utils.utils import (class_from_module, crop, dbref, display_len,
-                                 format_grid, get_all_typeclasses,
-                                 inherits_from, interactive, list_to_string,
-                                 variable_from_module)
+from evennia.utils.utils import (
+    class_from_module,
+    crop,
+    dbref,
+    display_len,
+    format_grid,
+    get_all_typeclasses,
+    inherits_from,
+    interactive,
+    list_to_string,
+    variable_from_module,
+)
 
 COMMAND_DEFAULT_CLASS = class_from_module(settings.COMMAND_DEFAULT_CLASS)
 
 _FUNCPARSER = None
 _ATTRFUNCPARSER = None
 
 # _KEY_REGEX = re.compile(r"(?P<attr>.*?)(?P<key>(\[.*\]\ *)+)?$")
@@ -214,32 +223,35 @@
     """
     adding permanent aliases for object
 
     Usage:
       alias <obj> [= [alias[,alias,alias,...]]]
       alias <obj> =
       alias/category <obj> = [alias[,alias,...]:<category>
+      alias/delete <obj> = <alias>
 
     Switches:
       category - requires ending input with :category, to store the
         given aliases with the given category.
+      delete - deletes all occurrences of the given alias, regardless
+        of category
 
     Assigns aliases to an object so it can be referenced by more
     than one name. Assign empty to remove all aliases from object. If
     assigning a category, all aliases given will be using this category.
 
     Observe that this is not the same thing as personal aliases
     created with the 'nick' command! Aliases set with alias are
     changing the object in question, making those aliases usable
     by everyone.
     """
 
     key = "@alias"
     aliases = "setobjalias"
-    switch_options = ("category",)
+    switch_options = ("category", "delete")
     locks = "cmd:perm(setobjalias) or perm(Builder)"
     help_category = "Building"
 
     method_type = "cmd_create"
 
     def func(self):
         """Set the aliases."""
@@ -248,20 +260,20 @@
 
         if not self.lhs:
             string = "Usage: alias <obj> [= [alias[,alias ...]]]"
             self.msg(string)
             return
         objname = self.lhs
 
-        # Find the object to receive aliases
+        # Find the object to receive/delete aliases
         obj = caller.search(objname)
         if not obj:
             return
-        if self.rhs is None:
-            # no =, so we just list aliases on object.
+        if self.rhs is None and "delete" not in self.switches:
+            # no =, and not deleting, so we just list aliases on object.
             aliases = obj.aliases.all(return_key_and_category=True)
             if aliases:
                 caller.msg(
                     "Aliases for %s: %s"
                     % (
                         obj.get_display_name(caller),
                         ", ".join(
@@ -276,26 +288,41 @@
             return
 
         if not (obj.access(caller, "control") or obj.access(caller, "edit")):
             caller.msg("You don't have permission to do that.")
             return
 
         if not self.rhs:
-            # we have given an empty =, so delete aliases
+            # we have given an empty =, so delete aliases.
+            # as a side-effect, 'alias/delete obj' and 'alias/delete obj='
+            # will also be caught here, which is fine
             old_aliases = obj.aliases.all()
             if old_aliases:
                 caller.msg(
                     "Cleared aliases from %s: %s"
                     % (obj.get_display_name(caller), ", ".join(old_aliases))
                 )
                 obj.aliases.clear()
             else:
                 caller.msg("No aliases to clear.")
             return
 
+        if "delete" in self.switches:
+            # delete all matching keys, regardless of category
+            existed = False
+            for key, category in obj.aliases.all(return_key_and_category=True):
+                if key == self.rhs:
+                    obj.aliases.remove(key=self.rhs, category=category)
+                    existed = True
+            if existed:
+                caller.msg("Alias '%s' deleted from %s." % (self.rhs, obj.get_display_name(caller)))
+            else:
+                caller.msg("%s has no alias '%s'." % (obj.get_display_name(caller), self.rhs))
+            return
+
         category = None
         if "category" in self.switches:
             if ":" in self.rhs:
                 rhs, category = self.rhs.rsplit(":", 1)
                 category = category.strip()
             else:
                 caller.msg(
@@ -2934,17 +2961,17 @@
         objdata["Permissions"] = self.format_permissions(obj)
         objdata["Locks"] = self.format_locks(obj)
         if current_cmdset and not (
             len(obj.cmdset.all()) == 1 and obj.cmdset.current.key == "_EMPTY_CMDSET"
         ):
             objdata["Stored Cmdset(s)"] = self.format_stored_cmdsets(obj)
             objdata["Merged Cmdset(s)"] = self.format_merged_cmdsets(obj, current_cmdset)
-            objdata[
-                f"Commands available to {obj.key} (result of Merged Cmdset(s))"
-            ] = self.format_current_cmds(obj, current_cmdset)
+            objdata[f"Commands available to {obj.key} (result of Merged Cmdset(s))"] = (
+                self.format_current_cmds(obj, current_cmdset)
+            )
         if self.object_type == "script":
             objdata["Description"] = self.format_script_desc(obj)
             objdata["Persistent"] = self.format_script_is_persistent(obj)
             objdata["Script Repeat"] = self.format_script_timer_data(obj)
         objdata["Scripts"] = self.format_scripts(obj)
         objdata["Tags"] = self.format_tags(obj)
         objdata["Persistent Attributes"] = self.format_attributes(obj)
@@ -3393,17 +3420,19 @@
             if maxrepeat:
                 rept = "%i/%i" % (maxrepeat - remaining, maxrepeat)
             else:
                 rept = "-/-"
 
             table.add_row(
                 f"#{script.id}",
-                f"{script.obj.key}({script.obj.dbref})"
-                if (hasattr(script, "obj") and script.obj)
-                else "<Global>",
+                (
+                    f"{script.obj.key}({script.obj.dbref})"
+                    if (hasattr(script, "obj") and script.obj)
+                    else "<Global>"
+                ),
                 script.key,
                 script.interval if script.interval > 0 else "--",
                 nextrep,
                 rept,
                 script.typeclass_path.rsplit(".", 1)[-1],
                 crop(script.desc, width=20),
             )
```

### Comparing `evennia-4.0.0/evennia/commands/default/cmdset_account.py` & `evennia-4.1.0/evennia/commands/default/cmdset_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/commands/default/cmdset_character.py` & `evennia-4.1.0/evennia/commands/default/cmdset_character.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module ties together all the commands default Character objects have
 available (i.e. IC commands). Note that some commands, such as
 communication-commands are instead put on the account level, in the
 Account cmdset. Account commands remain available also to Characters.
 """
+
 from evennia.commands.cmdset import CmdSet
 from evennia.commands.default import (
     admin,
     batchprocess,
     building,
     general,
     help,
```

### Comparing `evennia-4.0.0/evennia/commands/default/cmdset_unloggedin.py` & `evennia-4.1.0/evennia/commands/default/cmdset_unloggedin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module describes the unlogged state of the default game.
 The setting STATE_UNLOGGED should be set to the python path
 of the state instance in this module.
 """
+
 from evennia.commands.cmdset import CmdSet
 from evennia.commands.default import unloggedin
 
 
 class UnloggedinCmdSet(CmdSet):
     """
     Sets up the unlogged cmdset.
```

### Comparing `evennia-4.0.0/evennia/commands/default/comms.py` & `evennia-4.1.0/evennia/commands/default/comms.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 - channel
 - page
 - irc/rss/grapevine/discord linking
 
 """
 
 from django.conf import settings
+from django.db.models import Q
 
 from evennia.accounts import bots
 from evennia.accounts.models import AccountDB
 from evennia.comms.comms import DefaultChannel
 from evennia.comms.models import Msg
 from evennia.locks.lockhandler import LockException
 from evennia.utils import create, logger, search, utils
@@ -1334,16 +1335,32 @@
         """Implement function using the Msg methods"""
 
         # Since account_caller is set above, this will be an Account.
         caller = self.caller
 
         # get the messages we've sent (not to channels)
         pages_we_sent = Msg.objects.get_messages_by_sender(caller).order_by("-db_date_created")
+        # get only messages tagged as pages or not tagged at all (legacy pages)
+        pages_we_sent = pages_we_sent.filter(
+            Q(db_tags__db_key__iexact="page", db_tags__db_category__iexact="comms")
+            | Q(db_tags__isnull=True)
+        )
+        # we need to default to True to allow for legacy pages
+        pages_we_sent = [msg for msg in pages_we_sent if msg.access(caller, "read", default=True)]
+
         # get last messages we've got
         pages_we_got = Msg.objects.get_messages_by_receiver(caller).order_by("-db_date_created")
+        pages_we_got = pages_we_got.filter(
+            Q(db_tags__db_key__iexact="page", db_tags__db_category__iexact="comms")
+            | Q(db_tags__isnull=True)
+        )
+        # we need to default to True to allow for legacy pages
+        pages_we_got = [msg for msg in pages_we_got if msg.access(caller, "read", default=True)]
+
+        # get only messages tagged as pages or not tagged at all (legacy pages)
         targets, message, number = [], None, None
 
         if "last" in self.switches:
             if pages_we_sent:
                 recv = ",".join(obj.key for obj in pages_we_sent[0].receivers)
                 self.msg(f"You last paged |c{recv}|n:{pages_we_sent[0].message}")
                 return
@@ -1356,14 +1373,15 @@
                 for target in self.lhslist:
                     target_obj = self.caller.search(target)
                     if not target_obj:
                         return
                     targets.append(target_obj)
                 message = self.rhs.strip()
             else:
+                # no = sign, handler this as well
                 target, *message = self.args.split(" ", 1)
                 if target and target.isnumeric():
                     # a number to specify a historic page
                     number = int(target)
                 elif target:
                     target_obj = self.caller.search(target, quiet=True)
                     if target_obj:
@@ -1391,15 +1409,25 @@
                     return
 
             header = f"|wAccount|n |c{caller.key}|n |wpages:|n"
             if message.startswith(":"):
                 message = f"{caller.key} {message.strip(':').strip()}"
 
             # create the persistent message object
-            create.create_message(caller, message, receivers=targets)
+            create.create_message(
+                caller,
+                message,
+                receivers=targets,
+                locks=(
+                    f"read:id({caller.id}) or perm(Admin);"
+                    f"delete:id({caller.id}) or perm(Admin);"
+                    f"edit:id({caller.id}) or perm(Admin)"
+                ),
+                tags=[("page", "comms")],
+            )
 
             # tell the accounts they got a message.
             received = []
             rstrings = []
             for target in targets:
                 if not target.access(caller, "msg"):
                     rstrings.append(f"You are not allowed to page {target}.")
```

### Comparing `evennia-4.0.0/evennia/commands/default/general.py` & `evennia-4.1.0/evennia/commands/default/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 General Character commands usually available to all characters
 """
+
 import re
 
 import evennia
 from django.conf import settings
 from evennia.typeclasses.attributes import NickTemplateInvalid
 from evennia.utils import utils
 
@@ -374,66 +375,116 @@
                     f"|C{key}|n",
                     "{}|n".format(utils.crop(raw_ansi(desc or ""), width=50) or ""),
                 )
             string = f"|wYou are carrying:\n{table}"
         self.msg(text=(string, {"type": "inventory"}))
 
 
-class CmdGet(COMMAND_DEFAULT_CLASS):
+class NumberedTargetCommand(COMMAND_DEFAULT_CLASS):
+    """
+    A class that parses out an optional number component from the input string. This
+    class is intended to be inherited from to provide additional functionality, rather
+    than used on its own.
+    """
+
+    def parse(self):
+        """
+        Parser that extracts a `.number` property from the beginning of the input string.
+
+        For example, if the input string is "3 apples", this parser will set `self.number = 3` and
+        `self.args = "apples"`. If the input string is "apples", this parser will set
+        `self.number = 0` and `self.args = "apples"`.
+
+        """
+        super().parse()
+        self.number = 0
+        if hasattr(self, "lhs"):
+            # handle self.lhs but don't require it
+            count, *args = self.lhs.split(maxsplit=1)
+            # we only use the first word as a count if it's a number and
+            # there is more text afterwards
+            if args and count.isdecimal():
+                self.number = int(count)
+                self.lhs = args[0]
+        if self.args:
+            # check for numbering
+            count, *args = self.args.split(maxsplit=1)
+            # we only use the first word as a count if it's a number and
+            # there is more text afterwards
+            if args and count.isdecimal():
+                self.args = args[0]
+                # we only re-assign self.number if it wasn't already taken from self.lhs
+                if not self.number:
+                    self.number = int(count)
+
+
+class CmdGet(NumberedTargetCommand):
     """
     pick up something
 
     Usage:
       get <obj>
 
-    Picks up an object from your location and puts it in
-    your inventory.
+    Picks up an object from your location and puts it in your inventory.
     """
 
     key = "get"
     aliases = "grab"
-    locks = "cmd:all();view:perm(Developer);read:perm(Developer)"
+    locks = "cmd:all()"
     arg_regex = r"\s|$"
 
     def func(self):
         """implements the command."""
 
         caller = self.caller
 
         if not self.args:
-            caller.msg("Get what?")
-            return
-        obj = caller.search(self.args, location=caller.location)
-        if not obj:
+            self.msg("Get what?")
             return
-        if caller == obj:
-            caller.msg("You can't get yourself.")
-            return
-        if not obj.access(caller, "get"):
-            if obj.db.get_err_msg:
-                caller.msg(obj.db.get_err_msg)
-            else:
-                caller.msg("You can't get that.")
+        objs = caller.search(self.args, location=caller.location, stacked=self.number)
+        if not objs:
             return
+        # the 'stacked' search sometimes returns a list, sometimes not, so we make it always a list
+        # NOTE: this behavior may be a bug, see issue #3432
+        objs = utils.make_iter(objs)
 
-        # calling at_pre_get hook method
-        if not obj.at_pre_get(caller):
+        if len(objs) == 1 and caller == objs[0]:
+            self.msg("You can't get yourself.")
             return
 
-        success = obj.move_to(caller, quiet=True, move_type="get")
-        if not success:
-            caller.msg("This can't be picked up.")
+        # if we aren't allowed to get any of the objects, cancel the get
+        for obj in objs:
+            # check the locks
+            if not obj.access(caller, "get"):
+                if obj.db.get_err_msg:
+                    self.msg(obj.db.get_err_msg)
+                else:
+                    self.msg("You can't get that.")
+                return
+            # calling at_pre_get hook method
+            if not obj.at_pre_get(caller):
+                return
+
+        moved = []
+        # attempt to move all of the objects
+        for obj in objs:
+            if obj.move_to(caller, quiet=True, move_type="get"):
+                moved.append(obj)
+                # calling at_get hook method
+                obj.at_get(caller)
+
+        if not moved:
+            # none of the objects were successfully moved
+            self.msg("That can't be picked up.")
         else:
-            singular, _ = obj.get_numbered_name(1, caller)
-            caller.location.msg_contents(f"$You() $conj(pick) up {singular}.", from_obj=caller)
-            # calling at_get hook method
-            obj.at_get(caller)
+            obj_name = moved[0].get_numbered_name(len(moved), caller, return_string=True)
+            caller.location.msg_contents(f"$You() $conj(pick) up {obj_name}.", from_obj=caller)
 
 
-class CmdDrop(COMMAND_DEFAULT_CLASS):
+class CmdDrop(NumberedTargetCommand):
     """
     drop something
 
     Usage:
       drop <obj>
 
     Lets you drop an object from your inventory into the
@@ -450,38 +501,50 @@
         caller = self.caller
         if not self.args:
             caller.msg("Drop what?")
             return
 
         # Because the DROP command by definition looks for items
         # in inventory, call the search function using location = caller
-        obj = caller.search(
+        objs = caller.search(
             self.args,
             location=caller,
             nofound_string=f"You aren't carrying {self.args}.",
             multimatch_string=f"You carry more than one {self.args}:",
+            stacked=self.number,
         )
-        if not obj:
-            return
-
-        # Call the object script's at_pre_drop() method.
-        if not obj.at_pre_drop(caller):
+        if not objs:
             return
+        # the 'stacked' search sometimes returns a list, sometimes not, so we make it always a list
+        # NOTE: this behavior may be a bug, see issue #3432
+        objs = utils.make_iter(objs)
+
+        # if any objects fail the drop permission check, cancel the drop
+        for obj in objs:
+            # Call the object's at_pre_drop() method.
+            if not obj.at_pre_drop(caller):
+                return
 
-        success = obj.move_to(caller.location, quiet=True, move_type="drop")
-        if not success:
-            caller.msg("This couldn't be dropped.")
+        # do the actual dropping
+        moved = []
+        for obj in objs:
+            if obj.move_to(caller.location, quiet=True, move_type="drop"):
+                moved.append(obj)
+                # Call the object's at_drop() method.
+                obj.at_drop(caller)
+
+        if not moved:
+            # none of the objects were successfully moved
+            self.msg("That can't be dropped.")
         else:
-            singular, _ = obj.get_numbered_name(1, caller)
-            caller.location.msg_contents(f"$You() $conj(drop) {singular}.", from_obj=caller)
-            # Call the object script's at_drop() method.
-            obj.at_drop(caller)
+            obj_name = moved[0].get_numbered_name(len(moved), caller, return_string=True)
+            caller.location.msg_contents(f"$You() $conj(drop) {obj_name}.", from_obj=caller)
 
 
-class CmdGive(COMMAND_DEFAULT_CLASS):
+class CmdGive(NumberedTargetCommand):
     """
     give away something to someone
 
     Usage:
       give <inventory obj> <to||=> <target>
 
     Gives an item from your inventory to another person,
@@ -496,45 +559,58 @@
     def func(self):
         """Implement give"""
 
         caller = self.caller
         if not self.args or not self.rhs:
             caller.msg("Usage: give <inventory object> = <target>")
             return
+        # find the thing(s) to give away
         to_give = caller.search(
             self.lhs,
             location=caller,
             nofound_string=f"You aren't carrying {self.lhs}.",
             multimatch_string=f"You carry more than one {self.lhs}:",
+            stacked=self.number,
         )
+        if not to_give:
+            return
+        # find the target to give to
         target = caller.search(self.rhs)
-        if not (to_give and target):
+        if not target:
             return
 
-        singular, _ = to_give.get_numbered_name(1, caller)
+        # the 'stacked' search sometimes returns a list, sometimes not, so we make it always a list
+        # NOTE: this behavior may be a bug, see issue #3432
+        to_give = utils.make_iter(to_give)
+
+        singular, plural = to_give[0].get_numbered_name(len(to_give), caller)
         if target == caller:
-            caller.msg(f"You keep {singular} to yourself.")
-            return
-        if not to_give.location == caller:
-            caller.msg(f"You are not holding {singular}.")
+            caller.msg(f"You keep {plural if len(to_give) > 1 else singular} to yourself.")
             return
 
-        # calling at_pre_give hook method
-        if not to_give.at_pre_give(caller, target):
-            return
+        # if any of the objects aren't allowed to be given, cancel the give
+        for obj in to_give:
+            # calling at_pre_give hook method
+            if not obj.at_pre_give(caller, target):
+                return
+
+        # do the actual moving
+        moved = []
+        for obj in to_give:
+            if obj.move_to(target, quiet=True, move_type="give"):
+                moved.append(obj)
+                # Call the object's at_give() method.
+                obj.at_give(caller, target)
 
-        # give object
-        success = to_give.move_to(target, quiet=True, move_type="give")
-        if not success:
-            caller.msg(f"You could not give {singular} to {target.key}.")
+        if not moved:
+            caller.msg(f"You could not give that to {target.get_display_name(caller)}.")
         else:
-            caller.msg(f"You give {singular} to {target.key}.")
-            target.msg(f"{caller.key} gives you {singular}.")
-            # Call the object script's at_give() method.
-            to_give.at_give(caller, target)
+            obj_name = to_give[0].get_numbered_name(len(moved), caller, return_string=True)
+            caller.msg(f"You give {obj_name} to {target.get_display_name(caller)}.")
+            target.msg(f"{caller.get_display_name(target)} gives you {obj_name}.")
 
 
 class CmdSetDesc(COMMAND_DEFAULT_CLASS):
     """
     describe yourself
 
     Usage:
```

### Comparing `evennia-4.0.0/evennia/commands/default/help.py` & `evennia-4.1.0/evennia/commands/default/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -776,28 +776,30 @@
 
 
 class CmdSetHelp(CmdHelp):
     """
     Edit the help database.
 
     Usage:
-      sethelp[/switches] <topic>[[;alias;alias][,category[,locks]] [= <text>]
-
+      sethelp[/switches] <topic>[[;alias;alias][,category[,locks]]
+                [= <text or new category>]
     Switches:
       edit - open a line editor to edit the topic's help text.
       replace - overwrite existing help topic.
       append - add text to the end of existing topic with a newline between.
       extend - as append, but don't add a newline.
+      category - change category of existing help topic.
       delete - remove help topic.
 
     Examples:
       sethelp lore = In the beginning was ...
       sethelp/append pickpocketing,Thievery = This steals ...
       sethelp/replace pickpocketing, ,attr(is_thief) = This steals ...
       sethelp/edit thievery
+      sethelp/category thievery = classes
 
     If not assigning a category, the `settings.DEFAULT_HELP_CATEGORY` category
     will be used. If no lockstring is specified, everyone will be able to read
     the help entry.  Sub-topics are embedded in the help text.
 
     Note that this cannot modify command-help entries - these are modified
     in-code, outside the game.
@@ -836,15 +838,15 @@
     |
     | Text for the '<topic>/extra' subtopic
 
     """
 
     key = "sethelp"
     aliases = []
-    switch_options = ("edit", "replace", "append", "extend", "delete")
+    switch_options = ("edit", "replace", "append", "extend", "category", "delete")
     locks = "cmd:perm(Helper)"
     help_category = "Building"
     arg_regex = None
 
     def parse(self):
         """We want to use the default parser rather than the CmdHelp.parse"""
         return COMMAND_DEFAULT_CLASS.parse(self)
@@ -853,15 +855,15 @@
         """Implement the function"""
 
         switches = self.switches
         lhslist = self.lhslist
 
         if not self.args:
             self.msg(
-                "Usage: sethelp[/switches] <topic>[;alias;alias][,category[,locks,..] = <text>"
+                "Usage: sethelp[/switches] <topic>[[;alias;alias][,category[,locks]] [= <text or new category>]"
             )
             return
 
         nlist = len(lhslist)
         topicstr = lhslist[0] if nlist > 0 else ""
         if not topicstr:
             self.msg("You have to define a topic!")
@@ -949,15 +951,15 @@
                 if self.rhs:
                     # we assume append here.
                     old_entry.entrytext += "\n%s" % self.rhs
                 helpentry = old_entry
             else:
                 helpentry = create.create_help_entry(
                     topicstr,
-                    self.rhs,
+                    self.rhs if self.rhs is not None else "",
                     category=category,
                     locks=lockstring,
                     aliases=aliases,
                 )
             self.caller.db._editing_help = helpentry
 
             EvEditor(
@@ -982,14 +984,27 @@
                 old_entry.entrytext += " " + self.rhs
             else:
                 old_entry.entrytext += "\n%s" % self.rhs
             old_entry.aliases.add(aliases)
             self.msg(f"Entry updated:\n{old_entry.entrytext}{aliastxt}")
             return
 
+        if "category" in switches:
+            # set the category
+            if not old_entry:
+                self.msg(f"Could not find topic '{topicstr}'{aliastxt}.")
+                return
+            if not self.rhs:
+                self.msg("You must supply a category.")
+                return
+            category = self.rhs.lower()
+            old_entry.help_category = category
+            self.msg(f"Category for entry '{topicstr}'{aliastxt} changed to '{category}'.")
+            return
+
         if "delete" in switches or "del" in switches:
             # delete the help entry
             if not old_entry:
                 self.msg(f"Could not find topic '{topicstr}'{aliastxt}.")
                 return
             old_entry.delete()
             self.msg(f"Deleted help entry '{topicstr}'{aliastxt}.")
```

### Comparing `evennia-4.0.0/evennia/commands/default/muxcommand.py` & `evennia-4.1.0/evennia/commands/default/muxcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/commands/default/syscommands.py` & `evennia-4.1.0/evennia/commands/default/syscommands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/commands/default/system.py` & `evennia-4.1.0/evennia/commands/default/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 
 System commands
 
 """
 
-
 import code
 import datetime
 import os
 import sys
 import time
 import traceback
 
@@ -108,15 +107,14 @@
         Reload the system.
         """
         evennia.SESSION_HANDLER.announce_all(" Server resetting/restarting ...")
         evennia.SESSION_HANDLER.portal_reset_server()
 
 
 class CmdShutdown(COMMAND_DEFAULT_CLASS):
-
     """
     stop the server completely
 
     Usage:
       shutdown [announcement]
 
     Gracefully shut down both Server and Portal.
@@ -273,15 +271,14 @@
         "evennia": evennia,
         "ev": evennia,
         "inherits_from": utils.inherits_from,
     }
 
 
 class EvenniaPythonConsole(code.InteractiveConsole):
-
     """Evennia wrapper around a Python interactive console."""
 
     def __init__(self, caller):
         super().__init__(evennia_local_vars(caller))
         self.caller = caller
 
     def write(self, string):
```

### Comparing `evennia-4.0.0/evennia/commands/default/tests.py` & `evennia-4.1.0/evennia/commands/default/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,40 +10,48 @@
 main test suite started with
  > python game/manage.py test.
 
 """
 import datetime
 from unittest.mock import MagicMock, Mock, patch
 
-import evennia
 from anything import Anything
 from django.conf import settings
 from django.test import override_settings
+from parameterized import parameterized
+from twisted.internet import task
+
+import evennia
 from evennia import (
     DefaultCharacter,
     DefaultExit,
     DefaultObject,
     DefaultRoom,
     ObjectDB,
     search_object,
 )
 from evennia.commands import cmdparser
 from evennia.commands.cmdset import CmdSet
 from evennia.commands.command import Command, InterruptCommand
-from evennia.commands.default import account, admin, batchprocess, building, comms, general
+from evennia.commands.default import (
+    account,
+    admin,
+    batchprocess,
+    building,
+    comms,
+    general,
+)
 from evennia.commands.default import help as help_module
 from evennia.commands.default import syscommands, system, unloggedin
 from evennia.commands.default.cmdset_character import CharacterCmdSet
 from evennia.commands.default.muxcommand import MuxCommand
 from evennia.prototypes import prototypes as protlib
 from evennia.utils import create, gametime, utils
 from evennia.utils.test_resources import BaseEvenniaCommandTest  # noqa
 from evennia.utils.test_resources import BaseEvenniaTest, EvenniaCommandTest
-from parameterized import parameterized
-from twisted.internet import task
 
 # ------------------------------------------------------------
 # Command testing
 # ------------------------------------------------------------
 
 
 class TestGeneral(BaseEvenniaCommandTest):
@@ -104,23 +112,31 @@
 
     def test_nick_list(self):
         self.call(general.CmdNick(), "/list", "No nicks defined.")
         self.call(general.CmdNick(), "test1 = Hello", "Inputline-nick 'test1' mapped to 'Hello'.")
         self.call(general.CmdNick(), "/list", "Defined Nicks:")
 
     def test_get_and_drop(self):
-        self.call(general.CmdGet(), "Obj", "You pick up an Obj")
-        self.call(general.CmdDrop(), "Obj", "You drop an Obj")
+        self.call(general.CmdGet(), "Obj", "You pick up an Obj.")
+        self.call(general.CmdDrop(), "Obj", "You drop an Obj.")
+        # test stacking
+        self.obj2.key = "Obj"
+        self.call(general.CmdGet(), "2 Obj", "You pick up two Objs.")
+        self.call(general.CmdDrop(), "2 Obj", "You drop two Objs.")
 
     def test_give(self):
         self.call(general.CmdGive(), "Obj to Char2", "You aren't carrying Obj.")
         self.call(general.CmdGive(), "Obj = Char2", "You aren't carrying Obj.")
         self.call(general.CmdGet(), "Obj", "You pick up an Obj")
         self.call(general.CmdGive(), "Obj to Char2", "You give")
         self.call(general.CmdGive(), "Obj = Char", "You give", caller=self.char2)
+        # test stacking
+        self.obj2.key = "Obj"
+        self.obj2.location = self.char1
+        self.call(general.CmdGive(), "2 Obj = Char2", "You give two Objs")
 
     def test_mux_command(self):
         class CmdTest(MuxCommand):
             key = "test"
             switch_options = ("test", "testswitch", "testswitch2")
 
             def func(self):
@@ -193,14 +209,20 @@
         self.call(
             help_module.CmdSetHelp(),
             "testhelp, General = This is a test",
             "Topic 'testhelp' was successfully created.",
             cmdset=CharacterCmdSet(),
         )
         self.call(help_module.CmdHelp(), "testhelp", "Help for testhelp", cmdset=CharacterCmdSet())
+        self.call(
+            help_module.CmdSetHelp(),
+            "/category testhelp = misc",
+            "Category for entry 'testhelp' changed to 'misc'.",
+            cmdset=CharacterCmdSet(),
+        )
 
     @parameterized.expand(
         [
             (
                 "test",  # main help entry
                 (
                     "Help for test\n\n"
@@ -780,14 +802,32 @@
         self.call(building.CmdSetObjAlias(), "", "Usage: ")
         self.call(building.CmdSetObjAlias(), "NotFound =", "Could not find 'NotFound'.")
 
         self.call(building.CmdSetObjAlias(), "Obj", "Aliases for Obj: 'testobj1b'")
         self.call(building.CmdSetObjAlias(), "Obj2 =", "Cleared aliases from Obj2")
         self.call(building.CmdSetObjAlias(), "Obj2 =", "No aliases to clear.")
 
+        self.call(building.CmdSetObjAlias(), "Obj =", "Cleared aliases from Obj: testobj1b")
+        self.call(
+            building.CmdSetObjAlias(),
+            "/category Obj = testobj1b:category1",
+            "Alias(es) for 'Obj' set to 'testobj1b' (category: 'category1').",
+        )
+        self.call(
+            building.CmdSetObjAlias(),
+            "/category Obj = testobj1b:category2",
+            "Alias(es) for 'Obj' set to 'testobj1b,testobj1b' (category: 'category2').",
+        )
+        self.call(
+            building.CmdSetObjAlias(),  # delete both occurences of alias 'testobj1b'
+            "/delete Obj = testobj1b",
+            "Alias 'testobj1b' deleted from Obj.",
+        )
+        self.call(building.CmdSetObjAlias(), "Obj =", "No aliases to clear.")
+
     def test_copy(self):
         self.call(
             building.CmdCopy(),
             "Obj = TestObj2;TestObj2b, TestObj3;TestObj3b",
             "Copied Obj to 'TestObj3' (aliases: ['TestObj3b']",
         )
         self.call(building.CmdCopy(), "", "Usage: ")
@@ -1750,16 +1790,15 @@
             # Just to make sure we use a different location, in case someone changes
             # char1's default location in the future...
             spawnLoc = self.room1
 
         self.call(
             building.CmdSpawn(),
             "{'prototype_key':'GOBLIN', 'typeclass':'evennia.objects.objects.DefaultCharacter', "
-            "'key':'goblin', 'location':'%s'}"
-            % spawnLoc.dbref,
+            "'key':'goblin', 'location':'%s'}" % spawnLoc.dbref,
             "Spawned goblin",
         )
         goblin = get_object(self, "goblin")
         # Tests that the spawned object's type is a DefaultCharacter.
         self.assertIsInstance(goblin, DefaultCharacter)
         self.assertEqual(goblin.location, spawnLoc)
 
@@ -1799,16 +1838,15 @@
         )
 
         # Tests "spawn/noloc ...", but DO specify a location.
         # Location should be the specified location.
         self.call(
             building.CmdSpawn(),
             "/noloc {'prototype_parent':'TESTBALL', 'key': 'Ball', 'prototype_key': 'foo',"
-            " 'location':'%s'}"
-            % spawnLoc.dbref,
+            " 'location':'%s'}" % spawnLoc.dbref,
             "Spawned Ball",
         )
         ball = get_object(self, "Ball")
         self.assertEqual(ball.location, spawnLoc)
         ball.delete()
 
         # test calling spawn with an invalid prototype.
@@ -2044,14 +2082,19 @@
             "TestAccount2 = Test",
             (
                 "TestAccount2 is offline. They will see your message if they list their pages"
                 " later.|You paged TestAccount2 with: 'Test'."
             ),
             receiver=self.account,
         )
+        from evennia.comms.models import Msg
+
+        msgs = Msg.objects.filter(db_tags__db_key="page", db_tags__db_category="comms")
+        self.assertEqual(msgs[0].senders, [self.account])
+        self.assertEqual(msgs[0].receivers, [self.account2])
 
 
 @override_settings(DISCORD_BOT_TOKEN="notarealtoken", DISCORD_ENABLED=True)
 class TestDiscord(BaseEvenniaCommandTest):
     def setUp(self):
         super().setUp()
         self.channel = create.create_channel(key="testchannel", desc="A test channel")
```

### Comparing `evennia-4.0.0/evennia/commands/default/unloggedin.py` & `evennia-4.1.0/evennia/commands/default/unloggedin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Commands that are available from the connect screen.
 
 """
+
 import datetime
 import re
 from codecs import lookup as codecs_lookup
 
 from django.conf import settings
 
 import evennia
```

### Comparing `evennia-4.0.0/evennia/commands/tests.py` & `evennia-4.1.0/evennia/commands/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/comms.py` & `evennia-4.1.0/evennia/comms/comms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Base typeclass for in-game Channels.
 
 """
+
 import re
 
 from django.contrib.contenttypes.models import ContentType
 from django.urls import reverse
 from django.utils.text import slugify
 
 import evennia
```

### Comparing `evennia-4.0.0/evennia/comms/managers.py` & `evennia-4.1.0/evennia/comms/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 These managers define helper methods for accessing the database from
 Comm system components.
 
 """
 
-
 from django.conf import settings
 from django.db.models import Q
 
 from evennia.server import signals
 from evennia.typeclasses.managers import TypeclassManager, TypedObjectManager
 from evennia.utils import logger
 from evennia.utils.utils import class_from_module, dbref, make_iter
```

### Comparing `evennia-4.0.0/evennia/comms/migrations/0001_initial.py` & `evennia-4.1.0/evennia/comms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0003_auto_20140917_0756.py` & `evennia-4.1.0/evennia/comms/migrations/0003_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0005_auto_20150223_1517.py` & `evennia-4.1.0/evennia/comms/migrations/0005_auto_20150223_1517.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py` & `evennia-4.1.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0007_msg_db_tags.py` & `evennia-4.1.0/evennia/comms/migrations/0007_msg_db_tags.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0009_auto_20160921_1731.py` & `evennia-4.1.0/evennia/comms/migrations/0009_auto_20160921_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0010_auto_20161206_1912.py` & `evennia-4.1.0/evennia/comms/migrations/0010_auto_20161206_1912.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0011_auto_20170217_2039.py` & `evennia-4.1.0/evennia/comms/migrations/0011_auto_20170217_2039.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0011_auto_20170606_1731.py` & `evennia-4.1.0/evennia/comms/migrations/0011_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0013_auto_20170705_1726.py` & `evennia-4.1.0/evennia/comms/migrations/0013_auto_20170705_1726.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0014_auto_20170705_1736.py` & `evennia-4.1.0/evennia/comms/migrations/0014_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0015_auto_20170706_2041.py` & `evennia-4.1.0/evennia/comms/migrations/0015_auto_20170706_2041.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0017_auto_20190128_1820.py` & `evennia-4.1.0/evennia/comms/migrations/0017_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0018_auto_20191025_0831.py` & `evennia-4.1.0/evennia/comms/migrations/0018_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0019_auto_20210514_2032.py` & `evennia-4.1.0/evennia/comms/migrations/0019_auto_20210514_2032.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0020_auto_20210514_2210.py` & `evennia-4.1.0/evennia/comms/migrations/0020_auto_20210514_2210.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0021_auto_20210520_2137.py` & `evennia-4.1.0/evennia/comms/migrations/0021_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py` & `evennia-4.1.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/comms/models.py` & `evennia-4.1.0/evennia/comms/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 database.
 
 Channels are central objects that act as targets for Msgs. Accounts can
 connect to channels by use of a ChannelConnect object (this object is
 necessary to easily be able to delete connections on the fly).
 
 """
+
 from django.conf import settings
 from django.db import models
 from django.utils import timezone
 
 from evennia.comms import managers
 from evennia.locks.lockhandler import LockHandler
 from evennia.typeclasses.models import TypedObject
```

### Comparing `evennia-4.0.0/evennia/comms/tests.py` & `evennia-4.1.0/evennia/comms/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/README.md` & `evennia-4.1.0/evennia/contrib/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/awsstorage/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/awsstorage/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py` & `evennia-4.1.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,14 @@
             'allows sufficient "max_length".' % name
         )
     return os.path.join(dir_name, "{}{}".format(file_root, file_ext))
 
 
 @deconstructible
 class S3Boto3StorageFile(File):
-
     """
     The default file object used by the S3Boto3Storage backend.
     This file implements file streaming using boto's multipart
     uploading functionality. The file can be opened in read or
     write mode.
     This class extends Django's File class. However, the contained
     data is only the data contained in the current buffer. So you
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/awsstorage/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/awsstorage/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/building_menu/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/building_menu/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/building_menu/building_menu.py` & `evennia-4.1.0/evennia/contrib/base_systems/building_menu/building_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,14 @@
     )
 
 
 # Building menu commands and CmdSet
 
 
 class CmdNoInput(Command):
-
     """No input has been found."""
 
     key = _CMD_NOINPUT
     locks = "cmd:all()"
 
     def __init__(self, **kwargs):
         self.menu = kwargs.pop("building_menu", None)
@@ -348,15 +347,14 @@
         else:
             log_err("When CMDNOINPUT was called, the building menu couldn't be found")
             self.caller.msg("|rThe building menu couldn't be found, remove the CmdSet.|n")
             self.caller.cmdset.delete(BuildingMenuCmdSet)
 
 
 class CmdNoMatch(Command):
-
     """No input has been found."""
 
     key = _CMD_NOMATCH
     locks = "cmd:all()"
 
     def __init__(self, **kwargs):
         self.menu = kwargs.pop("building_menu", None)
@@ -390,15 +388,14 @@
                     self.menu.move(choice.key)
                     return
 
             self.msg("|rUnknown command: {}|n.".format(raw_string))
 
 
 class BuildingMenuCmdSet(CmdSet):
-
     """Building menu CmdSet."""
 
     key = "building_menu"
     priority = 5
     mergetype = "Replace"
 
     def at_cmdset_creation(self):
@@ -417,15 +414,14 @@
             self.add(cmd(building_menu=menu))
 
 
 # Menu classes
 
 
 class Choice:
-
     """A choice object, created by `add_choice`."""
 
     def __init__(
         self,
         title,
         key=None,
         aliases=None,
@@ -553,15 +549,14 @@
                 string=string,
                 caller=self.caller,
                 obj=self.obj,
             )
 
 
 class BuildingMenu:
-
     """
     Class allowing to create and set building menus to edit specific objects.
 
     A building menu is somewhat similar to `EvMenu`, but designed to edit
     objects by builders, although it can be used for players in some contexts.
     You could, for instance, create a building menu to edit a room with a
     sub-menu for the room's key, another for the room's description,
@@ -1196,15 +1191,14 @@
                 return
 
             return building_menu
 
 
 # Generic building menu and command
 class GenericBuildingMenu(BuildingMenu):
-
     """A generic building menu, allowing to edit any object.
 
     This is more a demonstration menu.  By default, it allows to edit the
     object key and description.  Nevertheless, it will be useful to demonstrate
     how building menus are meant to be used.
 
     """
@@ -1237,15 +1231,14 @@
                 back="|n or |y".join(self.keys_go_back)
             ),
         )
         self.add_choice_edit("description", key="d", attr="db.desc")
 
 
 class GenericBuildingCmd(Command):
-
     """
     Generic building command.
 
     Syntax:
       @edit [object]
 
     Open a building menu to edit the specified object.  This menu allows to
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/building_menu/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/building_menu/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/color_markups/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/color_markups/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/color_markups/color_markups.py` & `evennia-4.1.0/evennia/contrib/base_systems/color_markups/color_markups.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/color_markups/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/color_markups/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/components/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/__init__.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,12 +3,13 @@
 
 This is a basic Component System.
 It allows you to use components on typeclasses using a simple syntax.
 This helps writing isolated code and reusing it over multiple objects.
 
 See the docs for more information.
 """
+
 from . import exceptions  # noqa
 from .component import Component  # noqa
 from .dbfield import DBField, NDBField, TagField  # noqa
 from .holder import ComponentHolderMixin, ComponentProperty  # noqa
 from .listing import COMPONENT_LISTING, get_component_class  # noqa
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/component.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/component.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/dbfield.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/dbfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Components - ChrisLR 2022
 
 This file contains the Descriptors used to set Fields in Components
 """
+
 import typing
 
 from evennia.typeclasses.attributes import AttributeProperty, NAttributeProperty
 
 if typing.TYPE_CHECKING:
     from .components import Component
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/holder.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/holder.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/listing.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/listing.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/signals.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/components/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/components/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py` & `evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,14 @@
     return script
 
 
 # Scripts dealing in gametime (use `schedule`  to create it)
 
 
 class GametimeScript(DefaultScript):
-
     """Gametime-sensitive script."""
 
     def at_script_creation(self):
         """The script is created."""
         self.key = "unknown scr"
         self.interval = 100
         self.start_delay = True
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/custom_gametime/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/email_login/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/email_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/email_login/connection_screens.py` & `evennia-4.1.0/evennia/contrib/base_systems/email_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/email_login/email_login.py` & `evennia-4.1.0/evennia/contrib/base_systems/email_login/email_login.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/email_login/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/email_login/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/__init__.py` & `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 
 This allows you to connect both the regular webclient and a godot specific webclient.
 You can simply connect the resulting text to Godot's RichTextLabel and have the proper display.
 You could also pass extra data to this client for advanced functionality.
 
 See the docs for more information.
 """
+
 from evennia.contrib.base_systems.godotwebsocket.text2bbcode import (
     BBCODE_PARSER,
     parse_to_bbcode,
 )
 from evennia.contrib.base_systems.godotwebsocket.webclient import GodotWebSocketClient
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py` & `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/test_webclient.py` & `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py` & `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Godot Websocket - ChrisLR 2022
 
 This file contains the necessary code and data to convert text with color tags to bbcode (For godot)
 """
+
 from evennia.utils.ansi import *
 from evennia.utils.text2html import TextToHTMLparser
 
 # All xterm256 RGB equivalents
 
 XTERM256_FG = "\033[38;5;{}m"
 XTERM256_BG = "\033[48;5;{}m"
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/godotwebsocket/webclient.py` & `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/webclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Godot Websocket - ChrisLR 2022
 
 This file contains the code necessary to dedicate a port to communicate with Godot via Websockets.
 It uses the plugin system and should be plugged via settings as detailed in the readme.
 """
+
 import json
 
 from autobahn.twisted import WebSocketServerFactory
 from twisted.application import internet
 
 from evennia import settings
 from evennia.contrib.base_systems.godotwebsocket.text2bbcode import parse_to_bbcode
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Module containing the CallbackHandler for individual objects.
 """
 
 from collections import namedtuple
 
 
 class CallbackHandler(object):
-
     """
     The callback handler for a specific object.
 
     The script that contains all callbacks will be reached through this
     handler.  This handler is therefore a shortcut to be used by
     developers.  This handler (accessible through `obj.callbacks`) is a
     shortcut to manipulating callbacks within this object, getting,
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/commands.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 them and when.  You can then accept a specific callback:
   @call here = enter 1
 Use the /del switch to remove callbacks that should not be connected.
 """
 
 
 class CmdCallback(COMMAND_DEFAULT_CLASS):
-
     """
     Command to edit callbacks.
     """
 
     key = "@call"
     aliases = ["@callback", "@callbacks", "@calls"]
     locks = "cmd:perm({})".format(VALIDATING)
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/scripts.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from evennia.utils.utils import all_from_module, delay, pypath_to_realpath
 
 # Constants
 RE_LINE_ERROR = re.compile(r'^  File "\<string\>", line (\d+)')
 
 
 class EventHandler(DefaultScript):
-
     """
     The event handler that contains all events in a global script.
 
     This script shouldn't be created more than once.  It contains
     event (in a non-persistent attribute) and callbacks (in a
     persistent attribute).  The script method would help adding,
     editing and deleting these events and callbacks.
@@ -596,15 +595,14 @@
 
         self.db.tasks[task_id] = (now + delta, obj, callback_name, locals)
         delay(seconds, complete_task, task_id)
 
 
 # Script to call time-related events
 class TimeEventScript(DefaultScript):
-
     """Gametime-sensitive script."""
 
     def at_script_creation(self):
         """The script is created."""
         self.start_delay = True
         self.persistent = True
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 settings.EVENTS_CALENDAR = "standard"
 
 # Constants
 OLD_EVENTS = {}
 
 
 class TestEventHandler(BaseEvenniaTest):
-
     """
     Test cases of the event handler to add, edit or delete events.
     """
 
     def setUp(self):
         """Create the event handler."""
         super().setUp()
@@ -255,15 +254,14 @@
 
         # Delete the callback
         self.room1.callbacks.remove("dummy", 0)
         self.assertEqual(self.room1.callbacks.all(), {})
 
 
 class TestCmdCallback(BaseEvenniaCommandTest):
-
     """Test the @callback command."""
 
     def setUp(self):
         """Create the callback handler."""
         super().setUp()
         self.handler = create_script(
             "evennia.contrib.base_systems.ingame_python.scripts.EventHandler"
@@ -444,15 +442,14 @@
         # char1 will accept the callback
         self.call(CmdCallback(), "/accept here = time 1")
         callback = self.room1.callbacks.get("time")[0]
         self.assertEqual(callback.valid, True)
 
 
 class TestDefaultCallbacks(BaseEvenniaCommandTest):
-
     """Test the default callbacks."""
 
     def setUp(self):
         """Create the callback handler."""
         super().setUp()
         self.handler = create_script(
             "evennia.contrib.base_systems.ingame_python.scripts.EventHandler"
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/typeclasses.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/typeclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
 Variables you can use in this event:
     character: the character connected to this event.
 """
 
 
 @register_events
 class EventCharacter(DefaultCharacter):
-
     """Typeclass to represent a character and call event types."""
 
     _events = {
         "can_delete": (["character"], CHARACTER_CAN_DELETE),
         "can_move": (["character", "origin", "destination"], CHARACTER_CAN_MOVE),
         "can_part": (["character", "departing"], CHARACTER_CAN_PART),
         "can_say": (["speaker", "character", "message"], CHARACTER_CAN_SAY, phrase_event),
@@ -621,15 +620,14 @@
     origin: the exit's location (where the character was before moving).
     destination: the character's location after moving.
 """
 
 
 @register_events
 class EventExit(DefaultExit):
-
     """Modified exit including management of events."""
 
     _events = {
         "can_traverse": (["character", "exit", "room"], EXIT_CAN_TRAVERSE),
         "msg_arrive": (
             ["character", "exit", "origin", "destination", "message", "mapping"],
             EXIT_MSG_ARRIVE,
@@ -717,15 +715,14 @@
 Variables you can use in this event:
     object: the object connected to this event.
 """
 
 
 @register_events
 class EventObject(DefaultObject):
-
     """Default object with management of events."""
 
     _events = {
         "drop": (["character", "obj"], OBJECT_DROP),
         "get": (["character", "obj"], OBJECT_GET),
         "time": (["object"], OBJECT_TIME, None, time_event),
     }
@@ -888,15 +885,14 @@
     character: the character who is about to be un-puppeted in this room.
     room: the room connected to this event.
 """
 
 
 @register_events
 class EventRoom(DefaultRoom):
-
     """Default room with management of events."""
 
     _events = {
         "can_delete": (["room"], ROOM_CAN_DELETE),
         "can_move": (["character", "room"], ROOM_CAN_MOVE),
         "can_say": (["character", "room", "message"], ROOM_CAN_SAY, phrase_event),
         "delete": (["room"], ROOM_DELETE),
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/ingame_python/utils.py` & `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,14 @@
         if not keys or any(key.strip().lower() in words for key in keys.split(",")):
             to_call.append(callback)
 
     return to_call
 
 
 class InterruptEvent(RuntimeError):
-
     """
     Interrupt the current event.
 
     You shouldn't have to use this exception directly, probably use the
     `deny()` function that handles it instead.
 
     """
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/menu_login/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/menu_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/menu_login/connection_screens.py` & `evennia-4.1.0/evennia/contrib/base_systems/menu_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/menu_login/menu_login.py` & `evennia-4.1.0/evennia/contrib/base_systems/menu_login/menu_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         try:
             _ACCOUNT.objects.get(username__iexact=username)
         except _ACCOUNT.DoesNotExist:
             new_user = True
         else:
             new_user = False
 
-        if new_user and not settings.ACCOUNT_REGISTRATION_ENABLED:
+        if new_user and not settings.NEW_ACCOUNT_REGISTRATION_ENABLED:
             caller.msg("Registration is currently disabled.")
             return None
 
         # pass username/new_user into next node as kwargs
         return "node_enter_password", {"new_user": new_user, "username": username}
 
     callables = callables_from_module(_CONNECTION_SCREEN_MODULE)
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py` & `evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     # ...
     def at_cmdset_creation(self):
         # ...
         self.add(CmdSetLegacyComms)   # <----
 ```
 
 """
+
 from django.conf import settings
 
 from evennia.commands.cmdset import CmdSet
 from evennia.commands.default.comms import CmdChannel
 from evennia.utils import logger
 
 CHANNEL_DEFAULT_TYPECLASS = settings.BASE_CHANNEL_TYPECLASS
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/unixcommand/README.md` & `evennia-4.1.0/evennia/contrib/base_systems/unixcommand/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/unixcommand/tests.py` & `evennia-4.1.0/evennia/contrib/base_systems/unixcommand/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 
 from .unixcommand import UnixCommand
 
 
 class CmdDummy(UnixCommand):
-
     """A dummy UnixCommand."""
 
     key = "dummy"
 
     def init_parser(self):
         """Fill out options."""
         self.parser.add_argument("nb1", type=int, help="the first number")
```

### Comparing `evennia-4.0.0/evennia/contrib/base_systems/unixcommand/unixcommand.py` & `evennia-4.1.0/evennia/contrib/base_systems/unixcommand/unixcommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,22 +68,20 @@
 from textwrap import dedent
 
 from evennia import Command, InterruptCommand
 from evennia.utils.ansi import raw
 
 
 class ParseError(Exception):
-
     """An error occurred during parsing."""
 
     pass
 
 
 class UnixCommandParser(argparse.ArgumentParser):
-
     """A modifier command parser for unix commands.
 
     This parser is used to replace `argparse.ArgumentParser`.  It
     is aware of the command calling it, and can more easily report to
     the caller.  Some features (like the "brutal exit" of the original
     parser) are disabled or replaced.  This parser is used by UnixCommand
     and creating one directly isn't recommended nor necessary.  Even
@@ -179,15 +177,14 @@
 
         """
         if self.command:
             self.command.msg(self.format_help().strip())
 
 
 class HelpAction(argparse.Action):
-
     """Override the -h/--help action in the default parser.
 
     Using the default -h/--help will call the exit function in different
     ways, preventing the entire help message to be provided.  Hence
     this override.
 
     """
```

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/README.md` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/commands.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/menu.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This is started from the `evscaperoom` command.
 
 Here player user can set their own description as well as select to create a
 new room (to start from scratch) or join an existing room (with other players).
 
 """
+
 from evennia import EvMenu
 from evennia.utils import create, justify, list_to_string, logger
 from evennia.utils.evmenu import list_node
 
 from .room import EvscapeRoom
 from .utils import create_fantasy_word
```

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/objects.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 - Sittable    (can be sat on)
 - Liable      (can be lied down on)
 - Kneeable    (can be kneed down on)
 - Climbable   (can be climbed on)
 - Positionable (supports sit/lie/knee/climb at once)
 
 """
+
 import inspect
 import re
 
 from evennia import DefaultObject
 from evennia.utils.utils import list_to_string, wrap
 
 from .utils import create_evscaperoom_object, parse_for_perspectives, parse_for_things
```

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/room.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/room.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/scripts.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/state.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/state.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/states/README.md` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/tests.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Unit tests for the Evscaperoom
 
 """
+
 import inspect
 import pkgutil
 from os import path
 
 from evennia import InterruptCommand
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 from evennia.utils import mod_import
```

### Comparing `evennia-4.0.0/evennia/contrib/full_systems/evscaperoom/utils.py` & `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/barter/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/barter/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/barter/barter.py` & `evennia-4.1.0/evennia/contrib/game_systems/barter/barter.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/barter/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/barter/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/clothing/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/clothing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/clothing/clothing.py` & `evennia-4.1.0/evennia/contrib/game_systems/clothing/clothing.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,17 +68,19 @@
 with which to test the system:
 
     @create a pretty shirt : evennia.contrib.game_systems.clothing.ContribClothing
     @set shirt/clothing_type = 'top'
     wear shirt
 
 """
+
 from collections import defaultdict
 
 from django.conf import settings
+
 from evennia import DefaultCharacter, DefaultObject, default_cmds
 from evennia.commands.default.muxcommand import MuxCommand
 from evennia.utils import (
     at_search_result,
     crop,
     evtable,
     group_objects_by_key_and_desc,
```

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/clothing/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/clothing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/containers/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/containers/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/containers/containers.py` & `evennia-4.1.0/evennia/contrib/game_systems/containers/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 or implement the same locks/hooks in your own typeclasses.
 
 `ContribContainer` implements the following new methods:
 
     at_pre_get_from(getter, target, **kwargs) - called with the pre-get hooks
     at_pre_put_in(putter, target, **kwargs)   - called with the pre-put hooks
 """
+
 from django.conf import settings
 
 from evennia import AttributeProperty, CmdSet, DefaultObject
 from evennia.commands.default.general import CmdDrop, CmdGet, CmdLook
 from evennia.utils import class_from_module
 
 # establish the right inheritance for container objects
```

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/containers/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/containers/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/cooldowns/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/cooldowns/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/cooldowns/cooldowns.py` & `evennia-4.1.0/evennia/contrib/game_systems/cooldowns/cooldowns.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/cooldowns/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/cooldowns/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/crafting/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/crafting/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/crafting/crafting.py` & `evennia-4.1.0/evennia/contrib/game_systems/crafting/crafting.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         to change crafting return style in some way.
 
         Args:
             message(str): The message to send.
             **kwargs: Any optional properties relevant to this send.
 
         """
-        self.crafter.msg(message, {"type": "crafting"})
+        self.crafter.msg(text=(message, {"type": "crafting"}))
 
     def pre_craft(self, **kwargs):
         """
         Hook to override.
 
         This is called just before crafting operation and is normally
         responsible for validating the inputs, storing data on
@@ -611,17 +611,19 @@
         if self.output_names:
             assert len(self.output_names) == len(self.output_prototypes), (
                 f"Crafting {self.__class__}.output_names list must "
                 "have the same length as .output_prototypes."
             )
         else:
             self.output_names = [
-                prot.get("key", prot.get("typeclass", "unnamed"))
-                if isinstance(prot, dict)
-                else str(prot)
+                (
+                    prot.get("key", prot.get("typeclass", "unnamed"))
+                    if isinstance(prot, dict)
+                    else str(prot)
+                )
                 for prot in self.output_prototypes
             ]
 
         # don't allow reuse if we have consumables. If only tools we can reuse
         # over and over since nothing changes.
         self.allow_reuse = not bool(self.consumable_tags)
```

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/crafting/example_recipes.py` & `evennia-4.1.0/evennia/contrib/game_systems/crafting/example_recipes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/crafting/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/crafting/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             self.crafter, self.inp1, self.inp2, self.inp3, **self.kwargs
         )
 
     def test_msg(self):
         """Test messaging to crafter"""
 
         self.recipe.msg("message")
-        self.crafter.msg.assert_called_with("message", {"type": "crafting"})
+        self.crafter.msg.assert_called_with(text=("message", {"type": "crafting"}))
 
     def test_pre_craft(self):
         """Test validating hook"""
         self.recipe.pre_craft()
         self.assertEqual(self.recipe.validated_inputs, (self.inp1, self.inp2, self.inp3))
 
     def test_pre_craft_fail(self):
@@ -202,15 +202,15 @@
         )
 
         result = recipe.craft()
 
         self.assertEqual(result[0].key, "Result1")
         self.assertEqual(result[0].tags.all(), ["result1", "resultprot"])
         self.crafter.msg.assert_called_with(
-            recipe.success_message.format(outputs="Result1"), {"type": "crafting"}
+            text=(recipe.success_message.format(outputs="Result1"), {"type": "crafting"})
         )
 
         # make sure consumables are gone
         self.assertIsNone(self.cons1.pk)
         self.assertIsNone(self.cons2.pk)
         self.assertIsNone(self.cons3.pk)
         # make sure tools remain
@@ -231,15 +231,15 @@
         recipe = _MockRecipe(self.crafter, *(tools + consumables))
 
         result = recipe.craft()
 
         self.assertEqual(result[0].key, "Result1")
         self.assertEqual(result[0].tags.all(), ["result1", "resultprot"])
         self.crafter.msg.assert_called_with(
-            recipe.success_message.format(outputs="Result1"), {"type": "crafting"}
+            text=(recipe.success_message.format(outputs="Result1"), {"type": "crafting"})
         )
 
         # make sure consumables are gone
         for cons in consumables:
             self.assertIsNone(cons.pk)
         # make sure tools remain
         for tool in tools:
@@ -247,16 +247,18 @@
 
     def test_craft_missing_tool__fail(self):
         """Fail craft by missing tool2"""
         recipe = _MockRecipe(self.crafter, self.tool1, self.cons1, self.cons2, self.cons3)
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_tool_missing_message.format(outputs="Result1", missing="tool2"),
-            {"type": "crafting"},
+            text=(
+                recipe.error_tool_missing_message.format(outputs="Result1", missing="tool2"),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         # make sure tools remain
@@ -265,16 +267,18 @@
 
     def test_craft_missing_cons__fail(self):
         """Fail craft by missing cons3"""
         recipe = _MockRecipe(self.crafter, self.tool1, self.tool2, self.cons1, self.cons2)
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_consumable_missing_message.format(outputs="Result1", missing="cons3"),
-            {"type": "crafting"},
+            text=(
+                recipe.error_consumable_missing_message.format(outputs="Result1", missing="cons3"),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         # make sure tools remain
@@ -289,16 +293,18 @@
         recipe = _MockRecipe(self.crafter, self.tool1, self.tool2, self.cons1, self.cons2, cons4)
         recipe.consume_on_fail = True
 
         result = recipe.craft()
 
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_consumable_missing_message.format(outputs="Result1", missing="cons3"),
-            {"type": "crafting"},
+            text=(
+                recipe.error_consumable_missing_message.format(outputs="Result1", missing="cons3"),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are deleted even though we failed
         self.assertIsNone(self.cons1.pk)
         self.assertIsNone(self.cons2.pk)
         # the extra should also be gone
         self.assertIsNone(cons4.pk)
@@ -313,18 +319,20 @@
 
         wrong = create_object(key="wrong", tags=[("wrongtool", "crafting_tool")], nohome=True)
 
         recipe = _MockRecipe(self.crafter, self.tool1, self.tool2, self.cons1, self.cons2, wrong)
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_tool_excess_message.format(
-                outputs="Result1", excess=wrong.get_display_name(looker=self.crafter)
-            ),
-            {"type": "crafting"},
+            text=(
+                recipe.error_tool_excess_message.format(
+                    outputs="Result1", excess=wrong.get_display_name(looker=self.crafter)
+                ),
+                {"type": "crafting"},
+            )
         )
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         # make sure tools remain
         self.assertIsNotNone(self.tool1.pk)
@@ -338,18 +346,20 @@
 
         recipe = _MockRecipe(
             self.crafter, self.tool1, self.tool2, self.cons1, self.cons2, self.cons3, tool3
         )
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_tool_excess_message.format(
-                outputs="Result1", excess=tool3.get_display_name(looker=self.crafter)
-            ),
-            {"type": "crafting"},
+            text=(
+                recipe.error_tool_excess_message.format(
+                    outputs="Result1", excess=tool3.get_display_name(looker=self.crafter)
+                ),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         # make sure tools remain
@@ -365,18 +375,20 @@
 
         recipe = _MockRecipe(
             self.crafter, self.tool1, self.tool2, self.cons1, self.cons2, self.cons3, cons4
         )
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_consumable_excess_message.format(
-                outputs="Result1", excess=cons4.get_display_name(looker=self.crafter)
-            ),
-            {"type": "crafting"},
+            text=(
+                recipe.error_consumable_excess_message.format(
+                    outputs="Result1", excess=cons4.get_display_name(looker=self.crafter)
+                ),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         self.assertIsNotNone(cons4.pk)
@@ -392,15 +404,15 @@
         recipe = _MockRecipe(
             self.crafter, self.tool1, self.tool2, self.cons1, self.cons2, self.cons3, tool3
         )
         recipe.exact_tools = False
         result = recipe.craft()
         self.assertTrue(result)
         self.crafter.msg.assert_called_with(
-            recipe.success_message.format(outputs="Result1"), {"type": "crafting"}
+            text=(recipe.success_message.format(outputs="Result1"), {"type": "crafting"})
         )
 
         # make sure consumables are gone
         self.assertIsNone(self.cons1.pk)
         self.assertIsNone(self.cons2.pk)
         self.assertIsNone(self.cons3.pk)
         # make sure tools remain
@@ -415,15 +427,15 @@
         recipe = _MockRecipe(
             self.crafter, self.tool1, self.tool2, self.cons1, self.cons2, self.cons3, cons4
         )
         recipe.exact_consumables = False
         result = recipe.craft()
         self.assertTrue(result)
         self.crafter.msg.assert_called_with(
-            recipe.success_message.format(outputs="Result1"), {"type": "crafting"}
+            text=(recipe.success_message.format(outputs="Result1"), {"type": "crafting"})
         )
 
         # make sure consumables are gone
         self.assertIsNone(self.cons1.pk)
         self.assertIsNone(self.cons2.pk)
         self.assertIsNone(self.cons3.pk)
         # make sure tools remain
@@ -435,18 +447,20 @@
         recipe = _MockRecipe(
             self.crafter, self.tool2, self.tool1, self.cons1, self.cons2, self.cons3
         )
         recipe.exact_tool_order = True
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_tool_order_message.format(
-                outputs="Result1", missing=self.tool2.get_display_name(looker=self.crafter)
-            ),
-            {"type": "crafting"},
+            text=(
+                recipe.error_tool_order_message.format(
+                    outputs="Result1", missing=self.tool2.get_display_name(looker=self.crafter)
+                ),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         # make sure tools remain
@@ -458,18 +472,20 @@
         recipe = _MockRecipe(
             self.crafter, self.tool1, self.tool2, self.cons3, self.cons2, self.cons1
         )
         recipe.exact_consumable_order = True
         result = recipe.craft()
         self.assertFalse(result)
         self.crafter.msg.assert_called_with(
-            recipe.error_consumable_order_message.format(
-                outputs="Result1", missing=self.cons3.get_display_name(looker=self.crafter)
-            ),
-            {"type": "crafting"},
+            text=(
+                recipe.error_consumable_order_message.format(
+                    outputs="Result1", missing=self.cons3.get_display_name(looker=self.crafter)
+                ),
+                {"type": "crafting"},
+            )
         )
 
         # make sure consumables are still there
         self.assertIsNotNone(self.cons1.pk)
         self.assertIsNotNone(self.cons2.pk)
         self.assertIsNotNone(self.cons3.pk)
         # make sure tools remain
```

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/gendersub/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/gendersub/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/gendersub/gendersub.py` & `evennia-4.1.0/evennia/contrib/game_systems/gendersub/gendersub.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/gendersub/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/gendersub/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Test gendersub contrib.
 
 """
 
-
 from mock import patch
 
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 from evennia.utils.create import create_object
 
 from . import gendersub
```

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/mail/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/mail/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/mail/mail.py` & `evennia-4.1.0/evennia/contrib/game_systems/mail/mail.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/mail/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/mail/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/multidescer/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/multidescer/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/multidescer/multidescer.py` & `evennia-4.1.0/evennia/contrib/game_systems/multidescer/multidescer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class and add a line `self.add(CmdMultiDesc())` to the end
 of it.
 
 Reload the server and you should have the +desc command available (it
 will replace the default `desc` command).
 
 """
+
 import re
 
 from evennia import default_cmds
 from evennia.utils.eveditor import EvEditor
 from evennia.utils.utils import crop
 
 # regex for the set functionality
```

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/multidescer/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/multidescer/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/puzzles/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/puzzles/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/puzzles/puzzles.py` & `evennia-4.1.0/evennia/contrib/game_systems/puzzles/puzzles.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/puzzles/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/puzzles/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/README.md` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_basic.py` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_basic.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_equip.py` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_equip.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_items.py` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_items.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_magic.py` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_magic.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tb_range.py` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_range.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/game_systems/turnbattle/tests.py` & `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/extended_room/README.md` & `evennia-4.1.0/evennia/contrib/grid/extended_room/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/extended_room/extended_room.py` & `evennia-4.1.0/evennia/contrib/grid/extended_room/extended_room.py`

 * *Files 0% similar despite different names*

```diff
@@ -819,15 +819,14 @@
             caller.msg(
                 "You don't have permission to edit the description "
                 f"of {target.get_display_name(caller)}."
             )
 
 
 class CmdExtendedRoomDetail(default_cmds.MuxCommand):
-
     """
     sets a detail on a room
 
     Usage:
         @detail[/del] <key> [= <description>]
         @detail <key>;<alias>;... = description
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/extended_room/tests.py` & `evennia-4.1.0/evennia/contrib/grid/extended_room/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 Testing of ExtendedRoom contrib
 
 """
 
 import datetime
 
 from django.conf import settings
-from evennia import create_object
-from evennia.utils.test_resources import BaseEvenniaCommandTest, EvenniaTestCase
 from mock import Mock, patch
 from parameterized import parameterized
 
+from evennia import create_object
+from evennia.utils.test_resources import BaseEvenniaCommandTest, EvenniaTestCase
+
 from . import extended_room
 
 
 def _get_timestamp(season, time_of_day):
     """
     Utility to get a timestamp for a given season and time of day.
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/ingame_map_display/README.md` & `evennia-4.1.0/evennia/contrib/grid/ingame_map_display/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py` & `evennia-4.1.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 BASIC_MAP_SIZE = 5
 
 This changes the default map width/height. 2-5 for most clients is sensible.
 
 If you don't want the player to be able to specify the size of the map, ignore any
 arguments passed into the Map command.
 """
+
 import time
 
 from django.conf import settings
 
 from evennia import CmdSet
 from evennia.commands.default.muxcommand import MuxCommand
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/ingame_map_display/tests.py` & `evennia-4.1.0/evennia/contrib/grid/ingame_map_display/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Tests of ingame_map_display.
 
 """
 
-
 from typeclasses import exits, rooms
 
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 from evennia.utils.create import create_object
 
 from . import ingame_map_display
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/mapbuilder/README.md` & `evennia-4.1.0/evennia/contrib/grid/mapbuilder/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/mapbuilder/mapbuilder.py` & `evennia-4.1.0/evennia/contrib/grid/mapbuilder/mapbuilder.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/mapbuilder/tests.py` & `evennia-4.1.0/evennia/contrib/grid/mapbuilder/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/simpledoor/README.md` & `evennia-4.1.0/evennia/contrib/grid/simpledoor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/simpledoor/simpledoor.py` & `evennia-4.1.0/evennia/contrib/grid/simpledoor/simpledoor.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/simpledoor/tests.py` & `evennia-4.1.0/evennia/contrib/grid/simpledoor/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Tests of simpledoor.
 
 """
 
-
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 
 from . import simpledoor
 
 
 class TestSimpleDoor(BaseEvenniaCommandTest):
     def test_cmdopen(self):
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/slow_exit/README.md` & `evennia-4.1.0/evennia/contrib/grid/slow_exit/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/slow_exit/slow_exit.py` & `evennia-4.1.0/evennia/contrib/grid/slow_exit/slow_exit.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/slow_exit/tests.py` & `evennia-4.1.0/evennia/contrib/grid/slow_exit/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/wilderness/README.md` & `evennia-4.1.0/evennia/contrib/grid/wilderness/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/wilderness/tests.py` & `evennia-4.1.0/evennia/contrib/grid/wilderness/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/wilderness/wilderness.py` & `evennia-4.1.0/evennia/contrib/grid/wilderness/wilderness.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/README.md` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/commands.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/example.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/example.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/launchcmd.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/launchcmd.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/prototypes.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/prototypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     {'prototype_parent': 'xyz_room', ...}
 
 and/or
 
     {'prototype_parent': 'xyz_exit', ...}
 
 """
+
 from django.conf import settings
 
 try:
     room_override = settings.XYZROOM_PROTOTYPE_OVERRIDE
 except AttributeError:
     room_override = {}
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/tests.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 
 Tests for the XYZgrid system.
 
 """
+
 from random import randint
 from unittest import mock
 
 from django.test import TestCase
-from evennia.utils.test_resources import (BaseEvenniaCommandTest,
-                                          BaseEvenniaTest)
 from parameterized import parameterized
 
+from evennia.utils.test_resources import BaseEvenniaCommandTest, BaseEvenniaTest
+
 from . import commands, xymap, xymap_legend, xyzgrid, xyzroom
 
 MAP1 = """
 
  + 0 1 2
 
  1 #-#
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/utils.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/xymap.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 the LEGEND dict, mapping them to a particular character symbol. A `MapNode` can only be added
 on an even XY coordinate while `MapLink`s can be added anywhere on the xygrid.
 
 See `./example.py` for a full grid example.
 
 ----
 """
+
 import pickle
 from collections import defaultdict
 from os import mkdir
 from os.path import isdir, isfile
 from os.path import join as pathjoin
 
 try:
@@ -104,14 +105,15 @@
     from scipy.sparse.csgraph import dijkstra
 except ImportError as err:
     raise ImportError(
         f"{err}\nThe XYZgrid contrib requires "
         "the SciPy package. Install with `pip install scipy'."
     )
 from django.conf import settings
+
 from evennia.prototypes import prototypes as protlib
 from evennia.prototypes.spawner import flatten_prototype
 from evennia.utils import logger
 from evennia.utils.utils import is_iter, mod_import, variable_from_module
 
 from . import xymap_legend
 from .utils import BIGVAL, MapError, MapParserError
@@ -168,14 +170,15 @@
         '''
 
     So origo (0,0) is in the bottom-left and north is +y movement, south is -y movement
     while east/west is +/- x movement as expected. Adding numbers to axes is optional
     but recommended for readability!
 
     """
+
     mapcorner_symbol = "+"
     max_pathfinding_length = 500
     empty_symbol = " "
     # we normally only accept one single character for the legend key
     legend_key_exceptions = "\\"
 
     def __init__(self, map_module_or_dict, Z="map", xyzgrid=None):
@@ -471,18 +474,18 @@
 
                     # save the node to several different maps for different uses
                     # in both coordinate systems
                     iX, iY = ix // 2, iy // 2
                     max_X, max_Y = max(max_X, iX), max(max_Y, iY)
                     node_index += 1
 
-                    xygrid[ix][iy] = XYgrid[iX][iY] = node_index_map[
-                        node_index
-                    ] = mapnode_or_link_class(
-                        x=ix, y=iy, Z=self.Z, node_index=node_index, symbol=char, xymap=self
+                    xygrid[ix][iy] = XYgrid[iX][iY] = node_index_map[node_index] = (
+                        mapnode_or_link_class(
+                            x=ix, y=iy, Z=self.Z, node_index=node_index, symbol=char, xymap=self
+                        )
                     )
 
                 else:
                     # we have a link at this xygrid position (this is ok everywhere)
                     xygrid[ix][iy] = mapnode_or_link_class(
                         x=ix, y=iy, Z=self.Z, symbol=char, xymap=self
                     )
@@ -664,16 +667,15 @@
 
         Returns:
             list: A list of nodes that were spawned.
 
         """
         global _XYZROOMCLASS
         if not _XYZROOMCLASS:
-            from evennia.contrib.grid.xyzgrid.xyzroom import \
-                XYZRoom as _XYZROOMCLASS
+            from evennia.contrib.grid.xyzgrid.xyzroom import XYZRoom as _XYZROOMCLASS
         x, y = xy
         wildcard = "*"
         spawned = []
 
         # find existing nodes, in case some rooms need to be removed
         map_coords = [
             (node.X, node.Y)
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/xymap_legend.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap_legend.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         f"{err}\nThe XYZgrid contrib requires the SciPy package. Install with `pip install scipy'."
     )
 
 import uuid
 from collections import defaultdict
 
 from django.core import exceptions as django_exceptions
+
 from evennia.prototypes import spawner
 from evennia.utils.utils import class_from_module
 
-from .utils import (BIGVAL, MAPSCAN, REVERSE_DIRECTIONS, MapError,
-                    MapParserError)
+from .utils import BIGVAL, MAPSCAN, REVERSE_DIRECTIONS, MapError, MapParserError
 
 NodeTypeclass = None
 ExitTypeclass = None
 
 
 UUID_XYZ_NAMESPACE = uuid.uuid5(uuid.UUID(int=0), "xyzgrid")
 
@@ -840,14 +840,15 @@
         -o-   - w-e pass straight through, other link is sw-s
         /|
 
         -o    - invalid; impossible to know which input goes to which output
         /|
 
     """
+
     multilink = True
 
     def get_direction(self, start_direction):
         """
         Dynamically determine the direction based on a source direction and grid topology.
 
         """
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/xyzgrid.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzgrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 - Building new rooms/exits from scratch based on one or more Maps.
 - Updating the rooms/exits tied to an existing Map when the Map string
   of that map changes.
 - Fascilitate communication between the in-game entities and their Map.
 
 
 """
+
 from evennia.scripts.scripts import DefaultScript
 from evennia.utils import logger
 from evennia.utils.utils import variable_from_module
 
 from .xymap import XYMap
 from .xyzroom import XYZExit, XYZRoom
```

### Comparing `evennia-4.0.0/evennia/contrib/grid/xyzgrid/xyzroom.py` & `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzroom.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/buffs/README.md` & `evennia-4.1.0/evennia/contrib/rpg/buffs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/buffs/buff.py` & `evennia-4.1.0/evennia/contrib/rpg/buffs/buff.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 this instance, rather than directly manipulating the buff cache on the object. You can modify a buff's cache through various handler
 methods instead.
 
 You can see all the features of the `BaseBuff` class below, or browse `samplebuffs.py` to see how to create some common buffs. Buffs have
 many attributes and hook methods you can overload to create complex, interrelated buffs.
 
 """
+
 import time
 from random import random
 
 from evennia import Command
 from evennia.server import signals
 from evennia.typeclasses.attributes import AttributeProperty
 from evennia.utils import search, utils
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/buffs/samplebuffs.py` & `evennia-4.1.0/evennia/contrib/rpg/buffs/samplebuffs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/buffs/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/buffs/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests for the buff system contrib
 """
+
 from unittest.mock import Mock, call, patch
 
 from evennia import DefaultObject, create_object
 from evennia.contrib.rpg.buffs import buff
 from evennia.utils import create
 from evennia.utils.test_resources import EvenniaTest
 from evennia.utils.utils import lazy_property
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/character_creator/README.md` & `evennia-4.1.0/evennia/contrib/rpg/character_creator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/character_creator/character_creator.py` & `evennia-4.1.0/evennia/contrib/rpg/character_creator/character_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 In order to use the contrib, you will need to create your own chargen
 EvMenu. The included `example_menu.py` gives a number of useful techniques
 and examples, including how to allow players to choose and confirm
 character names from within the menu.
 
 """
+
 import string
 from random import choices
 
 from django.conf import settings
 
 from evennia import DefaultAccount
 from evennia.commands.default.muxcommand import MuxAccountCommand
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/character_creator/example_menu.py` & `evennia-4.1.0/evennia/contrib/rpg/character_creator/example_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/character_creator/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/character_creator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/dice/README.md` & `evennia-4.1.0/evennia/contrib/rpg/dice/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/dice/dice.py` & `evennia-4.1.0/evennia/contrib/rpg/dice/dice.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 If your system generates the dice dynamically you can also enter each part
 of the roll separately:
 
     dice.roll(3, 10, ("+", 2))  # 3d10 + 2
 
 
 """
+
 import re
 from ast import literal_eval
 from random import randint
 
 from evennia import CmdSet, default_cmds
 from evennia.utils.utils import simple_eval
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/dice/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/dice/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/health_bar/README.md` & `evennia-4.1.0/evennia/contrib/rpg/health_bar/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/health_bar/health_bar.py` & `evennia-4.1.0/evennia/contrib/rpg/health_bar/health_bar.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/health_bar/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/health_bar/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/llm/README.md` & `evennia-4.1.0/evennia/contrib/rpg/llm/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/llm/llm_client.py` & `evennia-4.1.0/evennia/contrib/rpg/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/llm/llm_npc.py` & `evennia-4.1.0/evennia/contrib/rpg/llm/llm_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/llm/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/llm/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/rpsystem/README.md` & `evennia-4.1.0/evennia/contrib/rpg/rpsystem/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/rpsystem/__init__.py` & `evennia-4.1.0/evennia/contrib/rpg/rpsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/rpsystem/rplanguage.py` & `evennia-4.1.0/evennia/contrib/rpg/rpsystem/rplanguage.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 The `auto_translations` keyword is useful, this accepts either a
 list or a path to a file of words (one per line) to automatically
 create fixed translations for according to the grammatical rules.
 This allows to quickly build a large corpus of translated words
 that never change (if this is desired).
 
 """
+
 import re
 from collections import defaultdict
 from random import choice, randint
 
 from evennia import DefaultScript
 from evennia.utils import logger
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/rpsystem/rpsystem.py` & `evennia-4.1.0/evennia/contrib/rpg/rpsystem/rpsystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,27 +144,33 @@
        Change `class Object(DefaultObject):` to
        `class Object(ContribRPObject):`
 4. Reload the server (`reload` or from console: "evennia reload")
 5. Force typeclass updates as required. Example for your character:
        `type/reset/force me = typeclasses.characters.Character`
 
 """
+
 import re
 from collections import defaultdict
 from string import punctuation
 
 import inflect
 from django.conf import settings
+
 from evennia.commands.cmdset import CmdSet
 from evennia.commands.command import Command
 from evennia.objects.models import ObjectDB
 from evennia.objects.objects import DefaultCharacter, DefaultObject
 from evennia.utils import ansi, logger
-from evennia.utils.utils import (iter_to_str, lazy_property, make_iter,
-                                 variable_from_module)
+from evennia.utils.utils import (
+    iter_to_str,
+    lazy_property,
+    make_iter,
+    variable_from_module,
+)
 
 _INFLECT = inflect.engine()
 
 _AT_SEARCH_RESULT = variable_from_module(*settings.SEARCH_AT_RESULT.rsplit(".", 1))
 # ------------------------------------------------------------
 # Emote parser
 # ------------------------------------------------------------
@@ -1273,14 +1279,16 @@
 
 
 class RPSystemCmdSet(CmdSet):
     """
     Mix-in for adding rp-commands to default cmdset.
     """
 
+    key = "rpsystem_cmdset"
+
     def at_cmdset_creation(self):
         self.add(CmdEmote())
         self.add(CmdSay())
         self.add(CmdSdesc())
         self.add(CmdPose())
         self.add(CmdRecog())
         self.add(CmdMask())
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/rpsystem/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/rpsystem/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Tests for RP system
 
 """
+
 import time
 
 from anything import Anything
+
 from evennia import DefaultObject, create_object, default_cmds
+from evennia.commands.default import building
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 from evennia.utils.test_resources import BaseEvenniaTest
 
 from . import rplanguage, rpsystem
 
 mtrans = {"testing": "1", "is": "2", "a": "3", "human": "4"}
 atrans = ["An", "automated", "advantageous", "repeatable", "faster"]
@@ -409,18 +412,27 @@
 
         # check locations and contents
         self.assertEqual(self.char1.location, self.room1)
         self.assertTrue(set(self.room1.contents).intersection(set([mushroom1, mushroom2])))
 
         expected_first_call = [
             "More than one match for 'Mushroom' (please narrow target):",
-            f" Mushroom-1 []",
-            f" Mushroom-2 []",
+            f" Mushroom-1",
+            f" Mushroom-2",
         ]
-
         self.call(default_cmds.CmdLook(), "Mushroom", "\n".join(expected_first_call))  # PASSES
 
         expected_second_call = f"Mushroom(#{mushroom1.id})\nThe first mushroom is brown."
         self.call(default_cmds.CmdLook(), "Mushroom-1", expected_second_call)  # FAILS
 
         expected_third_call = f"Mushroom(#{mushroom2.id})\nThe second mushroom is red."
         self.call(default_cmds.CmdLook(), "Mushroom-2", expected_third_call)  # FAILS
+
+        expected_fourth_call = "Alias(es) for 'Mushroom' set to 'fungus'."
+        self.call(building.CmdSetObjAlias(), "Mushroom-1 = fungus", expected_fourth_call)  # PASSES
+
+        expected_fifth_call = [
+            "More than one match for 'Mushroom' (please narrow target):",
+            f" Mushroom-1 [fungus]",
+            f" Mushroom-2",
+        ]
+        self.call(default_cmds.CmdLook(), "Mushroom", "\n".join(expected_fifth_call))  # PASSES
```

### Comparing `evennia-4.0.0/evennia/contrib/rpg/traits/README.md` & `evennia-4.1.0/evennia/contrib/rpg/traits/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/traits/tests.py` & `evennia-4.1.0/evennia/contrib/rpg/traits/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/rpg/traits/traits.py` & `evennia-4.1.0/evennia/contrib/rpg/traits/traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,14 @@
 
 ```
 
 ----
 
 """
 
-
 from functools import total_ordering
 from time import time
 
 from django.conf import settings
 
 from evennia.utils import logger
 from evennia.utils.dbserialize import _SaverDict
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/README.md` & `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev` & `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev` & `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py` & `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py` & `evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 To test, use
   script me = tutorial_examples.bodyfunctions.BodyFunctions
 
 The script will only send messages to the object it is stored on, so
 make sure to put it on yourself or you won't see any messages!
 
 """
+
 import random
 
 from evennia import DefaultScript
 
 
 class BodyFunctions(DefaultScript):
     """
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/bodyfunctions/tests.py` & `evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/tests.py`

 * *Files identical despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tests for the bodyfunctions.
 
 """
+
 from mock import Mock, patch
 
 from evennia.utils.test_resources import BaseEvenniaTest
 
 from .bodyfunctions import BodyFunctions
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/README.md` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/ai.py` & `evennia-4.1.0/evennia/server/game_index_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,232 +1,179 @@
 """
-NPC AI module for EvAdventure (WIP)
-
-This implements a simple state machine for NPCs to follow.
-
-The AIHandler class is stored on the NPC object and is queried by the game loop to determine what
-the NPC does next. This leads to the calling of one of the relevant state methods on the NPC, which
-is where the actual logic for the NPC's behaviour is implemented. Each state is responsible for
-switching to the next state when the conditions are met.
-
-The AIMixin class is a mixin that can be added to any object that needs AI. It provides the `.ai`
-reference to the AIHandler and a few basic `ai_*` methods for basic AI behaviour.
-
-
-Example usage:
-
-```python
-from evennia import create_object
-from .npc import EvadventureNPC
-from .ai import AIMixin
-
-class MyMob(AIMixin, EvadventureNPC):
-    pass
-
-mob = create_object(MyMob, key="Goblin", location=room)
-
-mob.ai.set_state("patrol")
-
-# tick the ai whenever needed
-mob.ai.run()
-
-```
+The client for sending data to the Evennia Game Index
 
 """
 
-import random
-
-from evennia.utils.logger import log_trace
-from evennia.utils.utils import lazy_property
+import platform
+import urllib.error
+import urllib.parse
+import urllib.request
+
+import django
+from django.conf import settings
+from twisted.internet import defer, protocol, reactor
+from twisted.internet.defer import inlineCallbacks
+from twisted.web.client import Agent, HTTPConnectionPool, _HTTP11ClientFactory
+from twisted.web.http_headers import Headers
+from twisted.web.iweb import IBodyProducer
+from zope.interface import implementer
+
+import evennia
+from evennia.accounts.models import AccountDB
+from evennia.utils import get_evennia_version, logger
+
+_EGI_HOST = "http://evennia-game-index.appspot.com"
+_EGI_REPORT_PATH = "/api/v1/game/check_in"
+
+
+class EvenniaGameIndexClient:
+    """
+    This client class is used for gathering and sending game details to the
+    Evennia Game Index. Since EGI is in the early goings, this isn't
+    incredibly configurable as far as to what is being sent.
+    """
+
+    def __init__(self, on_bad_request=None):
+        """
+        on_bad_request (callable, optional): Callable to trigger when a bad request was sent.
+
+        """
+        self.report_host = _EGI_HOST
+        self.report_path = _EGI_REPORT_PATH
+        self.report_url = self.report_host + self.report_path
+        self.logged_first_connect = False
+
+        self._on_bad_request = on_bad_request
+        # Oh, the humanity. Silence the factory start/stop messages.
+        self._conn_pool = HTTPConnectionPool(reactor)
+        self._conn_pool._factory = QuietHTTP11ClientFactory
+
+    @inlineCallbacks
+    def send_game_details(self):
+        """
+        This is where the magic happens. Send details about the game to the
+        Evennia Game Index.
+        """
+        status_code, response_body = yield self._form_and_send_request()
+        if status_code == 200:
+            if not self.logged_first_connect:
+                logger.log_infomsg("Successfully sent game details to Evennia Game Index.")
+                self.logged_first_connect = True
+            return
+        # At this point, either EGD is having issues or the payload we sent
+        # is improperly formed (probably due to mis-configuration).
+        logger.log_errmsg(
+            "Failed to send game details to Evennia Game Index. HTTP "
+            "status code was %s. Message was: %s" % (status_code, response_body)
+        )
 
-from .enums import Ability
+        if status_code == 400 and self._on_bad_request:
+            # Improperly formed request. Defer to the callback as far as what
+            # to do. Probably not a great idea to continue attempting to send
+            # to EGD, though.
+            self._on_bad_request()
+
+    def _form_and_send_request(self):
+        """
+        Build the request to send to the index.
+
+        """
+        agent = Agent(reactor, pool=self._conn_pool)
+        headers = {
+            b"User-Agent": [b"Evennia Game Index Client"],
+            b"Content-Type": [b"application/x-www-form-urlencoded"],
+        }
+        egi_config = settings.GAME_INDEX_LISTING
+        # We are using `or` statements below with dict.get() to avoid sending
+        # stringified 'None' values to the server.
+        try:
+            values = {
+                # Game listing stuff
+                "game_name": egi_config.get("game_name", settings.SERVERNAME),
+                "game_status": egi_config["game_status"],
+                "game_website": egi_config.get("game_website", ""),
+                "short_description": egi_config["short_description"],
+                "long_description": egi_config.get("long_description", ""),
+                "listing_contact": egi_config["listing_contact"],
+                # How to play
+                "telnet_hostname": egi_config.get("telnet_hostname", ""),
+                "telnet_port": egi_config.get("telnet_port", ""),
+                "web_client_url": egi_config.get("web_client_url", ""),
+                # Game stats
+                "connected_account_count": evennia.SESSION_HANDLER.account_count(),
+                "total_account_count": AccountDB.objects.num_total_accounts() or 0,
+                # System info
+                "evennia_version": get_evennia_version(),
+                "python_version": platform.python_version(),
+                "django_version": django.get_version(),
+                "server_platform": platform.platform(),
+            }
+        except KeyError as err:
+            raise KeyError(f"Error loading GAME_INDEX_LISTING: {err}")
+
+        data = urllib.parse.urlencode(values)
+
+        d = agent.request(
+            b"POST",
+            bytes(self.report_url, "utf-8"),
+            headers=Headers(headers),
+            bodyProducer=StringProducer(data),
+        )
 
+        d.addCallback(self.handle_egd_response)
+        return d
 
-class AIHandler:
-    def __init__(self, obj):
-        self.obj = obj
-        self.ai_state = obj.attributes.get("ai_state", category="ai_state", default="idle")
+    def handle_egd_response(self, response):
+        if 200 <= response.code < 300:
+            d = defer.succeed((response.code, "OK"))
+        else:
+            # Go through the horrifying process of getting the response body
+            # out of Twisted's plumbing.
+            d = defer.Deferred()
+            response.deliverBody(SimpleResponseReceiver(response.code, d))
+        return d
 
-    def set_state(self, state):
-        self.ai_state = state
-        self.obj.attributes.add("ai_state", state, category="ai_state")
 
-    def get_state(self):
-        return self.ai_state
+class SimpleResponseReceiver(protocol.Protocol):
+    """
+    Used for pulling the response body out of an HTTP response.
+    """
 
-    def get_targets(self):
-        """
-        Get a list of potential targets for the NPC to attack
-        """
-        return [obj for obj in self.obj.location.contents if hasattr(obj, "is_pc") and obj.is_pc]
+    def __init__(self, status_code, d):
+        self.status_code = status_code
+        self.buf = ""
+        self.d = d
 
-    def get_traversable_exits(self, exclude_destination=None):
-        return [
-            exi
-            for exi in self.obj.location.exits
-            if exi.destination != exclude_destination and exi.access(self, "traverse")
-        ]
+    def dataReceived(self, data):
+        self.buf += data
 
-    def random_probability(self, probabilities):
-        """
-        Given a dictionary of probabilities, return the key of the chosen probability.
+    def connectionLost(self, reason=protocol.connectionDone):
+        self.d.callback((self.status_code, self.buf))
 
-        """
-        r = random.random()
-        # sort probabilities from higheest to lowest, making sure to normalize them 0..1
-        prob_total = sum(probabilities.values())
-        sorted_probs = sorted(
-            ((key, prob / prob_total) for key, prob in probabilities.items()),
-            key=lambda x: x[1],
-            reverse=True,
-        )
-        total = 0
-        for key, prob in sorted_probs:
-            total += prob
-            if r <= total:
-                return key
 
-    def run(self):
-        try:
-            state = self.get_state()
-            getattr(self.obj, f"ai_{state}")()
-        except Exception:
-            log_trace(f"AI error in {self.obj.name} (running state: {state})")
-
-
-class AIMixin:
+@implementer(IBodyProducer)
+class StringProducer:
     """
-    Mixin for adding AI to an Object. This is a simple state machine. Just add more `ai_*` methods
-    to the object to make it do more things.
-
+    Used for feeding a request body to the tx HTTP client.
     """
 
-    # combat probabilities should add up to 1.0
-    combat_probabilities = {
-        "hold": 0.1,
-        "attack": 0.9,
-        "stunt": 0.0,
-        "item": 0.0,
-        "flee": 0.0,
-    }
-
-    @lazy_property
-    def ai(self):
-        return AIHandler(self)
-
-    def ai_idle(self):
-        pass
+    def __init__(self, body):
+        self.body = bytes(body, "utf-8")
+        self.length = len(body)
 
-    def ai_attack(self):
-        pass
+    def startProducing(self, consumer):
+        consumer.write(self.body)
+        return defer.succeed(None)
 
-    def ai_patrol(self):
+    def pauseProducing(self):
         pass
 
-    def ai_flee(self):
+    def stopProducing(self):
         pass
 
 
-class IdleMobMixin(AIMixin):
+class QuietHTTP11ClientFactory(_HTTP11ClientFactory):
     """
-    A simple mob that understands AI commands, but does nothing.
-
+    Silences the obnoxious factory start/stop messages in the default client.
     """
 
-    def ai_idle(self):
-        pass
-
-
-class AggressiveMobMixin(AIMixin):
-    """
-    A simple aggressive mob that can roam, attack and flee.
-
-    """
-
-    combat_probabilities = {
-        "hold": 0.0,
-        "attack": 0.85,
-        "stunt": 0.05,
-        "item": 0.0,
-        "flee": 0.05,
-    }
-
-    def ai_idle(self):
-        """
-        Do nothing, but switch to attack state if a target is found.
-
-        """
-        if self.ai.get_targets():
-            self.ai.set_state("attack")
-
-    def ai_attack(self):
-        """
-        Manage the attack/combat state of the mob.
-
-        """
-        if combathandler := self.nbd.combathandler:
-            # already in combat
-            allies, enemies = combathandler.get_sides(self)
-            action = self.ai.random_probability(self.combat_probabilities)
-
-            match action:
-                case "hold":
-                    combathandler.queue_action({"key": "hold"})
-                case "attack":
-                    combathandler.queue_action({"key": "attack", "target": random.choice(enemies)})
-                case "stunt":
-                    # choose a random ally to help
-                    combathandler.queue_action(
-                        {
-                            "key": "stunt",
-                            "recipient": random.choice(allies),
-                            "advantage": True,
-                            "stunt": Ability.STR,
-                            "defense": Ability.DEX,
-                        }
-                    )
-                case "item":
-                    # use a random item on a random ally
-                    target = random.choice(allies)
-                    valid_items = [item for item in self.contents if item.at_pre_use(self, target)]
-                    combathandler.queue_action(
-                        {"key": "item", "item": random.choice(valid_items), "target": target}
-                    )
-                case "flee":
-                    self.ai.set_state("flee")
-
-        if not (targets := self.ai.get_targets()):
-            self.ai.set_state("patrol")
-        else:
-            target = random.choice(targets)
-            self.execute_cmd(f"attack {target.key}")
-
-    def ai_patrol(self):
-        """
-        Patrol, moving randomly to a new room. If a target is found, switch to attack state.
-
-        """
-        if targets := self.ai.get_targets():
-            self.ai.set_state("attack")
-            self.execute_cmd(f"attack {random.choice(targets).key}")
-        else:
-            exits = self.ai.get_traversable_exits()
-            if exits:
-                exi = random.choice(exits)
-                self.execute_cmd(f"{exi.key}")
-
-    def ai_flee(self):
-        """
-        Flee from the current room, avoiding going back to the room from which we came. If no exits
-        are found, switch to patrol state.
-
-        """
-        current_room = self.location
-        past_room = self.attributes.get("past_room", category="ai_state", default=None)
-        exits = self.ai.get_traversable_exits(exclude_destination=past_room)
-        if exits:
-            self.attributes.set("past_room", current_room, category="ai_state")
-            exi = random.choice(exits)
-            self.execute_cmd(f"{exi.key}")
-        else:
-            # if in a dead end, patrol will allow for backing out
-            self.ai.set_state("patrol")
+    noisy = False
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/build_techdemo.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/build_techdemo.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/characters.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/chargen.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/chargen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 EvAdventure character generation.
 
 """
+
 from django.conf import settings
 
 from evennia.objects.models import ObjectDB
 from evennia.prototypes.spawner import spawn
 from evennia.utils.create import create_object
 from evennia.utils.evmenu import EvMenu
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/combat_base.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_base.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 Unlike in twitch-like combat, there is no movement while in turn-based combat. Fleeing is a select
 action that takes several vulnerable turns to complete.
 
 ----
 
 """
 
-
 import random
 from collections import defaultdict
 
 from evennia import AttributeProperty, CmdSet, Command, EvMenu
 from evennia.utils import inherits_from, list_to_string
 
 from .characters import EvAdventureCharacter
@@ -839,9 +838,11 @@
 
 
 class TurnCombatCmdSet(CmdSet):
     """
     CmdSet for the turn-based combat.
     """
 
+    key = "turncombat_cmdset"
+
     def at_cmdset_creation(self):
         self.add(CmdTurnAttack())
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/combat_twitch.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 EvAdventure Twitch-based combat
 
 This implements a 'twitch' (aka DIKU or other traditional muds) style of MUD combat.
 
 ----
 
 """
+
 from evennia import AttributeProperty, CmdSet, default_cmds
 from evennia.commands.command import Command, InterruptCommand
 from evennia.utils.utils import (
     display_len,
     inherits_from,
     list_to_string,
     pad,
@@ -556,22 +557,26 @@
 
 
 class TwitchCombatCmdSet(CmdSet):
     """
     Add to character, to be able to attack others in a twitch-style way.
     """
 
+    key = "twitch_combat_cmdset"
+
     def at_cmdset_creation(self):
         self.add(CmdAttack())
         self.add(CmdHold())
         self.add(CmdStunt())
         self.add(CmdUseItem())
         self.add(CmdWield())
 
 
 class TwitchLookCmdSet(CmdSet):
     """
     This will be added/removed dynamically when in combat.
     """
 
+    key = "twitch_look_cmdset"
+
     def at_cmdset_creation(self):
         self.add(CmdLook())
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/commands.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/dungeon.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/dungeon.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,50 +74,49 @@
     "southeast": (1, -1),
     "southwest": (-1, -1),
     "northwest": (-1, 1),
 }
 
 
 # --------------------------------------------------
-# Dungeon orchestrator and room / exits
+# Dungeon branch and room / exits
 # --------------------------------------------------
 
 
 class EvAdventureDungeonRoom(EvAdventureRoom):
     """
     Dangerous dungeon room.
 
     """
 
     allow_combat = AttributeProperty(True, autocreate=False)
     allow_death = AttributeProperty(True, autocreate=False)
 
     # dungeon generation attributes; set when room is created
-    back_exit = AttributeProperty(None, autocreate=False)
-    dungeon_orchestrator = AttributeProperty(None, autocreate=False)
+    dungeon_branch = AttributeProperty(None, autocreate=False)
     xy_coords = AttributeProperty(None, autocreate=False)
 
-    @property
-    def is_room_clear(self):
-        return not bool(self.tags.get("not_clear", category="dungeon_room"))
-
-    def clear_room(self):
-        self.tags.remove("not_clear", category="dungeon_room")
-
     def at_object_creation(self):
         """
         Set the `not_clear` tag on the room. This is removed when the room is
         'cleared', whatever that means for each room.
 
         We put this here rather than in the room-creation code so we can override
         easier (for example we may want an empty room which auto-clears).
 
         """
         self.tags.add("not_clear", category="dungeon_room")
 
+    def clear_room(self):
+        self.tags.remove("not_clear", category="dungeon_room")
+
+    @property
+    def is_room_clear(self):
+        return not bool(self.tags.get("not_clear", category="dungeon_room"))
+
     def get_display_footer(self, looker, **kwargs):
         """
         Show if the room is 'cleared' or not as part of its description.
 
         """
         if self.is_room_clear:
             return ""
@@ -136,44 +135,42 @@
         We want to block progressing forward unless the room is clear.
 
         """
         self.locks.add("traverse:not objloctag(not_clear, dungeon_room)")
 
     def at_traverse(self, traversing_object, target_location, **kwargs):
         """
-        Called when traversing. `target_location` will be None if the
-        target was not yet created. It checks the current location to get the
-        dungeon-orchestrator in use.
+        Called when traversing. `target_location` will be pointing back to ourselves if the target
+        was not yet created. It checks the current location to get the dungeon-branch in use.
 
         """
+        dungeon_branch = self.location.db.dungeon_branch
         if target_location == self.location:
-            self.destination = target_location = self.location.db.dungeon_orchestrator.new_room(
-                self
-            )
-            if self.id in self.location.dungeon_orchestrator.unvisited_exits:
-                self.location.dungeon_orchestrator.unvisited_exits.remove(self.id)
+            # destination points back to us - create a new room
+            self.destination = target_location = dungeon_branch.new_room(self)
+            dungeon_branch.register_exit_traversed(self)
 
         super().at_traverse(traversing_object, target_location, **kwargs)
 
     def at_failed_traverse(self, traversing_object, **kwargs):
         """
         Called when failing to traverse.
 
         """
         traversing_object.msg("You can't get through this way yet!")
 
 
-def room_generator(dungeon_orchestrator, depth, coords):
+def room_generator(dungeon_branch, depth, coords):
     """
     Plugin room generator
 
     This default one returns the same empty room.
 
     Args:
-        dungeon_orchestrator (EvAdventureDungeonOrchestrator): The current orchestrator.
+        dungeon_branch (EvAdventureDungeonBranch): The current dungeon branch.
         depth (int): The 'depth' of the dungeon (radial distance from start room) this
             new room will be placed at.
         coords (tuple): The `(x,y)` coords that the new room will be created at.
 
     """
     room_typeclass = EvAdventureDungeonRoom
 
@@ -194,43 +191,42 @@
 
     new_room = create.create_object(
         room_typeclass,
         key=key,
         attributes=(
             ("desc", desc),
             ("xy_coords", coords),
-            ("dungeon_orchestrator", dungeon_orchestrator),
+            ("dungeon_branch", dungeon_branch),
         ),
     )
     return new_room
 
 
-class EvAdventureDungeonOrchestrator(DefaultScript):
+class EvAdventureDungeonBranch(DefaultScript):
     """
-    One script is created per dungeon 'branch' created. The orchestrator is
+    One script is created per dungeon 'branch' created. The branch is
     responsible for determining what is created next when a character enters an
     exit within the dungeon.
 
     """
 
     # this determines how branching the dungeon will be
     max_unexplored_exits = 2
     max_new_exits_per_room = 2
 
     rooms = AttributeProperty(list())
     unvisited_exits = AttributeProperty(list())
-    highest_depth = AttributeProperty(0)
 
     last_updated = AttributeProperty(datetime.utcnow())
 
     # the room-generator function; copied from the same-name value on the start-room when the
-    # orchestrator is first created
+    # branch is first created
     room_generator = AttributeProperty(None, autocreate=False)
 
-    # (x,y): room coordinates used up by orchestrator
+    # (x,y): room coordinates used up by branch
     xy_grid = AttributeProperty(dict())
     start_room = AttributeProperty(None, autocreate=False)
 
     def register_exit_traversed(self, exit):
         """
         Tell the system the given exit was traversed. This allows us to track how many unvisited
         paths we have so as to not have it grow exponentially.
@@ -250,15 +246,15 @@
             location=location,
             aliases=_EXIT_ALIASES[exit_direction],
         )
         self.unvisited_exits.append(out_exit.id)
 
     def delete(self):
         """
-        Clean up the entire dungeon along with the orchestrator.
+        Clean up the entire dungeon along with the branch.
 
         """
         # first secure all characters in this branch back to the start room
         characters = search.search_object_by_tag(self.key, category="dungeon_character")
         start_room = self.start_room
         for character in characters:
             start_room.msg_contents(
@@ -270,15 +266,15 @@
                 "All turns dark ...|n\n\nThen you realize you are back where you started."
             )
             character.tags.remove(self.key, category="dungeon_character")
         # next delete all rooms in the dungeon (this will also delete exits)
         rooms = search.search_object_by_tag(self.key, category="dungeon_room")
         for room in rooms:
             room.delete()
-        # finally delete the orchestrator itself
+        # finally delete the branch itself
         super().delete()
 
     def new_room(self, from_exit):
         """
         Create a new Dungeon room leading from the provided exit.
 
         Args:
@@ -290,15 +286,15 @@
         # new one would get
         source_location = from_exit.location
         x, y = source_location.attributes.get("xy_coords", default=(0, 0))
         dx, dy = _EXIT_GRID_SHIFT.get(from_exit.key, (0, 1))
         new_x, new_y = (x + dx, y + dy)
 
         # the dungeon's depth acts as a measure of the current difficulty level. This is the radial
-        # distance from the (0, 0) (the entrance). The Orchestrator also tracks the highest
+        # distance from the (0, 0) (the entrance). The branch also tracks the highest
         # depth achieved.
         depth = int(sqrt(new_x**2 + new_y**2))
 
         new_room = self.room_generator(self, depth, (new_x, new_y))
 
         self.xy_grid[(new_x, new_y)] = new_room
 
@@ -344,16 +340,14 @@
                         # no room there (and not back to start room) - make an exit to it
                         self.create_out_exit(new_room, direction)
                         # we create this to avoid other rooms linking here, but don't create the
                         # room yet
                         self.xy_grid[target_coord] = None
                         break
 
-        self.highest_depth = max(self.highest_depth, depth)
-
         return new_room
 
 
 # --------------------------------------------------
 # Start room
 # --------------------------------------------------
 
@@ -374,80 +368,80 @@
         Flush the exit, so next traversal creates a new dungeon branch.
 
         """
         self.destination = self.location
 
     def at_traverse(self, traversing_object, target_location, **kwargs):
         """
-        When traversing create a new orchestrator if one is not already assigned.
+        When traversing create a new branch if one is not already assigned.
 
         """
         if target_location == self.location:
-            # make a global orchestrator script for this dungeon branch
+            # make a global branch script for this dungeon branch
             self.location.room_generator
-            dungeon_orchestrator = create.create_script(
-                EvAdventureDungeonOrchestrator,
-                key=f"dungeon_orchestrator_{self.key}_{datetime.utcnow()}",
+            dungeon_branch = create.create_script(
+                EvAdventureDungeonBranch,
+                key=f"dungeon_branch_{self.key}_{datetime.utcnow()}",
                 attributes=(
                     ("start_room", self.location),
                     ("room_generator", self.location.room_generator),
                 ),
             )
-            self.destination = target_location = dungeon_orchestrator.new_room(self)
+            self.destination = target_location = dungeon_branch.new_room(self)
             # make sure to tag character when entering so we can find them again later
-            traversing_object.tags.add(dungeon_orchestrator.key, category="dungeon_character")
+            traversing_object.tags.add(dungeon_branch.key, category="dungeon_character")
 
         super().at_traverse(traversing_object, target_location, **kwargs)
 
 
-class EvAdventureStartRoomResetter(DefaultScript):
+class EvAdventureDungeonBranchDeleter(DefaultScript):
     """
-    Simple ticker-script. Introduces a chance of the room's exits cycling every interval.
+    Cleanup script. After some time a dungeon branch will 'collapse', forcing all players in it
+    back to the start room.
 
     """
 
+    # set at creation time when the start room is created
+    branch_max_life = AttributeProperty(0, autocreate=False)
+
     def at_script_creation(self):
-        self.key = "evadventure_dungeon_startroom_resetter"
+        self.key = "evadventure_dungeon_branch_deleter"
 
     def at_repeat(self):
         """
-        Called every time the script repeats.
+        Go through all dungeon-branchs and find which ones are too old.
 
         """
-        room = self.obj
-        for exi in room.exits:
-            if inherits_from(exi, EvAdventureDungeonStartRoomExit) and random() < 0.5:
-                exi.reset_exit()
+        max_dt = timedelta(seconds=self.branch_max_life)
+        max_allowed_date = datetime.utcnow() - max_dt
 
+        for branch in EvAdventureDungeonBranch.objects.all():
+            if branch.last_updated < max_allowed_date:
+                # branch is too old; tell it to clean up and delete itself
+                branch.delete()
 
-class EvAdventureDungeonBranchDeleter(DefaultScript):
-    """
-    Cleanup script. After some time a dungeon branch will 'collapse', forcing all players in it
-    back to the start room.
 
+class EvAdventureStartRoomResetter(DefaultScript):
     """
+    Simple ticker-script. Introduces a chance of the room's exits cycling every interval.
 
-    # set at creation time when the start room is created
-    branch_max_life = AttributeProperty(0, autocreate=False)
+    """
 
     def at_script_creation(self):
-        self.key = "evadventure_dungeon_branch_deleter"
+        self.key = "evadventure_dungeon_startroom_resetter"
 
     def at_repeat(self):
         """
-        Go through all dungeon-orchestrators and find which ones are too old.
+        Called every time the script repeats.
 
         """
-        max_dt = timedelta(seconds=self.branch_max_life)
-        max_allowed_date = datetime.utcnow() - max_dt
-
-        for orchestrator in EvAdventureDungeonOrchestrator.objects.all():
-            if orchestrator.last_updated < max_allowed_date:
-                # orchestrator is too old; tell it to clean up and delete itself
-                orchestrator.delete()
+        room = self.obj
+        for exi in room.exits:
+            if inherits_from(exi, EvAdventureDungeonStartRoomExit) and random() < 0.5:
+                exi.reset_exit()
 
 
 class EvAdventureDungeonStartRoom(EvAdventureDungeonRoom):
     """
     The start room is the only permanent part of the dungeon. Exits leading from this room (except
     one leading back outside) each create/links to a separate dungeon branch/instance.
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/enums.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 To get the `value` of an enum (must always be hashable, useful for Attribute lookups), use
 `Ability.STR.value` (which would return 'strength' in our case).
 
 ----
 
 """
+
 from enum import Enum
 
 
 class Ability(Enum):
     """
     The six base abilities (defense is always bonus + 10)
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/equipment.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/npcs.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/npcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 EvAdventure NPCs. This includes both friends and enemies, only separated by their AI.
 
 """
+
 from random import choice
 
 from evennia import DefaultCharacter
 from evennia.typeclasses.attributes import AttributeProperty
 from evennia.typeclasses.tags import TagProperty
 from evennia.utils.evmenu import EvMenu
-from evennia.utils.utils import make_iter
+from evennia.utils.utils import lazy_property, make_iter
 
-from .ai import AggressiveMobMixin
+from .ai import AIHandler
 from .characters import LivingMixin
 from .enums import Ability, WieldLocation
 from .objects import get_bare_hands
 from .rules import dice
 
 
 class EvAdventureNPC(LivingMixin, DefaultCharacter):
@@ -244,74 +245,112 @@
         """
         attacker.msg(
             f"{self.key} brushes off the hit and shouts "
             '"|wHey! This is not the way to get a discount!|n"'
         )
 
 
-class EvAdventureMob(AggressiveMobMixin, EvAdventureNPC):
+class EvAdventureMob(EvAdventureNPC):
     """
     Mob (mobile) NPC; this is usually an enemy.
 
     """
 
-    # chance (%) that this enemy will loot you when defeating you
-    loot_chance = AttributeProperty(75, autocreate=False)
+    # change this to make the mob more or less likely to perform different actions
+    combat_probabilities = {
+        "hold": 0.0,
+        "attack": 0.85,
+        "stunt": 0.05,
+        "item": 0.0,
+        "flee": 0.05,
+    }
+
+    @lazy_property
+    def ai(self):
+        return AIHandler(self)
 
-    def at_defeat(self):
+    def ai_idle(self):
         """
-        Mobs die right away when defeated, no death-table rolls.
+        Do nothing.
 
         """
-        self.at_death()
+        pass
+
+    def ai_combat(self):
+        """
+        Manage the combat/combat state of the mob.
+
+        """
+        if combathandler := self.nbd.combathandler:
+            # already in combat
+            allies, enemies = combathandler.get_sides(self)
+            action = self.ai.random_probability(self.combat_probabilities)
+
+            match action:
+                case "hold":
+                    combathandler.queue_action({"key": "hold"})
+                case "combat":
+                    combathandler.queue_action({"key": "attack", "target": random.choice(enemies)})
+                case "stunt":
+                    # choose a random ally to help
+                    combathandler.queue_action(
+                        {
+                            "key": "stunt",
+                            "recipient": random.choice(allies),
+                            "advantage": True,
+                            "stunt": Ability.STR,
+                            "defense": Ability.DEX,
+                        }
+                    )
+                case "item":
+                    # use a random item on a random ally
+                    target = random.choice(allies)
+                    valid_items = [item for item in self.contents if item.at_pre_use(self, target)]
+                    combathandler.queue_action(
+                        {"key": "item", "item": random.choice(valid_items), "target": target}
+                    )
+                case "flee":
+                    self.ai.set_state("flee")
+
+        elif not (targets := self.ai.get_targets()):
+            self.ai.set_state("roam")
+        else:
+            target = random.choice(targets)
+            self.execute_cmd(f"attack {target.key}")
+
+    def ai_roam(self):
+        """
+        roam, moving randomly to a new room. If a target is found, switch to combat state.
+
+        """
+        if targets := self.ai.get_targets():
+            self.ai.set_state("combat")
+            self.execute_cmd(f"attack {random.choice(targets).key}")
+        else:
+            exits = self.ai.get_traversable_exits()
+            if exits:
+                exi = random.choice(exits)
+                self.execute_cmd(f"{exi.key}")
+
+    def ai_flee(self):
+        """
+        Flee from the current room, avoiding going back to the room from which we came. If no exits
+        are found, switch to roam state.
+
+        """
+        current_room = self.location
+        past_room = self.attributes.get("past_room", category="ai_state", default=None)
+        exits = self.ai.get_traversable_exits(exclude_destination=past_room)
+        if exits:
+            self.attributes.set("past_room", current_room, category="ai_state")
+            exi = random.choice(exits)
+            self.execute_cmd(f"{exi.key}")
+        else:
+            # if in a dead end, roam will allow for backing out
+            self.ai.set_state("roam")
 
-    def at_do_loot(self, looted):
+    def at_defeat(self):
         """
-        Called when mob gets to loot a PC.
+        Mobs die right away when defeated, no death-table rolls.
 
         """
-        if dice.roll("1d100") > self.loot_chance:
-            # don't loot
-            return
-
-        if looted.coins:
-            # looter prefer coins
-            loot = dice.roll("1d20")
-            if looted.coins < loot:
-                self.location.msg_location(
-                    "$You(looter) loots $You() for all coin!",
-                    from_obj=looted,
-                    mapping={"looter": self},
-                )
-            else:
-                self.location.msg_location(
-                    "$You(looter) loots $You() for |y{loot}|n coins!",
-                    from_obj=looted,
-                    mapping={"looter": self},
-                )
-        elif hasattr(looted, "equipment"):
-            # go through backpack, first usable, then wieldable, wearable items
-            # and finally stuff wielded
-            stealable = looted.equipment.get_usable_objects_from_backpack()
-            if not stealable:
-                stealable = looted.equipment.get_wieldable_objects_from_backpack()
-            if not stealable:
-                stealable = looted.equipment.get_wearable_objects_from_backpack()
-            if not stealable:
-                stealable = [looted.equipment.slots[WieldLocation.SHIELD_HAND]]
-            if not stealable:
-                stealable = [looted.equipment.slots[WieldLocation.HEAD]]
-            if not stealable:
-                stealable = [looted.equipment.slots[WieldLocation.ARMOR]]
-            if not stealable:
-                stealable = [looted.equipment.slots[WieldLocation.WEAPON_HAND]]
-            if not stealable:
-                stealable = [looted.equipment.slots[WieldLocation.TWO_HANDS]]
-
-            stolen = looted.equipment.remove(choice(stealable))
-            stolen.location = self
-
-            self.location.msg_location(
-                "$You(looter) steals {stolen.key} from $You()!",
-                from_obj=looted,
-                mapping={"looter": self},
-            )
+        self.at_death()
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/objects.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/random_tables.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/random_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/rooms.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/rules.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 The center of the rule system is the "RollEngine", which handles all rolling of dice
 and determining what the outcome is.
 
 ----
 
 """
+
 from random import randint
 
 from .enums import Ability
 from .random_tables import death_and_dismemberment as death_table
 
 # Basic rolls
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/shops.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/shops.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/mixins.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_ai.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 """
-Test the ai module.
+Test characters.
 
 """
-from unittest.mock import Mock, patch
 
-from evennia import create_object
+from evennia.utils import create
 from evennia.utils.test_resources import BaseEvenniaTest
 
 from ..characters import EvAdventureCharacter
-from ..npcs import EvAdventureMob
 
 
-class TestAI(BaseEvenniaTest):
+class TestCharacters(BaseEvenniaTest):
     def setUp(self):
         super().setUp()
-        self.npc = create_object(EvAdventureMob, key="Goblin", location=self.room1)
-        self.pc = create_object(EvAdventureCharacter, key="Player", location=self.room1)
+        self.character = create.create_object(EvAdventureCharacter, key="testchar")
 
-    def tearDown(self):
-        super().tearDown()
-        self.npc.delete()
-
-    @patch("evennia.contrib.tutorials.evadventure.ai.random.random")
-    @patch("evennia.contrib.tutorials.evadventure.ai.log_trace")
-    def test_ai_methods(self, mock_log_trace, mock_random):
-        self.assertEqual(self.npc.ai.get_state(), "idle")
-        self.npc.ai.set_state("patrol")
-        self.assertEqual(self.npc.ai.get_state(), "patrol")
-
-        self.assertEqual(self.npc.ai.get_targets(), [self.pc])
-        self.assertEqual(self.npc.ai.get_traversable_exits(), [self.exit])
-
-        probs = {"hold": 0.1, "attack": 0.5, "flee": 0.4}
-        mock_random.return_value = 0.3
-        self.assertEqual(self.npc.ai.random_probability(probs), "attack")
-        mock_random.return_value = 0.7
-        self.assertEqual(self.npc.ai.random_probability(probs), "flee")
-        mock_random.return_value = 0.95
-        self.assertEqual(self.npc.ai.random_probability(probs), "hold")
-
-    def test_ai_run(self):
-        self.npc.ai.set_state("patrol")
-        self.assertEqual(self.npc.ai.get_state(), "patrol")
-
-        self.npc.ai.run()
-        self.assertEqual(self.npc.ai.get_state(), "attack")
+    def test_abilities(self):
+        self.character.strength += 2
+        self.assertEqual(self.character.strength, 3)
+
+    def test_heal(self):
+        """Make sure we don't heal too much"""
+        self.character.hp = 0
+        self.character.hp_max = 8
+
+        self.character.heal(1)
+        self.assertEqual(self.character.hp, 1)
+        self.character.heal(100)
+        self.assertEqual(self.character.hp, 8)
+
+    def test_at_damage(self):
+        self.character.hp = 8
+        self.character.at_damage(5)
+        self.assertEqual(self.character.hp, 3)
+
+    def test_at_pay(self):
+        self.character.coins = 100
+
+        result = self.character.at_pay(60)
+        self.assertEqual(result, 60)
+        self.assertEqual(self.character.coins, 40)
+
+        # can't get more coins than we have
+        result = self.character.at_pay(100)
+        self.assertEqual(result, 40)
+        self.assertEqual(self.character.coins, 0)
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Test Dungeon orchestrator / procedurally generated dungeon rooms.
+Test Dungeon branch / procedurally generated dungeon rooms.
 
 """
 
 from unittest.mock import MagicMock
 
 from evennia.utils.create import create_object
 from evennia.utils.test_resources import BaseEvenniaTest
@@ -69,18 +69,18 @@
         self.assertEqual(self.character.location, self.start_room)
 
         # first go north, this should generate a new room
         new_room_north = self._move_character("north")
         self.assertNotEqual(self.start_room, new_room_north)
         self.assertTrue(inherits_from(new_room_north, dungeon.EvAdventureDungeonRoom))
 
-        # check if Orchestrator was created
-        orchestrator = new_room_north.db.dungeon_orchestrator
-        self.assertTrue(bool(orchestrator))
-        self.assertTrue(orchestrator.key.startswith("dungeon_orchestrator_north_"))
+        # check if Dungeon Branch was created
+        branch = new_room_north.db.dungeon_branch
+        self.assertTrue(bool(branch))
+        self.assertTrue(branch.key.startswith("dungeon_branch_north_"))
 
     def test_different_start_directions(self):
         # first go north, this should generate a new room
         new_room_north = self._move_character("north")
         self.assertNotEqual(self.start_room, new_room_north)
 
         # back to start room
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Test the EvAdventure equipment handler.
 
 """
 
-
 from unittest.mock import MagicMock, patch
 
 from parameterized import parameterized
 
 from evennia.utils.test_resources import BaseEvenniaTest
 
 from ..enums import Ability, WieldLocation
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py`

 * *Files 24% similar despite different names*

```diff
@@ -95,56 +95,54 @@
 
     def _fulfillC(self):
         """Fullfill quest step C"""
         self.character.db.test_quest_counter = 6
 
     def test_help(self):
         """Get help"""
-        # get help for all quests
-        help_txt = self.character.quests.get_help()
-        self.assertEqual(help_txt, ["|ctestquest|n\n A test quest!\n\n - You need to do A first."])
-
-        # get help for one specific quest
-        help_txt = self.character.quests.get_help(_TestQuest.key)
-        self.assertEqual(help_txt, ["|ctestquest|n\n A test quest!\n\n - You need to do A first."])
+        quest = self._get_quest()
+        # get help for a specific quest
+        help_txt = quest.help()
+        self.assertEqual(help_txt, "You need to do A first.")
 
         # help for finished quest
-        self._get_quest().is_completed = True
-        help_txt = self.character.quests.get_help()
-        self.assertEqual(help_txt, ["|ctestquest|n\n A test quest!\n\n - This quest is completed!"])
+        quest.complete()
+        help_txt = quest.help()
+        self.assertEqual(help_txt, "You have completed this quest.")
 
     def test_progress__fail(self):
         """
         Check progress without having any.
         """
-        # progress all quests
-        self.character.quests.progress()
-        # progress one quest
-        self.character.quests.progress(_TestQuest.key)
+        quest = self._get_quest()
+        # progress quest
+        quest.progress()
 
         # still on step A
-        self.assertEqual(self._get_quest().current_step, "A")
+        self.assertEqual(quest.current_step, "A")
 
     def test_progress(self):
         """
-        Fulfill the quest steps in sequess
+        Fulfill the quest steps in sequence.
 
         """
+        quest = self._get_quest()
+
         # A requires a certain object in inventory
         self._fulfillA()
-        self.character.quests.progress()
-        self.assertEqual(self._get_quest().current_step, "B")
+        quest.progress()
+        self.assertEqual(quest.current_step, "B")
 
         # B requires progress be called with specific kwarg
         # should not step (no kwarg)
-        self.character.quests.progress()
-        self.assertEqual(self._get_quest().current_step, "B")
+        quest.progress()
+        self.assertEqual(quest.current_step, "B")
 
         # should step (kwarg sent)
-        self.character.quests.progress(complete_quest_B=True)
-        self.assertEqual(self._get_quest().current_step, "C")
+        quest.progress(complete_quest_B=True)
+        self.assertEqual(quest.current_step, "C")
 
         # C requires a counter Attribute on char be high enough
         self._fulfillC()
-        self.character.quests.progress()
-        self.assertEqual(self._get_quest().current_step, "C")  # still on last step
-        self.assertEqual(self._get_quest().is_completed, True)
+        quest.progress()
+        self.assertEqual(quest.current_step, "C")  # still on last step
+        self.assertEqual(quest.is_completed, True)
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/evadventure/utils.py` & `evennia-4.1.0/evennia/contrib/tutorials/evadventure/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Various utilities.
 
 """
 
+import random
+
 _OBJ_STATS = """
 |c{key}|n
 Value: ~|y{value}|n coins{carried}
 
 {desc}
 
 Slots: |w{size}|n, Used from: |w{use_slot_name}|n
@@ -46,7 +48,31 @@
         use_slot_name=obj.inventory_use_slot.value,
         quality=getattr(obj, "quality", "N/A"),
         uses=getattr(obj, "uses", "N/A"),
         attack_type_name=attack_type.value if attack_type else "No attack",
         defense_type_name=defense_type.value if defense_type else "No defense",
         damage_roll=getattr(obj, "damage_roll", "None"),
     )
+
+
+def random_probability(self, probabilities):
+    """
+    Given a dictionary of probabilities, return the key of the chosen probability.
+
+    Args:
+        probabilities (dict): A dictionary of probabilities, where the key is the action and the
+            value is the probability of that action.
+
+    """
+    r = random.random()
+    # sort probabilities from higheest to lowest, making sure to normalize them 0..1
+    prob_total = sum(probabilities.values())
+    sorted_probs = sorted(
+        ((key, prob / prob_total) for key, prob in probabilities.items()),
+        key=lambda x: x[1],
+        reverse=True,
+    )
+    total = 0
+    for key, prob in sorted_probs:
+        total += prob
+        if r <= total:
+            return key
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/mirror/mirror.py` & `evennia-4.1.0/evennia/contrib/tutorials/mirror/mirror.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/red_button/README.md` & `evennia-4.1.0/evennia/contrib/tutorials/red_button/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/red_button/red_button.py` & `evennia-4.1.0/evennia/contrib/tutorials/red_button/red_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   time.
 
 Timers are handled by persistent delays on the button. These are examples of
 `evennia.utils.utils.delay` calls that wait a certain time before calling a method -
 such as when closing the lid and un-blinding a character.
 
 """
+
 import random
 
 from evennia import CmdSet, Command, DefaultObject
 from evennia.utils.utils import delay, interactive, repeat
 
 # Commands on the button (not all awailable at the same time)
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/talking_npc/README.md` & `evennia-4.1.0/evennia/contrib/tutorials/talking_npc/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/talking_npc/talking_npc.py` & `evennia-4.1.0/evennia/contrib/tutorials/talking_npc/talking_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/README.md` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/build.ev` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/build.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/mob.py` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/mob.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/objects.py` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/rooms.py` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/rooms.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 This defines special types of Rooms available in the tutorial. To keep
 everything in one place we define them together with the custom
 commands needed to control them. Those commands could also have been
 in a separate module (e.g. if they could have been re-used elsewhere.)
 
 """
 
-
 import random
 
 # the system error-handling module is defined in the settings. We load the
 # given setting here using utils.object_from_module. This way we can use
 # it regardless of if we change settings later.
 from django.conf import settings
```

### Comparing `evennia-4.0.0/evennia/contrib/tutorials/tutorial_world/tests.py` & `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/auditing/README.md` & `evennia-4.1.0/evennia/contrib/utils/auditing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/auditing/outputs.py` & `evennia-4.1.0/evennia/contrib/utils/auditing/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 objects, or if you want to perform geoip or ASN lookups on IPs before committing,
 or tag certain events with the results of a reputational lookup, this should be
 the easiest place to do it. Write a method and invoke it via
 `settings.AUDIT_CALLBACK` to have log data objects passed to it.
 
 Evennia contribution - Johnny 2017
 """
+
 import json
 import syslog
 
 from evennia.utils.logger import log_file
 
 
 def to_file(data):
```

### Comparing `evennia-4.0.0/evennia/contrib/utils/auditing/server.py` & `evennia-4.1.0/evennia/contrib/utils/auditing/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Auditable Server Sessions:
 Extension of the stock ServerSession that yields objects representing
 user inputs and system outputs.
 
 Evennia contribution - Johnny 2017
 """
+
 import os
 import re
 import socket
 
 from django.conf import settings as ev_settings
 from django.utils import timezone
```

### Comparing `evennia-4.0.0/evennia/contrib/utils/auditing/tests.py` & `evennia-4.1.0/evennia/contrib/utils/auditing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/fieldfill/README.md` & `evennia-4.1.0/evennia/contrib/utils/fieldfill/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/fieldfill/fieldfill.py` & `evennia-4.1.0/evennia/contrib/utils/fieldfill/fieldfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
         the player's input is considered valid - if it returns False,
         the input is rejected. Any other value returned will act as
         the field's new value, replacing the player's input. This
         allows for values that aren't strings or integers (such as
         object dbrefs). For boolean fields, return '0' or '1' to set
         the field to False or True.
 """
+
 import evennia
 from evennia import Command
 from evennia.utils import delay, evmenu, evtable, list_to_string, logger
 
 
 class FieldEvMenu(evmenu.EvMenu):
     """
```

### Comparing `evennia-4.0.0/evennia/contrib/utils/git_integration/README.md` & `evennia-4.1.0/evennia/contrib/utils/git_integration/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/git_integration/git_integration.py` & `evennia-4.1.0/evennia/contrib/utils/git_integration/git_integration.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/git_integration/tests.py` & `evennia-4.1.0/evennia/contrib/utils/git_integration/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/name_generator/README.md` & `evennia-4.1.0/evennia/contrib/utils/name_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/name_generator/btn_givennames.txt` & `evennia-4.1.0/evennia/contrib/utils/name_generator/btn_givennames.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/name_generator/btn_surnames.txt` & `evennia-4.1.0/evennia/contrib/utils/name_generator/btn_surnames.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/name_generator/namegen.py` & `evennia-4.1.0/evennia/contrib/utils/name_generator/namegen.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/name_generator/tests.py` & `evennia-4.1.0/evennia/contrib/utils/name_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/random_string_generator/README.md` & `evennia-4.1.0/evennia/contrib/utils/random_string_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/random_string_generator/random_string_generator.py` & `evennia-4.1.0/evennia/contrib/utils/random_string_generator/random_string_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,35 +55,32 @@
 from random import choice, randint, seed
 
 from evennia import DefaultScript, ScriptDB
 from evennia.utils.create import create_script
 
 
 class RejectedRegex(RuntimeError):
-
     """The provided regular expression has been rejected.
 
     More details regarding why this error occurred will be provided in
     the message.  The usual reason is the provided regular expression is
     not specific enough and could lead to inconsistent generating.
 
     """
 
     pass
 
 
 class ExhaustedGenerator(RuntimeError):
-
     """The generator hasn't any available strings to generate anymore."""
 
     pass
 
 
 class RandomStringGeneratorScript(DefaultScript):
-
     """
     The global script to hold all generators.
 
     It will be automatically created the first time `generate` is called
     on a RandomStringGenerator object.
 
     """
@@ -95,15 +92,14 @@
         self.persistent = True
 
         # Permanent data to be stored
         self.db.generated = {}
 
 
 class RandomStringGenerator:
-
     """
     A generator class to generate pseudo-random strings with a rule.
 
     The "rule" defining what the generator should provide in terms of
     string is given as a regular expression when creating instances of
     this class.  You can use the `all` method to get all generated strings,
     the `get` method to generate a new string, the `remove` method
```

### Comparing `evennia-4.0.0/evennia/contrib/utils/random_string_generator/tests.py` & `evennia-4.1.0/evennia/contrib/utils/random_string_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/tree_select/README.md` & `evennia-4.1.0/evennia/contrib/utils/tree_select/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/tree_select/tests.py` & `evennia-4.1.0/evennia/contrib/utils/tree_select/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/contrib/utils/tree_select/tree_select.py` & `evennia-4.1.0/evennia/contrib/utils/tree_select/tree_select.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/README.md` & `evennia-4.1.0/evennia/game_template/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/commands/README.md` & `evennia-4.1.0/evennia/game_template/commands/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/commands/command.py` & `evennia-4.1.0/evennia/game_template/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/commands/default_cmdsets.py` & `evennia-4.1.0/evennia/game_template/commands/default_cmdsets.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/gitignore` & `evennia-4.1.0/evennia/game_template/gitignore`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/README.md` & `evennia-4.1.0/evennia/game_template/server/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/at_initial_setup.py` & `evennia-4.1.0/evennia/game_template/server/conf/at_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/at_search.py` & `evennia-4.1.0/evennia/game_template/server/conf/at_search.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/at_server_startstop.py` & `evennia-4.1.0/evennia/game_template/server/conf/at_server_startstop.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/cmdparser.py` & `evennia-4.1.0/evennia/game_template/server/conf/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/connection_screens.py` & `evennia-4.1.0/evennia/game_template/server/conf/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/inlinefuncs.py` & `evennia-4.1.0/evennia/game_template/server/conf/inlinefuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/inputfuncs.py` & `evennia-4.1.0/evennia/game_template/server/conf/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/lockfuncs.py` & `evennia-4.1.0/evennia/game_template/server/conf/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/mssp.py` & `evennia-4.1.0/evennia/game_template/server/conf/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/portal_services_plugins.py` & `evennia-4.1.0/evennia/game_template/server/conf/portal_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/secret_settings.py` & `evennia-4.1.0/evennia/game_template/server/conf/secret_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/server_services_plugins.py` & `evennia-4.1.0/evennia/game_template/server/conf/server_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/serversession.py` & `evennia-4.1.0/evennia/game_template/server/conf/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/settings.py` & `evennia-4.1.0/evennia/game_template/server/conf/settings.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/conf/web_plugins.py` & `evennia-4.1.0/evennia/game_template/server/conf/web_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/server/logs/README.md` & `evennia-4.1.0/evennia/game_template/server/logs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/README.md` & `evennia-4.1.0/evennia/game_template/typeclasses/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/accounts.py` & `evennia-4.1.0/evennia/game_template/typeclasses/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/channels.py` & `evennia-4.1.0/evennia/game_template/typeclasses/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/characters.py` & `evennia-4.1.0/evennia/game_template/typeclasses/characters.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Characters are (by default) Objects setup to be puppeted by Accounts.
 They are what you "see" in game. The Character class in this module
 is setup to be the "default" character type created by the default
 creation commands.
 
 """
+
 from evennia.objects.objects import DefaultCharacter
 
 from .objects import ObjectParent
 
 
 class Character(ObjectParent, DefaultCharacter):
     """
```

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/exits.py` & `evennia-4.1.0/evennia/game_template/typeclasses/exits.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Exits
 
 Exits are connectors between Rooms. An exit always has a destination property
 set and has a single command defined on itself with the same name as its key,
 for allowing Characters to traverse the exit to its destination.
 
 """
+
 from evennia.objects.objects import DefaultExit
 
 from .objects import ObjectParent
 
 
 class Exit(ObjectParent, DefaultExit):
     """
```

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/objects.py` & `evennia-4.1.0/evennia/game_template/typeclasses/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Note that the default Character, Room and Exit does not inherit from
 this Object, but from their respective default implementations in the
 evennia library. If you want to use this class as a parent to change
 the other types, you can do so by adding this as a multiple
 inheritance.
 
 """
+
 from evennia.objects.objects import DefaultObject
 
 
 class ObjectParent:
     """
     This is a mixin that can be used to override *all* entities inheriting at
     some distance from DefaultObject (Objects, Exits, Characters and Rooms).
```

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/rooms.py` & `evennia-4.1.0/evennia/game_template/typeclasses/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/typeclasses/scripts.py` & `evennia-4.1.0/evennia/game_template/typeclasses/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/web/README.md` & `evennia-4.1.0/evennia/game_template/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/web/admin/urls.py` & `evennia-4.1.0/evennia/game_template/web/admin/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This reroutes from an URL to a python view-function/class.
 
 The main web/urls.py includes these routes for all urls starting with `admin/`
 (the `admin/` part should not be included again here).
 
 """
 
-
 from django.urls import path
 
 from evennia.web.admin.urls import urlpatterns as evennia_admin_urlpatterns
 
 # add patterns here
 urlpatterns = [
     # path("url-pattern", imported_python_view),
```

### Comparing `evennia-4.0.0/evennia/game_template/web/static/README.md` & `evennia-4.1.0/evennia/game_template/web/static/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/web/templates/README.md` & `evennia-4.1.0/evennia/game_template/web/templates/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/web/urls.py` & `evennia-4.1.0/evennia/game_template/web/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 This file includes the urls in website, webclient and admin. To override you
 should modify urls.py in those sub directories.
 
 Search the Django documentation for "URL dispatcher" for more help.
 
 """
+
 from django.urls import include, path
 
 # default evennia patterns
 from evennia.web.urls import urlpatterns as evennia_default_urlpatterns
 
 # add patterns
 urlpatterns = [
```

### Comparing `evennia-4.0.0/evennia/game_template/web/webclient/README.md` & `evennia-4.1.0/evennia/game_template/web/webclient/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/web/webclient/urls.py` & `evennia-4.1.0/evennia/game_template/web/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/web/website/README.md` & `evennia-4.1.0/evennia/game_template/web/website/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/world/batch_cmds.ev` & `evennia-4.1.0/evennia/game_template/world/batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/world/help_entries.py` & `evennia-4.1.0/evennia/game_template/world/help_entries.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/game_template/world/prototypes.py` & `evennia-4.1.0/evennia/game_template/world/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/help/filehelp.py` & `evennia-4.1.0/evennia/help/filehelp.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
         # validate and parse dicts into FileEntryHelp objects and make sure they are unique-by-key
         # by letting latter added ones override earlier ones.
         unique_help_entries = {}
 
         for dct in loaded_help_dicts:
             key = dct.get("key").lower().strip()
-            category = dct.get("category", _DEFAULT_HELP_CATEGORY).strip()
+            category = dct.get("category", _DEFAULT_HELP_CATEGORY).lower().strip()
             aliases = list(dct.get("aliases", []))
             entrytext = dct.get("text", "")
             locks = dct.get("locks", "")
 
             if not key and entrytext:
                 logger.error(f"Cannot load file-help-entry (missing key or text): {dct}")
                 continue
```

### Comparing `evennia-4.0.0/evennia/help/manager.py` & `evennia-4.1.0/evennia/help/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Custom manager for HelpEntry objects.
 """
+
 from django.db import IntegrityError
 
 from evennia.server import signals
 from evennia.typeclasses.managers import TypedObjectManager
 from evennia.utils import logger, utils
 from evennia.utils.utils import make_iter
```

### Comparing `evennia-4.0.0/evennia/help/migrations/0001_initial.py` & `evennia-4.1.0/evennia/help/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/help/migrations/0002_auto_20170606_1731.py` & `evennia-4.1.0/evennia/help/migrations/0002_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/help/migrations/0003_auto_20190128_1820.py` & `evennia-4.1.0/evennia/help/migrations/0003_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/help/migrations/0004_auto_20210520_2137.py` & `evennia-4.1.0/evennia/help/migrations/0004_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/help/migrations/0005_auto_20210530_1818.py` & `evennia-4.1.0/evennia/help/migrations/0005_auto_20210530_1818.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/help/models.py` & `evennia-4.1.0/evennia/help/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 functionality, the other one being the auto-generated command help
 that is created on the fly from each command's `__doc__` string. The
 persistent database system defined here is intended for all other
 forms of help that do not concern commands, like information about the
 game world, policy info, rules and similar.
 
 """
+
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.urls import reverse
 from django.utils.text import slugify
 
 from evennia.help.manager import HelpEntryManager
 from evennia.locks.lockhandler import LockHandler
```

### Comparing `evennia-4.0.0/evennia/help/tests.py` & `evennia-4.1.0/evennia/help/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,9 +134,9 @@
         # we just need anything here since we mock the load anyway
         storage = filehelp.FileHelpStorageHandler(help_file_modules=["dummypath"])
         result = storage.all()
 
         for inum, helpentry in enumerate(result):
             self.assertEqual(HELP_ENTRY_DICTS[inum]["key"], helpentry.key)
             self.assertEqual(HELP_ENTRY_DICTS[inum].get("aliases", []), helpentry.aliases)
-            self.assertEqual(HELP_ENTRY_DICTS[inum]["category"], helpentry.help_category)
+            self.assertEqual(HELP_ENTRY_DICTS[inum]["category"].lower(), helpentry.help_category)
             self.assertEqual(HELP_ENTRY_DICTS[inum]["text"], helpentry.entrytext)
```

### Comparing `evennia-4.0.0/evennia/help/utils.py` & `evennia-4.1.0/evennia/help/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Resources for indexing help entries and for splitting help entries into
 sub-categories.
 
 This is used primarily by the default `help` command.
 
 """
+
 import re
 
 from django.conf import settings
 
 # these are words that Lunr normally ignores but which we want to find
 # since we use them (e.g. as command names).
 # Lunr's default ignore-word list is found here:
```

### Comparing `evennia-4.0.0/evennia/locale/README` & `evennia-4.1.0/evennia/locale/README`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/de/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/de/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/es/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/es/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/fr/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/fr/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/it/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/it/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/ko/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/ko/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/la/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/la/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/pl/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/pl/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/pt/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/pt/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/ru/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/ru/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/sv/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/sv/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/zh/LC_MESSAGES/django.mo` & `evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locale/zh/LC_MESSAGES/django.po` & `evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locks/lockfuncs.py` & `evennia-4.1.0/evennia/locks/lockfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 Note that `accessing_obj` and `accessed_obj` can be any object type
 with a lock variable/field, so be careful to not expect
 a certain object type.
 
 """
 
-
 from ast import literal_eval
 
 from django.conf import settings
 
 import evennia
 from evennia.utils import utils
```

### Comparing `evennia-4.0.0/evennia/locks/lockhandler.py` & `evennia-4.1.0/evennia/locks/lockhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/locks/tests.py` & `evennia-4.1.0/evennia/locks/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/manager.py` & `evennia-4.1.0/evennia/objects/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Custom manager for Objects.
 """
+
 import re
 
 from django.conf import settings
 from django.db.models import Q
 from django.db.models.fields import exceptions
+
 from evennia.server import signals
 from evennia.typeclasses.managers import TypeclassManager, TypedObjectManager
 from evennia.utils.utils import (
     class_from_module,
     dbid_to_obj,
     is_iter,
     make_iter,
```

### Comparing `evennia-4.0.0/evennia/objects/migrations/0001_initial.py` & `evennia-4.1.0/evennia/objects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0002_auto_20140917_0756.py` & `evennia-4.1.0/evennia/objects/migrations/0002_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py` & `evennia-4.1.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0004_auto_20150118_1622.py` & `evennia-4.1.0/evennia/objects/migrations/0004_auto_20150118_1622.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0006_auto_20170606_1731.py` & `evennia-4.1.0/evennia/objects/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0007_objectdb_db_account.py` & `evennia-4.1.0/evennia/objects/migrations/0007_objectdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0008_auto_20170705_1736.py` & `evennia-4.1.0/evennia/objects/migrations/0008_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py` & `evennia-4.1.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0010_auto_20190128_1820.py` & `evennia-4.1.0/evennia/objects/migrations/0010_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0011_auto_20191025_0831.py` & `evennia-4.1.0/evennia/objects/migrations/0011_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py` & `evennia-4.1.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/objects/models.py` & `evennia-4.1.0/evennia/objects/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 admin should usually not have to deal directly with this database
 object layer.
 
 Attributes are separate objects that store values persistently onto
 the database object. Like everything else, they can be accessed
 transparently through the decorating TypeClass.
 """
+
 from collections import defaultdict
 
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.validators import validate_comma_separated_integer_list
 from django.db import models
+
 from evennia.objects.manager import ObjectDBManager
 from evennia.typeclasses.models import TypedObject
 from evennia.utils import logger
 from evennia.utils.utils import dbref, lazy_property, make_iter
 
 
 class ContentsHandler:
```

### Comparing `evennia-4.0.0/evennia/objects/objects.py` & `evennia-4.1.0/evennia/objects/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 This module defines the basic `DefaultObject` and its children
 `DefaultCharacter`, `DefaultAccount`, `DefaultRoom` and `DefaultExit`.
 These are the (default) starting points for all in-game visible
 entities.
 
-This is the v1.0 develop version (for ref in doc building).
-
 """
+
 import time
 import typing
 from collections import defaultdict
 
-import evennia
 import inflect
 from django.conf import settings
 from django.utils.translation import gettext as _
+
+import evennia
 from evennia.commands import cmdset
 from evennia.commands.cmdsethandler import CmdSetHandler
 from evennia.objects.manager import ObjectManager
 from evennia.objects.models import ObjectDB
 from evennia.scripts.scripthandler import ScriptHandler
 from evennia.server.signals import SIGNAL_EXIT_TRAVERSED
 from evennia.typeclasses.attributes import ModelAttributeBackend, NickHandler
 from evennia.typeclasses.models import TypeclassBase
 from evennia.utils import ansi, create, funcparser, logger, search
 from evennia.utils.utils import (
     class_from_module,
+    compress_whitespace,
     dbref,
     is_iter,
     iter_to_str,
     lazy_property,
     make_iter,
     to_str,
     variable_from_module,
@@ -57,15 +58,15 @@
     """
 
     def __init__(self, obj):
         """
         Initializes the handler.
 
         Args:
-            obj (Object): The object on which the handler is defined.
+            obj (DefaultObject): The object on which the handler is defined.
 
         """
         self.obj = obj
         self._sessid_cache = []
         self._recache()
 
     def _recache(self):
@@ -84,15 +85,15 @@
         """
         Get the sessions linked to this Object.
 
         Args:
             sessid (int, optional): A specific session id.
 
         Returns:
-            sessions (list): The sessions connected to this object. If `sessid` is given,
+            list: The sessions connected to this object. If `sessid` is given,
                 this is a list of one (or zero) elements.
 
         Notes:
             Aliased to `self.all()`.
 
         """
 
@@ -114,15 +115,15 @@
         return sessions
 
     def all(self):
         """
         Alias to get(), returning all sessions.
 
         Returns:
-            sessions (list): All sessions.
+            list: All sessions.
 
         """
         return self.get()
 
     def add(self, session):
         """
         Add session to handler.
@@ -149,15 +150,15 @@
             self.obj.save(update_fields=["db_sessid"])
 
     def remove(self, session):
         """
         Remove session from handler.
 
         Args:
-            session (Session or int): Session or session id to remove.
+            Session or int: Session or session id to remove.
 
         """
         try:
             sessid = session.sessid
         except AttributeError:
             sessid = session
 
@@ -177,27 +178,27 @@
         self.obj.save(update_fields=["db_sessid"])
 
     def count(self):
         """
         Get amount of sessions connected.
 
         Returns:
-            sesslen (int): Number of sessions handled.
+            int: Number of sessions handled.
 
         """
         return len(self._sessid_cache)
 
 
 #
 # Base class to inherit from.
 
 
 class DefaultObject(ObjectDB, metaclass=TypeclassBase):
     """
-    This is the root typeclass object, representing all entities that
+    This is the root Object typeclass, representing all entities that
     have an actual presence in-game. DefaultObjects generally have a
     location. They can also be manipulated and looked at. Game
     entities you define should inherit from DefaultObject at some distance.
 
     It is recommended to create children of this class using the
     `evennia.create_object()` function rather than to initialize the class
     directly - this will both set things up and efficiently save the object
@@ -217,50 +218,52 @@
     objects = ObjectManager()
 
     # populated by `return_appearance`
     appearance_template = """
 {header}
 |c{name}{extra_name_info}|n
 {desc}
-{exits}{characters}{things}
+{exits}
+{characters}
+{things}
 {footer}
     """
     # on-object properties
 
     @lazy_property
     def cmdset(self):
+        """CmdSetHandler"""
         return CmdSetHandler(self, True)
 
     @lazy_property
     def scripts(self):
+        """ScriptHandler"""
         return ScriptHandler(self)
 
     @lazy_property
     def nicks(self):
+        """NickHandler"""
         return NickHandler(self, ModelAttributeBackend)
 
     @lazy_property
     def sessions(self):
+        """SessionHandler"""
         return ObjectSessionHandler(self)
 
     @property
     def is_connected(self):
-        # we get an error for objects subscribed to channels without this
+        """True if this object is associated with an Account with any connected sessions."""
         if self.account:  # seems sane to pass on the account
             return self.account.is_connected
         else:
             return False
 
     @property
     def has_account(self):
-        """
-        Convenience property for checking if an active account is
-        currently connected to this object.
-
-        """
+        """True is this object has an associated account."""
         return self.sessions.count()
 
     def get_cmdset_providers(self) -> dict[str, "CmdSetProvider"]:
         """
         Overrideable method which returns a dictionary of every kind of object which
         has a cmdsethandler linked to this Object, and should participate in cmdset
         merging.
@@ -273,60 +276,57 @@
         out = {"object": self}
         if self.account:
             out["account"] = self.account
         return out
 
     @property
     def is_superuser(self):
-        """
-        Check if user has an account, and if so, if it is a superuser.
-
-        """
+        """True if this object has an account and that account is a superuser."""
         return (
             self.db_account
             and self.db_account.is_superuser
             and not self.db_account.attributes.get("_quell")
         )
 
     def contents_get(self, exclude=None, content_type=None):
         """
         Returns the contents of this object, i.e. all
         objects that has this object set as its location.
         This should be publically available.
 
         Args:
-            exclude (Object): Object to exclude from returned
+            exclude (DefaultObject): Object to exclude from returned
                 contents list
             content_type (str): A content_type to filter by. None for no
                 filtering.
 
         Returns:
-            contents (list): List of contents of this Object.
+            list: List of contents of this Object.
 
         Notes:
-            Also available as the `contents` property, minus exclusion
-            and filtering.
+            Also available as the `.contents` property, but that doesn't allow for exclusion and
+            filtering on content-types.
 
         """
         return self.contents_cache.get(exclude=exclude, content_type=content_type)
 
     def contents_set(self, *args):
-        "You cannot replace this property"
+        "Makes sure `.contents` is read-only. Raises `AttributeError` if trying to set it."
         raise AttributeError(
             "{}.contents is read-only. Use obj.move_to or "
             "obj.location to move an object here.".format(self.__class__)
         )
 
     contents = property(contents_get, contents_set, contents_set, contents_set)
 
     @property
     def exits(self):
         """
         Returns all exits from this object, i.e. all objects at this
-        location having the property destination != `None`.
+        location having the property .destination != `None`.
 
         """
         return [exi for exi in self.contents if exi.destination]
 
     # search methods and hooks
 
     def get_search_query_replacement(self, searchdata, **kwargs):
@@ -354,39 +354,39 @@
         replacements, such as 'me' always being an alias for this object.
 
         Args:
             searchdata (str): The search string to replace.
             **kwargs (any): These are the same as passed to the `search` method.
 
         Returns:
-            tuple: `(should_return, str or Obj)`, where `should_return` is a boolean indicating
-            the `.search` method should return the result immediately without further
+            tuple: A tuple `(should_return, str or Obj)`, where `should_return` is a boolean
+            indicating the `.search` method should return the result immediately without further
             processing. If `should_return` is `True`, the second element of the tuple is the result
             that is returned.
 
         """
         if isinstance(searchdata, str):
             match searchdata.lower():
                 case "me" | "self":
                     return True, self
                 case "here":
                     return True, self.location
         return False, searchdata
 
     def get_search_candidates(self, searchdata, **kwargs):
         """
-        Get the candidates for a search. Also the `candidates` provided to the
-        search function is included, and could be modified in-place here.
+        Helper for the `.search` method. Get the candidates for a search. Also the `candidates`
+        provided to the search function is included, and could be modified in-place here.
 
         Args:
             searchdata (str): The search criterion (could be modified by `get_search_query_replacement`).
             **kwargs (any): These are the same as passed to the `search` method.
 
         Returns:
-            list: A list of objects to search between.
+            list: A list of objects possibly relevant for the search.
 
         Notes:
             If `searchdata` is a #dbref, this method should always return `None`. This is because
             the search should always be global in this case. If `candidates` were already given,
             they should be used as is. If `location` was given, the candidates should be based on
             that.
 
@@ -430,26 +430,30 @@
         candidates=None,
         exact=False,
         use_dbref=None,
         tags=None,
         **kwargs,
     ):
         """
-        This is a wrapper for actually searching for objects, used by the `search` method.
-        This is broken out into a separate method to allow for easier overriding in child classes.
+        Helper for the `.search` method. This is a wrapper for actually searching for objects, used
+        by the `search` method. This is broken out into a separate method to allow for easier
+        overriding in child classes.
 
         Args:
             searchdata (str): The search criterion.
             attribute_name (str): The attribute to search on (default is `.
             typeclass (Typeclass or list): The typeclass to search for.
             candidates (list): A list of objects to search between.
             exact (bool): Require exact match.
             use_dbref (bool): Allow dbref search.
             tags (list): Tags to search for.
 
+        Returns:
+            queryset or iterable: The result of the search.
+
         """
 
         return ObjectDB.objects.search_object(
             searchdata,
             attribute_name=attribute_name,
             typeclass=typeclass,
             candidates=candidates,
@@ -463,18 +467,18 @@
         This method is called by the search method to allow for handling of multi-match
         results that should be stacked.
 
         Args:
             results (list): The list of results from the search.
 
         Returns:
-            tuple: `(stacked, results)`, where `stacked` is a boolean indicating if the
-                result is stacked and `results` is the list of results to return. If `stacked`
-                is True, the ".search" method will return `results` immediately without further
-                processing (it will not result in a multimatch-error).
+            tuple: A tuple `(stacked, results)`, where `stacked` is a boolean indicating if the
+            result is stacked and `results` is the list of results to return. If `stacked`
+            is True, the ".search" method will return `results` immediately without further
+            processing (it will not result in a multimatch-error).
 
         Notes:
             The `stacked` keyword argument is an integer that controls the max size of each stack
             (if >0). It's important to make sure to only stack _identical_ objects, otherwise we
             risk losing track of objects.
 
         """
@@ -700,24 +704,25 @@
             searchdata (str): Search criterion - the key or dbref of the account
                 to search for. If this is "here" or "me", search
                 for the account connected to this object.
             quiet (bool): Returns the results as a list rather than
                 echo eventual standard error messages. Default `False`.
 
         Returns:
-            result (Account, None or list): Just what is returned depends on
-                the `quiet` setting:
-                    - `quiet=True`: No match or multumatch auto-echoes errors
-                      to self.msg, then returns `None`. The esults are passed
-                      through `settings.SEARCH_AT_RESULT` and
-                      `settings.SEARCH_AT_MULTIMATCH_INPUT`. If there is a
-                      unique match, this will be returned.
-                    - `quiet=True`: No automatic error messaging is done, and
-                      what is returned is always a list with 0, 1 or more
-                      matching Accounts.
+            DefaultAccount, None or list: What is returned depends on
+            the `quiet` setting:
+
+            - `quiet=False`: No match or multumatch auto-echoes errors
+              to self.msg, then returns `None`. The esults are passed
+              through `settings.SEARCH_AT_RESULT` and
+              `settings.SEARCH_AT_MULTIMATCH_INPUT`. If there is a
+              unique match, this will be returned.
+            - `quiet=True`: No automatic error messaging is done, and
+              what is returned is always a list with 0, 1 or more
+              matching Accounts.
 
         """
         if isinstance(searchdata, str):
             # searchdata is a string; wrap some common self-references
             if searchdata.lower() in ("me", "self"):
                 return [self.account] if quiet else self.account
 
@@ -742,23 +747,23 @@
         Keyword Args:
             Other keyword arguments will be added to the found command
             object instace as variables before it executes.  This is
             unused by default Evennia but may be used to set flags and
             change operating paramaters for commands at run-time.
 
         Returns:
-            defer (Deferred): This is an asynchronous Twisted object that
-                will not fire until the command has actually finished
-                executing. To overload this one needs to attach
-                callback functions to it, with addCallback(function).
-                This function will be called with an eventual return
-                value from the command execution. This return is not
-                used at all by Evennia by default, but might be useful
-                for coders intending to implement some sort of nested
-                command structure.
+            Deferred: This is an asynchronous Twisted object that
+            will not fire until the command has actually finished
+            executing. To overload this one needs to attach
+            callback functions to it, with addCallback(function).
+            This function will be called with an eventual return
+            value from the command execution. This return is not
+            used at all by Evennia by default, but might be useful
+            for coders intending to implement some sort of nested
+            command structure.
 
         """
         # break circular import issues
         global _CMDHANDLER
         if not _CMDHANDLER:
             from evennia.commands.cmdhandler import cmdhandler as _CMDHANDLER
 
@@ -769,36 +774,35 @@
         )
         return _CMDHANDLER(self, raw_string, callertype="object", session=session, **kwargs)
 
     def msg(self, text=None, from_obj=None, session=None, options=None, **kwargs):
         """
         Emits something to a session attached to the object.
 
-        Args:
-            text (str or tuple, optional): The message to send. This
+        Keyword Args:
+            text (str or tuple): The message to send. This
                 is treated internally like any send-command, so its
                 value can be a tuple if sending multiple arguments to
                 the `text` oob command.
-            from_obj (obj or list, optional): object that is sending. If
+            from_obj (DefaultObject, DefaultAccount, Session, or list): object that is sending. If
                 given, at_msg_send will be called. This value will be
                 passed on to the protocol. If iterable, will execute hook
                 on all entities in it.
-            session (Session or list, optional): Session or list of
+            session (Session or list): Session or list of
                 Sessions to relay data to, if any. If set, will force send
                 to these sessions. If unset, who receives the message
                 depends on the MULTISESSION_MODE.
-            options (dict, optional): Message-specific option-value
+            options (dict): Message-specific option-value
                 pairs. These will be applied at the protocol level.
-        Keyword Args:
-            any (string or tuples): All kwarg keys not listed above
+            **kwargs (string or tuples): All kwarg keys not listed above
                 will be treated as send-command names and their arguments
                 (which can be a string or a tuple).
 
         Notes:
-            `at_msg_receive` will be called on this Object.
+            The `at_msg_receive` method will be called on this Object.
             All extra kwargs will be passed on to the protocol.
 
         """
         # try send hooks
         if from_obj:
             for obj in make_iter(from_obj):
                 try:
@@ -823,24 +827,14 @@
             kwargs["text"] = text
 
         # relay to session(s)
         sessions = make_iter(session) if session else self.sessions.all()
         for session in sessions:
             session.data_out(**kwargs)
 
-    def get_contents_unique(self, caller=None):
-        """
-        Get a mapping of contents  that are visually unique to the caller, along with
-        how many of each there are.
-
-        Args:
-            caller (Object, optional): The object to check visibility from. If not given,
-                the current object will be used.
-        """
-
     def for_contents(self, func, exclude=None, **kwargs):
         """
         Runs a function on every object contained within this one.
 
         Args:
             func (callable): Function to call. This must have the
                 formal call sign func(obj, **kwargs), where obj is the
@@ -909,19 +903,20 @@
             For 'director-stance' reporting (Name says/Name says), use {key}
             syntax directly. For both `{key}` and `You/you(key)`,
             `mapping[key].get_display_name(looker=recipient)` may be called
             depending on who the recipient is.
 
         Examples:
 
-            Let's assume
-            - `player1.key -> "Player1"`,
-              `player1.get_display_name(looker=player2) -> "The First girl"`
-            - `player2.key -> "Player2"`,
-              `player2.get_display_name(looker=player1) -> "The Second girl"`
+            Let's assume:
+
+            - `player1.key` -> "Player1",
+            - `player1.get_display_name(looker=player2)` -> "The First girl"
+            - `player2.key` -> "Player2",
+            - `player2.get_display_name(looker=player1)` -> "The Second girl"
 
             Actor-stance:
             ::
 
                 char.location.msg_contents(
                     "$You() $conj(attack) $you(defender).",
                     from_obj=player1,
@@ -966,17 +961,19 @@
                 receiver=receiver,
                 mapping=mapping,
             )
 
             # director-stance replacements
             outmessage = outmessage.format_map(
                 {
-                    key: obj.get_display_name(looker=receiver)
-                    if hasattr(obj, "get_display_name")
-                    else str(obj)
+                    key: (
+                        obj.get_display_name(looker=receiver)
+                        if hasattr(obj, "get_display_name")
+                        else str(obj)
+                    )
                     for key, obj in mapping.items()
                 }
             )
 
             receiver.msg(text=(outmessage, outkwargs), from_obj=from_obj, **kwargs)
 
     def move_to(
@@ -990,59 +987,56 @@
         move_type="move",
         **kwargs,
     ):
         """
         Moves this object to a new location.
 
         Args:
-            destination (Object): Reference to the object to move to. This
+            destination (DefaultObject): Reference to the object to move to. This
                 can also be an exit object, in which case the
                 destination property is used as destination.
             quiet (bool): If true, turn off the calling of the emit hooks
                 (announce_move_to/from etc)
-            emit_to_obj (Object): object to receive error messages
+            emit_to_obj (DefaultObject): object to receive error messages
             use_destination (bool): Default is for objects to use the "destination"
                  property of destinations as the target to move to. Turning off this
                  keyword allows objects to move "inside" exit objects.
             to_none (bool): Allow destination to be None. Note that no hooks are run when
                  moving to a None location. If you want to run hooks, run them manually
                  (and make sure they can manage None locations).
             move_hooks (bool): If False, turn off the calling of move-related hooks
                 (at_pre/post_move etc) with quiet=True, this is as quiet a move
                 as can be done.
             move_type (str): The "kind of move" being performed, such as "teleport", "traverse",
                 "get", "give", or "drop". The value can be arbitrary. By default, it only affects
                 the text message generated by announce_move_to and announce_move_from by defining
                 their {"type": move_type} for outgoing text. This can be used for altering
                 messages and/or overloaded hook behaviors.
-
-        Keyword Args:
-          Passed on to announce_move_to and announce_move_from hooks.
-          Exits will set the "exit_obj" kwarg to themselves.
+            **kwargs: Passed on to announce_move_to and announce_move_from hooks. Exits will set
+                the "exit_obj" kwarg to themselves.
 
         Returns:
-            result (bool): True/False depending on if there were problems with the move.
-                    This method may also return various error messages to the
-                    `emit_to_obj`.
+            bool: True/False depending on if there were problems with the move. This method may also
+            return various error messages to the `emit_to_obj`.
 
         Notes:
             No access checks are done in this method, these should be handled before
             calling `move_to`.
 
-            The `DefaultObject` hooks called (if `move_hooks=True`) are, in order:
+        The `DefaultObject` hooks called (if `move_hooks=True`) are, in order:
 
-             1. `self.at_pre_move(destination)` (abort if return False)
-             2. `source_location.at_pre_object_leave(self, destination)` (abort if return False)
-             3. `destination.at_pre_object_receive(self, source_location)` (abort if return False)
-             4. `source_location.at_object_leave(self, destination)`
-             5. `self.announce_move_from(destination)`
-             6. (move happens here)
-             7. `self.announce_move_to(source_location)`
-             8. `destination.at_object_receive(self, source_location)`
-             9. `self.at_post_move(source_location)`
+        1. `self.at_pre_move(destination)` (abort if return False)
+        2. `source_location.at_pre_object_leave(self, destination)` (abort if return False)
+        3. `destination.at_pre_object_receive(self, source_location)` (abort if return False)
+        4. `source_location.at_object_leave(self, destination)`
+        5. `self.announce_move_from(destination)`
+        6. (move happens here)
+        7. `self.announce_move_to(source_location)`
+        8. `destination.at_object_receive(self, source_location)`
+        9. `self.at_post_move(source_location)`
 
         """
 
         def logerr(string="", err=None):
             """Simple log helper method"""
             logger.log_trace()
             self.msg("%s%s" % (string, "" if err is None else " (%s)" % err))
@@ -1207,20 +1201,20 @@
     def get_default_lockstring(
         cls, account: "DefaultAccount" = None, caller: "DefaultObject" = None, **kwargs
     ):
         """
         Classmethod called during .create() to determine default locks for the object.
 
         Args:
-            account (Account): Account to attribute this object to.
+            account (DefaultAccount): Account to attribute this object to.
             caller (DefaultObject): The object which is creating this one.
             **kwargs: Arbitrary input.
 
         Returns:
-            lockstring (str): A lockstring to use for this object.
+            str: A lockstring to use for this object.
         """
         pid = f"pid({account.id})" if account else None
         cid = f"id({caller.id})" if caller else None
         admin = "perm(Admin)"
         trio = " or ".join([x for x in [pid, cid, admin] if x])
         return ";".join([f"{x}:{trio}" for x in ["control", "delete", "edit"]])
 
@@ -1240,23 +1234,25 @@
         Provides a friendlier interface to the utils.create_object() function.
 
         Args:
             key (str): Name of the new object.
 
 
         Keyword Args:
-            account (Account): Account to attribute this object to.
+            account (DefaultAccount): Account to attribute this object to.
             caller (DefaultObject): The object which is creating this one.
             description (str): Brief description for this object.
             ip (str): IP address of creator (for object auditing).
             method (str): The method of creation. Defaults to "create".
 
         Returns:
-            object (Object): A newly created object of the given typeclass.
-            errors (list): A list of errors in string form, if any.
+            tuple: A tuple (Object, errors): A newly created object of the given typeclass. This
+            will be `None` if there are errors. The second element is then a list of errors that
+            occurred during creation. If this is empty, it's safe to assume the object was created
+            successfully.
 
         """
         errors = []
         obj = None
 
         # Get IP address of creator, if available
         ip = kwargs.pop("ip", "")
@@ -1304,15 +1300,15 @@
         by changing some settings, use ObjectDB.object.copy_object()
         directly.
 
         Args:
             new_key (string): New key/name of copied object. If new_key is not
                 specified, the copy will be named <old_key>_copy by default.
         Returns:
-            copy (Object): A copy of this object.
+            Object: A copy of this object.
 
         """
 
         def find_clone_key():
             """
             Append 01, 02 etc to obj.key. Checks next higher number in the
             same location, then adds the next number available
@@ -1334,30 +1330,27 @@
 
     def at_object_post_copy(self, new_obj, **kwargs):
         """
         Called by DefaultObject.copy(). Meant to be overloaded. In case there's extra data not
         covered by .copy(), this can be used to deal with it.
 
         Args:
-            new_obj (Object): The new Copy of this object.
+            new_obj (DefaultObject): The new Copy of this object.
 
-        Returns:
-            None
         """
         pass
 
     def delete(self):
         """
         Deletes this object.  Before deletion, this method makes sure
         to move all contained objects to their respective home
         locations, as well as clean up all exits to/from the object.
 
         Returns:
-            noerror (bool): Returns whether or not the delete completed
-                successfully or not.
+            bool: Whether or not the delete completed successfully or not.
 
         """
         global _ScriptDB
         if not _ScriptDB:
             from evennia.scripts.models import ScriptDB as _ScriptDB
 
         if not self.pk or not self.at_object_delete():
@@ -1401,68 +1394,84 @@
         self, accessing_obj, access_type="read", default=False, no_superuser_bypass=False, **kwargs
     ):
         """
         Determines if another object has permission to access this object
         in whatever way.
 
         Args:
-          accessing_obj (Object): Object trying to access this one.
+          accessing_obj (DefaultObject): Object trying to access this one.
           access_type (str, optional): Type of access sought.
           default (bool, optional): What to return if no lock of access_type was found.
           no_superuser_bypass (bool, optional): If `True`, don't skip
             lock check for superuser (be careful with this one).
-
-        Keyword Args:
-          Passed on to the at_access hook along with the result of the access check.
+          **kwargs: Passed on to the at_access hook along with the result of the access check.
 
         """
         result = super().access(
             accessing_obj,
             access_type=access_type,
             default=default,
             no_superuser_bypass=no_superuser_bypass,
         )
         self.at_access(result, accessing_obj, access_type, **kwargs)
         return result
 
+    def filter_visible(self, obj_list, looker, **kwargs):
+        """
+        Filter a list of objects to only include those that are visible to the looker.
+
+        Args:
+            obj_list (list): List of objects to filter.
+            looker (DefaultObject): Object doing the looking.
+            **kwargs: Arbitrary data for use when overriding.
+        Returns:
+            list: The filtered list of visible objects.
+        Notes:
+            By default this simply checks the 'view' and 'search' locks on each object in the list.
+            Override this
+            method to implement custom visibility mechanics.
+
+        """
+        return [
+            obj
+            for obj in obj_list
+            if (obj.access(looker, "view") and obj.access(looker, "search", default=True))
+        ]
+
     # name and return_appearance hooks
 
     def get_display_name(self, looker=None, **kwargs):
         """
         Displays the name of the object in a viewer-aware manner.
 
         Args:
-            looker (TypedObject): The object or account that is looking
-                at/getting inforamtion for this object. If not given, `.name` will be
-                returned, which can in turn be used to display colored data.
+            looker (DefaultObject): The object or account that is looking at or getting information
+                for this object.
 
         Returns:
-            str: A name to display for this object. This can contain color codes and may
-                be customized based on `looker`. By default this contains the `.key` of the object,
-                followed by the DBREF if this user is privileged to control said object.
+            str: A name to display for this object. By default this returns the `.name` of the object.
 
         Notes:
-            This function could be extended to change how object names appear to users in character,
-            but be wary. This function does not change an object's keys or aliases when searching,
-            and is expected to produce something useful for builders.
+            This function can be extended to change how object names appear to users in character,
+            but it does not change an object's keys or aliases when searching.
 
         """
         return self.name
 
     def get_extra_display_name_info(self, looker=None, **kwargs):
         """
         Adds any extra display information to the object's name. By default this is is the
         object's dbref in parentheses, if the looker has permission to see it.
 
         Args:
-            looker (Object): The object looking at this object.
+            looker (DefaultObject): The object looking at this object.
 
         Returns:
             str: The dbref of this object, if the looker has permission to see it. Otherwise, an
-                empty string is returned.
+            empty string is returned.
 
         Notes:
             By default, this becomes a string (#dbref) attached to the object's name.
 
         """
         if looker and self.locks.check_lockstring(looker, "perm(Builder)"):
             return f"(#{self.id})"
@@ -1474,30 +1483,36 @@
         by return_appearance and is used for grouping multiple same-named of this object. Note that
         this will be called on *every* member of a group even though the plural name will be only
         shown once. Also the singular display version, such as 'an apple', 'a tree' is determined
         from this method.
 
         Args:
             count (int): Number of objects of this type
-            looker (Object): Onlooker. Not used by default.
+            looker (DefaultObject): Onlooker. Not used by default.
 
         Keyword Args:
             key (str): Optional key to pluralize. If not given, the object's `.get_display_name()`
                 method is used.
             return_string (bool): If `True`, return only the singular form if count is 0,1 or
                 the plural form otherwise. If `False` (default), return both forms as a tuple.
+            no_article (bool): If `True`, do not return an article if `count` is 1.
 
         Returns:
             tuple: This is a tuple `(str, str)` with the singular and plural forms of the key
-                including the count.
+            including the count.
 
         Examples:
-            ::
-                obj.get_numbered_name(3, looker, key="foo") -> ("a foo", "three foos")
+        ::
 
+            obj.get_numbered_name(3, looker, key="foo")
+                  -> ("a foo", "three foos")
+            obj.get_numbered_name(1, looker, key="Foobert", return_string=True)
+                  -> "a Foobert"
+            obj.get_numbered_name(1, looker, key="Foobert", return_string=True, no_article=True)
+                  -> "Foobert"
         """
         plural_category = "plural_key"
         key = kwargs.get("key", self.get_display_name(looker))
         raw_key = self.name
         key = ansi.ANSIString(key)  # this is needed to allow inflection of colored names
         try:
             plural = _INFLECT.plural(key, count)
@@ -1510,163 +1525,158 @@
             # we need to wipe any old plurals/an/a in case key changed in the interrim
             self.aliases.clear(category=plural_category)
             self.aliases.add(plural, category=plural_category)
             # save the singular form as an alias here too so we can display "an egg" and also
             # look at 'an egg'.
             self.aliases.add(singular, category=plural_category)
 
+        if kwargs.get("no_article") and count == 1:
+            if kwargs.get("return_string"):
+                return key
+            return key, key
+
         if kwargs.get("return_string"):
-            return singular if count in (0, 1) else plural
+            return singular if count == 1 else plural
 
         return singular, plural
 
     def get_display_header(self, looker, **kwargs):
         """
         Get the 'header' component of the object description. Called by `return_appearance`.
 
         Args:
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The header display string.
 
         """
         return ""
 
     def get_display_desc(self, looker, **kwargs):
         """
         Get the 'desc' component of the object description. Called by `return_appearance`.
 
         Args:
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The desc display string.
 
         """
         return self.db.desc or "You see nothing special."
 
     def get_display_exits(self, looker, **kwargs):
         """
         Get the 'exits' component of the object description. Called by `return_appearance`.
 
         Args:
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The exits display data.
 
         """
-
-        def _filter_visible(obj_list):
-            return (obj for obj in obj_list if obj != looker and obj.access(looker, "view"))
-
-        exits = _filter_visible(self.contents_get(content_type="exit"))
+        exits = self.filter_visible(self.contents_get(content_type="exit"), looker, **kwargs)
         exit_names = iter_to_str(exi.get_display_name(looker, **kwargs) for exi in exits)
 
         return f"|wExits:|n {exit_names}" if exit_names else ""
 
     def get_display_characters(self, looker, **kwargs):
         """
         Get the 'characters' component of the object description. Called by `return_appearance`.
 
         Args:
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The character display data.
 
         """
-
-        def _filter_visible(obj_list):
-            return (obj for obj in obj_list if obj != looker and obj.access(looker, "view"))
-
-        characters = _filter_visible(self.contents_get(content_type="character"))
+        characters = self.filter_visible(
+            self.contents_get(content_type="character"), looker, **kwargs
+        )
         character_names = iter_to_str(
             char.get_display_name(looker, **kwargs) for char in characters
         )
 
-        return f"\n|wCharacters:|n {character_names}" if character_names else ""
+        return f"|wCharacters:|n {character_names}" if character_names else ""
 
     def get_display_things(self, looker, **kwargs):
         """
         Get the 'things' component of the object description. Called by `return_appearance`.
 
         Args:
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The things display data.
 
         """
-
-        def _filter_visible(obj_list):
-            return (obj for obj in obj_list if obj != looker and obj.access(looker, "view"))
-
         # sort and handle same-named things
-        things = _filter_visible(self.contents_get(content_type="object"))
+        things = self.filter_visible(self.contents_get(content_type="object"), looker, **kwargs)
 
         grouped_things = defaultdict(list)
         for thing in things:
             grouped_things[thing.get_display_name(looker, **kwargs)].append(thing)
 
         thing_names = []
         for thingname, thinglist in sorted(grouped_things.items()):
             nthings = len(thinglist)
             thing = thinglist[0]
             singular, plural = thing.get_numbered_name(nthings, looker, key=thingname)
             thing_names.append(singular if nthings == 1 else plural)
         thing_names = iter_to_str(thing_names)
-        return f"\n|wYou see:|n {thing_names}" if thing_names else ""
+        return f"|wYou see:|n {thing_names}" if thing_names else ""
 
     def get_display_footer(self, looker, **kwargs):
         """
         Get the 'footer' component of the object description. Called by `return_appearance`.
 
         Args:
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The footer display string.
 
         """
         return ""
 
     def format_appearance(self, appearance, looker, **kwargs):
         """
         Final processing of the entire appearance string. Called by `return_appearance`.
 
         Args:
             appearance (str): The compiled appearance string.
-            looker (Object): Object doing the looking.
+            looker (DefaultObject): Object doing the looking.
             **kwargs: Arbitrary data for use when overriding.
         Returns:
             str: The final formatted output.
 
         """
-        return appearance.strip()
+        return compress_whitespace(appearance).strip()
 
     def return_appearance(self, looker, **kwargs):
         """
         Main callback used by 'look' for the object to describe itself.
         This formats a description. By default, this looks for the `appearance_template`
         string set on this class and populates it with formatting keys
-            'name', 'desc', 'exits', 'characters', 'things' as well as
-            (currently empty) 'header'/'footer'. Each of these values are
-            retrieved by a matching method `.get_display_*`, such as `get_display_name`,
-            `get_display_footer` etc.
+        'name', 'desc', 'exits', 'characters', 'things' as well as
+        (currently empty) 'header'/'footer'. Each of these values are
+        retrieved by a matching method `.get_display_*`, such as `get_display_name`,
+        `get_display_footer` etc.
 
         Args:
-            looker (Object): Object doing the looking. Passed into all helper methods.
+            looker (DefaultObject): Object doing the looking. Passed into all helper methods.
             **kwargs (dict): Arbitrary, optional arguments for users
                 overriding the call. This is passed into all helper methods.
 
         Returns:
             str: The description of this entity. By default this includes
-                the entity's name, description and any contents inside it.
+            the entity's name, description and any contents inside it.
 
         Notes:
             To simply change the layout of how the object displays itself (like
             adding some line decorations or change colors of different sections),
             you can simply edit `.appearance_template`. You only need to override
             this method (and/or its helpers) if you want to change what is passed
             into the template or want the most control over output.
@@ -1839,97 +1849,96 @@
         Called just before cmdsets on this object are requested by the
         command handler. If changes need to be done on the fly to the
         cmdset before passing them on to the cmdhandler, this is the
         place to do it. This is called also if the object currently
         have no cmdsets.
 
         Keyword Args:
-            caller (Object, Account or Session): The object requesting the cmdsets.
+            caller (DefaultObject, DefaultAccount or Session): The object requesting the cmdsets.
             current (CmdSet): The current merged cmdset.
             force_init (bool): If `True`, force a re-build of the cmdset. (seems unused)
             **kwargs: Arbitrary input for overloads.
 
         """
         pass
 
     def get_cmdsets(self, caller, current, **kwargs):
         """
         Called by the CommandHandler to get a list of cmdsets to merge.
 
         Args:
-            caller (obj): The object requesting the cmdsets.
+            caller (DefaultObject): The object requesting the cmdsets.
             current (cmdset): The current merged cmdset.
             **kwargs: Arbitrary input for overloads.
 
         Returns:
             tuple: A tuple of (current, cmdsets), which is probably self.cmdset.current and self.cmdset.cmdset_stack
         """
         return self.cmdset.current, list(self.cmdset.cmdset_stack)
 
     def at_pre_puppet(self, account, session=None, **kwargs):
         """
         Called just before an Account connects to this object to puppet
         it.
 
         Args:
-            account (Account): This is the connecting account.
+            account (DefaultAccount): This is the connecting account.
             session (Session): Session controlling the connection.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     def at_post_puppet(self, **kwargs):
         """
         Called just after puppeting has been completed and all
         Account<->Object links have been established.
 
         Args:
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
-        Note:
-            You can use `self.account` and `self.sessions.get()` to get
-            account and sessions at this point; the last entry in the
-            list from `self.sessions.get()` is the latest Session
+        Notes:
+            You can use `self.account` and `self.sessions.get()` to get account and sessions at this
+            point; the last entry in the list from `self.sessions.get()` is the latest Session
             puppeting this Object.
 
         """
         self.msg(f"You become |w{self.key}|n.")
         self.account.db._last_puppet = self
 
     def at_pre_unpuppet(self, **kwargs):
         """
         Called just before beginning to un-connect a puppeting from
         this Account.
 
         Args:
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
-        Note:
+        Notes:
             You can use `self.account` and `self.sessions.get()` to get
             account and sessions at this point; the last entry in the
             list from `self.sessions.get()` is the latest Session
             puppeting this Object.
 
         """
         pass
 
     def at_post_unpuppet(self, account=None, session=None, **kwargs):
         """
         Called just after the Account successfully disconnected from
         this object, severing all connections.
 
         Args:
-            account (Account): The account object that just disconnected
+            account (DefaultAccount): The account object that just disconnected
                 from this object. This can be `None` if this is called
                 automatically (such as after a cleanup operation).
             session (Session): Session id controlling the connection that
                 just disconnected.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     def at_server_reload(self):
         """
@@ -1956,83 +1965,85 @@
         customize error messages in a central location or other effects
         based on the access result.
 
         Args:
             result (bool): The outcome of the access call.
             accessing_obj (Object or Account): The entity trying to gain access.
             access_type (str): The type of access that was requested.
-
-        Keyword Args:
-            Unused by default, added for possible expandability in a game.
+            **kwargs: Arbitrary, optional arguments. Unused by default.
 
         """
         pass
 
     # hooks called when moving the object
 
     def at_pre_move(self, destination, move_type="move", **kwargs):
         """
         Called just before starting to move this object to
         destination. Return False to abort move.
 
         Args:
-            destination (Object): The object we are moving to
+            destination (DefaultObject): The object we are moving to
             move_type (str): The type of move. "give", "traverse", etc.
                 This is an arbitrary string provided to obj.move_to().
                 Useful for altering messages or altering logic depending
                 on the kind of movement.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Returns:
             bool: If we should move or not.
 
         Notes:
-            If this method returns False/None, the move is cancelled
+            If this method returns `False` or `None`, the move is cancelled
             before it is even started.
 
         """
         return True
 
     def at_pre_object_leave(self, leaving_object, destination, **kwargs):
         """
         Called just before this object is about lose an object that was
         previously 'inside' it. Return False to abort move.
 
         Args:
-            leaving_object (Object): The object that is about to leave.
-            destination (Object): Where object is going to.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            leaving_object (DefaultObject): The object that is about to leave.
+            destination (DefaultObject): Where object is going to.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
         Returns:
             bool: If `leaving_object` should be allowed to leave or not.
 
-        Notes: If this method returns False, None, the move is canceled before
+        Notes:
+
+            If this method returns `False` or `None`, the move is canceled before
             it even started.
 
         """
         return True
 
     def at_pre_object_receive(self, arriving_object, source_location, **kwargs):
         """
         Called just before this object received another object. If this
         method returns `False`, the move is aborted and the moved entity
         remains where it was.
 
         Args:
-            arriving_object (Object): The object moved into this one
-            source_location (Object): Where `moved_object` came from.
+            arriving_object (DefaultObject): The object moved into this one
+            source_location (DefaultObject): Where `moved_object` came from.
                 Note that this could be `None`.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Returns:
             bool: If False, abort move and `moved_obj` remains where it was.
 
-        Notes: If this method returns False, None, the move is canceled before
+        Notes:
+
+            If this method returns `False` or `None`, the move is canceled before
             it even started.
 
         """
         return True
 
     # deprecated alias
     at_before_move = at_pre_move
@@ -2040,31 +2051,34 @@
     def announce_move_from(self, destination, msg=None, mapping=None, move_type="move", **kwargs):
         """
         Called if the move is to be announced. This is
         called while we are still standing in the old
         location.
 
         Args:
-            destination (Object): The place we are going to.
+            destination (DefaultObject): The place we are going to.
             msg (str, optional): a replacement message.
             mapping (dict, optional): additional mapping objects.
             move_type (str): The type of move. "give", "traverse", etc.
                 This is an arbitrary string provided to obj.move_to().
                 Useful for altering messages or altering logic depending
                 on the kind of movement.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
-        You can override this method and call its parent with a
-        message to simply change the default message.  In the string,
-        you can use the following as mappings (between braces):
-            object: the object which is moving.
-            exit: the exit from which the object is moving (if found).
-            origin: the location of the object before the move.
-            destination: the location of the object after moving.
+        Notes:
+
+            You can override this method and call its parent with a
+            message to simply change the default message.  In the string,
+            you can use the following as mappings:
+
+            - `{object}`: the object which is moving.
+            - `{exit}`: the exit from which the object is moving (if found).
+            - `{origin}`: the location of the object before the move.
+            - `{destination}`: the location of the object after moving.
 
         """
         if not self.location:
             return
         if msg:
             string = msg
         else:
@@ -2092,32 +2106,35 @@
 
     def announce_move_to(self, source_location, msg=None, mapping=None, move_type="move", **kwargs):
         """
         Called after the move if the move was not quiet. At this point
         we are standing in the new location.
 
         Args:
-            source_location (Object): The place we came from
+            source_location (DefaultObject): The place we came from
             msg (str, optional): the replacement message if location.
             mapping (dict, optional): additional mapping objects.
             move_type (str): The type of move. "give", "traverse", etc.
                 This is an arbitrary string provided to obj.move_to().
                 Useful for altering messages or altering logic depending
                 on the kind of movement.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
+
             You can override this method and call its parent with a
             message to simply change the default message.  In the string,
             you can use the following as mappings (between braces):
-                object: the object which is moving.
-                exit: the exit from which the object is moving (if found).
-                origin: the location of the object before the move.
-                destination: the location of the object after moving.
+
+
+            - `{object}`: the object which is moving.
+            - `{exit}`: the exit from which the object is moving (if found).
+            - `{origin}`: the location of the object before the move.
+            - `{destination}`: the location of the object after moving.
 
         """
 
         if not source_location and self.location.has_account:
             # This was created from nowhere and added to an account's
             # inventory; it's probably the result of a create command.
             string = _("You now have {name} in your possession.").format(
@@ -2163,58 +2180,58 @@
     def at_post_move(self, source_location, move_type="move", **kwargs):
         """
         Called after move has completed, regardless of quiet mode or
         not.  Allows changes to the object due to the location it is
         now in.
 
         Args:
-            source_location (Object): Where we came from. This may be `None`.
+            source_location (DefaultObject): Where we came from. This may be `None`.
             move_type (str): The type of move. "give", "traverse", etc.
                 This is an arbitrary string provided to obj.move_to().
                 Useful for altering messages or altering logic depending
                 on the kind of movement.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     # deprecated
     at_after_move = at_post_move
 
     def at_object_leave(self, moved_obj, target_location, move_type="move", **kwargs):
         """
         Called just before an object leaves from inside this object
 
         Args:
-            moved_obj (Object): The object leaving
-            target_location (Object): Where `moved_obj` is going.
+            moved_obj (DefaultObject): The object leaving
+            target_location (DefaultObject): Where `moved_obj` is going.
             move_type (str): The type of move. "give", "traverse", etc.
                 This is an arbitrary string provided to obj.move_to().
                 Useful for altering messages or altering logic depending
                 on the kind of movement.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     def at_object_receive(self, moved_obj, source_location, move_type="move", **kwargs):
         """
         Called after an object has been moved into this object.
 
         Args:
-            moved_obj (Object): The object moved into this one
-            source_location (Object): Where `moved_object` came from.
+            moved_obj (DefaultObject): The object moved into this one
+            source_location (DefaultObject): Where `moved_object` came from.
                 Note that this could be `None`.
             move_type (str): The type of move. "give", "traverse", etc.
                 This is an arbitrary string provided to obj.move_to().
                 Useful for altering messages or altering logic depending
                 on the kind of movement.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     def at_traverse(self, traversing_object, target_location, **kwargs):
         """
@@ -2223,31 +2240,31 @@
         `traversing_object.move_to(target_location)`. It is normally
         only implemented by Exit objects. If it returns False (usually
         because `move_to` returned False), `at_post_traverse` below
         should not be called and instead `at_failed_traverse` should be
         called.
 
         Args:
-            traversing_object (Object): Object traversing us.
-            target_location (Object): Where target is going.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            traversing_object (DefaultObject): Object traversing us.
+            target_location (DefaultObject): Where target is going.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     def at_post_traverse(self, traversing_object, source_location, **kwargs):
         """
         Called just after an object successfully used this object to
         traverse to another object (i.e. this object is a type of
         Exit)
 
         Args:
-            traversing_object (Object): The object traversing us.
-            source_location (Object): Where `traversing_object` came from.
+            traversing_object (DefaultObject): The object traversing us.
+            source_location (DefaultObject): Where `traversing_object` came from.
             **kwargs (dict): Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
             The target location should normally be available as `self.destination`.
         """
         pass
@@ -2257,16 +2274,16 @@
 
     def at_failed_traverse(self, traversing_object, **kwargs):
         """
         This is called if an object fails to traverse this object for
         some reason.
 
         Args:
-            traversing_object (Object): The object that failed traversing us.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            traversing_object (DefaultObject): The object that failed traversing us.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
             Using the default exits, this hook will not be called if an
             Attribute `err_traverse` is defined - this will in that case be
             read for an error string instead.
 
@@ -2285,17 +2302,15 @@
         Consider this a pre-processing method before msg is passed on
         to the user session. If this method returns False, the msg
         will not be passed on.
 
         Args:
             text (str, optional): The message received.
             from_obj (any, optional): The object sending the message.
-
-        Keyword Args:
-            This includes any keywords sent to the `msg` method.
+            **kwargs: This includes any keywords sent to the `msg` method.
 
         Returns:
             receive (bool): If this message should be received.
 
         Notes:
             If this method returns False, the `msg` operation
             will abort without sending the message.
@@ -2307,75 +2322,70 @@
         """
         This is a hook that is called when *this* object sends a
         message to another object with `obj.msg(text, to_obj=obj)`.
 
         Args:
             text (str, optional): Text to send.
             to_obj (any, optional): The object to send to.
-
-        Keyword Args:
-            Keywords passed from msg()
+            **kwargs: Keywords passed from msg().
 
         Notes:
             Since this method is executed by `from_obj`, if no `from_obj`
             was passed to `DefaultCharacter.msg` this hook will never
             get called.
 
         """
         pass
 
     # hooks called by the default cmdset.
 
     def get_visible_contents(self, looker, **kwargs):
         """
+        DEPRECATED
         Get all contents of this object that a looker can see (whatever that means, by default it
-        checks the 'view' and 'search' locks), grouped by type. Helper method to return_appearance.
+        checks the 'view' and 'search' locks and excludes the looker themselves), grouped by type.
+        Helper method to return_appearance.
 
         Args:
-            looker (Object): The entity looking.
-            **kwargs (any): Passed from `return_appearance`. Unused by default.
+            looker (DefaultObject): The entity looking.
+            **kwargs: Passed from `return_appearance`. Unused by default.
 
         Returns:
             dict: A dict of lists categorized by type. Byt default this
-                contains 'exits', 'characters' and 'things'. The elements of these
-                lists are the actual objects.
+            contains 'exits', 'characters' and 'things'. The elements of these
+            lists are the actual objects.
 
         """
 
-        def filter_visible(obj_list):
-            return [
-                obj
-                for obj in obj_list
-                if obj != looker
-                and obj.access(looker, "view")
-                and obj.access(looker, "search", default=True)
-            ]
+        def _filter_visible(obj_list):
+            return [obj for obj in self.filter_visible(obj_list, looker, **kwargs) if obj != looker]
 
         return {
-            "exits": filter_visible(self.contents_get(content_type="exit")),
-            "characters": filter_visible(self.contents_get(content_type="character")),
-            "things": filter_visible(self.contents_get(content_type="object")),
+            "exits": _filter_visible(self.contents_get(content_type="exit")),
+            "characters": _filter_visible(self.contents_get(content_type="character")),
+            "things": _filter_visible(self.contents_get(content_type="object")),
         }
 
     def get_content_names(self, looker, **kwargs):
         """
+        DEPRECATED
         Get the proper names for all contents of this object. Helper method
         for return_appearance.
 
         Args:
-            looker (Object): The entity looking.
-            **kwargs (any): Passed from `return_appearance`. Passed into
+            looker (DefaultObject): The entity looking.
+            **kwargs: Passed from `return_appearance`. Passed into
                 `get_display_name` for each found entity.
 
         Returns:
             dict: A dict of lists categorized by type. Byt default this
-                contains 'exits', 'characters' and 'things'. The elements
-                of these lists are strings - names of the objects that
-                can depend on the looker and also be grouped in the case
-                of multiple same-named things etc.
+            contains 'exits', 'characters' and 'things'. The elements
+            of these lists are strings - names of the objects that
+            can depend on the looker and also be grouped in the case
+            of multiple same-named things etc.
 
         Notes:
             This method shouldn't add extra coloring to the names beyond what is
             already given by the .get_display_name() (and the .name field) already.
             Per-type coloring can be applied in `return_appearance`.
 
         """
@@ -2405,25 +2415,24 @@
     def at_look(self, target, **kwargs):
         """
         Called when this object performs a look. It allows to
         customize just what this means. It will not itself
         send any data.
 
         Args:
-            target (Object): The target being looked at. This is
+            target (DefaultObject): The target being looked at. This is
                 commonly an object or the current location. It will
                 be checked for the "view" type access.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call. This will be passed into
                 return_appearance, get_display_name and at_desc but is not used
                 by default.
 
         Returns:
-            lookstring (str): A ready-processed look string
-                potentially ready to return to the looker.
+            str: A ready-processed look string potentially ready to return to the looker.
 
         """
         if not target.access(self, "view"):
             try:
                 return "Could not view '%s'." % target.get_display_name(self, **kwargs)
             except AttributeError:
                 return "Could not view '%s'." % target.key
@@ -2438,32 +2447,32 @@
 
     def at_desc(self, looker=None, **kwargs):
         """
         This is called whenever someone looks at this object.
 
         Args:
             looker (Object, optional): The object requesting the description.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         pass
 
     def at_pre_get(self, getter, **kwargs):
         """
         Called by the default `get` command before this object has been
         picked up.
 
         Args:
-            getter (Object): The object about to get this object.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            getter (DefaultObject): The object about to get this object.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Returns:
-            shouldget (bool): If the object should be gotten or not.
+            bool: If the object should be gotten or not.
 
         Notes:
             If this method returns False/None, the getting is cancelled
             before it is even started.
         """
         return True
 
@@ -2472,16 +2481,16 @@
 
     def at_get(self, getter, **kwargs):
         """
         Called by the default `get` command when this object has been
         picked up.
 
         Args:
-            getter (Object): The object getting this object.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            getter (DefaultObject): The object getting this object.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
             This hook cannot stop the pickup from happening. Use
             permissions or the at_pre_get() hook for that.
 
         """
@@ -2489,41 +2498,41 @@
 
     def at_pre_give(self, giver, getter, **kwargs):
         """
         Called by the default `give` command before this object has been
         given.
 
         Args:
-            giver (Object): The object about to give this object.
-            getter (Object): The object about to get this object.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            giver (DefaultObject): The object about to give this object.
+            getter (DefaultObject): The object about to get this object.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Returns:
             shouldgive (bool): If the object should be given or not.
 
         Notes:
-            If this method returns False/None, the giving is cancelled
+            If this method returns `False` or `None`, the giving is cancelled
             before it is even started.
 
         """
         return True
 
     # deprecated
     at_before_give = at_pre_give
 
     def at_give(self, giver, getter, **kwargs):
         """
         Called by the default `give` command when this object has been
         given.
 
         Args:
-            giver (Object): The object giving this object.
-            getter (Object): The object getting this object.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            giver (DefaultObject): The object giving this object.
+            getter (DefaultObject): The object getting this object.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
             This hook cannot stop the give from happening. Use
             permissions or the at_pre_give() hook for that.
 
         """
@@ -2531,23 +2540,23 @@
 
     def at_pre_drop(self, dropper, **kwargs):
         """
         Called by the default `drop` command before this object has been
         dropped.
 
         Args:
-            dropper (Object): The object which will drop this object.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            dropper (DefaultObject): The object which will drop this object.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Returns:
-            shoulddrop (bool): If the object should be dropped or not.
+            bool: If the object should be dropped or not.
 
         Notes:
-            If this method returns False/None, the dropping is cancelled
+            If this method returns `False` or `None`, the dropping is cancelled
             before it is even started.
 
         """
         if not self.locks.get("drop"):
             # TODO: This if-statment will be removed in Evennia 1.0
             return True
         if not self.access(dropper, "drop", default=False):
@@ -2560,16 +2569,16 @@
 
     def at_drop(self, dropper, **kwargs):
         """
         Called by the default `drop` command when this object has been
         dropped.
 
         Args:
-            dropper (Object): The object which just dropped this object.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            dropper (DefaultObject): The object which just dropped this object.
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
             This hook cannot stop the drop from happening. Use
             permissions or the at_pre_drop() hook for that.
 
         """
@@ -2587,19 +2596,19 @@
         Args:
             message (str): The suggested say/whisper text spoken by self.
         Keyword Args:
             whisper (bool): If True, this is a whisper rather than
                 a say. This is sent by the whisper command by default.
                 Other verbal commands could use this hook in similar
                 ways.
-            receivers (Object or iterable): If set, this is the target or targets for the
+            receivers (DefaultObject or iterable): If set, this is the target or targets for the
                 say/whisper.
 
         Returns:
-            message (str): The (possibly modified) text to be spoken.
+            str: The (possibly modified) text to be spoken.
 
         """
         return message
 
     # deprecated
     at_before_say = at_pre_say
 
@@ -2622,42 +2631,44 @@
         re-writing it completely.
 
         Args:
             message (str): The message to convey.
             msg_self (bool or str, optional): If boolean True, echo `message` to self. If a string,
                 return that message. If False or unset, don't echo to self.
             msg_location (str, optional): The message to echo to self's location.
-            receivers (Object or iterable, optional): An eventual receiver or receivers of the
+            receivers (DefaultObject or iterable, optional): An eventual receiver or receivers of the
                 message (by default only used by whispers).
             msg_receivers(str): Specific message to pass to the receiver(s). This will parsed
                 with the {receiver} placeholder replaced with the given receiver.
         Keyword Args:
             whisper (bool): If this is a whisper rather than a say. Kwargs
                 can be used by other verbal commands in a similar way.
             mapping (dict): Pass an additional mapping to the message.
 
         Notes:
 
 
             Messages can contain {} markers. These are substituted against the values
             passed in the `mapping` argument.
+            ::
 
                 msg_self = 'You say: "{speech}"'
                 msg_location = '{object} says: "{speech}"'
                 msg_receivers = '{object} whispers: "{speech}"'
 
             Supported markers by default:
-                {self}: text to self-reference with (default 'You')
-                {speech}: the text spoken/whispered by self.
-                {object}: the object speaking.
-                {receiver}: replaced with a single receiver only for strings meant for a specific
-                    receiver (otherwise 'None').
-                {all_receivers}: comma-separated list of all receivers,
-                                 if more than one, otherwise same as receiver
-                {location}: the location where object is.
+
+            - {self}: text to self-reference with (default 'You')
+            - {speech}: the text spoken/whispered by self.
+            - {object}: the object speaking.
+            - {receiver}: replaced with a single receiver only for strings meant for a specific
+              receiver (otherwise 'None').
+            - {all_receivers}: comma-separated list of all receivers,
+              if more than one, otherwise same as receiver
+            - {location}: the location where object is.
 
         """
         msg_type = "say"
         if kwargs.get("whisper", False):
             # whisper mode
             msg_type = "whisper"
             msg_self = (
@@ -2678,17 +2689,19 @@
 
         if msg_self:
             self_mapping = {
                 "self": "You",
                 "object": self.get_display_name(self),
                 "location": location.get_display_name(self) if location else None,
                 "receiver": None,
-                "all_receivers": ", ".join(recv.get_display_name(self) for recv in receivers)
-                if receivers
-                else None,
+                "all_receivers": (
+                    ", ".join(recv.get_display_name(self) for recv in receivers)
+                    if receivers
+                    else None
+                ),
                 "speech": message,
             }
             self_mapping.update(custom_mapping)
             self.msg(text=(msg_self.format_map(self_mapping), {"type": msg_type}), from_obj=self)
 
         if receivers and msg_receivers:
             receiver_mapping = {
@@ -2700,17 +2713,19 @@
                 "speech": message,
             }
             for receiver in make_iter(receivers):
                 individual_mapping = {
                     "object": self.get_display_name(receiver),
                     "location": location.get_display_name(receiver),
                     "receiver": receiver.get_display_name(receiver),
-                    "all_receivers": ", ".join(recv.get_display_name(recv) for recv in receivers)
-                    if receivers
-                    else None,
+                    "all_receivers": (
+                        ", ".join(recv.get_display_name(recv) for recv in receivers)
+                        if receivers
+                        else None
+                    ),
                 }
                 receiver_mapping.update(individual_mapping)
                 receiver_mapping.update(custom_mapping)
                 receiver.msg(
                     text=(msg_receivers.format_map(receiver_mapping), {"type": msg_type}),
                     from_obj=self,
                 )
@@ -2765,20 +2780,21 @@
     def get_default_lockstring(
         cls, account: "DefaultAccount" = None, caller: "DefaultObject" = None, **kwargs
     ):
         """
         Classmethod called during .create() to determine default locks for the object.
 
         Args:
-            account (Account): Account to attribute this object to.
+            account (DefaultAccount): Account to attribute this object to.
             caller (DefaultObject): The object which is creating this one.
             **kwargs: Arbitrary input.
 
         Returns:
-            lockstring (str): A lockstring to use for this object.
+            str: A lockstring to use for this object.
+
         """
         pid = f"pid({account.id})" if account else None
         character = kwargs.get("character", None)
         cid = f"id({character})" if character else None
 
         puppet = "puppet:" + " or ".join(
             [x for x in [pid, cid, "perm(Developer)", "pperm(Developer)"] if x]
@@ -2882,42 +2898,50 @@
             logger.log_err(e)
 
         return obj, errors
 
     @classmethod
     def normalize_name(cls, name):
         """
-        Normalize the character name prior to creating. Note that this should be refactored to
-        support i18n for non-latin scripts, but as we (currently) have no bug reports requesting
-        better support of non-latin character sets, requiring character names to be latinified is an
-        acceptable option.
+        Normalize the character name prior to creating.
 
         Args:
             name (str) : The name of the character
 
         Returns:
-            latin_name (str) : A valid name.
+            str : A valid, latinized name.
+
+        Notes:
+
+            The main purpose of this is to make sure that character names are not created with
+            special unicode characters that look visually identical to latin charaters. This could
+            be used to impersonate other characters.
+
+            This method should be refactored to support i18n for non-latin names, but as we
+            (currently) have no bug reports requesting better support of non-latin character sets,
+            requiring character names to be latinified is an acceptable default option.
+
         """
 
         from evennia.utils.utils import latinify
 
         latin_name = latinify(name, default="X")
         return latin_name
 
     @classmethod
     def validate_name(cls, name, account=None) -> typing.Optional[str]:
         """
         Validate the character name prior to creating. Overload this function to add custom validators
 
         Args:
             name (str) : The name of the character
-        Kwargs:
+        Keyword Args:
             account (DefaultAccount, optional) : The account creating the character.
         Returns:
-            error (str, optional) : A non-empty error message if there is a problem, otherwise False.
+            str or None: A non-empty error message if there is a problem, otherwise `None`.
 
         """
         if account and cls.objects.filter_family(db_key__iexact=name):
             return f"|rA character named '|w{name}|r' already exists.|n"
 
     def basetype_setup(self):
         """
@@ -2954,15 +2978,15 @@
     # deprecated
     at_after_move = at_post_move
 
     def at_pre_puppet(self, account, session=None, **kwargs):
         """
         Return the character from storage in None location in `at_post_unpuppet`.
         Args:
-            account (Account): This is the connecting account.
+            account (DefaultAccount): This is the connecting account.
             session (Session): Session controlling the connection.
 
         """
         if self.location is None:
             # Make sure character's location is never None before being puppeted.
             # Return to last location (or home, which should always exist)
             location = self.db.prelogout_location if self.db.prelogout_location else self.home
@@ -2981,15 +3005,16 @@
         """
         Called just after puppeting has been completed and all
         Account<->Object links have been established.
 
         Args:
             **kwargs (dict): Arbitrary, optional arguments for users
                 overriding the call (unused by default).
-        Note:
+        Notes:
+
             You can use `self.account` and `self.sessions.get()` to get
             account and sessions at this point; the last entry in the
             list from `self.sessions.get()` is the latest Session
             puppeting this Object.
 
         """
         self.msg(_("\nYou become |c{name}|n.\n").format(name=self.key))
@@ -3006,23 +3031,24 @@
     def at_post_unpuppet(self, account=None, session=None, **kwargs):
         """
         We stove away the character when the account goes ooc/logs off,
         otherwise the character object will remain in the room also
         after the account logged off ("headless", so to say).
 
         Args:
-            account (Account): The account object that just disconnected
+            account (DefaultAccount): The account object that just disconnected
                 from this object.
             session (Session): Session controlling the connection that
                 just disconnected.
         Keyword Args:
             reason (str): If given, adds a reason for the unpuppet. This
                 is set when the user is auto-unpuppeted due to being link-dead.
-            **kwargs (dict): Arbitrary, optional arguments for users
+            **kwargs: Arbitrary, optional arguments for users
                 overriding the call (unused by default).
+
         """
         if not self.sessions.count():
             # only remove this char from grid if no sessions control it anymore.
             if self.location:
 
                 def message(obj, from_obj):
                     obj.msg(
@@ -3100,16 +3126,17 @@
                 object (along with normal Admin perms). If not given, default
             caller (DefaultObject): The object which is creating this one.
             description (str): Brief description for this object.
             ip (str): IP address of creator (for object auditing).
             method (str): The method used to create the room. Defaults to "create".
 
         Returns:
-            room (Object): A newly created Room of the given typeclass.
-            errors (list): A list of errors in string form, if any.
+            tuple: A tuple `(Object, error)` with the newly created Room of the given typeclass,
+            or `None` if there was an error. If there was an error, `error` will be a list of
+            error strings.
 
         """
         errors = []
         obj = None
 
         # Get IP address of creator, if available
         ip = kwargs.pop("ip", "")
@@ -3153,16 +3180,15 @@
             errors.append(f"An error occurred while creating this '{key}' object: {e}")
             logger.log_err(e)
 
         return obj, errors
 
     def basetype_setup(self):
         """
-        Simple room setup setting locks to make sure the room
-        cannot be picked up.
+        Simple room setup setting locks to make sure the room cannot be picked up.
 
         """
 
         super().basetype_setup()
         self.locks.add(
             ";".join(["get:false()", "puppet:false()", "teleport:false()", "teleport_here:true()"])
         )  # would be weird to puppet a room ...
@@ -3202,21 +3228,21 @@
                 self.obj.at_failed_traverse(self.caller)
 
     def get_extra_info(self, caller, **kwargs):
         """
         Shows a bit of information on where the exit leads.
 
         Args:
-            caller (Object): The object (usually a character) that entered an ambiguous command.
+            caller (DefaultObject): The object (usually a character) that entered an ambiguous command.
             **kwargs (dict): Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Returns:
-            A string with identifying information to disambiguate the command, conventionally with a
-            preceding space.
+            str: A string with identifying information to disambiguate the command, conventionally
+            with a preceding space.
 
         """
         if self.obj.destination:
             return " (exit to %s)" % self.obj.destination.get_display_name(caller, **kwargs)
         else:
             return " (%s)" % self.obj.get_display_name(caller, **kwargs)
 
@@ -3250,15 +3276,15 @@
         Helper function for creating an exit command set + command.
 
         The command of this cmdset has the same name as the Exit
         object and allows the exit to react when the account enter the
         exit's name, triggering the movement between rooms.
 
         Args:
-            exidbobj (Object): The DefaultExit object to base the command on.
+            exidbobj (DefaultObject): The DefaultExit object to base the command on.
 
         """
 
         # create an exit command. We give the properties here,
         # to always trigger metaclass preparations
         cmd = self.exit_command(
             key=exidbobj.db_key.strip().lower(),
@@ -3300,23 +3326,24 @@
 
         Args:
             key (str): Name of the new Exit, as it should appear from the
                 source room.
             location (Room): The room to create this exit in.
 
         Keyword Args:
-            account (AccountDB): Account to associate this Exit with.
-            caller (ObjectDB): The Object creating this Object.
+            account (DefaultAccountDB): Account to associate this Exit with.
+            caller (DefaultObject): The Object creating this Object.
             description (str): Brief description for this object.
             ip (str): IP address of creator (for object auditing).
             destination (Room): The room to which this exit should go.
 
         Returns:
-            exit (Object): A newly created Room of the given typeclass.
-            errors (list): A list of errors in string form, if any.
+            tuple: A tuple `(Object, errors)`, where the object is the newly
+            created exit of the given typeclass, or `None` if there was an error.
+            If there was an error, `errors` will be a list of error strings.
 
         """
         errors = []
         obj = None
 
         # Get IP address of creator, if available
         ip = kwargs.pop("ip", "")
@@ -3362,15 +3389,15 @@
             errors.append(f"An error occurred while creating this '{key}' object: {e}")
             logger.log_err(e)
 
         return obj, errors
 
     def basetype_setup(self):
         """
-        Setup exit-security
+        Setup exit-security.
 
         You should normally not need to overload this - if you do make
         sure you include all the functionality in this method.
 
         """
         super().basetype_setup()
 
@@ -3396,15 +3423,15 @@
         Called just before cmdsets on this object are requested by the
         command handler. If changes need to be done on the fly to the
         cmdset before passing them on to the cmdhandler, this is the
         place to do it. This is called also if the object currently
         has no cmdsets.
 
         Keyword Args:
-            caller (Object, Account or Session): The object requesting the cmdsets.
+            caller (DefaultObject, DefaultAccount or Session): The object requesting the cmdsets.
             current (CmdSet): The current merged cmdset.
             force_init (bool): If `True`, force a re-build of the cmdset
                 (for example to update aliases).
 
         """
 
         if "force_init" in kwargs or not self.cmdset.has_cmdset("ExitCmdSet", must_be_default=True):
@@ -3412,25 +3439,26 @@
             self.cmdset.add_default(self.create_exit_cmdset(self), persistent=False)
 
     def at_init(self):
         """
         This is called when this objects is re-loaded from cache. When
         that happens, we make sure to remove any old ExitCmdSet cmdset
         (this most commonly occurs when renaming an existing exit)
+
         """
         self.cmdset.remove_default()
 
     def at_traverse(self, traversing_object, target_location, **kwargs):
         """
         This implements the actual traversal. The traverse lock has
         already been checked (in the Exit command) at this point.
 
         Args:
-            traversing_object (Object): Object traversing us.
-            target_location (Object): Where target is going.
+            traversing_object (DefaultObject): Object traversing us.
+            target_location (DefaultObject): Where target is going.
             **kwargs (dict): Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         """
         source_location = traversing_object.location
         if traversing_object.move_to(target_location, move_type="traverse", exit_obj=self):
             self.at_post_traverse(traversing_object, source_location)
@@ -3443,15 +3471,15 @@
                 self.at_failed_traverse(traversing_object)
 
     def at_failed_traverse(self, traversing_object, **kwargs):
         """
         Overloads the default hook to implement a simple default error message.
 
         Args:
-            traversing_object (Object): The object that failed traversing us.
+            traversing_object (DefaultObject): The object that failed traversing us.
             **kwargs (dict): Arbitrary, optional arguments for users
                 overriding the call (unused by default).
 
         Notes:
             Using the default exits, this hook will not be called if an
             Attribute `err_traverse` is defined - this will in that case be
             read for an error string instead.
@@ -3462,16 +3490,18 @@
     def get_return_exit(self, return_all=False):
         """
         Get the exits that pair with this one in its destination room
         (i.e. returns to its location)
 
         Args:
             return_all (bool): Whether to return available results as a
-                               list or single matching exit.
+                               queryset or single matching exit.
 
         Returns:
-            queryset or exit (Exit): The matching exit(s).
+            Exit or queryset: The matching exit(s). If `return_all` is `True`, this
+            will be a queryset of all matching exits. Otherwise, it will be the first Exit matched.
+
         """
         query = ObjectDB.objects.filter(db_location=self.destination, db_destination=self.location)
         if return_all:
             return query
         return query.first()
```

### Comparing `evennia-4.0.0/evennia/objects/tests.py` & `evennia-4.1.0/evennia/objects/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,20 @@
             f" perm(Admin);edit:pid({self.account.id}) or perm(Admin)"
         )
         self.assertEqual(
             DefaultCharacter.get_default_lockstring(account=self.account, caller=self.char1),
             pattern,
         )
 
+    def test_get_name_without_article(self):
+        self.assertEqual(self.obj1.get_numbered_name(1, self.char1, return_string=True), "an Obj")
+        self.assertEqual(
+            self.obj1.get_numbered_name(1, self.char1, return_string=True, no_article=True), "Obj"
+        )
+
 
 class TestObjectManager(BaseEvenniaTest):
     "Test object manager methods"
 
     def test_get_object_with_account(self):
         query = ObjectDB.objects.get_object_with_account("TestAccount").first()
         self.assertEqual(query, self.char1)
```

### Comparing `evennia-4.0.0/evennia/prototypes/README.md` & `evennia-4.1.0/evennia/prototypes/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/prototypes/menus.py` & `evennia-4.1.0/evennia/prototypes/menus.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/prototypes/protfuncs.py` & `evennia-4.1.0/evennia/prototypes/protfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/prototypes/prototypes.py` & `evennia-4.1.0/evennia/prototypes/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/prototypes/spawner.py` & `evennia-4.1.0/evennia/prototypes/spawner.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,14 @@
 in code. To replace a default prototype, add the same-name prototype in a
 custom module read later in the settings.PROTOTYPE_MODULES list. To remove a default
 prototype, override its name with an empty dict.
 
 
 """
 
-
 import copy
 import hashlib
 import time
 
 from django.conf import settings
 from django.utils.translation import gettext as _
```

### Comparing `evennia-4.0.0/evennia/prototypes/tests.py` & `evennia-4.1.0/evennia/prototypes/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/manager.py` & `evennia-4.1.0/evennia/scripts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0001_initial.py` & `evennia-4.1.0/evennia/scripts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0002_auto_20150118_1625.py` & `evennia-4.1.0/evennia/scripts/migrations/0002_auto_20150118_1625.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py` & `evennia-4.1.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0004_auto_20150306_1354.py` & `evennia-4.1.0/evennia/scripts/migrations/0004_auto_20150306_1354.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0006_auto_20150310_2249.py` & `evennia-4.1.0/evennia/scripts/migrations/0006_auto_20150310_2249.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0008_auto_20170606_1731.py` & `evennia-4.1.0/evennia/scripts/migrations/0008_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0009_scriptdb_db_account.py` & `evennia-4.1.0/evennia/scripts/migrations/0009_scriptdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0010_auto_20170705_1736.py` & `evennia-4.1.0/evennia/scripts/migrations/0010_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py` & `evennia-4.1.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0012_auto_20190128_1820.py` & `evennia-4.1.0/evennia/scripts/migrations/0012_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0013_auto_20191025_0831.py` & `evennia-4.1.0/evennia/scripts/migrations/0013_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0014_auto_20210520_2137.py` & `evennia-4.1.0/evennia/scripts/migrations/0014_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/migrations/0015_convert_contrib_paths.py` & `evennia-4.1.0/evennia/scripts/migrations/0015_convert_contrib_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/models.py` & `evennia-4.1.0/evennia/scripts/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 - Switch to a different state, such as entering a text editor,
   start combat or enter a dark room.
 - Merge a new cmdset with the default one for changing which
   commands are available at a particular time
 - Give the account/object a time-limited bonus/effect
 
 """
+
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 
 from evennia.scripts.manager import ScriptDBManager
 from evennia.typeclasses.models import TypedObject
 from evennia.utils.utils import dbref, to_str
```

### Comparing `evennia-4.0.0/evennia/scripts/monitorhandler.py` & `evennia-4.1.0/evennia/scripts/monitorhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 - Field-monitor - track a object's specific database field and perform
     an action whenever that field *changes* for whatever reason.
 - Attribute-monitor tracks an object's specific Attribute and perform
     an action whenever that Attribute *changes* for whatever reason.
 
 """
+
 import inspect
 from collections import defaultdict
 
 from evennia.server.models import ServerConfig
 from evennia.utils import logger, variable_from_module
 from evennia.utils.dbserialize import dbserialize, dbunserialize
```

### Comparing `evennia-4.0.0/evennia/scripts/ondemandhandler.py` & `evennia-4.1.0/evennia/scripts/ondemandhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/scripthandler.py` & `evennia-4.1.0/evennia/scripts/scripthandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The script handler makes sure to check through all stored scripts to
 make sure they are still relevant. A scripthandler is automatically
 added to all game objects. You access it through the property
 `scripts` on the game object.
 
 """
+
 from django.utils.translation import gettext as _
 
 from evennia.scripts.models import ScriptDB
 from evennia.utils import create, logger
 
 
 class ScriptHandler(object):
```

### Comparing `evennia-4.0.0/evennia/scripts/scripts.py` & `evennia-4.1.0/evennia/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/scripts/taskhandler.py` & `evennia-4.1.0/evennia/scripts/taskhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,14 @@
             task_id (int): global task id for this task.
 
         """
         return self.task_id
 
 
 class TaskHandler:
-
     """A light singleton wrapper allowing to access permanent tasks.
 
     When `utils.delay` is called, the task handler is used to create
     the task.
 
     Task handler will automatically remove uncalled but canceled from task
     handler. By default this will not occur until a canceled task
```

### Comparing `evennia-4.0.0/evennia/scripts/tests.py` & `evennia-4.1.0/evennia/scripts/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 Unit tests for the scripts package
 
 """
 
 from collections import defaultdict
 from unittest import TestCase, mock
 
+from parameterized import parameterized
+
 from evennia import DefaultScript
 from evennia.objects.objects import DefaultObject
 from evennia.scripts.manager import ScriptDBManager
 from evennia.scripts.models import ObjectDoesNotExist, ScriptDB
 from evennia.scripts.monitorhandler import MonitorHandler
 from evennia.scripts.ondemandhandler import OnDemandHandler, OnDemandTask
 from evennia.scripts.scripts import DoNothing, ExtendedLoopingCall
 from evennia.scripts.tickerhandler import TickerHandler
 from evennia.utils.create import create_script
 from evennia.utils.dbserialize import dbserialize
 from evennia.utils.test_resources import BaseEvenniaTest, EvenniaTest
-from parameterized import parameterized
 
 
 class TestScript(BaseEvenniaTest):
     def test_create(self):
         "Check the script can be created via the convenience method."
         with mock.patch("evennia.scripts.scripts.DefaultScript.at_init") as mockinit:
             obj, errors = DefaultScript.create("useless-machine")
```

### Comparing `evennia-4.0.0/evennia/scripts/tickerhandler.py` & `evennia-4.1.0/evennia/scripts/tickerhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 ```
 
 If one wants to duplicate TICKER_HANDLER's auto-saving feature in
 a  custom handler one can make a custom `AT_STARTSTOP_MODULE` entry to
 call the handler's `save()` and `restore()` methods when the server reboots.
 
 """
+
 import inspect
 
 from django.core.exceptions import ObjectDoesNotExist
 from twisted.internet.defer import inlineCallbacks
 
 from evennia.scripts.scripts import ExtendedLoopingCall
 from evennia.server.models import ServerConfig
```

### Comparing `evennia-4.0.0/evennia/server/amp_client.py` & `evennia-4.1.0/evennia/server/amp_client.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/connection_wizard.py` & `evennia-4.1.0/evennia/server/connection_wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Link Evennia to external resources (wizard plugin for evennia_launcher)
 
 """
+
 import pprint
 import sys
 from os import path
 
 from django.conf import settings
 
 from evennia.utils.utils import list_to_string, mod_import
```

### Comparing `evennia-4.0.0/evennia/server/deprecations.py` & `evennia-4.1.0/evennia/server/deprecations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module contains historical deprecations that the Evennia launcher
 checks for.
 
 These all print to the terminal.
 """
+
 import os
 
 
 def check_errors(settings):
     """
     Check for deprecations that are critical errors and should stop
     the launcher.
```

### Comparing `evennia-4.0.0/evennia/server/evennia_launcher.py` & `evennia-4.1.0/evennia/server/evennia_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/game_index_client/README.md` & `evennia-4.1.0/evennia/server/game_index_client/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/game_index_client/client.py` & `evennia-4.1.0/evennia/server/portal/ttype.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,191 @@
 """
-The client for sending data to the Evennia Game Index
+TTYPE (MTTS) - Mud Terminal Type Standard
+
+This module implements the TTYPE telnet protocol as per
+http://tintin.sourceforge.net/mtts/. It allows the server to ask the
+client about its capabilities. If the client also supports TTYPE, it
+will return with information such as its name, if it supports colour
+etc. If the client does not support TTYPE, this will be ignored.
+
+All data will be stored on the protocol's protocol_flags dictionary,
+under the 'TTYPE' key.
 
 """
-import platform
-import urllib.error
-import urllib.parse
-import urllib.request
-
-import django
-from django.conf import settings
-from twisted.internet import defer, protocol, reactor
-from twisted.internet.defer import inlineCallbacks
-from twisted.web.client import Agent, HTTPConnectionPool, _HTTP11ClientFactory
-from twisted.web.http_headers import Headers
-from twisted.web.iweb import IBodyProducer
-from zope.interface import implementer
-
-import evennia
-from evennia.accounts.models import AccountDB
-from evennia.utils import get_evennia_version, logger
 
-_EGI_HOST = "http://evennia-game-index.appspot.com"
-_EGI_REPORT_PATH = "/api/v1/game/check_in"
+# telnet option codes
+TTYPE = bytes([24])  # b"\x18"
+IS = bytes([0])  # b"\x00"
+SEND = bytes([1])  # b"\x01"
 
+# terminal capabilities and their codes
+MTTS = [
+    (2048, "SSL"),
+    (1024, "MSLP"),
+    (512, "MNES"),
+    (256, "TRUECOLOR"),
+    (128, "PROXY"),
+    (64, "SCREENREADER"),
+    (32, "OSC_COLOR_PALETTE"),
+    (16, "MOUSE_TRACKING"),
+    (8, "XTERM256"),
+    (4, "UTF-8"),
+    (2, "VT100"),
+    (1, "ANSI"),
+]
 
-class EvenniaGameIndexClient:
+
+class Ttype:
     """
-    This client class is used for gathering and sending game details to the
-    Evennia Game Index. Since EGI is in the early goings, this isn't
-    incredibly configurable as far as to what is being sent.
+    Handles ttype negotiations. Called and initiated by the
+    telnet protocol.
+
     """
 
-    def __init__(self, on_bad_request=None):
+    def __init__(self, protocol):
         """
-        on_bad_request (callable, optional): Callable to trigger when a bad request was sent.
+        Initialize ttype by storing protocol on ourselves and calling
+        the client to see if it supporst ttype.
 
-        """
-        self.report_host = _EGI_HOST
-        self.report_path = _EGI_REPORT_PATH
-        self.report_url = self.report_host + self.report_path
-        self.logged_first_connect = False
+        Args:
+            protocol (Protocol): The protocol instance.
 
-        self._on_bad_request = on_bad_request
-        # Oh, the humanity. Silence the factory start/stop messages.
-        self._conn_pool = HTTPConnectionPool(reactor)
-        self._conn_pool._factory = QuietHTTP11ClientFactory
+        Notes:
+            The `self.ttype_step` indicates how far in the data
+            retrieval we've gotten.
 
-    @inlineCallbacks
-    def send_game_details(self):
-        """
-        This is where the magic happens. Send details about the game to the
-        Evennia Game Index.
         """
-        status_code, response_body = yield self._form_and_send_request()
-        if status_code == 200:
-            if not self.logged_first_connect:
-                logger.log_infomsg("Successfully sent game details to Evennia Game Index.")
-                self.logged_first_connect = True
-            return
-        # At this point, either EGD is having issues or the payload we sent
-        # is improperly formed (probably due to mis-configuration).
-        logger.log_errmsg(
-            "Failed to send game details to Evennia Game Index. HTTP "
-            "status code was %s. Message was: %s" % (status_code, response_body)
-        )
-
-        if status_code == 400 and self._on_bad_request:
-            # Improperly formed request. Defer to the callback as far as what
-            # to do. Probably not a great idea to continue attempting to send
-            # to EGD, though.
-            self._on_bad_request()
-
-    def _form_and_send_request(self):
-        """
-        Build the request to send to the index.
-
-        """
-        agent = Agent(reactor, pool=self._conn_pool)
-        headers = {
-            b"User-Agent": [b"Evennia Game Index Client"],
-            b"Content-Type": [b"application/x-www-form-urlencoded"],
-        }
-        egi_config = settings.GAME_INDEX_LISTING
-        # We are using `or` statements below with dict.get() to avoid sending
-        # stringified 'None' values to the server.
-        try:
-            values = {
-                # Game listing stuff
-                "game_name": egi_config.get("game_name", settings.SERVERNAME),
-                "game_status": egi_config["game_status"],
-                "game_website": egi_config.get("game_website", ""),
-                "short_description": egi_config["short_description"],
-                "long_description": egi_config.get("long_description", ""),
-                "listing_contact": egi_config["listing_contact"],
-                # How to play
-                "telnet_hostname": egi_config.get("telnet_hostname", ""),
-                "telnet_port": egi_config.get("telnet_port", ""),
-                "web_client_url": egi_config.get("web_client_url", ""),
-                # Game stats
-                "connected_account_count": evennia.SESSION_HANDLER.account_count(),
-                "total_account_count": AccountDB.objects.num_total_accounts() or 0,
-                # System info
-                "evennia_version": get_evennia_version(),
-                "python_version": platform.python_version(),
-                "django_version": django.get_version(),
-                "server_platform": platform.platform(),
-            }
-        except KeyError as err:
-            raise KeyError(f"Error loading GAME_INDEX_LISTING: {err}")
-
-        data = urllib.parse.urlencode(values)
-
-        d = agent.request(
-            b"POST",
-            bytes(self.report_url, "utf-8"),
-            headers=Headers(headers),
-            bodyProducer=StringProducer(data),
-        )
-
-        d.addCallback(self.handle_egd_response)
-        return d
-
-    def handle_egd_response(self, response):
-        if 200 <= response.code < 300:
-            d = defer.succeed((response.code, "OK"))
-        else:
-            # Go through the horrifying process of getting the response body
-            # out of Twisted's plumbing.
-            d = defer.Deferred()
-            response.deliverBody(SimpleResponseReceiver(response.code, d))
-        return d
-
-
-class SimpleResponseReceiver(protocol.Protocol):
-    """
-    Used for pulling the response body out of an HTTP response.
-    """
-
-    def __init__(self, status_code, d):
-        self.status_code = status_code
-        self.buf = ""
-        self.d = d
-
-    def dataReceived(self, data):
-        self.buf += data
-
-    def connectionLost(self, reason=protocol.connectionDone):
-        self.d.callback((self.status_code, self.buf))
+        self.ttype_step = 0
+        self.protocol = protocol
+        # we set FORCEDENDLINE for clients not supporting ttype
+        self.protocol.protocol_flags["FORCEDENDLINE"] = True
+        self.protocol.protocol_flags["TTYPE"] = False
+        # is it a safe bet to assume ANSI is always supported?
+        self.protocol.protocol_flags["ANSI"] = True
+        # setup protocol to handle ttype initialization and negotiation
+        self.protocol.negotiationMap[TTYPE] = self.will_ttype
+        # ask if client will ttype, connect callback if it does.
+        self.protocol.do(TTYPE).addCallbacks(self.will_ttype, self.wont_ttype)
 
+    def wont_ttype(self, option):
+        """
+        Callback if ttype is not supported by client.
 
-@implementer(IBodyProducer)
-class StringProducer:
-    """
-    Used for feeding a request body to the tx HTTP client.
-    """
+        Args:
+            option (Option): Not used.
 
-    def __init__(self, body):
-        self.body = bytes(body, "utf-8")
-        self.length = len(body)
+        """
+        self.protocol.protocol_flags["TTYPE"] = False
+        self.protocol.handshake_done()
 
-    def startProducing(self, consumer):
-        consumer.write(self.body)
-        return defer.succeed(None)
+    def will_ttype(self, option):
+        """
+        Handles negotiation of the ttype protocol once the client has
+        confirmed that it will respond with the ttype protocol.
 
-    def pauseProducing(self):
-        pass
+        Args:
+            option (Option): Not used.
 
-    def stopProducing(self):
-        pass
+        Notes:
+            The negotiation proceeds in several steps, each returning a
+            certain piece of information about the client. All data is
+            stored on protocol.protocol_flags under the TTYPE key.
 
+        """
+        options = self.protocol.protocol_flags
 
-class QuietHTTP11ClientFactory(_HTTP11ClientFactory):
-    """
-    Silences the obnoxious factory start/stop messages in the default client.
-    """
+        if options and options.get("TTYPE", False) or self.ttype_step > 3:
+            return
 
-    noisy = False
+        try:
+            option = b"".join(option).lstrip(IS).decode()
+        except TypeError:
+            # option is not on a suitable form for joining
+            pass
+
+        if self.ttype_step == 0:
+            # just start the request chain
+            self.protocol.requestNegotiation(TTYPE, SEND)
+
+        elif self.ttype_step == 1:
+            # this is supposed to be the name of the client/terminal.
+            # For clients not supporting the extended TTYPE
+            # definition, subsequent calls will just repeat-return this.
+            try:
+                clientname = option.upper()
+            except AttributeError:
+                # malformed option (not a string)
+                clientname = "UNKNOWN"
+
+            # use name to identify support for xterm256. Many of these
+            # only support after a certain version, but all support
+            # it since at least 4 years. We assume recent client here for now.
+            xterm256 = False
+            if clientname.startswith("MUDLET"):
+                # supports xterm256 stably since 1.1 (2010?)
+                xterm256 = clientname.split("MUDLET", 1)[1].strip() >= "1.1"
+                # Mudlet likes GA's on a prompt line for the prompt trigger to
+                # match, if it's not wanting NOGOAHEAD.
+                if not self.protocol.protocol_flags["NOGOAHEAD"]:
+                    self.protocol.protocol_flags["NOGOAHEAD"] = True
+                    self.protocol.protocol_flags["NOPROMPTGOAHEAD"] = False
+
+            if (
+                clientname.startswith("XTERM")
+                or clientname.endswith("-256COLOR")
+                or clientname
+                in (
+                    "ATLANTIS",  # > 0.9.9.0 (aug 2009)
+                    "CMUD",  # > 3.04 (mar 2009)
+                    "KILDCLIENT",  # > 2.2.0 (sep 2005)
+                    "MUDLET",  # > beta 15 (sep 2009)
+                    "MUSHCLIENT",  # > 4.02 (apr 2007)
+                    "PUTTY",  # > 0.58 (apr 2005)
+                    "BEIP",  # > 2.00.206 (late 2009) (BeipMu)
+                    "POTATO",  # > 2.00 (maybe earlier)
+                    "TINYFUGUE",  # > 4.x (maybe earlier)
+                )
+            ):
+                xterm256 = True
+
+            # all clients supporting TTYPE at all seem to support ANSI
+            self.protocol.protocol_flags["ANSI"] = True
+            self.protocol.protocol_flags["XTERM256"] = xterm256
+            self.protocol.protocol_flags["CLIENTNAME"] = clientname
+            self.protocol.requestNegotiation(TTYPE, SEND)
+
+        elif self.ttype_step == 2:
+            # this is a term capabilities flag
+            term = option
+            tupper = term.upper()
+            # identify xterm256 based on flag
+            xterm256 = (
+                tupper.endswith("-256COLOR")
+                or tupper.endswith("XTERM")  # Apple Terminal, old Tintin
+                and not tupper.endswith("-COLOR")  # old Tintin, Putty
+            )
+            if xterm256:
+                self.protocol.protocol_flags["ANSI"] = True
+                self.protocol.protocol_flags["XTERM256"] = xterm256
+            self.protocol.protocol_flags["TERM"] = term
+            # request next information
+            self.protocol.requestNegotiation(TTYPE, SEND)
+
+        elif self.ttype_step == 3:
+            # the MTTS bitstring identifying term capabilities
+            if option.startswith("MTTS"):
+                option = option[4:].strip()
+                if option.isdigit():
+                    # a number - determine the actual capabilities
+                    option = int(option)
+                    support = dict(
+                        (capability, True) for bitval, capability in MTTS if option & bitval > 0
+                    )
+                    self.protocol.protocol_flags.update(support)
+                else:
+                    # some clients send erroneous MTTS as a string. Add directly.
+                    self.protocol.protocol_flags[option.upper()] = True
+
+            self.protocol.protocol_flags["TTYPE"] = True
+            # we must sync ttype once it'd done
+            self.protocol.handshake_done()
+        self.ttype_step += 1
```

### Comparing `evennia-4.0.0/evennia/server/game_index_client/service.py` & `evennia-4.1.0/evennia/server/game_index_client/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Service for integrating the Evennia Game Index client into Evennia.
 
 """
+
 from twisted.application.service import Service
 from twisted.internet import reactor
 from twisted.internet.task import LoopingCall
 
 from evennia.utils import logger
 
 from .client import EvenniaGameIndexClient
```

### Comparing `evennia-4.0.0/evennia/server/initial_setup.py` & `evennia-4.1.0/evennia/server/initial_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module handles initial database propagation, which is only run the first time the game starts.
 It will create some default objects (notably give #1 its evennia-specific properties, and create the
 Limbo room). It will also hooks, and then perform an initial restart.
 
 Everything starts at handle_setup()
 """
 
-
 import time
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 
 import evennia
 from evennia.accounts.models import AccountDB
```

### Comparing `evennia-4.0.0/evennia/server/inputfuncs.py` & `evennia-4.1.0/evennia/server/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/manager.py` & `evennia-4.1.0/evennia/server/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Custom manager for ServerConfig objects.
 """
+
 from django.db import models
 
 
 class ServerConfigManager(models.Manager):
     """
     This ServerConfigManager implements methods for searching and
     manipulating ServerConfigs directly from the database.
```

### Comparing `evennia-4.0.0/evennia/server/migrations/0001_initial.py` & `evennia-4.1.0/evennia/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/migrations/0002_auto_20190128_2311.py` & `evennia-4.1.0/evennia/server/migrations/0002_auto_20190128_2311.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/models.py` & `evennia-4.1.0/evennia/server/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 This holds persistent server configuration flags.
 
 Config values should usually be set through the
 manager's conf() method.
 
 """
+
 from django.db import models
 
 from evennia.server.manager import ServerConfigManager
 from evennia.utils import logger, picklefield, utils
 from evennia.utils.dbserialize import from_pickle, to_pickle
 from evennia.utils.idmapper.models import WeakSharedMemoryModel
```

### Comparing `evennia-4.0.0/evennia/server/portal/amp.py` & `evennia-4.1.0/evennia/server/portal/amp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/portal/amp_server.py` & `evennia-4.1.0/evennia/server/portal/amp_server.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The Evennia Portal service acts as an AMP-server, handling AMP
 communication to the AMP clients connecting to it (by default
 these are the Evennia Server and the evennia launcher).
 
 """
+
 import os
 import sys
 from subprocess import STDOUT, Popen
 
 from django.conf import settings
 from twisted.internet import protocol
 
@@ -32,15 +33,14 @@
     sep = ";" if _is_windows() else ":"
     env = os.environ.copy()
     env["PYTHONPATH"] = sep.join(sys.path)
     return env
 
 
 class AMPServerFactory(protocol.ServerFactory):
-
     """
     This factory creates AMP Server connection. This acts as the 'Portal'-side communication to the
     'Server' process.
 
     """
 
     noisy = False
```

### Comparing `evennia-4.0.0/evennia/server/portal/discord.py` & `evennia-4.1.0/evennia/server/portal/discord.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 The Discord API uses a mix of websockets and REST API endpoints.
 
 In order for this integration to work, you need to have your own
 discord bot set up via https://discord.com/developers/applications
 with the MESSAGE CONTENT toggle switched on, and your bot token
 added to `server/conf/secret_settings.py` as your  DISCORD_BOT_TOKEN
 """
+
 import json
 import os
 from io import BytesIO
 from random import random
 
 from autobahn.twisted.websocket import (
     WebSocketClientFactory,
```

### Comparing `evennia-4.0.0/evennia/server/portal/grapevine.py` & `evennia-4.1.0/evennia/server/portal/grapevine.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/portal/irc.py` & `evennia-4.1.0/evennia/server/portal/irc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/portal/mccp.py` & `evennia-4.1.0/evennia/server/portal/mccp.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 as normal.  Note: On modern hardware you are not likely to notice the
 effect of MCCP unless you have extremely heavy traffic or sits on a
 terribly slow connection.
 
 This protocol is implemented by the telnet protocol importing
 mccp_compress and calling it from its write methods.
 """
+
 import zlib
 
 # negotiations for v1 and v2 of the protocol
 MCCP = bytes([86])  # b"\x56"
 FLUSH = zlib.Z_SYNC_FLUSH
```

### Comparing `evennia-4.0.0/evennia/server/portal/mssp.py` & `evennia-4.1.0/evennia/server/portal/mssp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 http://tintin.sourceforge.net/mssp/.  MSSP allows web portals and
 listings to have their crawlers find the mud and automatically
 extract relevant information about it, such as genre, how many
 active players and so on.
 
 
 """
+
 from django.conf import settings
 
 from evennia.utils import utils
 
 MSSP = bytes([70])  # b"\x46"
 MSSP_VAR = bytes([1])  # b"\x01"
 MSSP_VAL = bytes([2])  # b"\x02"
```

### Comparing `evennia-4.0.0/evennia/server/portal/mxp.py` & `evennia-4.1.0/evennia/server/portal/mxp.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 More information can be found on the following links:
 http://www.zuggsoft.com/zmud/mxp.htm
 http://www.mushclient.com/mushclient/mxp.htm
 http://www.gammon.com.au/mushclient/addingservermxp.htm
 
 """
+
 import re
 
 from django.conf import settings
 
 LINKS_SUB = re.compile(r"\|lc(.*?)\|lt(.*?)\|le", re.DOTALL)
 URL_SUB = re.compile(r"\|lu(.*?)\|lt(.*?)\|le", re.DOTALL)
```

### Comparing `evennia-4.0.0/evennia/server/portal/naws.py` & `evennia-4.1.0/evennia/server/portal/naws.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 This implements the NAWS telnet option as per
 https://www.ietf.org/rfc/rfc1073.txt
 
 NAWS allows telnet clients to report their current window size to the
 client and update it when the size changes
 
 """
+
 from codecs import encode as codecs_encode
 
 from django.conf import settings
 
 NAWS = bytes([31])  # b"\x1f"
 IS = bytes([0])  # b"\x00"
```

### Comparing `evennia-4.0.0/evennia/server/portal/portal.py` & `evennia-4.1.0/evennia/server/portal/portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 the game engine.
 
 This module should be started with the 'twistd' executable since it
 sets up all the networking features.  (this is done automatically
 by game/evennia.py).
 
 """
+
 import os
 import sys
 
 import django
 from twisted.logger import globalLogPublisher
 
 django.setup()
```

### Comparing `evennia-4.0.0/evennia/server/portal/portalsessionhandler.py` & `evennia-4.1.0/evennia/server/portal/portalsessionhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Sessionhandler for portal sessions.
 
 """
 
-
 import time
 from collections import deque, namedtuple
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 from twisted.internet import reactor
```

### Comparing `evennia-4.0.0/evennia/server/portal/rss.py` & `evennia-4.1.0/evennia/server/portal/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 RSS parser for Evennia
 
 This connects an RSS feed to an in-game Evennia channel, sending messages
 to the channel whenever the feed updates.
 
 """
+
 from django.conf import settings
 from twisted.internet import task, threads
 
 from evennia.server.session import Session
 from evennia.utils import logger
 
 RSS_ENABLED = settings.RSS_ENABLED
```

### Comparing `evennia-4.0.0/evennia/server/portal/service.py` & `evennia-4.1.0/evennia/server/portal/service.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/portal/ssh.py` & `evennia-4.1.0/evennia/server/portal/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,26 +30,27 @@
 
 try:
     from twisted.conch.ssh.keys import Key
 except ImportError:
     raise ImportError(_SSH_IMPORT_ERROR)
 
 from django.conf import settings
-from evennia.accounts.models import AccountDB
-from evennia.utils import ansi
-from evennia.utils.utils import class_from_module, to_str
 from twisted.conch import interfaces as iconch
 from twisted.conch.insults import insults
 from twisted.conch.manhole import Manhole, recvline
 from twisted.conch.manhole_ssh import ConchFactory, TerminalRealm, _Glue
 from twisted.conch.ssh import common
 from twisted.conch.ssh.userauth import SSHUserAuthServer
 from twisted.internet import defer, protocol
 from twisted.python import components
 
+from evennia.accounts.models import AccountDB
+from evennia.utils import ansi
+from evennia.utils.utils import class_from_module, to_str
+
 _RE_N = re.compile(r"\|n$")
 _RE_SCREENREADER_REGEX = re.compile(
     r"%s" % settings.SCREENREADER_REGEX_STRIP, re.DOTALL + re.MULTILINE
 )
 _GAME_DIR = settings.GAME_DIR
 _PRIVATE_KEY_FILE = os.path.join(_GAME_DIR, "server", "ssh-private.key")
 _PUBLIC_KEY_FILE = os.path.join(_GAME_DIR, "server", "ssh-public.key")
```

### Comparing `evennia-4.0.0/evennia/server/portal/ssl.py` & `evennia-4.1.0/evennia/server/portal/ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This is a simple context factory for auto-creating
 SSL keys and certificates.
 
 """
+
 import os
 import sys
 
 try:
     import OpenSSL
     from twisted.internet import ssl as twisted_ssl
 except ImportError as error:
```

### Comparing `evennia-4.0.0/evennia/server/portal/suppress_ga.py` & `evennia-4.1.0/evennia/server/portal/suppress_ga.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         Args:
             protocol (Protocol): The active protocol instance.
 
         """
         self.protocol = protocol
 
         self.protocol.protocol_flags["NOGOAHEAD"] = True
-        self.protocol.protocol_flags[
-            "NOPROMPTGOAHEAD"
-        ] = True  # Used to send a GA after a prompt line only, set in TTYPE (per client)
+        self.protocol.protocol_flags["NOPROMPTGOAHEAD"] = (
+            True  # Used to send a GA after a prompt line only, set in TTYPE (per client)
+        )
         # tell the client that we prefer to suppress GA ...
         self.protocol.will(SUPPRESS_GA).addCallbacks(self.will_suppress_ga, self.wont_suppress_ga)
 
     def wont_suppress_ga(self, option):
         """
         Called when client requests to not suppress GA.
```

### Comparing `evennia-4.0.0/evennia/server/portal/telnet.py` & `evennia-4.1.0/evennia/server/portal/telnet.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/portal/telnet_oob.py` & `evennia-4.1.0/evennia/server/portal/telnet_oob.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 - MSDP (Mud Server Data Protocol), as per http://tintin.sourceforge.net/msdp/
 - GMCP (Generic Mud Communication Protocol) as per
   http://www.ironrealms.com/rapture/manual/files/FeatGMCP-txt.html#Generic_MUD_Communication_Protocol%28GMCP%29
 
 ----
 
 """
+
 import json
 import re
 
 # General Telnet
 from twisted.conch.telnet import IAC, SB, SE
 
 from evennia.utils.utils import is_iter
```

### Comparing `evennia-4.0.0/evennia/server/portal/telnet_ssl.py` & `evennia-4.1.0/evennia/server/portal/telnet_ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 client supporting Telnet SSL.
 
 The protocol will try to automatically create the private key and certificate on the server side
 when starting and will warn if this was not possible. These will appear as files ssl.key and
 ssl.cert in mygame/server/.
 
 """
+
 import os
 
 try:
     from OpenSSL import crypto
     from twisted.internet import ssl as twisted_ssl
 except ImportError as error:
     errstr = """
```

### Comparing `evennia-4.0.0/evennia/server/portal/tests.py` & `evennia-4.1.0/evennia/server/portal/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/portal/ttype.py` & `evennia-4.1.0/evennia/server/throttle.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,191 +1,225 @@
-"""
-TTYPE (MTTS) - Mud Terminal Type Standard
+import time
+from collections import deque
 
-This module implements the TTYPE telnet protocol as per
-http://tintin.sourceforge.net/mtts/. It allows the server to ask the
-client about its capabilities. If the client also supports TTYPE, it
-will return with information such as its name, if it supports colour
-etc. If the client does not support TTYPE, this will be ignored.
-
-All data will be stored on the protocol's protocol_flags dictionary,
-under the 'TTYPE' key.
-
-"""
-
-# telnet option codes
-TTYPE = bytes([24])  # b"\x18"
-IS = bytes([0])  # b"\x00"
-SEND = bytes([1])  # b"\x01"
-
-# terminal capabilities and their codes
-MTTS = [
-    (2048, "SSL"),
-    (1024, "MSLP"),
-    (512, "MNES"),
-    (256, "TRUECOLOR"),
-    (128, "PROXY"),
-    (64, "SCREENREADER"),
-    (32, "OSC_COLOR_PALETTE"),
-    (16, "MOUSE_TRACKING"),
-    (8, "XTERM256"),
-    (4, "UTF-8"),
-    (2, "VT100"),
-    (1, "ANSI"),
-]
+from django.core.cache import caches
+from django.utils.translation import gettext as _
 
+from evennia.utils import logger
 
-class Ttype:
+
+class Throttle:
     """
-    Handles ttype negotiations. Called and initiated by the
-    telnet protocol.
+    Keeps a running count of failed actions per IP address.
+
+    Available methods indicate whether or not the number of failures exceeds a
+    particular threshold.
 
+    This version of the throttle is usable by both the terminal server as well
+    as the web server, imposes limits on memory consumption by using deques
+    with length limits instead of open-ended lists, and uses native Django
+    caches for automatic key eviction and persistence configurability.
     """
 
-    def __init__(self, protocol):
+    error_msg = _("Too many failed attempts; you must wait a few minutes before trying again.")
+
+    def __init__(self, **kwargs):
+        """
+        Allows setting of throttle parameters.
+
+        Keyword Args:
+            name (str): Name of this throttle.
+            limit (int): Max number of failures before imposing limiter. If `None`,
+                the throttle is disabled.
+            timeout (int): number of timeout seconds after
+                max number of tries has been reached.
+            cache_size (int): Max number of attempts to record per IP within a
+                rolling window; this is NOT the same as the limit after which
+                the throttle is imposed!
+        """
+        try:
+            self.storage = caches["throttle"]
+        except Exception:
+            logger.log_trace("Throttle: Errors encountered; using default cache.")
+            self.storage = caches["default"]
+
+        self.name = kwargs.get("name", "undefined-throttle")
+        self.limit = kwargs.get("limit", 5)
+        self.cache_size = kwargs.get("cache_size", self.limit)
+        self.timeout = kwargs.get("timeout", 5 * 60)
+
+    def get_cache_key(self, *args, **kwargs):
+        """
+        Creates a 'prefixed' key containing arbitrary terms to prevent key
+        collisions in the same namespace.
+
+        """
+        return "-".join((self.name, *args))
+
+    def touch(self, key, *args, **kwargs):
+        """
+        Refreshes the timeout on a given key and ensures it is recorded in the
+        key register.
+
+        Args:
+            key(str): Key of entry to renew.
+
+        """
+        cache_key = self.get_cache_key(key)
+        if self.storage.touch(cache_key, self.timeout):
+            self.record_key(key)
+
+    def get(self, ip=None):
+        """
+        Convenience function that returns the storage table, or part of.
+
+        Args:
+            ip (str, optional): IP address of requestor
+
+        Returns:
+            storage (dict): When no IP is provided, returns a dict of all
+                current IPs being tracked and the timestamps of their recent
+                failures.
+            timestamps (deque): When an IP is provided, returns a deque of
+                timestamps of recent failures only for that IP.
+
+        """
+        if ip:
+            cache_key = self.get_cache_key(str(ip))
+            return self.storage.get(cache_key, deque(maxlen=self.cache_size))
+        else:
+            keys_key = self.get_cache_key("keys")
+            keys = self.storage.get_or_set(keys_key, set(), self.timeout)
+            data = self.storage.get_many((self.get_cache_key(x) for x in keys))
+
+            found_keys = set(data.keys())
+            if len(keys) != len(found_keys):
+                self.storage.set(keys_key, found_keys, self.timeout)
+
+            return data
+
+    def update(self, ip, failmsg="Exceeded threshold."):
         """
-        Initialize ttype by storing protocol on ourselves and calling
-        the client to see if it supporst ttype.
+        Store the time of the latest failure.
 
         Args:
-            protocol (Protocol): The protocol instance.
+            ip (str): IP address of requestor
+            failmsg (str, optional): Message to display in logs upon activation
+                of throttle.
 
-        Notes:
-            The `self.ttype_step` indicates how far in the data
-            retrieval we've gotten.
+        Returns:
+            None
 
         """
-        self.ttype_step = 0
-        self.protocol = protocol
-        # we set FORCEDENDLINE for clients not supporting ttype
-        self.protocol.protocol_flags["FORCEDENDLINE"] = True
-        self.protocol.protocol_flags["TTYPE"] = False
-        # is it a safe bet to assume ANSI is always supported?
-        self.protocol.protocol_flags["ANSI"] = True
-        # setup protocol to handle ttype initialization and negotiation
-        self.protocol.negotiationMap[TTYPE] = self.will_ttype
-        # ask if client will ttype, connect callback if it does.
-        self.protocol.do(TTYPE).addCallbacks(self.will_ttype, self.wont_ttype)
+        cache_key = self.get_cache_key(ip)
+
+        # Get current status
+        previously_throttled = self.check(ip)
+
+        # Get previous failures, if any
+        entries = self.storage.get(cache_key, [])
+        entries.append(time.time())
+
+        # Store updated record
+        self.storage.set(cache_key, deque(entries, maxlen=self.cache_size), self.timeout)
+
+        # See if this update caused a change in status
+        currently_throttled = self.check(ip)
+
+        # If this makes it engage, log a single activation event
+        if not previously_throttled and currently_throttled:
+            logger.log_sec(
+                f"Throttle Activated: {failmsg} (IP: {ip}, "
+                f"{self.limit} hits in {self.timeout} seconds.)"
+            )
+
+        self.record_ip(ip)
 
-    def wont_ttype(self, option):
+    def remove(self, ip, *args, **kwargs):
         """
-        Callback if ttype is not supported by client.
+        Clears data stored for an IP from the throttle.
 
         Args:
-            option (Option): Not used.
+            ip(str): IP to clear.
 
         """
-        self.protocol.protocol_flags["TTYPE"] = False
-        self.protocol.handshake_done()
+        exists = self.get(ip)
+        if not exists:
+            return False
+
+        cache_key = self.get_cache_key(ip)
+        self.storage.delete(cache_key)
+        self.unrecord_ip(ip)
 
-    def will_ttype(self, option):
+        # Return True if NOT exists
+        return not bool(self.get(ip))
+
+    def record_ip(self, ip, *args, **kwargs):
         """
-        Handles negotiation of the ttype protocol once the client has
-        confirmed that it will respond with the ttype protocol.
+        Tracks keys as they are added to the cache (since there is no way to
+        get a list of keys after-the-fact).
 
         Args:
-            option (Option): Not used.
+            ip(str): IP being added to cache. This should be the original
+                IP, not the cache-prefixed key.
 
-        Notes:
-            The negotiation proceeds in several steps, each returning a
-            certain piece of information about the client. All data is
-            stored on protocol.protocol_flags under the TTYPE key.
+        """
+        keys_key = self.get_cache_key("keys")
+        keys = self.storage.get(keys_key, set())
+        keys.add(ip)
+        self.storage.set(keys_key, keys, self.timeout)
+        return True
 
+    def unrecord_ip(self, ip, *args, **kwargs):
         """
-        options = self.protocol.protocol_flags
+        Forces removal of a key from the key registry.
 
-        if options and options.get("TTYPE", False) or self.ttype_step > 3:
-            return
+        Args:
+            ip(str): IP to remove from list of keys.
 
+        """
+        keys_key = self.get_cache_key("keys")
+        keys = self.storage.get(keys_key, set())
         try:
-            option = b"".join(option).lstrip(IS).decode()
-        except TypeError:
-            # option is not on a suitable form for joining
-            pass
-
-        if self.ttype_step == 0:
-            # just start the request chain
-            self.protocol.requestNegotiation(TTYPE, SEND)
-
-        elif self.ttype_step == 1:
-            # this is supposed to be the name of the client/terminal.
-            # For clients not supporting the extended TTYPE
-            # definition, subsequent calls will just repeat-return this.
-            try:
-                clientname = option.upper()
-            except AttributeError:
-                # malformed option (not a string)
-                clientname = "UNKNOWN"
-
-            # use name to identify support for xterm256. Many of these
-            # only support after a certain version, but all support
-            # it since at least 4 years. We assume recent client here for now.
-            xterm256 = False
-            if clientname.startswith("MUDLET"):
-                # supports xterm256 stably since 1.1 (2010?)
-                xterm256 = clientname.split("MUDLET", 1)[1].strip() >= "1.1"
-                # Mudlet likes GA's on a prompt line for the prompt trigger to
-                # match, if it's not wanting NOGOAHEAD.
-                if not self.protocol.protocol_flags["NOGOAHEAD"]:
-                    self.protocol.protocol_flags["NOGOAHEAD"] = True
-                    self.protocol.protocol_flags["NOPROMPTGOAHEAD"] = False
-
-            if (
-                clientname.startswith("XTERM")
-                or clientname.endswith("-256COLOR")
-                or clientname
-                in (
-                    "ATLANTIS",  # > 0.9.9.0 (aug 2009)
-                    "CMUD",  # > 3.04 (mar 2009)
-                    "KILDCLIENT",  # > 2.2.0 (sep 2005)
-                    "MUDLET",  # > beta 15 (sep 2009)
-                    "MUSHCLIENT",  # > 4.02 (apr 2007)
-                    "PUTTY",  # > 0.58 (apr 2005)
-                    "BEIP",  # > 2.00.206 (late 2009) (BeipMu)
-                    "POTATO",  # > 2.00 (maybe earlier)
-                    "TINYFUGUE",  # > 4.x (maybe earlier)
-                )
-            ):
-                xterm256 = True
-
-            # all clients supporting TTYPE at all seem to support ANSI
-            self.protocol.protocol_flags["ANSI"] = True
-            self.protocol.protocol_flags["XTERM256"] = xterm256
-            self.protocol.protocol_flags["CLIENTNAME"] = clientname
-            self.protocol.requestNegotiation(TTYPE, SEND)
-
-        elif self.ttype_step == 2:
-            # this is a term capabilities flag
-            term = option
-            tupper = term.upper()
-            # identify xterm256 based on flag
-            xterm256 = (
-                tupper.endswith("-256COLOR")
-                or tupper.endswith("XTERM")  # Apple Terminal, old Tintin
-                and not tupper.endswith("-COLOR")  # old Tintin, Putty
-            )
-            if xterm256:
-                self.protocol.protocol_flags["ANSI"] = True
-                self.protocol.protocol_flags["XTERM256"] = xterm256
-            self.protocol.protocol_flags["TERM"] = term
-            # request next information
-            self.protocol.requestNegotiation(TTYPE, SEND)
-
-        elif self.ttype_step == 3:
-            # the MTTS bitstring identifying term capabilities
-            if option.startswith("MTTS"):
-                option = option[4:].strip()
-                if option.isdigit():
-                    # a number - determine the actual capabilities
-                    option = int(option)
-                    support = dict(
-                        (capability, True) for bitval, capability in MTTS if option & bitval > 0
-                    )
-                    self.protocol.protocol_flags.update(support)
-                else:
-                    # some clients send erroneous MTTS as a string. Add directly.
-                    self.protocol.protocol_flags[option.upper()] = True
-
-            self.protocol.protocol_flags["TTYPE"] = True
-            # we must sync ttype once it'd done
-            self.protocol.handshake_done()
-        self.ttype_step += 1
+            keys.remove(ip)
+            self.storage.set(keys_key, keys, self.timeout)
+            return True
+        except KeyError:
+            return False
+
+    def check(self, ip):
+        """
+        This will check the session's address against the
+        storage dictionary to check they haven't spammed too many
+        fails recently.
+
+        Args:
+            ip (str): IP address of requestor
+
+        Returns:
+            throttled (bool): True if throttling is active,
+                False otherwise.
+
+        """
+        if self.limit is None:
+            # throttle is disabled
+            return False
+
+        now = time.time()
+        ip = str(ip)
+
+        cache_key = self.get_cache_key(ip)
+
+        # checking mode
+        latest_fails = self.storage.get(cache_key)
+        if latest_fails and len(latest_fails) >= self.limit:
+            # too many fails recently
+            if now - latest_fails[-1] < self.timeout:
+                # too soon - timeout in play
+                self.touch(cache_key)
+                return True
+            else:
+                # timeout has passed. clear faillist
+                self.remove(ip)
+                return False
+        else:
+            return False
```

### Comparing `evennia-4.0.0/evennia/server/portal/webclient.py` & `evennia-4.1.0/evennia/server/portal/webclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 `["inputfunc_name", [args], {kwarg}]`
 
 which represents an "inputfunc" to be called on the Evennia side with *args, **kwargs.
 The most common inputfunc is "text", which takes just the text input
 from the command line and interprets it as an Evennia Command: `["text", ["look"], {}]`
 
 """
+
 import html
 import json
 import re
 
 from autobahn.exception import Disconnected
 from autobahn.twisted.websocket import WebSocketServerProtocol
 from django.conf import settings
```

### Comparing `evennia-4.0.0/evennia/server/portal/webclient_ajax.py` & `evennia-4.1.0/evennia/server/portal/webclient_ajax.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 /webclientdata - this url is called by the ajax chat using
                  POST requests (long-polling when necessary)
                  The WebClient resource in this module will
                  handle these requests and act as a gateway
                  to sessions connected over the webclient.
 
 """
+
 import html
 import json
 import re
 import time
 
 from django.conf import settings
 from django.utils.functional import Promise
```

### Comparing `evennia-4.0.0/evennia/server/profiling/dummyrunner.py` & `evennia-4.1.0/evennia/server/profiling/dummyrunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
    DUMMYRUNNER_ACTIONS_MODULE = <path.to.your.module>
 
 in your settings. See utils.dummyrunner_actions.py
 for instructions on how to define this module.
 
 """
 
-
 import random
 import sys
 import time
 from argparse import ArgumentParser
 
 import django
 from twisted.conch import telnet
```

### Comparing `evennia-4.0.0/evennia/server/profiling/dummyrunner_settings.py` & `evennia-4.1.0/evennia/server/profiling/dummyrunner_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 TIMESTEP with a chance given by CHANCE_OF_ACTION by in the order given
 (no randomness) and allows for setting up a more complex chain of
 commands (such as creating an account and logging in).
 
 ----
 
 """
+
 import random
 import string
 
 # Dummy runner settings
 
 # Time between each dummyrunner "tick", in seconds. Each dummy
 # will be called with this frequency.
```

### Comparing `evennia-4.0.0/evennia/server/profiling/memplot.py` & `evennia-4.1.0/evennia/server/profiling/memplot.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/profiling/settings_mixin.py` & `evennia-4.1.0/evennia/server/profiling/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/profiling/test_queries.py` & `evennia-4.1.0/evennia/server/profiling/test_queries.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/profiling/tests.py` & `evennia-4.1.0/evennia/server/profiling/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/profiling/timetrace.py` & `evennia-4.1.0/evennia/server/profiling/timetrace.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/server.py` & `evennia-4.1.0/evennia/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 engine.
 
 This module should be started with the 'twistd' executable since it sets up all
 the networking features.  (this is done automatically by
 evennia/server/server_runner.py).
 
 """
+
 import os
 import sys
 
 import django
 from twisted.logger import globalLogPublisher
 
 django.setup()
```

### Comparing `evennia-4.0.0/evennia/server/serversession.py` & `evennia-4.1.0/evennia/server/serversession.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This defines a the Server's generic session object. This object represents
 a connection to the outside world but don't know any details about how the
 connection actually happens (so it's the same for telnet, web, ssh etc).
 
 It is stored on the Server side (as opposed to protocol-specific sessions which
 are stored on the Portal side)
 """
+
 import time
 
 from django.conf import settings
 from django.utils import timezone
 
 from evennia.commands.cmdsethandler import CmdSetHandler
 from evennia.comms.models import ChannelDB
```

### Comparing `evennia-4.0.0/evennia/server/service.py` & `evennia-4.1.0/evennia/server/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains the main EvenniaService class, which is the very core of the
 Evennia server. It is instantiated by the evennia/server/server.py module.
 """
+
 import importlib
 import time
 import traceback
 
 import django
 from django.conf import settings
 from django.db import connection
@@ -326,20 +327,21 @@
             # run the update
 
             # from evennia.accounts.models import AccountDB
             for i, prev, curr in (
                 (i, tup[0], tup[1]) for i, tup in enumerate(settings_compare) if i in mismatches
             ):
                 # update the database
-                self.info_dict[
-                    "info"
-                ] = " %s:\n '%s' changed to '%s'. Updating unchanged entries in database ..." % (
-                    settings_names[i],
-                    prev,
-                    curr,
+                self.info_dict["info"] = (
+                    " %s:\n '%s' changed to '%s'. Updating unchanged entries in database ..."
+                    % (
+                        settings_names[i],
+                        prev,
+                        curr,
+                    )
                 )
                 if i == 0:
                     evennia.ObjectDB.objects.filter(db_cmdset_storage__exact=prev).update(
                         db_cmdset_storage=curr
                     )
                 if i == 1:
                     evennia.AccountDB.objects.filter(db_cmdset_storage__exact=prev).update(
```

### Comparing `evennia-4.0.0/evennia/server/session.py` & `evennia-4.1.0/evennia/server/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module defines a generic session class. All connection instances
 (both on Portal and Server side) should inherit from this class.
 
 """
+
 import time
 
 from django.conf import settings
 
 # ------------------------------------------------------------
 # Server Session
 # ------------------------------------------------------------
```

### Comparing `evennia-4.0.0/evennia/server/sessionhandler.py` & `evennia-4.1.0/evennia/server/sessionhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
      for the game. These sessions has no knowledge about
      how they are connected to the world.
 - PortalSessionHandler - this stores sessions created by
      twisted protocols. These are dumb connectors that
      handle network communication but holds no game info.
 
 """
+
 import time
 from codecs import decode as codecs_decode
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 
 import evennia
```

### Comparing `evennia-4.0.0/evennia/server/signals.py` & `evennia-4.1.0/evennia/server/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     # ...
 ```
 
 This is used on top of hooks to make certain features easier to add to contribs
 without necessitating a full takeover of hooks that may be in high demand.
 
 """
+
 from collections import defaultdict
 
 from django.dispatch import Signal
 
 # The sender is the created Account. This is triggered at the very end of
 # Account.create() after the Account is created. Note that this will *not* fire
 # if calling create.create_account alone, since going through the Account.create()
```

### Comparing `evennia-4.0.0/evennia/server/tests/test_amp_connection.py` & `evennia-4.1.0/evennia/server/tests/test_amp_connection.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/tests/test_initial_setup.py` & `evennia-4.1.0/evennia/server/tests/test_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/tests/test_launcher.py` & `evennia-4.1.0/evennia/server/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/tests/test_misc.py` & `evennia-4.1.0/evennia/server/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/tests/test_server.py` & `evennia-4.1.0/evennia/server/tests/test_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Test the main server component
 
 """
+
 from unittest import TestCase
 
 from django.test import override_settings
 from mock import DEFAULT, MagicMock, call, patch
 
 import evennia
 
@@ -21,75 +22,80 @@
         # Running this first line ensures that the EVENNIA_SERVICE is instantiated.
         from evennia.server import server
 
         self.server = evennia.EVENNIA_SERVER_SERVICE
 
     @override_settings(IDMAPPER_CACHE_MAXSIZE=1000)
     def test__server_maintenance_reset(self):
-        with patch.object(self.server, "_flush_cache", new=MagicMock()) as mockflush, patch.object(
-            evennia, "ServerConfig", new=MagicMock()
-        ) as mockconf, patch.multiple(
-            "evennia.server.service",
-            LoopingCall=DEFAULT,
-            connection=DEFAULT,
-        ) as mocks:
+        with (
+            patch.object(self.server, "_flush_cache", new=MagicMock()) as mockflush,
+            patch.object(evennia, "ServerConfig", new=MagicMock()) as mockconf,
+            patch.multiple(
+                "evennia.server.service",
+                LoopingCall=DEFAULT,
+                connection=DEFAULT,
+            ) as mocks,
+        ):
             self.server.maintenance_count = 0
 
             mocks["connection"].close = MagicMock()
             mockconf.objects.conf = MagicMock(return_value=456)
 
             # flush cache
             self.server.server_maintenance()
             mockconf.objects.conf.assert_called_with("runtime", 456)
 
     @override_settings(IDMAPPER_CACHE_MAXSIZE=1000)
     def test__server_maintenance_flush(self):
-        with patch.multiple(
-            "evennia.server.service",
-            LoopingCall=DEFAULT,
-            connection=DEFAULT,
-        ) as mocks, patch.object(
-            evennia, "ServerConfig", new=MagicMock()
-        ) as mockconf, patch.object(
-            self.server, "_flush_cache", new=MagicMock()
-        ) as mockflush:
+        with (
+            patch.multiple(
+                "evennia.server.service",
+                LoopingCall=DEFAULT,
+                connection=DEFAULT,
+            ) as mocks,
+            patch.object(evennia, "ServerConfig", new=MagicMock()) as mockconf,
+            patch.object(self.server, "_flush_cache", new=MagicMock()) as mockflush,
+        ):
             mocks["connection"].close = MagicMock()
             mockconf.objects.conf = MagicMock(return_value=100)
             self.server.maintenance_count = 5 - 1
             # flush cache
             self.server.server_maintenance()
             self.server._flush_cache.assert_called_with(1000)
 
     @override_settings(IDMAPPER_CACHE_MAXSIZE=1000)
     def test__server_maintenance_close_connection(self):
-        with patch.multiple(
-            "evennia.server.service",
-            LoopingCall=DEFAULT,
-            connection=DEFAULT,
-        ) as mocks, patch.object(evennia, "ServerConfig", new=MagicMock()) as mockconf:
+        with (
+            patch.multiple(
+                "evennia.server.service",
+                LoopingCall=DEFAULT,
+                connection=DEFAULT,
+            ) as mocks,
+            patch.object(evennia, "ServerConfig", new=MagicMock()) as mockconf,
+        ):
             self.server._flush_cache = MagicMock()
             self.server.maintenance_count = (60 * 7) - 1
             self.server._last_server_time_snapshot = 0
             mocks["connection"].close = MagicMock()
             mockconf.objects.conf = MagicMock(return_value=100)
             self.server.server_maintenance()
             mocks["connection"].close.assert_called()
 
     @override_settings(IDLE_TIMEOUT=10)
     def test__server_maintenance_idle_time(self):
-        with patch.multiple(
-            "evennia.server.service",
-            LoopingCall=DEFAULT,
-            connection=DEFAULT,
-            time=DEFAULT,
-        ) as mocks, patch.object(
-            evennia, "ServerConfig", new=MagicMock()
-        ) as mockconf, patch.object(
-            evennia, "SESSION_HANDLER", new=MagicMock()
-        ) as mocksess:
+        with (
+            patch.multiple(
+                "evennia.server.service",
+                LoopingCall=DEFAULT,
+                connection=DEFAULT,
+                time=DEFAULT,
+            ) as mocks,
+            patch.object(evennia, "ServerConfig", new=MagicMock()) as mockconf,
+            patch.object(evennia, "SESSION_HANDLER", new=MagicMock()) as mocksess,
+        ):
             self.server.maintenance_count = (3600 * 7) - 1
             self.server._last_server_time_snapshot = 0
             sess1 = MagicMock()
             sess2 = MagicMock()
             sess3 = MagicMock()
             sess4 = MagicMock()
             sess1.cmd_last = 100  # should time out
@@ -110,21 +116,21 @@
 
             self.server.server_maintenance()
             reason = "idle timeout exceeded"
             calls = [call(sess1, reason=reason), call(sess4, reason=reason)]
             mocksess.disconnect.assert_has_calls(calls, any_order=True)
 
     def test_update_defaults(self):
-        with patch.object(evennia, "ObjectDB", new=MagicMock()) as mockobj, patch.object(
-            evennia, "AccountDB", new=MagicMock()
-        ) as mockacc, patch.object(evennia, "ScriptDB", new=MagicMock()) as mockscr, patch.object(
-            evennia, "ChannelDB", new=MagicMock()
-        ) as mockchan, patch.object(
-            evennia, "ServerConfig", new=MagicMock()
-        ) as mockconf:
+        with (
+            patch.object(evennia, "ObjectDB", new=MagicMock()) as mockobj,
+            patch.object(evennia, "AccountDB", new=MagicMock()) as mockacc,
+            patch.object(evennia, "ScriptDB", new=MagicMock()) as mockscr,
+            patch.object(evennia, "ChannelDB", new=MagicMock()) as mockchan,
+            patch.object(evennia, "ServerConfig", new=MagicMock()) as mockconf,
+        ):
             for m in (mockscr, mockobj, mockacc, mockchan):
                 m.objects.filter = MagicMock()
 
             # fake mismatches
             settings_names = (
                 "CMDSET_CHARACTER",
                 "CMDSET_ACCOUNT",
@@ -216,17 +222,18 @@
 
     def tearDown(self):
         for obj in self.objects:
             obj.delete()
 
     @override_settings(TEST_ENVIRONMENT=True)
     def test_run_init_hooks(self):
-        with patch.object(
-            self.server, "at_server_reload_start", new=MagicMock()
-        ) as reload, patch.object(self.server, "at_server_cold_start", new=MagicMock()) as cold:
+        with (
+            patch.object(self.server, "at_server_reload_start", new=MagicMock()) as reload,
+            patch.object(self.server, "at_server_cold_start", new=MagicMock()) as cold,
+        ):
             self.server.run_init_hooks("reload")
             self.server.run_init_hooks("reset")
             self.server.run_init_hooks("shutdown")
 
             for obj in self.objects:
                 obj.at_init.assert_called()
```

### Comparing `evennia-4.0.0/evennia/server/tests/testrunner.py` & `evennia-4.1.0/evennia/server/tests/testrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Main test-suite runner of Evennia. The runner collates tests from
 all over the code base and runs them.
 
 Runs as part of the Evennia's test suite with 'evennia test evennia"
 
 """
+
 from django.test.runner import DiscoverRunner
 
 
 class EvenniaTestSuiteRunner(DiscoverRunner):
     """
     Pointed to by the TEST_RUNNER setting.
     This test runner only runs tests on the apps specified in evennia/
```

### Comparing `evennia-4.0.0/evennia/server/validators.py` & `evennia-4.1.0/evennia/server/validators.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/server/webserver.py` & `evennia-4.1.0/evennia/server/webserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 application.
 
 (Lots of thanks to http://github.com/clemesha/twisted-wsgi-django for
 a great example/aid on how to do this.)
 
 
 """
+
 import urllib.parse
 from urllib.parse import quote as urlquote
 
 from django.conf import settings
 from django.core.wsgi import get_wsgi_application
 from twisted.application import internet
 from twisted.internet import defer, reactor
```

### Comparing `evennia-4.0.0/evennia/settings_default.py` & `evennia-4.1.0/evennia/settings_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Hint: Don't copy&paste over more from this file than you actually want
 to change.  Anything you don't copy&paste will thus retain its default
 value - which may change as Evennia is developed. This way you can
 always be sure of what you have changed and what is default behaviour.
 
 """
+
 import os
 import sys
 
 from django.contrib.messages import constants as messages
 from django.urls import reverse_lazy
 
 ######################################################################
```

### Comparing `evennia-4.0.0/evennia/typeclasses/attributes.py` & `evennia-4.1.0/evennia/typeclasses/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Attributes are also used to implement Nicks. This module also contains
 the Attribute- and NickHandlers as well as the `NAttributeHandler`,
 which is a non-db version of Attributes.
 
 
 """
+
 import fnmatch
 import re
 from collections import defaultdict
 
 from django.conf import settings
 from django.db import models
 from django.utils.encoding import smart_str
```

### Comparing `evennia-4.0.0/evennia/typeclasses/managers.py` & `evennia-4.1.0/evennia/typeclasses/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This implements the common managers that are used by the
 abstract models in dbobjects.py (and which are thus shared by
 all Attributes and TypedObjects).
 
 """
+
 import shlex
 
 from django.db.models import Count, ExpressionWrapper, F, FloatField, Q
 from django.db.models.functions import Cast
 
 from evennia.typeclasses.attributes import Attribute
 from evennia.typeclasses.tags import Tag
```

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0001_initial.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py` & `evennia-4.1.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/typeclasses/models.py` & `evennia-4.1.0/evennia/typeclasses/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 The admin should usually not have to deal directly  with the database object
 layer.
 
 This module also contains the Managers for the respective models; inherit from
 these to create custom managers.
 
 """
+
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import signals
 from django.db.models.base import ModelBase
 from django.urls import reverse
```

### Comparing `evennia-4.0.0/evennia/typeclasses/tags.py` & `evennia-4.1.0/evennia/typeclasses/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 objects at the same time.
 
 Tags are used for tagging, obviously, but the data structure is also
 used for storing Aliases and Permissions. This module contains the
 respective handlers.
 
 """
+
 from collections import defaultdict
 
 from django.conf import settings
 from django.db import models
 
 from evennia.locks.lockfuncs import perm as perm_lockfunc
 from evennia.utils.utils import make_iter, to_str
```

### Comparing `evennia-4.0.0/evennia/typeclasses/tests.py` & `evennia-4.1.0/evennia/typeclasses/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/ansi.py` & `evennia-4.1.0/evennia/utils/ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 "This is |[=jText on dark grey background"
 
 ```
 
 ----
 
 """
+
 import functools
 import re
 from collections import OrderedDict
 
 from django.conf import settings
 
 from evennia.utils import logger, utils
```

### Comparing `evennia-4.0.0/evennia/utils/batchprocessors.py` & `evennia-4.1.0/evennia/utils/batchprocessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     #INSERT another_batch_file
 
     #CODE
 
     script = create.create_script()
 
 """
+
 import codecs
 import re
 import sys
 import traceback
 
 from django.conf import settings
```

### Comparing `evennia-4.0.0/evennia/utils/containers.py` & `evennia-4.1.0/evennia/utils/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 available as properties on the singleton)
 
 evennia.GLOBAL_SCRIPTS
 evennia.OPTION_CLASSES
 
 """
 
-
 from pickle import dumps
 
 from django.conf import settings
 from django.db.utils import OperationalError, ProgrammingError
 
 from evennia.utils import logger
 from evennia.utils.utils import callables_from_module, class_from_module
```

### Comparing `evennia-4.0.0/evennia/utils/create.py` & `evennia-4.1.0/evennia/utils/create.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/dbserialize.py` & `evennia-4.1.0/evennia/utils/dbserialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 classes. These are iterables that track their position in a nested
 structure and makes sure to send updates up to their root. This is
 used by Attributes - without it, one would not be able to update mutables
 in-situ, e.g `obj.db.mynestedlist[3][5] = 3` would never be saved and
 be out of sync with the database.
 
 """
+
 from collections import OrderedDict, defaultdict, deque
 from collections.abc import MutableMapping, MutableSequence, MutableSet
 from functools import update_wrapper
 
 try:
     from pickle import UnpicklingError, dumps, loads
 except ImportError:
```

### Comparing `evennia-4.0.0/evennia/utils/eveditor.py` & `evennia-4.1.0/evennia/utils/eveditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
          persistent=True, code=False)
 ```
 
 The editor can also be used to format Python code and be made to
 survive a reload. See the `EvEditor` class for more details.
 
 """
+
 import re
 
 from django.conf import settings
 from django.utils.translation import gettext as _
 
 from evennia import CmdSet
 from evennia.commands import cmdhandler
@@ -84,15 +85,15 @@
 
  :dd <l>     - delete last line or line(s) <l>
  :dw <l> <w> - delete word or regex <w> in entire buffer or on line <l>
  :DD         - clear entire buffer
 
  :y  <l>        - yank (copy) line(s) <l> to the copy buffer
  :x  <l>        - cut line(s) <l> and store it in the copy buffer
- :p  <l>        - put (paste) previously copied line(s) directly after <l>
+ :p  <l>        - put (paste) previously copied line(s) directly before <l>
  :i  <l> <txt>  - insert new text <txt> at line <l>. Old line will move down
  :r  <l> <txt>  - replace line <l> with text <txt>
  :I  <l> <txt>  - insert text at the beginning of line <l>
  :A  <l> <txt>  - append text after the end of line <l>
 
  :s <l> <w> <txt> - search/replace word or regex <w> in buffer or on line <l>
 
@@ -301,20 +302,21 @@
         # form <lstart>:<lend>. Either of the ends could be missing, to
         # mean start/end of buffer respectively.
 
         lstart, lend = cline, cline + 1
         linerange = False
         if arglist and arglist[0].count(":") == 1:
             part1, part2 = arglist[0].split(":")
-            if part1 and part1.isdigit():
-                lstart = min(max(0, int(part1)) - 1, nlines)
-                linerange = True
-            if part2 and part2.isdigit():
-                lend = min(lstart + 1, int(part2)) + 1
-                linerange = True
+            lstart = min(max(1, int(part1)), nlines) - 1 if utils.value_is_integer(part1) else 0
+            lend = (
+                min(max(lstart + 1, int(part2)), nlines)
+                if utils.value_is_integer(part2)
+                else nlines
+            )
+            linerange = True
         elif arglist and arglist[0].isdigit():
             lstart = min(max(0, int(arglist[0]) - 1), nlines)
             lend = lstart + 1
             linerange = True
         if linerange:
             arglist = arglist[1:]
 
@@ -410,15 +412,15 @@
                 # display the current level of identation
                 indent = editor._indent
                 if indent < 0:
                     indent = "off"
 
                 self.caller.msg("|b%02i|||n (|g%s|n) %s" % (cline, indent, raw(line)))
             else:
-                self.caller.msg("|b%02i|||n %s" % (cline, raw(self.args)))
+                self.caller.msg("|b%02i|||n %s" % (cline, raw(line)))
 
 
 class CmdEditorGroup(CmdEditorBase):
     """
     Commands for the editor
     """
 
@@ -467,15 +469,16 @@
 
         """
         caller = self.caller
         editor = caller.ndb._eveditor
 
         linebuffer = self.linebuffer
         lstart, lend = self.lstart, self.lend
-        cmd = self.cmdstring
+        # preserve the cmdname including case (otherwise uu and UU would be the same)
+        cmd = self.raw_string[: len(self.cmdstring)]
         echo_mode = self.editor._echo_mode
 
         if cmd == ":":
             # Echo buffer
             if self.linerange:
                 buf = linebuffer[lstart:lend]
                 editor.display_buffer(buf=buf, offset=lstart)
```

### Comparing `evennia-4.0.0/evennia/utils/evennia-mode.el` & `evennia-4.1.0/evennia/utils/evennia-mode.el`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/evform.py` & `evennia-4.1.0/evennia/utils/evform.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/evmenu.py` & `evennia-4.1.0/evennia/utils/evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/evmore.py` & `evennia-4.1.0/evennia/utils/evmore.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/evtable.py` & `evennia-4.1.0/evennia/utils/evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/funcparser.py` & `evennia-4.1.0/evennia/utils/funcparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 ```
 
 The `FuncParser` also accepts a direct dict mapping of `{'name': callable, ...}`.
 
 ---
 
 """
+
 import dataclasses
 import inspect
 import random
 
 from django.conf import settings
 
 from evennia.utils import logger, search
```

### Comparing `evennia-4.0.0/evennia/utils/gametime.py` & `evennia-4.1.0/evennia/utils/gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/idmapper/LICENSE.md` & `evennia-4.1.0/evennia/utils/idmapper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/idmapper/README_evennia.md` & `evennia-4.1.0/evennia/utils/idmapper/README_evennia.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/idmapper/README_orig.rst` & `evennia-4.1.0/evennia/utils/idmapper/README_orig.rst`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/idmapper/manager.py` & `evennia-4.1.0/evennia/utils/idmapper/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 IDmapper extension to the default manager.
 """
+
 from django.db.models.manager import Manager
 
 
 class SharedMemoryManager(Manager):
     # TODO: improve on this implementation
     # We need a way to handle reverse lookups so that this model can
     # still use the singleton cache, but the active model isn't required
```

### Comparing `evennia-4.0.0/evennia/utils/idmapper/models.py` & `evennia-4.1.0/evennia/utils/idmapper/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/idmapper/tests.py` & `evennia-4.1.0/evennia/utils/idmapper/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/logger.py` & `evennia-4.1.0/evennia/utils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 arbitrary files in $GAME_DIR/server/logs.
 
 Note: All logging functions have two aliases, log_type() and
 log_typemsg(). This is for historical, back-compatible reasons.
 
 """
 
-
 import os
 import time
 from datetime import datetime
 from traceback import format_exc
 
 from twisted import logger as twisted_logger
 from twisted.internet.threads import deferToThread
```

### Comparing `evennia-4.0.0/evennia/utils/optionclasses.py` & `evennia-4.1.0/evennia/utils/optionclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/optionhandler.py` & `evennia-4.1.0/evennia/utils/optionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/picklefield.py` & `evennia-4.1.0/evennia/utils/picklefield.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/search.py` & `evennia-4.1.0/evennia/utils/search.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/test_resources.py` & `evennia-4.1.0/evennia/utils/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,33 +18,40 @@
 
 - `EvenniaTestMixin` - A class mixin for creating the test environment objects, for
   making custom tests.
 - `EvenniaCommandMixin` - A class mixin that adds support for command testing with the .call()
   helper. Used by the command-test classes, but can be used for making a customt test class.
 
 """
+
 import re
 import sys
 import types
 
-import evennia
 from django.conf import settings
 from django.test import TestCase, override_settings
+from mock import MagicMock, Mock, patch
+from twisted.internet.defer import Deferred
+
+import evennia
 from evennia import settings_default
 from evennia.accounts.accounts import DefaultAccount
 from evennia.commands.command import InterruptCommand
 from evennia.commands.default.muxcommand import MuxCommand
-from evennia.objects.objects import DefaultCharacter, DefaultExit, DefaultObject, DefaultRoom
+from evennia.objects.objects import (
+    DefaultCharacter,
+    DefaultExit,
+    DefaultObject,
+    DefaultRoom,
+)
 from evennia.scripts.scripts import DefaultScript
 from evennia.server.serversession import ServerSession
 from evennia.utils import ansi, create
 from evennia.utils.idmapper.models import flush_cache
 from evennia.utils.utils import all_from_module, to_str
-from mock import MagicMock, Mock, patch
-from twisted.internet.defer import Deferred
 
 _RE_STRIP_EVMENU = re.compile(r"^\+|-+\+|\+-+|--+|\|(?:\s|$)", re.MULTILINE)
 
 
 # set up a 'pristine' setting, unaffected by any changes in mygame
 DEFAULT_SETTING_RESETS = dict(
     CONNECTION_SCREEN_MODULE="evennia.game_template.server.conf.connection_screens",
```

### Comparing `evennia-4.0.0/evennia/utils/tests/data/evform_example.py` & `evennia-4.1.0/evennia/utils/tests/data/evform_example.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/data/evmenu_example.py` & `evennia-4.1.0/evennia/utils/tests/data/evmenu_example.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_ansi.py` & `evennia-4.1.0/evennia/utils/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_batchprocessors.py` & `evennia-4.1.0/evennia/utils/tests/test_batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_containers.py` & `evennia-4.1.0/evennia/utils/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_create_functions.py` & `evennia-4.1.0/evennia/utils/tests/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_dbserialize.py` & `evennia-4.1.0/evennia/utils/tests/test_dbserialize.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_eveditor.py` & `evennia-4.1.0/evennia/utils/tests/test_eveditor.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,87 @@
 """
 
 from evennia.commands.default.tests import BaseEvenniaCommandTest
 from evennia.utils import eveditor
 
 
 class TestEvEditor(BaseEvenniaCommandTest):
+    def test_eveditor_ranges(self):
+        eveditor.EvEditor(self.char1)
+        self.call(
+            eveditor.CmdEditorGroup(),
+            "",
+            raw_string=":",
+            msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
+        )
+        self.call(eveditor.CmdLineInput(), "line 1", raw_string="line 1", msg="01line 1")
+        self.call(eveditor.CmdLineInput(), "line 2", raw_string="line 2", msg="02line 2")
+        self.call(eveditor.CmdLineInput(), "line 3", raw_string="line 3", msg="03line 3")
+        self.call(eveditor.CmdLineInput(), "line 4", raw_string="line 4", msg="04line 4")
+        self.call(eveditor.CmdLineInput(), "line 5", raw_string="line 5", msg="05line 5")
+        self.call(
+            eveditor.CmdEditorGroup(),
+            "",  # list whole buffer
+            raw_string=":",
+            msg="Line Editor []\n01line 1\n02line 2\n"
+            "03line 3\n04line 4\n05line 5\n"
+            "[l:05 w:010 c:0034](:h for help)",
+        )
+        self.call(
+            eveditor.CmdEditorGroup(),
+            ":",  # list empty range
+            raw_string=":",
+            msg="Line Editor []\n01line 1\n02line 2\n"
+            "03line 3\n04line 4\n05line 5\n"
+            "[l:05 w:010 c:0034](:h for help)",
+        )
+        self.call(
+            eveditor.CmdEditorGroup(),
+            ":4",  # list from start to line 4
+            raw_string=":",
+            msg="Line Editor []\n01line 1\n02line 2\n"
+            "03line 3\n04line 4\n"
+            "[l:04 w:008 c:0027](:h for help)",
+        )
+        self.call(
+            eveditor.CmdEditorGroup(),
+            "2:",  # list from line 2 to end
+            raw_string=":",
+            msg="Line Editor []\n02line 2\n03line 3\n"
+            "04line 4\n05line 5\n"
+            "[l:04 w:008 c:0027](:h for help)",
+        )
+        self.call(
+            eveditor.CmdEditorGroup(),
+            "-10:10",  # try to list invalid range (too large)
+            raw_string=":",
+            msg="Line Editor []\n01line 1\n02line 2\n"
+            "03line 3\n04line 4\n05line 5\n"
+            "[l:05 w:010 c:0034](:h for help)",
+        )
+        self.call(
+            eveditor.CmdEditorGroup(),
+            "3:1",  # try to list invalid range (reversed)
+            raw_string=":",
+            msg="Line Editor []\n03line 3\n" "[l:01 w:002 c:0006](:h for help)",
+        )
+
     def test_eveditor_view_cmd(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":h",
+            raw_string=":h",
             msg="<txt>  - any non-command is appended to the end of the buffer.",
         )
         # empty buffer
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         # input a string
         self.call(
             eveditor.CmdLineInput(),
             "First test line",
             raw_string="First test line",
@@ -37,280 +97,290 @@
             msg="02Second test line",
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "First test line\nSecond test line")
 
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",  # view buffer
+            raw_string=":",  # view buffer
             msg="Line Editor []\n01First test line\n"
             "02Second test line\n[l:02 w:006 c:0032](:h for help)",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring="::",  # view buffer, no linenums
+            raw_string="::",  # view buffer, no linenums
             msg="Line Editor []\nFirst test line\n"
             "Second test line\n[l:02 w:006 c:0032](:h for help)",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":::",  # add single : alone on row
+            raw_string=":::",  # add single : alone on row
             msg="Single ':' added to buffer.",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01First test line\n"
             "02Second test line\n03:\n[l:03 w:007 c:0034](:h for help)",
         )
 
         self.call(
-            eveditor.CmdEditorGroup(), "", cmdstring=":dd", msg="Deleted line 3."  # delete line
+            eveditor.CmdEditorGroup(), "", raw_string=":dd", msg="Deleted line 3."  # delete line
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "First test line\nSecond test line")
-        self.call(eveditor.CmdEditorGroup(), "", cmdstring=":u", msg="Undid one step.")  # undo
+        self.call(eveditor.CmdEditorGroup(), "", raw_string=":u", msg="Undid one step.")  # undo
         self.assertEqual(
             self.char1.ndb._eveditor.get_buffer(), "First test line\nSecond test line\n:"
         )
-        self.call(eveditor.CmdEditorGroup(), "", cmdstring=":uu", msg="Redid one step.")  # redo
+        self.call(eveditor.CmdEditorGroup(), "", raw_string=":uu", msg="Redid one step.")  # redo
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "First test line\nSecond test line")
-        self.call(eveditor.CmdEditorGroup(), "", cmdstring=":u", msg="Undid one step.")  # undo
+        self.call(eveditor.CmdEditorGroup(), "", raw_string=":u", msg="Undid one step.")  # undo
         self.assertEqual(
             self.char1.ndb._eveditor.get_buffer(), "First test line\nSecond test line\n:"
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01First test line\n"
             "02Second test line\n03:\n[l:03 w:007 c:0034](:h for help)",
         )
 
         self.call(
             eveditor.CmdEditorGroup(),
             "Second",
-            cmdstring=":dw",  # delete by word
+            raw_string=":dw",  # delete by word
             msg="Removed Second for lines 1-4.",
         )
-        self.call(eveditor.CmdEditorGroup(), "", cmdstring=":u", msg="Undid one step.")  # undo
+        self.call(eveditor.CmdEditorGroup(), "", raw_string=":u", msg="Undid one step.")  # undo
         self.call(
             eveditor.CmdEditorGroup(),
             "2 Second",
-            cmdstring=":dw",  # delete by word/line
+            raw_string=":dw",  # delete by word/line
             msg="Removed Second for line 2.",
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "First test line\n test line\n:")
 
         self.call(
-            eveditor.CmdEditorGroup(), "2", cmdstring=":p", msg="Copy buffer is empty."  # paste
+            eveditor.CmdEditorGroup(), "2", raw_string=":p", msg="Copy buffer is empty."  # paste
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "2",
-            cmdstring=":y",  # yank
+            raw_string=":y",  # yank
             msg="Line 2, [' test line'] yanked.",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "2",
-            cmdstring=":p",  # paste
+            raw_string=":p",  # paste
             msg="Pasted buffer [' test line'] to line 2.",
         )
         self.assertEqual(
             self.char1.ndb._eveditor.get_buffer(), "First test line\n test line\n test line\n:"
         )
 
         self.call(
-            eveditor.CmdEditorGroup(), "3", cmdstring=":x", msg="Line 3, [' test line'] cut."  # cut
+            eveditor.CmdEditorGroup(),
+            "3",
+            raw_string=":x",
+            msg="Line 3, [' test line'] cut.",  # cut
         )
 
         self.call(
             eveditor.CmdEditorGroup(),
             "2 New Second line",
-            cmdstring=":i",  # insert
+            raw_string=":i",  # insert
             msg="Inserted 1 new line(s) at line 2.",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "2 New Replaced Second line",  # replace
-            cmdstring=":r",
+            raw_string=":r",
             msg="Replaced 1 line(s) at line 2.",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "2 Inserted-",  # insert beginning line
-            cmdstring=":I",
+            raw_string=":I",
             msg="Inserted text at beginning of line 2.",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "2 -End",  # append end line
-            cmdstring=":A",
+            raw_string=":A",
             msg="Appended text to end of line 2.",
         )
 
         self.assertEqual(
             self.char1.ndb._eveditor.get_buffer(),
             "First test line\nInserted-New Replaced Second line-End\n test line\n:",
         )
 
+        self.call(
+            eveditor.CmdLineInput(),
+            "  Whitespace   echo    test     line.",
+            raw_string="  Whitespace   echo    test     line.",
+            msg="05  Whitespace   echo    test     line.",
+        )
+
     def test_eveditor_COLON_UU(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         self.call(
             eveditor.CmdLineInput(),
             'First test "line".',
             raw_string='First test "line".',
-            msg='01First test "line" .',
+            msg='01First test "line".',
         )
         self.call(
             eveditor.CmdLineInput(),
             "Second 'line'.",
             raw_string="Second 'line'.",
-            msg="02Second 'line' .",
+            msg="02Second 'line'.",
         )
         self.assertEqual(
             self.char1.ndb._eveditor.get_buffer(), "First test \"line\".\nSecond 'line'."
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":UU",
+            raw_string=":UU",
             msg="Reverted all changes to the buffer back to original state.",
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "")
 
     def test_eveditor_search_and_replace(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         self.call(eveditor.CmdLineInput(), "line 1.", raw_string="line 1.", msg="01line 1.")
         self.call(eveditor.CmdLineInput(), "line 2.", raw_string="line 2.", msg="02line 2.")
         self.call(eveditor.CmdLineInput(), "line 3.", raw_string="line 3.", msg="03line 3.")
         self.call(
             eveditor.CmdEditorGroup(),
             "2:3",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n02line 2.\n03line 3.\n[l:02 w:004 c:0015](:h for help)",
         )
         self.call(
             eveditor.CmdEditorGroup(),
             "1:2 line LINE",
-            cmdstring=":s",
+            raw_string=":s",
             msg="Search-replaced line -> LINE for lines 1-2.",
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "LINE 1.\nLINE 2.\nline 3.")
         self.call(
             eveditor.CmdEditorGroup(),
             "line MINE",
-            cmdstring=":s",
+            raw_string=":s",
             msg="Search-replaced line -> MINE for lines 1-3.",
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "LINE 1.\nLINE 2.\nMINE 3.")
 
     def test_eveditor_COLON_DD(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         self.call(eveditor.CmdLineInput(), "line 1.", raw_string="line 1.", msg="01line 1.")
         self.call(eveditor.CmdLineInput(), "line 2.", raw_string="line 2.", msg="02line 2.")
         self.call(eveditor.CmdLineInput(), "line 3.", raw_string="line 3.", msg="03line 3.")
         self.call(
-            eveditor.CmdEditorGroup(), "", cmdstring=":DD", msg="Cleared 3 lines from buffer."
+            eveditor.CmdEditorGroup(), "", raw_string=":DD", msg="Cleared 3 lines from buffer."
         )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "")
 
     def test_eveditor_COLON_F(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         self.call(eveditor.CmdLineInput(), "line 1", raw_string="line 1", msg="01line 1")
-        self.call(eveditor.CmdEditorGroup(), "1:2", cmdstring=":f", msg="Flood filled lines 1-2.")
+        self.call(eveditor.CmdEditorGroup(), "1:2", raw_string=":f", msg="Flood filled line 1.")
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "line 1")
 
     def test_eveditor_COLON_J(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         self.call(eveditor.CmdLineInput(), "line 1", raw_string="line 1", msg="01line 1")
         self.call(eveditor.CmdLineInput(), "l 2", raw_string="l 2", msg="02l 2")
         self.call(eveditor.CmdLineInput(), "l 3", raw_string="l 3", msg="03l 3")
         self.call(eveditor.CmdLineInput(), "l 4", raw_string="l 4", msg="04l 4")
-        self.call(eveditor.CmdEditorGroup(), "2 r", cmdstring=":j", msg="Right-justified line 2.")
-        self.call(eveditor.CmdEditorGroup(), "3 c", cmdstring=":j", msg="Center-justified line 3.")
-        self.call(eveditor.CmdEditorGroup(), "4 f", cmdstring=":j", msg="Full-justified line 4.")
+        self.call(eveditor.CmdEditorGroup(), "2 r", raw_string=":j", msg="Right-justified line 2.")
+        self.call(eveditor.CmdEditorGroup(), "3 c", raw_string=":j", msg="Center-justified line 3.")
+        self.call(eveditor.CmdEditorGroup(), "4 f", raw_string=":j", msg="Full-justified line 4.")
         l1, l2, l3, l4 = tuple(self.char1.ndb._eveditor.get_buffer().split("\n"))
         self.assertEqual(l1, "line 1")
         self.assertEqual(l2, " " * 75 + "l 2")
         self.assertEqual(l3, " " * 37 + "l 3" + " " * 38)
         self.assertEqual(l4, "l" + " " * 76 + "4")
 
     def test_eveditor_bad_commands(self):
         eveditor.EvEditor(self.char1)
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":",
+            raw_string=":",
             msg="Line Editor []\n01\n[l:01 w:000 c:0000](:h for help)",
         )
         self.call(eveditor.CmdLineInput(), "line 1.", raw_string="line 1.", msg="01line 1.")
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":dw",
+            raw_string=":dw",
             msg="You must give a search word to delete.",
         )
         # self.call(
         #     eveditor.CmdEditorGroup(),
         #     raw_string="",
-        #     cmdstring=":i",
+        #     raw_string=":i",
         #     msg="You need to enter a new line and where to insert it.",
         # )
         # self.call(
         #     eveditor.CmdEditorGroup(),
         #     "",
-        #     cmdstring=":I",
+        #     raw_string=":I",
         #     msg="You need to enter text to insert.",
         # )
         # self.call(
         #     eveditor.CmdEditorGroup(),
         #     "",
-        #     cmdstring=":r",
+        #     raw_string=":r",
         #     msg="You need to enter a replacement string.",
         # )
         self.call(
             eveditor.CmdEditorGroup(),
             "",
-            cmdstring=":s",
+            raw_string=":s",
             msg="You must give a search word and something to replace it with.",
         )
         # self.call(
         #     eveditor.CmdEditorGroup(),
         #     "",
-        #     cmdstring=":f",
+        #     raw_string=":f",
         #     msg="Valid justifications are [f]ull (default), [c]enter, [r]right or [l]eft"
         # )
         self.assertEqual(self.char1.ndb._eveditor.get_buffer(), "line 1.")
```

### Comparing `evennia-4.0.0/evennia/utils/tests/test_evform.py` & `evennia-4.1.0/evennia/utils/tests/test_evform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Unit tests for the EvForm text form generator
 
 """
+
 from unittest import skip
 
 from django.test import TestCase
 
 from evennia.utils import ansi, evform, evtable
```

### Comparing `evennia-4.0.0/evennia/utils/tests/test_evmenu.py` & `evennia-4.1.0/evennia/utils/tests/test_evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_evtable.py` & `evennia-4.1.0/evennia/utils/tests/test_evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_funcparser.py` & `evennia-4.1.0/evennia/utils/tests/test_funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_gametime.py` & `evennia-4.1.0/evennia/utils/tests/test_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_search.py` & `evennia-4.1.0/evennia/utils/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_tagparsing.py` & `evennia-4.1.0/evennia/utils/tests/test_tagparsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Unit tests for all sorts of inline text-tag parsing, like ANSI, html conversion, inlinefuncs etc
 
 """
+
 import re
 
 from django.test import TestCase, override_settings
 
 from evennia.utils import funcparser
 from evennia.utils.ansi import ANSIString
 from evennia.utils.text2html import TextToHTMLparser
```

### Comparing `evennia-4.0.0/evennia/utils/tests/test_text2html.py` & `evennia-4.1.0/evennia/utils/tests/test_text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/tests/test_utils.py` & `evennia-4.1.0/evennia/utils/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 
 import os.path
 import random
 from datetime import datetime, timedelta
 
 import mock
 from django.test import TestCase
+from parameterized import parameterized
+from twisted.internet import task
+
 from evennia.utils import utils
 from evennia.utils.ansi import ANSIString
 from evennia.utils.test_resources import BaseEvenniaTest
-from parameterized import parameterized
-from twisted.internet import task
 
 
 class TestIsIter(TestCase):
     def test_is_iter(self):
         self.assertEqual(True, utils.is_iter([1, 2, 3, 4]))
         self.assertEqual(False, utils.is_iter("This is not an iterable"))
 
@@ -49,14 +50,51 @@
         self.assertEqual("TestDedent", utils.dedent("   TestDedent"))
         # Leading whitespace, multi line
         input_string = "  hello\n  world"
         expected_string = "hello\nworld"
         self.assertEqual(expected_string, utils.dedent(input_string))
 
 
+class TestCompressWhitespace(TestCase):
+    def test_compress_whitespace(self):
+        # No text, return no text
+        self.assertEqual("", utils.compress_whitespace(""))
+        # If no whitespace is exceeded, should return the same
+        self.assertEqual(
+            "One line\nTwo  spaces", utils.compress_whitespace("One line\nTwo  spaces")
+        )
+        # Extra newlines are removed
+        self.assertEqual(
+            "First line\nSecond line", utils.compress_whitespace("First line\n\nSecond line")
+        )
+        # Extra spaces are removed
+        self.assertEqual("Too  many  spaces", utils.compress_whitespace("Too   many      spaces"))
+        # "Invisible" extra lines with whitespace are removed
+        self.assertEqual(
+            "First line\nSecond line", utils.compress_whitespace("First line\n    \n \nSecond line")
+        )
+        # Max kwargs are respected
+        self.assertEqual(
+            "First line\n\nSecond line",
+            utils.compress_whitespace(
+                "First line\n\nSecond  line", max_spacing=1, max_linebreaks=2
+            ),
+        )
+
+    def test_preserve_indents(self):
+        """Ensure that indentation spacing is preserved."""
+        indented = """\
+Hanging Indents
+    they're great
+    let's keep them\
+"""
+        # since there is no doubled-up spacing besides indents, input should equal output
+        self.assertEqual(indented, utils.compress_whitespace(indented))
+
+
 class TestListToString(TestCase):
     """
     Default function header from time.py:
     list_to_string(inlist, sep=",", endsep=", and", addquote=False)
 
     Examples:
      with defaults:
```

### Comparing `evennia-4.0.0/evennia/utils/tests/test_validatorfuncs.py` & `evennia-4.1.0/evennia/utils/tests/test_validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/text2html.py` & `evennia-4.1.0/evennia/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/utils.py` & `evennia-4.1.0/evennia/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 from ast import literal_eval
 from collections import OrderedDict, defaultdict
 from inspect import getmembers, getmodule, getmro, ismodule, trace
 from os.path import join as osjoin
 from string import punctuation
 from unicodedata import east_asian_width
 
-import evennia
 from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.core.validators import validate_email as django_validate_email
 from django.utils import timezone
 from django.utils.html import strip_tags
 from django.utils.translation import gettext as _
-from evennia.utils import logger
 from simpleeval import simple_eval
 from twisted.internet import reactor, threads
 from twisted.internet.defer import returnValue  # noqa - used as import target
 from twisted.internet.task import deferLater
 
+import evennia
+from evennia.utils import logger
+
 _MULTIMATCH_TEMPLATE = settings.SEARCH_MULTIMATCH_TEMPLATE
 _EVENNIA_DIR = settings.EVENNIA_DIR
 _GAME_DIR = settings.GAME_DIR
 _IS_MAIN_THREAD = threading.current_thread().name == "MainThread"
 
 ENCODINGS = settings.ENCODINGS
 
@@ -468,14 +469,40 @@
         return f"{sep} ".join(str(v) for v in iterable[:-1]) + f"{endsep} {iterable[-1]}"
 
 
 # legacy aliases
 list_to_string = iter_to_str
 iter_to_string = iter_to_str
 
+re_empty = re.compile("\n\s*\n")
+
+
+def compress_whitespace(text, max_linebreaks=1, max_spacing=2):
+    """
+    Removes extra sequential whitespace in a block of text. This will also remove any trailing
+    whitespace at the end.
+
+    Args:
+        text (str):   A string which may contain excess internal whitespace.
+
+    Keyword args:
+        max_linebreaks (int):  How many linebreak characters are allowed to occur in a row.
+        max_spacing (int):     How many spaces are allowed to occur in a row.
+
+    """
+    text = text.rstrip()
+    # replaces any non-visible lines that are just whitespace characters with actual empty lines
+    # this allows the blank-line compression to eliminate them if needed
+    text = re_empty.sub("\n\n", text)
+    # replace groups of extra spaces with the maximum number of spaces
+    text = re.sub(f"(?<=\S) {{{max_spacing},}}", " " * max_spacing, text)
+    # replace groups of extra newlines with the maximum number of newlines
+    text = re.sub(f"\n{{{max_linebreaks},}}", "\n" * max_linebreaks, text)
+    return text
+
 
 def wildcard_to_regexp(instring):
     """
     Converts a player-supplied string that may have wildcards in it to
     regular expressions. This is useful for name matching.
 
     Args:
@@ -2041,15 +2068,15 @@
                 except IndexError:
                     # we extended past edge of grid, crop or move to next line
                     if ic == 0:
                         row = crop(element, width)
                     else:
                         row += " " * max(0, width - lrow)
                     rows.append(row)
-                    row = ""
+                    row = element
                     ic = 0
                 else:
                     # add a new slot
                     row += element + " " * max(0, averlen - wl)
                     ic += 1
 
             if ie >= nelements - 1:
@@ -2373,29 +2400,27 @@
         for num, result in enumerate(matches):
             # we need to consider that result could be a Command, where .aliases
             # is a list of strings
             if hasattr(result.aliases, "all"):
                 # result is a typeclassed entity where `.aliases` is an AliasHandler.
                 aliases = result.aliases.all(return_objs=True)
                 # remove pluralization aliases
-                aliases = [
-                    alias
-                    for alias in aliases
-                    if hasattr(alias, "category") and alias.category not in ("plural_key",)
-                ]
+                aliases = [alias.db_key for alias in aliases if alias.db_category != "plural_key"]
             else:
                 # result is likely a Command, where `.aliases` is a list of strings.
                 aliases = result.aliases
 
             error += _MULTIMATCH_TEMPLATE.format(
                 number=num + 1,
-                name=result.get_display_name(caller)
-                if hasattr(result, "get_display_name")
-                else query,
-                aliases=" [{alias}]".format(alias=";".join(aliases) if aliases else ""),
+                name=(
+                    result.get_display_name(caller)
+                    if hasattr(result, "get_display_name")
+                    else query
+                ),
+                aliases=" [{alias}]".format(alias=";".join(aliases)) if aliases else "",
                 info=result.get_extra_info(caller),
             )
         matches = None
     else:
         # exactly one match
         matches = matches[0]
 
@@ -3048,7 +3073,25 @@
 
     for addr in reversed(addresses):
         if all(not match_ip(addr, pattern) for pattern in exclude):
             return addr
 
     logger.log_warn("ip_from_request: No valid IP address found in request. Using remote_addr.")
     return remote_addr
+
+
+def value_is_integer(value):
+    """
+    Determines if a value can be type-cast to an integer.
+
+    Args:
+        value (any): The value to check.
+
+    Returns:
+        result (bool): Whether it can be type-cast to an integer or not.
+    """
+    try:
+        int(value)
+    except ValueError:
+        return False
+
+    return True
```

### Comparing `evennia-4.0.0/evennia/utils/validatorfuncs.py` & `evennia-4.1.0/evennia/utils/validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/verb_conjugation/LICENSE.txt` & `evennia-4.1.0/evennia/utils/verb_conjugation/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/verb_conjugation/conjugate.py` & `evennia-4.1.0/evennia/utils/verb_conjugation/conjugate.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/verb_conjugation/pronouns.py` & `evennia-4.1.0/evennia/utils/verb_conjugation/pronouns.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 3rd person male         he       him       his        his        himself
 3rd person female       she      her       her        hers       herself
 3rd person neutral      it       it        its        its        itself
 3rd person plural       they     them      their      theirs     themselves
 ====================  =======  ========  ==========  ==========  ===========
 """
+
 from evennia.utils.utils import copy_word_case, is_iter
 
 DEFAULT_PRONOUN_TYPE = "subject pronoun"
 DEFAULT_VIEWPOINT = "2nd person"
 DEFAULT_GENDER = "neutral"
 
 PRONOUN_TYPES = [
```

### Comparing `evennia-4.0.0/evennia/utils/verb_conjugation/tests.py` & `evennia-4.1.0/evennia/utils/verb_conjugation/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/utils/verb_conjugation/verbs.txt` & `evennia-4.1.0/evennia/utils/verb_conjugation/verbs.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/README.md` & `evennia-4.1.0/evennia/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/accounts.py` & `evennia-4.1.0/evennia/web/admin/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/attributes.py` & `evennia-4.1.0/evennia/web/admin/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/comms.py` & `evennia-4.1.0/evennia/web/admin/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/frontpage.py` & `evennia-4.1.0/evennia/web/admin/frontpage.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/help.py` & `evennia-4.1.0/evennia/web/admin/help.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This defines how to edit help entries in Admin.
 """
+
 from django import forms
 from django.contrib import admin
 
 from evennia.help.models import HelpEntry
 
 from .tags import TagInline
```

### Comparing `evennia-4.0.0/evennia/web/admin/objects.py` & `evennia-4.1.0/evennia/web/admin/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/scripts.py` & `evennia-4.1.0/evennia/web/admin/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/admin/tags.py` & `evennia-4.1.0/evennia/web/admin/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Tag admin
 
 """
 
-
 import traceback
 from datetime import datetime
 
 from django import forms
 from django.contrib import admin
 
 from evennia.typeclasses.tags import Tag
```

### Comparing `evennia-4.0.0/evennia/web/admin/urls.py` & `evennia-4.1.0/evennia/web/admin/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Rerouting admin frontpage to evennia version.
 
 These patterns are all under the admin/* namespace.
 
 """
+
 from django.conf import settings
 from django.contrib import admin
 from django.urls import include, path
 
 from . import frontpage
 
 urlpatterns = [
```

### Comparing `evennia-4.0.0/evennia/web/admin/utils.py` & `evennia-4.1.0/evennia/web/admin/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/api/README.md` & `evennia-4.1.0/evennia/web/api/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/api/filters.py` & `evennia-4.1.0/evennia/web/api/filters.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 that is retrieved in GET requests. By default, Django Rest Framework uses the
 'django-filter' package as its backend. Django-filter also has a section in its
 documentation specifically regarding DRF integration.
 
 https://django-filter.readthedocs.io/en/latest/guide/rest_framework.html
 
 """
+
 from typing import Union
 
 from django.db.models import Q
 from django_filters.filters import EMPTY_VALUES, CharFilter
 from django_filters.rest_framework.filterset import FilterSet
 
 from evennia.accounts.models import AccountDB
@@ -134,15 +135,14 @@
             "db_is_active",
             "db_persistent",
             "db_interval",
         ]
 
 
 class HelpFilterSet(FilterSet):
-
     """
     Filter for help entries
 
     """
 
     name = CharFilter(lookup_expr="iexact", method="filter_name", field_name="db_key")
     category = CharFilter(lookup_expr="iexact", method="filter_name", field_name="db_category")
```

### Comparing `evennia-4.0.0/evennia/web/api/permissions.py` & `evennia-4.1.0/evennia/web/api/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Sets up an api-access permission check using the in-game permission hierarchy.
 
 """
 
-
 from django.conf import settings
 from rest_framework import permissions
 
 from evennia.locks.lockhandler import check_perm
 
 
 class EvenniaPermission(permissions.BasePermission):
```

### Comparing `evennia-4.0.0/evennia/web/api/serializers.py` & `evennia-4.1.0/evennia/web/api/serializers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/api/tests.py` & `evennia-4.1.0/evennia/web/api/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tests for the REST API.
 
 """
+
 from collections import namedtuple
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.test import override_settings
 from django.urls import include, path, reverse
 from rest_framework.test import APIClient
```

### Comparing `evennia-4.0.0/evennia/web/api/urls.py` & `evennia-4.1.0/evennia/web/api/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/api/views.py` & `evennia-4.1.0/evennia/web/api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Views are the functions that are called by different url endpoints. The Django
 Rest Framework provides collections called 'ViewSets', which can generate a
 number of views for the common CRUD operations.
 
 """
+
 from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework import status
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework.viewsets import ModelViewSet
 
 from evennia.accounts.models import AccountDB
```

### Comparing `evennia-4.0.0/evennia/web/static/rest_framework/images/favicon.ico` & `evennia-4.1.0/evennia/web/static/rest_framework/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/css/goldenlayout.css` & `evennia-4.1.0/evennia/web/static/webclient/css/goldenlayout.css`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/css/webclient.css` & `evennia-4.1.0/evennia/web/static/webclient/css/webclient.css`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff` & `evennia-4.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/evennia.js` & `evennia-4.1.0/evennia/web/static/webclient/js/evennia.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/clienthelp.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/clienthelp.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/default_in.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_in.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/default_out.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_out.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/font.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/font.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/goldenlayout.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/history.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/history.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/hotbuttons.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/hotbuttons.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/html.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/html.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/iframe.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/iframe.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/message_routing.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/message_routing.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/multimedia.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/multimedia.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/notifications.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/notifications.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/oob.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/oob.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/options2.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/options2.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/popups.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/popups.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/plugins/text2html.js` & `evennia-4.1.0/evennia/web/static/webclient/js/plugins/text2html.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/js/webclient_gui.js` & `evennia-4.1.0/evennia/web/static/webclient/js/webclient_gui.js`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/webclient/media/notification.wav` & `evennia-4.1.0/evennia/web/static/webclient/media/notification.wav`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/website/css/website.css` & `evennia-4.1.0/evennia/web/static/website/css/website.css`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/website/images/evennia_logo.png` & `evennia-4.1.0/evennia/web/static/website/images/evennia_logo.png`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/website/images/evennia_logo_festive.png` & `evennia-4.1.0/evennia/web/static/website/images/evennia_logo_festive.png`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/static/website/images/favicon.ico` & `evennia-4.1.0/evennia/web/static/website/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/admin/app_list.html` & `evennia-4.1.0/evennia/web/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/admin/frontpage.html` & `evennia-4.1.0/evennia/web/templates/admin/frontpage.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/rest_framework/api.html` & `evennia-4.1.0/evennia/web/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/webclient/base.html` & `evennia-4.1.0/evennia/web/templates/webclient/base.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/webclient/webclient.html` & `evennia-4.1.0/evennia/web/templates/webclient/webclient.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/500.html` & `evennia-4.1.0/evennia/web/templates/website/500.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/_menu.html` & `evennia-4.1.0/evennia/web/templates/website/_menu.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/base.html` & `evennia-4.1.0/evennia/web/templates/website/base.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/channel_detail.html` & `evennia-4.1.0/evennia/web/templates/website/channel_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/channel_list.html` & `evennia-4.1.0/evennia/web/templates/website/channel_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/character_form.html` & `evennia-4.1.0/evennia/web/templates/website/character_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/character_list.html` & `evennia-4.1.0/evennia/web/templates/website/character_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/character_manage_list.html` & `evennia-4.1.0/evennia/web/templates/website/character_manage_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/generic_form.html` & `evennia-4.1.0/evennia/web/templates/website/generic_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/help_detail.html` & `evennia-4.1.0/evennia/web/templates/website/help_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/help_list.html` & `evennia-4.1.0/evennia/web/templates/website/help_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/homepage/accounts-widget.html` & `evennia-4.1.0/evennia/web/templates/website/homepage/accounts-widget.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/homepage/database-stats-widget.html` & `evennia-4.1.0/evennia/web/templates/website/homepage/database-stats-widget.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/homepage/evennia-widget.html` & `evennia-4.1.0/evennia/web/templates/website/homepage/evennia-widget.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/homepage/main-content.html` & `evennia-4.1.0/evennia/web/templates/website/homepage/main-content.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/index.html` & `evennia-4.1.0/evennia/web/templates/website/index.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/object_confirm_delete.html` & `evennia-4.1.0/evennia/web/templates/website/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/object_detail.html` & `evennia-4.1.0/evennia/web/templates/website/object_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/object_list.html` & `evennia-4.1.0/evennia/web/templates/website/object_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/pagination.html` & `evennia-4.1.0/evennia/web/templates/website/pagination.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/logged_out.html` & `evennia-4.1.0/evennia/web/templates/website/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/login.html` & `evennia-4.1.0/evennia/web/templates/website/registration/login.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_change_done.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_change_form.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_reset_complete.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_reset_confirm.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_reset_done.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_reset_email.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/password_reset_form.html` & `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/registration/register.html` & `evennia-4.1.0/evennia/web/templates/website/registration/register.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templates/website/tbi.html` & `evennia-4.1.0/evennia/web/templates/website/tbi.html`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/templatetags/addclass.py` & `evennia-4.1.0/evennia/web/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/urls.py` & `evennia-4.1.0/evennia/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/adminsite.py` & `evennia-4.1.0/evennia/web/utils/adminsite.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/apache_wsgi.conf` & `evennia-4.1.0/evennia/web/utils/apache_wsgi.conf`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/backends.py` & `evennia-4.1.0/evennia/web/utils/backends.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/evennia_modpy_apache.conf` & `evennia-4.1.0/evennia/web/utils/evennia_modpy_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/evennia_wsgi_apache.conf` & `evennia-4.1.0/evennia/web/utils/evennia_wsgi_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/general_context.py` & `evennia-4.1.0/evennia/web/utils/general_context.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 context without having to repeatedly include it.
 
 For this to work, this file is included in the settings file, in the
 TEMPLATES["OPTIONS"]["context_processors"] list.
 
 """
 
-
 import os
 
 from django.conf import settings
+
 from evennia.utils.utils import get_evennia_version
 
 # Setup lists of the most relevant apps so
 # the adminsite becomes more readable.
 
 GAME_NAME = None
 GAME_SLOGAN = None
```

### Comparing `evennia-4.0.0/evennia/web/utils/middleware.py` & `evennia-4.1.0/evennia/web/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/utils/tests.py` & `evennia-4.1.0/evennia/web/utils/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/webclient/views.py` & `evennia-4.1.0/evennia/web/webclient/views.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/website/forms.py` & `evennia-4.1.0/evennia/web/website/forms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/website/tests.py` & `evennia-4.1.0/evennia/web/website/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/website/urls.py` & `evennia-4.1.0/evennia/web/website/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This redirects to website sub-pages.
 
 """
+
 from django.conf import settings
 from django.contrib import admin
 from django.urls import include, path
 
 from .views import accounts, channels, characters, errors
 from .views import help as helpviews
 from .views import index
```

### Comparing `evennia-4.0.0/evennia/web/website/views/accounts.py` & `evennia-4.1.0/evennia/web/website/views/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Views for managing accounts.
 
 """
 
-
 from django.conf import settings
 from django.contrib import messages
 from django.http import HttpResponseRedirect
 from django.urls import reverse_lazy
 
 from evennia.utils import class_from_module
 from evennia.web.website import forms
```

### Comparing `evennia-4.0.0/evennia/web/website/views/channels.py` & `evennia-4.1.0/evennia/web/website/views/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/website/views/characters.py` & `evennia-4.1.0/evennia/web/website/views/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 from django.db.models.functions import Lower
 from django.http import HttpResponseRedirect
 from django.urls import reverse_lazy
 from django.utils.encoding import iri_to_uri
 from django.utils.http import url_has_allowed_host_and_scheme
 from django.views.generic import ListView
 from django.views.generic.base import RedirectView
+
 from evennia.utils import class_from_module
 from evennia.web.website import forms
 
 from .mixins import TypeclassMixin
-from .objects import (ObjectCreateView, ObjectDeleteView, ObjectDetailView,
-                      ObjectUpdateView)
+from .objects import (
+    ObjectCreateView,
+    ObjectDeleteView,
+    ObjectDetailView,
+    ObjectUpdateView,
+)
 
 
 class CharacterMixin(TypeclassMixin):
     """
     This is a "mixin", a modifier of sorts.
 
     Any view class with this in its inheritance list will be modified to work
@@ -120,31 +125,32 @@
         char = self.get_object()
 
         # Get the page the user came from
         next_page = self.request.GET.get("next", self.success_url)
 
         # since next_page is untrusted input from the user, we need to check it's safe to
         next_page = iri_to_uri(next_page)
-        if not url_has_allowed_host_and_scheme(url=next_page,
-                                               allowed_hosts={self.request.get_host()},
-                                               require_https=self.request.is_secure()):
+        if not url_has_allowed_host_and_scheme(
+            url=next_page,
+            allowed_hosts={self.request.get_host()},
+            require_https=self.request.is_secure(),
+        ):
             next_page = self.success_url
 
         if char:
             # If the account owns the char, store the ID of the char in the
             # Django request's session (different from Evennia session!).
             # We do this because characters don't serialize well.
             self.request.session["puppet"] = int(char.pk)
             messages.success(self.request, "You become '%s'!" % char)
         else:
             # If the puppeting failed, clear out the cached puppet value
             self.request.session["puppet"] = None
             messages.error(self.request, "You cannot become '%s'." % char)
 
-
         return next_page
 
 
 class CharacterManageView(LoginRequiredMixin, CharacterMixin, ListView):
     """
     This view provides a mechanism by which a logged-in player can browse,
     edit, or delete their own characters.
```

### Comparing `evennia-4.0.0/evennia/web/website/views/help.py` & `evennia-4.1.0/evennia/web/website/views/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Views to manipulate help entries.
 
 Multi entry object type supported added by DaveWithTheNiceHat 2021
     Pull Request #2429
 """
+
 from django.conf import settings
 from django.http import HttpResponseBadRequest
 from django.utils.text import slugify
 from django.views.generic import DetailView, ListView
 
 from evennia.help.filehelp import FILE_HELP_ENTRIES
 from evennia.help.models import HelpEntry
```

### Comparing `evennia-4.0.0/evennia/web/website/views/index.py` & `evennia-4.1.0/evennia/web/website/views/index.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia/web/website/views/mixins.py` & `evennia-4.1.0/evennia/web/website/views/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 These are mixins for class-based views, granting functionality.
 
 """
+
 from django.views.generic import DetailView
 from django.views.generic.edit import CreateView, DeleteView, UpdateView
 
 
 class TypeclassMixin:
     """
     This is a "mixin", a modifier of sorts.
```

### Comparing `evennia-4.0.0/evennia/web/website/views/objects.py` & `evennia-4.1.0/evennia/web/website/views/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia.egg-info/PKG-INFO` & `evennia-4.1.0/evennia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 4.0.0
+Version: 4.1.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-4.0.0/evennia.egg-info/SOURCES.txt` & `evennia-4.1.0/evennia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/evennia.egg-info/requires.txt` & `evennia-4.1.0/evennia.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.0.0/pyproject.toml` & `evennia-4.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evennia"
-version = "4.0.0"
+version = "4.1.0"
 maintainers = [{ name = "Griatch", email = "griatch@gmail.com" }]
 description = "A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc)."
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "BSD" }
 keywords = [
   "MUD",
```

### Comparing `evennia-4.0.0/setup.py` & `evennia-4.1.0/setup.py`

 * *Files identical despite different names*

