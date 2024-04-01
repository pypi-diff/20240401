# Comparing `tmp/spellbot-9.6.0.tar.gz` & `tmp/spellbot-9.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spellbot-9.6.0.tar", max compression
+gzip compressed data, was "spellbot-9.7.0.tar", max compression
```

## Comparing `spellbot-9.6.0.tar` & `spellbot-9.7.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-9.6.0/LICENSE.md
--rw-r--r--   0        0        0    11020 2023-12-11 18:35:09.859783 spellbot-9.6.0/README.md
--rw-r--r--   0        0        0     3621 2024-01-31 04:52:13.172223 spellbot-9.6.0/pyproject.toml
--rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-9.6.0/src/spellbot/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-25 03:19:31.669125 spellbot-9.6.0/src/spellbot/_version.py
--rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-9.6.0/src/spellbot/actions/__init__.py
--rw-r--r--   0        0        0    16657 2024-01-26 19:35:36.678250 spellbot-9.6.0/src/spellbot/actions/admin_action.py
--rw-r--r--   0        0        0     3577 2023-10-04 20:26:02.206484 spellbot-9.6.0/src/spellbot/actions/base_action.py
--rw-r--r--   0        0        0     2578 2024-01-26 19:35:36.678455 spellbot-9.6.0/src/spellbot/actions/block_action.py
--rw-r--r--   0        0        0     1719 2023-10-04 20:26:02.206670 spellbot-9.6.0/src/spellbot/actions/config_action.py
--rw-r--r--   0        0        0     4951 2023-10-04 20:26:02.206863 spellbot-9.6.0/src/spellbot/actions/leave_action.py
--rw-r--r--   0        0        0    19660 2024-01-26 19:35:36.678658 spellbot-9.6.0/src/spellbot/actions/lfg_action.py
--rw-r--r--   0        0        0     3253 2024-01-26 19:35:36.678865 spellbot-9.6.0/src/spellbot/actions/score_action.py
--rw-r--r--   0        0        0     7517 2023-12-12 01:25:50.877929 spellbot-9.6.0/src/spellbot/actions/tasks_action.py
--rw-r--r--   0        0        0      996 2023-10-04 20:26:02.207631 spellbot-9.6.0/src/spellbot/actions/verify_action.py
--rw-r--r--   0        0        0     4824 2024-01-26 19:35:36.679117 spellbot-9.6.0/src/spellbot/actions/watch_action.py
--rw-r--r--   0        0        0     3470 2023-10-17 21:34:04.984133 spellbot-9.6.0/src/spellbot/cli.py
--rw-r--r--   0        0        0     6715 2024-01-15 05:47:30.079395 spellbot-9.6.0/src/spellbot/client.py
--rw-r--r--   0        0        0     2082 2023-10-04 20:26:02.208297 spellbot-9.6.0/src/spellbot/cogs/__init__.py
--rw-r--r--   0        0        0     1992 2024-01-26 19:35:36.679324 spellbot-9.6.0/src/spellbot/cogs/about_cog.py
--rw-r--r--   0        0        0    11941 2023-10-17 21:30:53.733467 spellbot-9.6.0/src/spellbot/cogs/admin_cog.py
--rw-r--r--   0        0        0     2235 2023-11-26 20:42:37.444094 spellbot-9.6.0/src/spellbot/cogs/block_cog.py
--rw-r--r--   0        0        0     1708 2023-10-04 20:26:02.208634 spellbot-9.6.0/src/spellbot/cogs/config_cog.py
--rw-r--r--   0        0        0     1672 2023-10-17 21:30:53.733656 spellbot-9.6.0/src/spellbot/cogs/events_cog.py
--rw-r--r--   0        0        0     1806 2023-10-16 00:46:59.592231 spellbot-9.6.0/src/spellbot/cogs/leave_cog.py
--rw-r--r--   0        0        0     1999 2023-10-17 21:30:53.733828 spellbot-9.6.0/src/spellbot/cogs/lfg_cog.py
--rw-r--r--   0        0        0     3128 2023-04-25 03:19:31.674236 spellbot-9.6.0/src/spellbot/cogs/owner_cog.py
--rw-r--r--   0        0        0     2210 2023-11-26 20:42:37.444318 spellbot-9.6.0/src/spellbot/cogs/score_cog.py
--rw-r--r--   0        0        0     1130 2023-04-25 03:19:31.674692 spellbot-9.6.0/src/spellbot/cogs/sync_cog.py
--rw-r--r--   0        0        0     3485 2023-10-04 20:26:02.209316 spellbot-9.6.0/src/spellbot/cogs/tasks_cog.py
--rw-r--r--   0        0        0     1658 2023-04-25 03:19:31.675274 spellbot-9.6.0/src/spellbot/cogs/verify_cog.py
--rw-r--r--   0        0        0     2672 2023-10-04 20:26:02.209482 spellbot-9.6.0/src/spellbot/cogs/watch_cog.py
--rw-r--r--   0        0        0     4708 2023-10-04 20:26:02.209682 spellbot-9.6.0/src/spellbot/database.py
--rw-r--r--   0        0        0     1864 2024-01-29 02:08:47.334112 spellbot-9.6.0/src/spellbot/enums.py
--rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-9.6.0/src/spellbot/environment.py
--rw-r--r--   0        0        0     1125 2023-04-25 03:19:31.676087 spellbot-9.6.0/src/spellbot/errors.py
--rw-r--r--   0        0        0      939 2023-04-25 03:19:31.676348 spellbot-9.6.0/src/spellbot/logs.py
--rw-r--r--   0        0        0     5005 2024-01-31 04:50:24.265672 spellbot-9.6.0/src/spellbot/metrics.py
--rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-9.6.0/src/spellbot/migrations/alembic.ini
--rw-r--r--   0        0        0     1638 2023-04-25 03:19:31.676886 spellbot-9.6.0/src/spellbot/migrations/env.py
--rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-9.6.0/src/spellbot/migrations/script.py.mako
--rw-r--r--   0        0        0     2924 2023-10-04 20:26:02.209820 spellbot-9.6.0/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py
--rw-r--r--   0        0        0     1412 2023-10-04 21:07:34.717844 spellbot-9.6.0/src/spellbot/migrations/versions/1503d49ae8e1_adds_created_at_and_updated_at_to_more_.py
--rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-9.6.0/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
--rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-9.6.0/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
--rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-9.6.0/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
--rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-9.6.0/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
--rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-9.6.0/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
--rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-9.6.0/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
--rw-r--r--   0        0        0      814 2023-10-17 21:30:53.734098 spellbot-9.6.0/src/spellbot/migrations/versions/b2d4a9aa1aed_adds_default_format_to_channel.py
--rw-r--r--   0        0        0      476 2023-10-04 20:26:02.209939 spellbot-9.6.0/src/spellbot/migrations/versions/c03099407b40_support_extra_message_content.py
--rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-9.6.0/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
--rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-9.6.0/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
--rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-9.6.0/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
--rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-9.6.0/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
--rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-9.6.0/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
--rw-r--r--   0        0        0     1436 2023-10-17 21:30:53.734307 spellbot-9.6.0/src/spellbot/models/__init__.py
--rw-r--r--   0        0        0     3372 2023-10-04 20:40:25.401304 spellbot-9.6.0/src/spellbot/models/award.py
--rw-r--r--   0        0        0     2635 2023-10-04 21:07:34.718050 spellbot-9.6.0/src/spellbot/models/base.py
--rw-r--r--   0        0        0     1493 2023-10-04 21:07:34.718261 spellbot-9.6.0/src/spellbot/models/block.py
--rw-r--r--   0        0        0     4593 2023-11-02 17:50:09.483011 spellbot-9.6.0/src/spellbot/models/channel.py
--rw-r--r--   0        0        0     1059 2023-10-04 20:34:58.485690 spellbot-9.6.0/src/spellbot/models/config.py
--rw-r--r--   0        0        0    11055 2024-01-26 19:35:36.679639 spellbot-9.6.0/src/spellbot/models/game.py
--rw-r--r--   0        0        0     2714 2023-11-02 17:50:09.483390 spellbot-9.6.0/src/spellbot/models/guild.py
--rw-r--r--   0        0        0     1707 2023-11-02 17:50:09.483577 spellbot-9.6.0/src/spellbot/models/play.py
--rw-r--r--   0        0        0      855 2023-11-02 17:44:44.999754 spellbot-9.6.0/src/spellbot/models/queue.py
--rw-r--r--   0        0        0     4381 2023-11-02 17:42:54.141332 spellbot-9.6.0/src/spellbot/models/user.py
--rw-r--r--   0        0        0      952 2023-10-04 20:26:02.211355 spellbot-9.6.0/src/spellbot/models/verify.py
--rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-9.6.0/src/spellbot/models/watch.py
--rw-r--r--   0        0        0    19340 2023-12-12 01:18:55.704911 spellbot-9.6.0/src/spellbot/operations.py
--rw-r--r--   0        0        0     1059 2023-04-25 03:19:31.678344 spellbot-9.6.0/src/spellbot/services/__init__.py
--rw-r--r--   0        0        0     3202 2023-10-04 20:26:02.211733 spellbot-9.6.0/src/spellbot/services/awards.py
--rw-r--r--   0        0        0     5946 2023-10-17 21:30:53.734897 spellbot-9.6.0/src/spellbot/services/channels.py
--rw-r--r--   0        0        0     1555 2023-10-04 20:26:02.212048 spellbot-9.6.0/src/spellbot/services/configs.py
--rw-r--r--   0        0        0    16010 2024-01-31 04:50:24.265901 spellbot-9.6.0/src/spellbot/services/games.py
--rw-r--r--   0        0        0     4880 2023-11-02 17:50:09.484028 spellbot-9.6.0/src/spellbot/services/guilds.py
--rw-r--r--   0        0        0     7637 2023-10-17 21:30:53.735085 spellbot-9.6.0/src/spellbot/services/plays.py
--rw-r--r--   0        0        0    15575 2023-11-02 17:50:09.484399 spellbot-9.6.0/src/spellbot/services/users.py
--rw-r--r--   0        0        0     1631 2023-10-04 20:26:02.212868 spellbot-9.6.0/src/spellbot/services/verifies.py
--rw-r--r--   0        0        0      504 2023-10-04 20:26:02.213006 spellbot-9.6.0/src/spellbot/services/watches.py
--rw-r--r--   0        0        0     3991 2024-01-26 19:35:36.680093 spellbot-9.6.0/src/spellbot/settings.py
--rw-r--r--   0        0        0     2377 2023-10-04 20:26:02.213317 spellbot-9.6.0/src/spellbot/spelltable.py
--rw-r--r--   0        0        0    11375 2023-12-12 01:15:07.924888 spellbot-9.6.0/src/spellbot/utils.py
--rw-r--r--   0        0        0      295 2023-04-26 18:55:38.771824 spellbot-9.6.0/src/spellbot/views/__init__.py
--rw-r--r--   0        0        0      302 2023-04-25 03:19:31.680995 spellbot-9.6.0/src/spellbot/views/base_view.py
--rw-r--r--   0        0        0     4108 2024-01-02 03:43:15.077144 spellbot-9.6.0/src/spellbot/views/lfg_view.py
--rw-r--r--   0        0        0     2530 2024-01-02 03:43:15.077403 spellbot-9.6.0/src/spellbot/views/setup_view.py
--rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-9.6.0/src/spellbot/web/__init__.py
--rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-9.6.0/src/spellbot/web/api/__init__.py
--rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-9.6.0/src/spellbot/web/api/ping.py
--rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-9.6.0/src/spellbot/web/api/record.py
--rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-9.6.0/src/spellbot/web/builder.py
--rw-r--r--   0        0        0      689 2023-11-24 20:31:01.432756 spellbot-9.6.0/src/spellbot/web/server.py
--rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-9.6.0/src/spellbot/web/templates/channel_record.html.j2
--rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-9.6.0/src/spellbot/web/templates/record.css
--rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-9.6.0/src/spellbot/web/templates/record_base.html.j2
--rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-9.6.0/src/spellbot/web/templates/table2CSV.js
--rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-9.6.0/src/spellbot/web/templates/user_record.html.j2
--rw-r--r--   0        0        0    13100 1970-01-01 00:00:00.000000 spellbot-9.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 21:36:17.595731 spellbot-9.7.0/LICENSE.md
+-rw-r--r--   0        0        0    11020 2023-12-11 18:35:09.859783 spellbot-9.7.0/README.md
+-rw-r--r--   0        0        0     3630 2024-02-02 23:51:31.438634 spellbot-9.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0      183 2023-04-18 21:36:17.604155 spellbot-9.7.0/src/spellbot/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-25 03:19:31.669125 spellbot-9.7.0/src/spellbot/_version.py
+-rw-r--r--   0        0        0      586 2023-04-18 21:36:17.604317 spellbot-9.7.0/src/spellbot/actions/__init__.py
+-rw-r--r--   0        0        0    16657 2024-01-26 19:35:36.678250 spellbot-9.7.0/src/spellbot/actions/admin_action.py
+-rw-r--r--   0        0        0     3577 2023-10-04 20:26:02.206484 spellbot-9.7.0/src/spellbot/actions/base_action.py
+-rw-r--r--   0        0        0     2578 2024-01-26 19:35:36.678455 spellbot-9.7.0/src/spellbot/actions/block_action.py
+-rw-r--r--   0        0        0     1719 2023-10-04 20:26:02.206670 spellbot-9.7.0/src/spellbot/actions/config_action.py
+-rw-r--r--   0        0        0     4951 2023-10-04 20:26:02.206863 spellbot-9.7.0/src/spellbot/actions/leave_action.py
+-rw-r--r--   0        0        0    19660 2024-01-26 19:35:36.678658 spellbot-9.7.0/src/spellbot/actions/lfg_action.py
+-rw-r--r--   0        0        0     3253 2024-01-26 19:35:36.678865 spellbot-9.7.0/src/spellbot/actions/score_action.py
+-rw-r--r--   0        0        0     7569 2024-02-02 23:41:49.630463 spellbot-9.7.0/src/spellbot/actions/tasks_action.py
+-rw-r--r--   0        0        0      996 2023-10-04 20:26:02.207631 spellbot-9.7.0/src/spellbot/actions/verify_action.py
+-rw-r--r--   0        0        0     4824 2024-01-26 19:35:36.679117 spellbot-9.7.0/src/spellbot/actions/watch_action.py
+-rw-r--r--   0        0        0     3470 2023-10-17 21:34:04.984133 spellbot-9.7.0/src/spellbot/cli.py
+-rw-r--r--   0        0        0     6715 2024-01-15 05:47:30.079395 spellbot-9.7.0/src/spellbot/client.py
+-rw-r--r--   0        0        0     2082 2023-10-04 20:26:02.208297 spellbot-9.7.0/src/spellbot/cogs/__init__.py
+-rw-r--r--   0        0        0     1992 2024-01-26 19:35:36.679324 spellbot-9.7.0/src/spellbot/cogs/about_cog.py
+-rw-r--r--   0        0        0    11941 2023-10-17 21:30:53.733467 spellbot-9.7.0/src/spellbot/cogs/admin_cog.py
+-rw-r--r--   0        0        0     2235 2023-11-26 20:42:37.444094 spellbot-9.7.0/src/spellbot/cogs/block_cog.py
+-rw-r--r--   0        0        0     1708 2023-10-04 20:26:02.208634 spellbot-9.7.0/src/spellbot/cogs/config_cog.py
+-rw-r--r--   0        0        0     1672 2023-10-17 21:30:53.733656 spellbot-9.7.0/src/spellbot/cogs/events_cog.py
+-rw-r--r--   0        0        0     1806 2023-10-16 00:46:59.592231 spellbot-9.7.0/src/spellbot/cogs/leave_cog.py
+-rw-r--r--   0        0        0     1999 2023-10-17 21:30:53.733828 spellbot-9.7.0/src/spellbot/cogs/lfg_cog.py
+-rw-r--r--   0        0        0     3128 2023-04-25 03:19:31.674236 spellbot-9.7.0/src/spellbot/cogs/owner_cog.py
+-rw-r--r--   0        0        0     2210 2023-11-26 20:42:37.444318 spellbot-9.7.0/src/spellbot/cogs/score_cog.py
+-rw-r--r--   0        0        0     1130 2023-04-25 03:19:31.674692 spellbot-9.7.0/src/spellbot/cogs/sync_cog.py
+-rw-r--r--   0        0        0     3485 2023-10-04 20:26:02.209316 spellbot-9.7.0/src/spellbot/cogs/tasks_cog.py
+-rw-r--r--   0        0        0     1658 2023-04-25 03:19:31.675274 spellbot-9.7.0/src/spellbot/cogs/verify_cog.py
+-rw-r--r--   0        0        0     2672 2023-10-04 20:26:02.209482 spellbot-9.7.0/src/spellbot/cogs/watch_cog.py
+-rw-r--r--   0        0        0     4708 2023-10-04 20:26:02.209682 spellbot-9.7.0/src/spellbot/database.py
+-rw-r--r--   0        0        0     1864 2024-01-29 02:08:47.334112 spellbot-9.7.0/src/spellbot/enums.py
+-rw-r--r--   0        0        0      198 2023-04-18 21:36:17.606364 spellbot-9.7.0/src/spellbot/environment.py
+-rw-r--r--   0        0        0     1125 2023-04-25 03:19:31.676087 spellbot-9.7.0/src/spellbot/errors.py
+-rw-r--r--   0        0        0      939 2023-04-25 03:19:31.676348 spellbot-9.7.0/src/spellbot/logs.py
+-rw-r--r--   0        0        0     5005 2024-01-31 04:50:24.265672 spellbot-9.7.0/src/spellbot/metrics.py
+-rw-r--r--   0        0        0      657 2023-04-18 21:36:17.606641 spellbot-9.7.0/src/spellbot/migrations/alembic.ini
+-rw-r--r--   0        0        0     1638 2023-04-25 03:19:31.676886 spellbot-9.7.0/src/spellbot/migrations/env.py
+-rw-r--r--   0        0        0      493 2023-04-18 21:36:17.606757 spellbot-9.7.0/src/spellbot/migrations/script.py.mako
+-rw-r--r--   0        0        0     2924 2023-10-04 20:26:02.209820 spellbot-9.7.0/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py
+-rw-r--r--   0        0        0     1412 2023-10-04 21:07:34.717844 spellbot-9.7.0/src/spellbot/migrations/versions/1503d49ae8e1_adds_created_at_and_updated_at_to_more_.py
+-rw-r--r--   0        0        0      591 2023-04-18 21:36:17.606851 spellbot-9.7.0/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py
+-rw-r--r--   0        0        0      645 2023-04-18 21:36:17.606902 spellbot-9.7.0/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py
+-rw-r--r--   0        0        0      630 2023-04-18 21:36:17.606959 spellbot-9.7.0/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py
+-rw-r--r--   0        0        0      469 2023-04-18 21:36:17.607018 spellbot-9.7.0/src/spellbot/migrations/versions/7abc75daaa94_adds_channel_motd_column.py
+-rw-r--r--   0        0        0      641 2023-04-18 21:36:17.607072 spellbot-9.7.0/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py
+-rw-r--r--   0        0        0      776 2023-04-18 21:36:17.607126 spellbot-9.7.0/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py
+-rw-r--r--   0        0        0      814 2023-10-17 21:30:53.734098 spellbot-9.7.0/src/spellbot/migrations/versions/b2d4a9aa1aed_adds_default_format_to_channel.py
+-rw-r--r--   0        0        0      476 2023-10-04 20:26:02.209939 spellbot-9.7.0/src/spellbot/migrations/versions/c03099407b40_support_extra_message_content.py
+-rw-r--r--   0        0        0      609 2023-04-18 21:36:17.607196 spellbot-9.7.0/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py
+-rw-r--r--   0        0        0    10922 2023-04-18 21:36:17.607252 spellbot-9.7.0/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py
+-rw-r--r--   0        0        0      843 2023-04-18 21:36:17.607322 spellbot-9.7.0/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py
+-rw-r--r--   0        0        0      474 2023-04-18 21:36:17.607382 spellbot-9.7.0/src/spellbot/migrations/versions/ef54f035a75c_adds_an_index_on_plays_by_game_id.py
+-rw-r--r--   0        0        0      987 2023-04-18 21:36:17.607447 spellbot-9.7.0/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py
+-rw-r--r--   0        0        0     1436 2023-10-17 21:30:53.734307 spellbot-9.7.0/src/spellbot/models/__init__.py
+-rw-r--r--   0        0        0     3372 2023-10-04 20:40:25.401304 spellbot-9.7.0/src/spellbot/models/award.py
+-rw-r--r--   0        0        0     2635 2023-10-04 21:07:34.718050 spellbot-9.7.0/src/spellbot/models/base.py
+-rw-r--r--   0        0        0     1493 2023-10-04 21:07:34.718261 spellbot-9.7.0/src/spellbot/models/block.py
+-rw-r--r--   0        0        0     4593 2023-11-02 17:50:09.483011 spellbot-9.7.0/src/spellbot/models/channel.py
+-rw-r--r--   0        0        0     1059 2023-10-04 20:34:58.485690 spellbot-9.7.0/src/spellbot/models/config.py
+-rw-r--r--   0        0        0    11055 2024-01-26 19:35:36.679639 spellbot-9.7.0/src/spellbot/models/game.py
+-rw-r--r--   0        0        0     2714 2023-11-02 17:50:09.483390 spellbot-9.7.0/src/spellbot/models/guild.py
+-rw-r--r--   0        0        0     1707 2023-11-02 17:50:09.483577 spellbot-9.7.0/src/spellbot/models/play.py
+-rw-r--r--   0        0        0      855 2023-11-02 17:44:44.999754 spellbot-9.7.0/src/spellbot/models/queue.py
+-rw-r--r--   0        0        0     4381 2023-11-02 17:42:54.141332 spellbot-9.7.0/src/spellbot/models/user.py
+-rw-r--r--   0        0        0      952 2023-10-04 20:26:02.211355 spellbot-9.7.0/src/spellbot/models/verify.py
+-rw-r--r--   0        0        0     1085 2023-04-18 21:36:17.608274 spellbot-9.7.0/src/spellbot/models/watch.py
+-rw-r--r--   0        0        0    19340 2023-12-12 01:18:55.704911 spellbot-9.7.0/src/spellbot/operations.py
+-rw-r--r--   0        0        0     1059 2023-04-25 03:19:31.678344 spellbot-9.7.0/src/spellbot/services/__init__.py
+-rw-r--r--   0        0        0     3202 2023-10-04 20:26:02.211733 spellbot-9.7.0/src/spellbot/services/awards.py
+-rw-r--r--   0        0        0     5946 2023-10-17 21:30:53.734897 spellbot-9.7.0/src/spellbot/services/channels.py
+-rw-r--r--   0        0        0     1555 2023-10-04 20:26:02.212048 spellbot-9.7.0/src/spellbot/services/configs.py
+-rw-r--r--   0        0        0    16056 2024-02-02 23:44:03.651726 spellbot-9.7.0/src/spellbot/services/games.py
+-rw-r--r--   0        0        0     4880 2023-11-02 17:50:09.484028 spellbot-9.7.0/src/spellbot/services/guilds.py
+-rw-r--r--   0        0        0     7637 2023-10-17 21:30:53.735085 spellbot-9.7.0/src/spellbot/services/plays.py
+-rw-r--r--   0        0        0    15575 2023-11-02 17:50:09.484399 spellbot-9.7.0/src/spellbot/services/users.py
+-rw-r--r--   0        0        0     1631 2023-10-04 20:26:02.212868 spellbot-9.7.0/src/spellbot/services/verifies.py
+-rw-r--r--   0        0        0      504 2023-10-04 20:26:02.213006 spellbot-9.7.0/src/spellbot/services/watches.py
+-rw-r--r--   0        0        0     3991 2024-01-26 19:35:36.680093 spellbot-9.7.0/src/spellbot/settings.py
+-rw-r--r--   0        0        0     2377 2023-10-04 20:26:02.213317 spellbot-9.7.0/src/spellbot/spelltable.py
+-rw-r--r--   0        0        0    11375 2023-12-12 01:15:07.924888 spellbot-9.7.0/src/spellbot/utils.py
+-rw-r--r--   0        0        0      295 2023-04-26 18:55:38.771824 spellbot-9.7.0/src/spellbot/views/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-25 03:19:31.680995 spellbot-9.7.0/src/spellbot/views/base_view.py
+-rw-r--r--   0        0        0     4108 2024-01-02 03:43:15.077144 spellbot-9.7.0/src/spellbot/views/lfg_view.py
+-rw-r--r--   0        0        0     2530 2024-01-02 03:43:15.077403 spellbot-9.7.0/src/spellbot/views/setup_view.py
+-rw-r--r--   0        0        0      177 2023-04-18 21:36:17.609697 spellbot-9.7.0/src/spellbot/web/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-18 21:36:17.609773 spellbot-9.7.0/src/spellbot/web/api/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-18 21:36:17.609830 spellbot-9.7.0/src/spellbot/web/api/ping.py
+-rw-r--r--   0        0        0     2712 2023-04-18 21:36:17.609889 spellbot-9.7.0/src/spellbot/web/api/record.py
+-rw-r--r--   0        0        0     1744 2023-04-18 21:36:17.609962 spellbot-9.7.0/src/spellbot/web/builder.py
+-rw-r--r--   0        0        0      689 2023-11-24 20:31:01.432756 spellbot-9.7.0/src/spellbot/web/server.py
+-rw-r--r--   0        0        0     1661 2023-04-18 21:36:17.610335 spellbot-9.7.0/src/spellbot/web/templates/channel_record.html.j2
+-rw-r--r--   0        0        0     5352 2023-04-18 21:36:17.610438 spellbot-9.7.0/src/spellbot/web/templates/record.css
+-rw-r--r--   0        0        0     6365 2023-04-18 21:36:17.610540 spellbot-9.7.0/src/spellbot/web/templates/record_base.html.j2
+-rw-r--r--   0        0        0     1978 2023-04-18 21:36:17.610647 spellbot-9.7.0/src/spellbot/web/templates/table2CSV.js
+-rw-r--r--   0        0        0     2509 2023-04-18 21:36:17.610747 spellbot-9.7.0/src/spellbot/web/templates/user_record.html.j2
+-rw-r--r--   0        0        0    13100 1970-01-01 00:00:00.000000 spellbot-9.7.0/PKG-INFO
```

### Comparing `spellbot-9.6.0/LICENSE.md` & `spellbot-9.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/README.md` & `spellbot-9.7.0/README.md`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/pyproject.toml` & `spellbot-9.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -103,24 +103,24 @@
 license = 'MIT'
 name = 'spellbot'
 packages = [
   {include = "spellbot", from = "src"},
 ]
 readme = 'README.md'
 repository = 'https://github.com/lexicalunit/spellbot'
-version = "9.6.0"
+version = "9.7.0"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.4"
 aiohttp-jinja2 = "^1.5.1"
 aiohttp-retry = "^2.8.3"
 alembic = "^1.10.3"
 asgiref = "^3.7.1"
 babel = "^2.12.1"
-certifi = ">=2022.12.7,<2024.0.0"
+certifi = ">=2022.12.7,<2025.0.0"
 click = ">=8.1.3, !=8.1.4"
 coloredlogs = "^15.0.1"
 datadog = ">=0.45,<0.49"
 ddtrace = ">=1.12,<3.0"
 discord-py = "^2.3.2"
 dunamai = "^1.16.0"
 expiringdict = "^1.2.2"
@@ -129,15 +129,15 @@
 hupper = "^1.12"
 importlib-resources = ">=5.12,<7.0"
 packaging = "^23.1"
 psycopg2-binary = "^2.9.6"
 python = ">=3.10,<4"
 python-dateutil = "^2.8.2"
 python-dotenv = "^1.0.0"
-pytz = "^2023.3"
+pytz = ">=2023.3,<2025.0"
 pyyaml = "^6.0"
 requests = "^2.28.2"
 sqlalchemy = "^2.0.18"
 sqlalchemy-utils = "^0.41.1"
 supervisor = "^4.2.5"
 toml = "^0.10.2"
 uvloop = "^0.17.0"
```

### Comparing `spellbot-9.6.0/src/spellbot/_version.py` & `spellbot-9.7.0/src/spellbot/_version.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/__init__.py` & `spellbot-9.7.0/src/spellbot/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/admin_action.py` & `spellbot-9.7.0/src/spellbot/actions/admin_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/base_action.py` & `spellbot-9.7.0/src/spellbot/actions/base_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/block_action.py` & `spellbot-9.7.0/src/spellbot/actions/block_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/config_action.py` & `spellbot-9.7.0/src/spellbot/actions/config_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/leave_action.py` & `spellbot-9.7.0/src/spellbot/actions/leave_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/lfg_action.py` & `spellbot-9.7.0/src/spellbot/actions/lfg_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/score_action.py` & `spellbot-9.7.0/src/spellbot/actions/score_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/tasks_action.py` & `spellbot-9.7.0/src/spellbot/actions/tasks_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,40 +158,40 @@
             await rollback_session()
 
     async def expire_games(self, games: list[dict[str, Any]]) -> None:
         batch = 0
         for game in games:
             game_id = game["id"]
             logger.info("expiring game %s...", game_id)
-            await self.services.games.delete_games([game_id])
-            await self.expire_game(game)
+            dequeued = await self.services.games.delete_games([game_id])
+            await self.expire_game(game, dequeued)
 
             batch += 1
             if batch >= 5:  # pragma: no cover
                 await asyncio.sleep(5)
                 batch = 0
             else:
                 await asyncio.sleep(1)
 
-    async def expire_game(self, game: dict[str, Any]) -> None:
+    async def expire_game(self, game: dict[str, Any], dequeued: int) -> None:
         message_xid = game["message_xid"]
         if message_xid is None:
             return
 
         guild_xid = game["guild_xid"]
         channel_xid = game["channel_xid"]
         chan = await safe_fetch_text_channel(self.bot, guild_xid, channel_xid)
         if not chan:
             return
 
         if not (post := safe_get_partial_message(chan, guild_xid, message_xid)):
             return
 
         channel_data = await self.services.channels.select(channel_xid)
-        if channel_data and channel_data["delete_expired"]:
+        if not dequeued or channel_data and channel_data["delete_expired"]:
             await safe_delete_message(post)
         else:
             await safe_update_embed(
                 post,
                 content="Sorry, this game was expired due to inactivity.",
                 embed=None,
                 view=None,
```

### Comparing `spellbot-9.6.0/src/spellbot/actions/verify_action.py` & `spellbot-9.7.0/src/spellbot/actions/verify_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/actions/watch_action.py` & `spellbot-9.7.0/src/spellbot/actions/watch_action.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cli.py` & `spellbot-9.7.0/src/spellbot/cli.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/client.py` & `spellbot-9.7.0/src/spellbot/client.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/__init__.py` & `spellbot-9.7.0/src/spellbot/cogs/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/about_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/about_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/admin_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/admin_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/block_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/block_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/config_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/config_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/events_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/events_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/leave_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/leave_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/lfg_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/lfg_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/owner_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/owner_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/score_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/score_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/sync_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/sync_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/tasks_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/tasks_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/verify_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/verify_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/cogs/watch_cog.py` & `spellbot-9.7.0/src/spellbot/cogs/watch_cog.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/database.py` & `spellbot-9.7.0/src/spellbot/database.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/enums.py` & `spellbot-9.7.0/src/spellbot/enums.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/errors.py` & `spellbot-9.7.0/src/spellbot/errors.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/logs.py` & `spellbot-9.7.0/src/spellbot/logs.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/metrics.py` & `spellbot-9.7.0/src/spellbot/metrics.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/alembic.ini` & `spellbot-9.7.0/src/spellbot/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/env.py` & `spellbot-9.7.0/src/spellbot/migrations/env.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/01766a5fb976_support_multiple_queues.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/1503d49ae8e1_adds_created_at_and_updated_at_to_more_.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/1503d49ae8e1_adds_created_at_and_updated_at_to_more_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/42f55401ef2b_adds_removeable_role_awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/6267f69c5dfd_remove_legacy_prefix.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/6e982c9318a6_adds_voice_category_per_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/8b560fcec5f7_add_games_deleted_at_column_for_soft_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/a1caf292fe93_adds_verified_only_and_unverified_only_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/b2d4a9aa1aed_adds_default_format_to_channel.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/b2d4a9aa1aed_adds_default_format_to_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/c0bc12b1b482_adds_delete_expired_column_to_.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/c35c18ddd228_initial_database_schema.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/ee653a3075c6_adds_user_configuration_per_guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py` & `spellbot-9.7.0/src/spellbot/migrations/versions/fd7ff2703f57_move_points_config_to_channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/__init__.py` & `spellbot-9.7.0/src/spellbot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/award.py` & `spellbot-9.7.0/src/spellbot/models/award.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/base.py` & `spellbot-9.7.0/src/spellbot/models/base.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/block.py` & `spellbot-9.7.0/src/spellbot/models/block.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/channel.py` & `spellbot-9.7.0/src/spellbot/models/channel.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/config.py` & `spellbot-9.7.0/src/spellbot/models/config.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/game.py` & `spellbot-9.7.0/src/spellbot/models/game.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/guild.py` & `spellbot-9.7.0/src/spellbot/models/guild.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/play.py` & `spellbot-9.7.0/src/spellbot/models/play.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/queue.py` & `spellbot-9.7.0/src/spellbot/models/queue.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/user.py` & `spellbot-9.7.0/src/spellbot/models/user.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/verify.py` & `spellbot-9.7.0/src/spellbot/models/verify.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/models/watch.py` & `spellbot-9.7.0/src/spellbot/models/watch.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/operations.py` & `spellbot-9.7.0/src/spellbot/operations.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/__init__.py` & `spellbot-9.7.0/src/spellbot/services/__init__.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/awards.py` & `spellbot-9.7.0/src/spellbot/services/awards.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/channels.py` & `spellbot-9.7.0/src/spellbot/services/channels.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/configs.py` & `spellbot-9.7.0/src/spellbot/services/configs.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/games.py` & `spellbot-9.7.0/src/spellbot/services/games.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # pylint: disable=too-many-public-methods
 from __future__ import annotations
 
+import logging
 from datetime import datetime, timedelta
 from typing import Any, Optional, cast
 
 import discord
 import pytz
 from asgiref.sync import sync_to_async
 from ddtrace import tracer
 from sqlalchemy import func, select, update
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.orm import aliased
 from sqlalchemy.sql.expression import and_, asc, column, or_
 from sqlalchemy.sql.functions import count
 
 from ..database import DatabaseSession
-from ..metrics import add_span_kv
 from ..models import (
     Block,
     Game,
     GameStatus,
     Play,
     Queue,
     UserAward,
     Watch,
 )
 from ..settings import Settings
 
+logger = logging.getLogger(__name__)
+
 MAX_SPELLTABLE_LINK_LEN = Game.spelltable_link.property.columns[0].type.length  # type: ignore
 
 
 class GamesService:
     game: Optional[Game] = None
 
     @sync_to_async()
@@ -468,28 +470,27 @@
                 ),
             )
         )
         return [record.to_dict() for record in records]
 
     @sync_to_async()
     @tracer.wrap()
-    def delete_games(self, game_ids: list[int]) -> None:
+    def delete_games(self, game_ids: list[int]) -> int:
         query = (
             update(Game).where(Game.id.in_(game_ids)).values(deleted_at=datetime.now(tz=pytz.utc))
         )
         DatabaseSession.execute(query)
         dequeued = (
             DatabaseSession.query(Queue)
             .filter(Queue.game_id.in_(game_ids))
-            .delete(
-                synchronize_session=False,
-            )
+            .delete(synchronize_session=False)
         )
-        add_span_kv("dequeued", dequeued)
+        logger.info("dequeued %s players from games %s", dequeued, game_ids)
         DatabaseSession.commit()
+        return dequeued
 
     @sync_to_async()
     @tracer.wrap()
     def message_xids(self, game_ids: list[int]) -> list[int]:
         query = select(
             Game.message_xid,  # type: ignore
         ).where(Game.id.in_(game_ids))
```

### Comparing `spellbot-9.6.0/src/spellbot/services/guilds.py` & `spellbot-9.7.0/src/spellbot/services/guilds.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/plays.py` & `spellbot-9.7.0/src/spellbot/services/plays.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/users.py` & `spellbot-9.7.0/src/spellbot/services/users.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/services/verifies.py` & `spellbot-9.7.0/src/spellbot/services/verifies.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/settings.py` & `spellbot-9.7.0/src/spellbot/settings.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/spelltable.py` & `spellbot-9.7.0/src/spellbot/spelltable.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/utils.py` & `spellbot-9.7.0/src/spellbot/utils.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/views/lfg_view.py` & `spellbot-9.7.0/src/spellbot/views/lfg_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/views/setup_view.py` & `spellbot-9.7.0/src/spellbot/views/setup_view.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/api/record.py` & `spellbot-9.7.0/src/spellbot/web/api/record.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/builder.py` & `spellbot-9.7.0/src/spellbot/web/builder.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/server.py` & `spellbot-9.7.0/src/spellbot/web/server.py`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/templates/channel_record.html.j2` & `spellbot-9.7.0/src/spellbot/web/templates/channel_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/templates/record.css` & `spellbot-9.7.0/src/spellbot/web/templates/record.css`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/templates/record_base.html.j2` & `spellbot-9.7.0/src/spellbot/web/templates/record_base.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/templates/table2CSV.js` & `spellbot-9.7.0/src/spellbot/web/templates/table2CSV.js`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/src/spellbot/web/templates/user_record.html.j2` & `spellbot-9.7.0/src/spellbot/web/templates/user_record.html.j2`

 * *Files identical despite different names*

### Comparing `spellbot-9.6.0/PKG-INFO` & `spellbot-9.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spellbot
-Version: 9.6.0
+Version: 9.7.0
 Summary: The Discord bot for SpellTable
 Home-page: http://spellbot.io/
 License: MIT
 Keywords: discord,magic,bot,mtg,SpellTable
 Author: Amy Troschinetz
 Author-email: spellbot@lexicalunit.com
 Requires-Python: >=3.10,<4
@@ -18,15 +18,15 @@
 Classifier: Topic :: Games/Entertainment :: Board Games
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiohttp-jinja2 (>=1.5.1,<2.0.0)
 Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0)
 Requires-Dist: alembic (>=1.10.3,<2.0.0)
 Requires-Dist: asgiref (>=3.7.1,<4.0.0)
 Requires-Dist: babel (>=2.12.1,<3.0.0)
-Requires-Dist: certifi (>=2022.12.7,<2024.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2025.0.0)
 Requires-Dist: click (>=8.1.3,!=8.1.4)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: datadog (>=0.45,<0.49)
 Requires-Dist: ddtrace (>=1.12,<3.0)
 Requires-Dist: discord-py (>=2.3.2,<3.0.0)
 Requires-Dist: dunamai (>=1.16.0,<2.0.0)
 Requires-Dist: expiringdict (>=1.2.2,<2.0.0)
@@ -34,15 +34,15 @@
 Requires-Dist: humanize (>=4.6.0,<5.0.0)
 Requires-Dist: hupper (>=1.12,<2.0)
 Requires-Dist: importlib-resources (>=5.12,<7.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: pytz (>=2023.3,<2025.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.18,<3.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: supervisor (>=4.2.5,<5.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: spellbot Version: 9.6.0 Summary: The Discord bot
+Metadata-Version: 2.1 Name: spellbot Version: 9.7.0 Summary: The Discord bot
 for SpellTable Home-page: http://spellbot.io/ License: MIT Keywords:
 discord,magic,bot,mtg,SpellTable Author: Amy Troschinetz Author-email:
 spellbot@lexicalunit.com Requires-Python: >=3.10,<4 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Communications :: Chat Classifier: Topic :: Games/Entertainment :: Board Games
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: aiohttp-jinja2
 (>=1.5.1,<2.0.0) Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0) Requires-Dist:
 alembic (>=1.10.3,<2.0.0) Requires-Dist: asgiref (>=3.7.1,<4.0.0) Requires-
-Dist: babel (>=2.12.1,<3.0.0) Requires-Dist: certifi (>=2022.12.7,<2024.0.0)
+Dist: babel (>=2.12.1,<3.0.0) Requires-Dist: certifi (>=2022.12.7,<2025.0.0)
 Requires-Dist: click (>=8.1.3,!=8.1.4) Requires-Dist: coloredlogs
 (>=15.0.1,<16.0.0) Requires-Dist: datadog (>=0.45,<0.49) Requires-Dist: ddtrace
 (>=1.12,<3.0) Requires-Dist: discord-py (>=2.3.2,<3.0.0) Requires-Dist: dunamai
 (>=1.16.0,<2.0.0) Requires-Dist: expiringdict (>=1.2.2,<2.0.0) Requires-Dist:
 gunicorn (>=20.1,<22.0) Requires-Dist: humanize (>=4.6.0,<5.0.0) Requires-Dist:
 hupper (>=1.12,<2.0) Requires-Dist: importlib-resources (>=5.12,<7.0) Requires-
 Dist: packaging (>=23.1,<24.0) Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: python-dotenv
-(>=1.0.0,<2.0.0) Requires-Dist: pytz (>=2023.3,<2024.0) Requires-Dist: pyyaml
+(>=1.0.0,<2.0.0) Requires-Dist: pytz (>=2023.3,<2025.0) Requires-Dist: pyyaml
 (>=6.0,<7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
 sqlalchemy (>=2.0.18,<3.0.0) Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: supervisor (>=4.2.5,<5.0.0) Requires-Dist: toml
 (>=0.10.2,<0.11.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Requires-Dist:
 wrapt (>=1.15.0,<2.0.0) Project-URL: Repository, https://github.com/
 lexicalunit/spellbot Description-Content-Type: text/markdown [spellbot]#
 SpellBot [![build][build-badge]][build] [![uptime][uptime-badge]][uptime] [!
```

