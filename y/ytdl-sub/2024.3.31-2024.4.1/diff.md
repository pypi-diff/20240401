# Comparing `tmp/ytdl-sub-2024.3.31.tar.gz` & `tmp/ytdl-sub-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2024.3.31.tar", last modified: Sun Mar 31 05:06:04 2024, max compression
+gzip compressed data, was "ytdl-sub-2024.4.1.tar", last modified: Mon Apr  1 11:25:38 2024, max compression
```

## Comparing `ytdl-sub-2024.3.31.tar` & `ytdl-sub-2024.4.1.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.548701 ytdl-sub-2024.3.31/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-03-31 05:06:04.548701 ytdl-sub-2024.3.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-31 05:06:04.548701 ytdl-sub-2024.3.31/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.516701 ytdl-sub-2024.3.31/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.520701 ytdl-sub-2024.3.31/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-31 05:05:45.000000 ytdl-sub-2024.3.31/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.520701 ytdl-sub-2024.3.31/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/output_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/output_transaction_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.524701 ytdl-sub-2024.3.31/src/ytdl_sub/cli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/parsers/dl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/cli/parsers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.524701 ytdl-sub-2024.3.31/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.524701 ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/plugin_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/plugin_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/preset_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.524701 ytdl-sub-2024.3.31/src/ytdl_sub/config/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/validators/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/config/validators/variable_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.524701 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.524701 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.528701 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.528701 ytdl-sub-2024.3.31/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.528701 ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/function_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    41385 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/variable_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/variable_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.528701 ytdl-sub-2024.3.31/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/entries/variables/override_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.532701 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/file_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/filter_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/filter_include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.532701 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/throttle_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.532701 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.532701 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.532701 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.532701 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/singles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.536701 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music_videos/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.536701 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23678 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.536701 ytdl-sub-2024.3.31/src/ytdl_sub/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.536701 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/boolean_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/conditional_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/json_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/numeric_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/regex_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/string_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/script_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.540701 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/resolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/types/variable_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.540701 ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/exception_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/name_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.540701 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.540701 ytdl-sub-2024.3.31/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.544701 ytdl-sub-2024.3.31/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/scriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.544701 ytdl-sub-2024.3.31/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.544701 ytdl-sub-2024.3.31/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-03-31 05:05:44.000000 ytdl-sub-2024.3.31/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:06:04.544701 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-03-31 05:06:04.000000 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-03-31 05:06:04.000000 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 05:06:04.000000 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-31 05:06:04.000000 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 05:06:04.000000 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 05:06:04.000000 ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.046893 ytdl-sub-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-01 11:25:38.046893 ytdl-sub-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-01 11:25:38.046893 ytdl-sub-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.014893 ytdl-sub-2024.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.018893 ytdl-sub-2024.4.1/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 11:25:22.000000 ytdl-sub-2024.4.1/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.018893 ytdl-sub-2024.4.1/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_transaction_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.018893 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/dl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/preset_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/variable_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.026893 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/function_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42267 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.026893 ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/override_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/file_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/throttle_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/singles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.034893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.034893 ytdl-sub-2024.4.1/src/ytdl_sub/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.034893 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/boolean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/conditional_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/json_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/numeric_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/regex_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/string_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/script_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/resolvable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exception_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/name_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/scriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-01 11:25:38.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2024.3.31/LICENSE` & `ytdl-sub-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/PKG-INFO` & `ytdl-sub-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2024.3.31
+Version: 2024.4.1
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2024.3.31/README.md` & `ytdl-sub-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/pyproject.toml` & `ytdl-sub-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/setup.cfg` & `ytdl-sub-2024.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/cli/entrypoint.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/cli/output_summary.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_summary.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/cli/output_transaction_log.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_transaction_log.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/cli/parsers/dl.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/dl.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/cli/parsers/main.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/overrides.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/overrides.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Optional
 from typing import Set
 
 import mergedeep
 
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.script.variable_definitions import VARIABLES
+from ytdl_sub.entries.variables.override_variables import REQUIRED_OVERRIDE_VARIABLE_NAMES
 from ytdl_sub.entries.variables.override_variables import OverrideHelpers
-from ytdl_sub.entries.variables.override_variables import SubscriptionVariables
 from ytdl_sub.script.parser import parse
 from ytdl_sub.script.script import Script
 from ytdl_sub.script.utils.exceptions import ScriptVariableNotResolved
 from ytdl_sub.utils.exceptions import InvalidVariableNameException
 from ytdl_sub.utils.exceptions import StringFormattingException
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.script import ScriptUtils
@@ -58,14 +58,15 @@
         DictFormatterValidator.__init__(self, name, value)
         Scriptable.__init__(self, initialize_base_script=True)
 
         for key in self._keys:
             self.ensure_variable_name_valid(key)
 
         self.unresolvable.add(VARIABLES.entry_metadata.variable_name)
+        self.unresolvable.update(REQUIRED_OVERRIDE_VARIABLE_NAMES)
 
     def ensure_added_plugin_variable_valid(self, added_variable: str) -> bool:
         """
         Returns False if the variable exists as a non-override.
 
         Raises
         ------
@@ -123,26 +124,19 @@
         mergedeep.merge(
             initial_variables,
             self.dict_with_format_strings,
             unresolved_variables if unresolved_variables else {},
         )
         return ScriptUtils.add_sanitized_variables(initial_variables)
 
-    def initialize_script(
-        self, subscription_name: str, unresolved_variables: Set[str]
-    ) -> "Overrides":
+    def initialize_script(self, unresolved_variables: Set[str]) -> "Overrides":
         """
-        Initialize the override script with override variables + any unresolved variables
+        Initialize the override script with any unresolved variables
         """
         self.script.add(
-            ScriptUtils.add_sanitized_variables(
-                {SubscriptionVariables.subscription_name(): subscription_name}
-            )
-        )
-        self.script.add(
             self.initial_variables(
                 unresolved_variables={
                     var_name: f"{{%throw('Plugin variable {var_name} has not been created yet')}}"
                     for var_name in unresolved_variables
                 }
             )
         )
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/plugin.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/plugin_mapping.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin_mapping.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/plugin/preset_plugins.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/preset.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/preset.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,17 +194,15 @@
         self.plugins: PresetPlugins = self._validate_and_get_plugins()
         self.overrides = self._validate_key(key="overrides", validator=Overrides, default={})
 
         VariableValidation(
             downloader_options=self.downloader_options,
             output_options=self.output_options,
             plugins=self.plugins,
-        ).initialize_overrides(
-            subscription_name=self.name, overrides=self.overrides
-        ).ensure_proper_usage()
+        ).initialize_preset_overrides(overrides=self.overrides).ensure_proper_usage()
 
     @property
     def name(self) -> str:
         """
         Returns
         -------
         Name of the preset
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/validators/options.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/config/validators/variable_validation.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/variable_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,32 @@
 from ytdl_sub.config.overrides import Overrides
 from ytdl_sub.config.plugin.plugin_mapping import PluginMapping
 from ytdl_sub.config.plugin.plugin_operation import PluginOperation
 from ytdl_sub.config.plugin.preset_plugins import PresetPlugins
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.validators.options import OptionsValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
-from ytdl_sub.entries.variables.override_variables import SubscriptionVariables
+from ytdl_sub.entries.variables.override_variables import REQUIRED_OVERRIDE_VARIABLE_NAMES
 from ytdl_sub.script.script import Script
 from ytdl_sub.script.script import _is_function
 from ytdl_sub.utils.scriptable import BASE_SCRIPT
 from ytdl_sub.validators.string_formatter_validators import to_variable_dependency_format_string
 from ytdl_sub.validators.string_formatter_validators import validate_formatters
 
+# Entry variables to mock during validation
+_DUMMY_ENTRY_VARIABLES: Dict[str, str] = {
+    name: to_variable_dependency_format_string(
+        # pylint: disable=protected-access
+        script=BASE_SCRIPT,
+        parsed_format_string=BASE_SCRIPT._variables[name]
+        # pylint: enable=protected-access
+    )
+    for name in BASE_SCRIPT.variable_names
+}
+
 
 def _add_dummy_variables(variables: Iterable[str]) -> Dict[str, str]:
     dummy_variables: Dict[str, str] = {}
     for var in variables:
         dummy_variables[var] = ""
         dummy_variables[f"{var}_sanitized"] = ""
 
@@ -68,28 +79,15 @@
         for plugin_modified_variables in plugin_options.modified_variables().values():
             modified_variables = plugin_modified_variables
 
         yield plugin_options, added_variables, modified_variables
 
 
 def _override_variables(overrides: Overrides) -> Set[str]:
-    return set(list(overrides.initial_variables().keys())) | {
-        SubscriptionVariables.subscription_name()
-    }
-
-
-_DUMMY_ENTRY_VARIABLES: Dict[str, str] = {
-    name: to_variable_dependency_format_string(
-        # pylint: disable=protected-access
-        script=BASE_SCRIPT,
-        parsed_format_string=BASE_SCRIPT._variables[name]
-        # pylint: enable=protected-access
-    )
-    for name in BASE_SCRIPT.variable_names
-}
+    return set(list(overrides.initial_variables().keys()))
 
 
 class VariableValidation:
     def __init__(
         self,
         downloader_options: MultiUrlValidator,
         output_options: OutputOptions,
@@ -99,21 +97,19 @@
         self.output_options = output_options
         self.plugins = plugins
 
         self.script: Optional[Script] = None
         self.resolved_variables: Set[str] = set()
         self.unresolved_variables: Set[str] = set()
 
-    def initialize_overrides(
-        self, subscription_name: str, overrides: Overrides
-    ) -> "VariableValidation":
+    def initialize_preset_overrides(self, overrides: Overrides) -> "VariableValidation":
         """
         Do some gymnastics to initialize the Overrides script.
         """
-        override_variables = _override_variables(overrides)
+        override_variables = set(list(overrides.initial_variables().keys()))
 
         # Set resolved variables as all entry + override variables
         # at this point to generate every possible added/modified variable
         self.resolved_variables = set(_DUMMY_ENTRY_VARIABLES.keys()) | override_variables
         plugin_variables: Set[str] = set()
 
         for (
@@ -141,52 +137,59 @@
 
         # Then update resolved variables to reflect that
         self.resolved_variables -= self.unresolved_variables
 
         # Initialize overrides with unresolved variables + modified variables to throw an error.
         # For modified variables, this is to prevent a resolve(update=True) to setting any
         # dependencies until it has been explicitly added
-        overrides = overrides.initialize_script(
-            subscription_name=subscription_name, unresolved_variables=self.unresolved_variables
-        )
+        overrides = overrides.initialize_script(unresolved_variables=self.unresolved_variables)
 
         # copy the script and mock entry variables
         self.script = copy.deepcopy(overrides.script)
         self.script.add(
             variables=_add_dummy_overrides(overrides=overrides)
             | _add_dummy_variables(variables=plugin_variables)
             | _DUMMY_ENTRY_VARIABLES
         )
 
         return self
 
     def _update_script(self) -> None:
         _ = self.script.resolve(unresolvable=self.unresolved_variables, update=True)
 
-    def _add_variables(self, plugin_op: PluginOperation, options: OptionsValidator) -> Set[str]:
+    def _add_subscription_override_variables(self) -> None:
+        """
+        Add dummy subscription variables for script validation
+        """
+        self.resolved_variables |= REQUIRED_OVERRIDE_VARIABLE_NAMES
+
+    def _add_variables(self, plugin_op: PluginOperation, options: OptionsValidator) -> None:
+        """
+        Add dummy variables for script validation
+        """
         added_variables = options.added_variables(
             resolved_variables=self.resolved_variables,
             unresolved_variables=self.unresolved_variables,
             plugin_op=plugin_op,
         ).get(plugin_op, set())
         modified_variables = options.modified_variables().get(plugin_op, set())
 
         resolved_variables = added_variables | modified_variables
 
         self.resolved_variables |= resolved_variables
         self.unresolved_variables -= resolved_variables
 
-        return added_variables
-
     def ensure_proper_usage(self) -> None:
         """
         Validate variables resolve as plugins are executed, and return
         a mock script which contains actualized added variables from the plugins
         """
+
         self._add_variables(PluginOperation.DOWNLOADER, options=self.downloader_options)
+        self._add_subscription_override_variables()
 
         # Metadata variables to be added
         for plugin_options in PluginMapping.order_options_by(
             self.plugins.zipped(), PluginOperation.MODIFY_ENTRY_METADATA
         ):
             self._add_variables(PluginOperation.MODIFY_ENTRY_METADATA, options=plugin_options)
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
                         VARIABLE_SCRIPTS[inj.variable_name],
                     )
                     for inj in v.injected_variables()
                 }
             )
             entries.append(entry)
 
+        # TODO: MATCH A URL TO A URL_VALIDATOR !!!
         for entry in sorted(entries, key=lambda ent: ent.get(v.download_index, int)):
             # Remove each entry from the live download archive since it will get re-added
             # unless it is filtered
             self._enhanced_download_archive.mapping.remove_entry(entry.uid)
             yield entry
 
             # If the original entry file_path is no longer maintained in the new mapping, then
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ytdl_sub.config.plugin.plugin import Plugin
 from ytdl_sub.config.validators.options import TOptionsValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
-class SourcePluginExtension(Plugin[TOptionsValidator], ABC):
+class SourcePluginExtension(Plugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
     are the plugin options.
     """
 
     @final
     def ytdl_options(self) -> Optional[Dict]:
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from ytdl_sub.downloaders.ytdlp import YTDLP
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.entry_parent import EntryParent
 from ytdl_sub.entries.script.variable_definitions import VARIABLES
 from ytdl_sub.entries.script.variable_definitions import VariableDefinitions
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.logger import Logger
+from ytdl_sub.utils.script import ScriptUtils
 from ytdl_sub.utils.thumbnail import ThumbnailTypes
 from ytdl_sub.utils.thumbnail import download_and_convert_url_thumbnail
 from ytdl_sub.utils.thumbnail import try_convert_download_thumbnail
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 v: VariableDefinitions = VARIABLES
 
@@ -37,31 +38,50 @@
 
 class URLDownloadState:
     def __init__(self, entries_total: int):
         self.entries_total = entries_total
         self.entries_downloaded = 0
 
 
-class UrlDownloaderThumbnailPlugin(SourcePluginExtension):
+class UrlDownloaderBasePluginExtension(SourcePluginExtension[MultiUrlValidator]):
+    def _match_entry_to_url_validator(self, entry: Entry) -> UrlValidator:
+        """
+        Handle matching a URL to its original validator. This is for .info.json updates
+        when older entries have missing variables
+        """
+        input_url_idx = entry.get(v.ytdl_sub_input_url_index, int)
+        entry_input_url = entry.get(v.ytdl_sub_input_url, str)
+
+        if 0 <= input_url_idx < len(self.plugin_options.urls.list):
+            validator = self.plugin_options.urls.list[input_url_idx]
+            if self.overrides.apply_formatter(validator.url) == entry_input_url:
+                return validator
+
+        # Match the first validator based on the URL, if one exists
+        for validator in self.plugin_options.urls.list:
+            if self.overrides.apply_formatter(validator.url) == entry_input_url:
+                return validator
+
+        # Return the first validator if none exist
+        return self.plugin_options.urls.list[0]
+
+
+class UrlDownloaderThumbnailPlugin(UrlDownloaderBasePluginExtension):
     def __init__(
         self,
         options: MultiUrlValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
             options=options,
             overrides=overrides,
             enhanced_download_archive=enhanced_download_archive,
         )
         self._thumbnails_downloaded: Set[str] = set()
-        self._collection_url_mapping: Dict[str, UrlValidator] = {
-            self.overrides.apply_formatter(collection_url.url): collection_url
-            for collection_url in options.urls.list
-        }
 
     def _download_parent_thumbnails(
         self,
         thumbnail_list_info: UrlThumbnailListValidator,
         entry: Entry,
         parent: EntryParent,
     ) -> None:
@@ -132,54 +152,40 @@
         In addition, convert the entry thumbnail to jpg
         """
         # We always convert entry thumbnails to jpgs, and is performed here to be done
         # as early as possible in the plugin pipeline (downstream plugins depend on it being jpg)
         if not self.is_dry_run:
             try_convert_download_thumbnail(entry=entry)
 
-        if (input_url := entry.get(v.ytdl_sub_input_url, str)) in self._collection_url_mapping:
-            self._download_url_thumbnails(
-                collection_url=self._collection_url_mapping[input_url],
-                entry=entry,
-            )
+        self._download_url_thumbnails(
+            collection_url=self._match_entry_to_url_validator(entry=entry),
+            entry=entry,
+        )
         return entry
 
 
-class UrlDownloaderCollectionVariablePlugin(SourcePluginExtension):
+class UrlDownloaderCollectionVariablePlugin(UrlDownloaderBasePluginExtension):
     def __init__(
         self,
         options: MultiUrlValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
             options=options,
             overrides=overrides,
             enhanced_download_archive=enhanced_download_archive,
         )
         self._thumbnails_downloaded: Set[str] = set()
-        self._collection_url_mapping: Dict[str, UrlValidator] = {
-            self.overrides.apply_formatter(collection_url.url): collection_url
-            for collection_url in options.urls.list
-        }
 
     def modify_entry_metadata(self, entry: Entry) -> Optional[Entry]:
         """
         Add collection variables to the entry
         """
-        # COLLECTION_URL is a recent variable that may not exist for old entries when updating.
-        # Try to use source_webpage_url if it does not exist
-        entry_collection_url = entry.get(v.ytdl_sub_input_url, str)
-
-        # If the collection URL cannot find its mapping, use the last URL
-        collection_url = (
-            self._collection_url_mapping.get(entry_collection_url)
-            or list(self._collection_url_mapping.values())[-1]
-        )
-
+        collection_url = self._match_entry_to_url_validator(entry=entry)
         entry.add(collection_url.variables.dict_with_format_strings)
 
         return entry
 
 
 class MultiUrlDownloader(SourcePlugin[MultiUrlValidator]):
     """
@@ -228,57 +234,63 @@
             download_ytdl_options=download_ytdl_options,
             metadata_ytdl_options=metadata_ytdl_options,
             overrides=overrides,
         )
         self._downloaded_entries: Set[str] = set()
         self._url_state: Optional[URLDownloadState] = None
 
-    @property
-    def download_ytdl_options(self) -> Dict:
+    def download_ytdl_options(self, url_idx: Optional[int] = None) -> Dict:
         """
         Returns
         -------
         YTLD options dict for downloading
         """
         return (
             self._download_ytdl_options_builder.clone()
             .add(self.ytdl_option_defaults(), before=True)
+            .add(
+                self.plugin_options.urls.list[url_idx].ytdl_options.dict
+                if url_idx is not None
+                else None,
+                before=True,
+            )
             .to_dict()
         )
 
-    @property
-    def metadata_ytdl_options(self) -> Dict:
+    def metadata_ytdl_options(self, ytdl_option_overrides: Dict) -> Dict:
         """
         Returns
         -------
         YTDL options dict for fetching metadata
         """
+
         return (
             self._metadata_ytdl_options_builder.clone()
             .add(self.ytdl_option_defaults(), before=True)
+            .add(ytdl_option_overrides, before=True)
             .to_dict()
         )
 
     @property
     def is_dry_run(self) -> bool:
         """
         Returns
         -------
         True if dry-run is enabled. False otherwise.
         """
-        return self.download_ytdl_options.get("skip_download", False)
+        return self.download_ytdl_options().get("skip_download", False)
 
     @property
     def is_entry_thumbnails_enabled(self) -> bool:
         """
         Returns
         -------
         True if entry thumbnails should be downloaded. False otherwise.
         """
-        return self.download_ytdl_options.get("writethumbnail", False)
+        return self.download_ytdl_options().get("writethumbnail", False)
 
     ###############################################################################################
     # DOWNLOAD FUNCTIONS
 
     def _is_downloaded(self, entry: Entry) -> bool:
         return entry.ytdl_uid() in self._downloaded_entries
 
@@ -297,15 +309,15 @@
         does not break when downloading from subset urls.
 
         Parameters
         ----------
         clear_info_json_files
             Whether to delete info.json files after yield
         """
-        archive_path = self.download_ytdl_options.get("download_archive", "")
+        archive_path = self.download_ytdl_options().get("download_archive", "")
         backup_archive_path = f"{archive_path}.backup"
 
         # If archive path exists, maintain download archive is enable
         if archive_file_exists := archive_path and os.path.isfile(archive_path):
             archive_file_exists = True
 
             # If a backup exists, it's the one prior to any downloading, use that.
@@ -332,15 +344,17 @@
                 if path.endswith(".info.json")
             ]
             for info_json_file in info_json_files:
                 FileHandler.delete(info_json_file)
 
     def _extract_entry_info_with_retry(self, entry: Entry) -> Entry:
         download_entry_dict = YTDLP.extract_info_with_retry(
-            ytdl_options_overrides=self.download_ytdl_options,
+            ytdl_options_overrides=self.download_ytdl_options(
+                url_idx=entry.get(v.ytdl_sub_input_url_index, int)
+            ),
             is_downloaded_fn=None if self.is_dry_run else entry.is_downloaded,
             is_thumbnail_downloaded_fn=None
             if (self.is_dry_run or not self.is_entry_thumbnails_enabled)
             else entry.is_thumbnail_downloaded_via_ytdlp,
             url=entry.webpage_url,
         )
         return Entry(
@@ -348,35 +362,37 @@
             working_directory=self.working_directory,
         )
 
     def _iterate_child_entries(
         self, entries: List[Entry], download_reversed: bool
     ) -> Iterator[Entry]:
         # Iterate a list of entries, and delete the entries after yielding
-        indices = list(range(len(entries)))
+        entries_to_iter: List[Optional[Entry]] = entries
+
+        indices = list(range(len(entries_to_iter)))
         if download_reversed:
             indices = reversed(indices)
 
         for idx in indices:
             self._url_state.entries_downloaded += 1
 
-            if self._is_downloaded(entries[idx]):
+            if self._is_downloaded(entries_to_iter[idx]):
                 download_logger.info(
                     "Already downloaded entry %d/%d: %s",
                     self._url_state.entries_downloaded,
                     self._url_state.entries_total,
-                    entries[idx].title,
+                    entries_to_iter[idx].title,
                 )
-                del entries[idx]
+                entries_to_iter[idx] = None
                 continue
 
-            yield entries[idx]
-            self._mark_downloaded(entries[idx])
+            yield entries_to_iter[idx]
+            self._mark_downloaded(entries_to_iter[idx])
 
-            del entries[idx]
+            entries_to_iter[idx] = None
 
     def _iterate_parent_entry(
         self, parent: EntryParent, download_reversed: bool
     ) -> Iterator[Entry]:
         for entry_child in self._iterate_child_entries(
             entries=parent.entry_children(), download_reversed=download_reversed
         ):
@@ -386,23 +402,23 @@
         for parent_child in reversed(parent.parent_children()):
             for entry_child in self._iterate_parent_entry(
                 parent=parent_child, download_reversed=download_reversed
             ):
                 yield entry_child
 
     def _download_url_metadata(
-        self, url: str, include_sibling_metadata: bool
+        self, url: str, include_sibling_metadata: bool, ytdl_options_overrides: Dict
     ) -> Tuple[List[EntryParent], List[Entry]]:
         """
         Downloads only info.json files and forms EntryParent trees
         """
         with self._separate_download_archives():
             entry_dicts = YTDLP.extract_info_via_info_json(
                 working_directory=self.working_directory,
-                ytdl_options_overrides=self.metadata_ytdl_options,
+                ytdl_options_overrides=ytdl_options_overrides,
                 log_prefix_on_info_json_dl="Downloading metadata for",
                 url=url,
             )
 
         parents = EntryParent.from_entry_dicts(
             url=url,
             entry_dicts=entry_dicts,
@@ -435,42 +451,58 @@
                     yield entry_child
 
             for orphan in self._iterate_child_entries(
                 entries=orphans, download_reversed=download_reversed
             ):
                 yield orphan
 
+    def _download_metadata(self, url: str, validator: UrlValidator) -> Iterable[Entry]:
+        metadata_ytdl_options = self.metadata_ytdl_options(
+            ytdl_option_overrides=validator.ytdl_options.dict
+        )
+        download_reversed = ScriptUtils.bool_formatter_output(
+            self.overrides.apply_formatter(validator.download_reverse)
+        )
+
+        parents, orphan_entries = self._download_url_metadata(
+            url=url,
+            include_sibling_metadata=validator.include_sibling_metadata,
+            ytdl_options_overrides=metadata_ytdl_options,
+        )
+
+        # TODO: Encapsulate this logic into its own class
+        self._url_state = URLDownloadState(
+            entries_total=sum(parent.num_children() for parent in parents) + len(orphan_entries)
+        )
+
+        download_logger.info("Beginning downloads for %s", url)
+        for entry in self._iterate_entries(
+            parents=parents,
+            orphans=orphan_entries,
+            download_reversed=download_reversed,
+        ):
+            yield entry
+
     def download_metadata(self) -> Iterable[Entry]:
         """The function to perform the download of all media entries"""
         # download the bottom-most urls first since they are top-priority
-        for collection_url in reversed(self.collection.urls.list):
+        for idx, url_validator in reversed(list(enumerate(self.collection.urls.list))):
             # URLs can be empty. If they are, then skip
-            if not (url := self.overrides.apply_formatter(collection_url.url)):
+            if not (url := self.overrides.apply_formatter(url_validator.url)):
                 continue
 
-            parents, orphan_entries = self._download_url_metadata(
-                url=url, include_sibling_metadata=collection_url.include_sibling_metadata
-            )
-
-            # TODO: Encapsulate this logic into its own class
-            self._url_state = URLDownloadState(
-                entries_total=sum(parent.num_children() for parent in parents) + len(orphan_entries)
-            )
-
-            download_logger.info(
-                "Beginning downloads for %s", self.overrides.apply_formatter(collection_url.url)
-            )
-            for entry in self._iterate_entries(
-                parents=parents,
-                orphans=orphan_entries,
-                download_reversed=collection_url.download_reverse,
-            ):
+            for entry in self._download_metadata(url=url, validator=url_validator):
                 entry.initialize_script(self.overrides).add(
-                    {v.ytdl_sub_input_url: self.overrides.apply_formatter(collection_url.url)}
+                    {
+                        v.ytdl_sub_input_url: url,
+                        v.ytdl_sub_input_url_index: idx,
+                        v.ytdl_sub_input_url_count: len(self.collection.urls.list),
+                    }
                 )
+
                 yield entry
 
     def download(self, entry: Entry) -> Optional[Entry]:
         """
         Parameters
         ----------
         entry
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Set
 
 from ytdl_sub.config.plugin.plugin_operation import PluginOperation
+from ytdl_sub.config.preset_options import YTDLOptions
 from ytdl_sub.config.validators.options import OptionsValidator
 from ytdl_sub.script.parser import parse
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
+from ytdl_sub.validators.string_formatter_validators import OverridesBooleanFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import OverridesStringFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.validators import BoolValidator
 from ytdl_sub.validators.validators import ListValidator
 
 
 class UrlThumbnailValidator(StrictDictValidator):
@@ -45,14 +47,15 @@
 class UrlValidator(StrictDictValidator):
     _required_keys = {"url"}
     _optional_keys = {
         "variables",
         "source_thumbnails",
         "playlist_thumbnails",
         "download_reverse",
+        "ytdl_options",
         "include_sibling_metadata",
     }
 
     @classmethod
     def partial_validate(cls, name: str, value: Any) -> None:
         """
         Partially validate a YouTube collection url
@@ -73,15 +76,18 @@
         self._source_thumbnails = self._validate_key_if_present(
             key="source_thumbnails", validator=UrlThumbnailListValidator, default=[]
         )
         self._playlist_thumbnails = self._validate_key_if_present(
             key="playlist_thumbnails", validator=UrlThumbnailListValidator, default=[]
         )
         self._download_reverse = self._validate_key(
-            key="download_reverse", validator=BoolValidator, default=True
+            key="download_reverse", validator=OverridesBooleanFormatterValidator, default="True"
+        )
+        self._ytdl_options = self._validate_key(
+            key="ytdl_options", validator=YTDLOptions, default={}
         )
         self._include_sibling_metadata = self._validate_key(
             key="include_sibling_metadata", validator=BoolValidator, default=False
         )
 
     @property
     def url(self) -> OverridesStringFormatterValidator:
@@ -144,20 +150,28 @@
         ``name`` is the file name relative to the output directory to store the thumbnail.
         ``uid`` is the yt-dlp thumbnail ID. Can specify ``latest_entry`` to use the latest entry's
         thumbnail.
         """
         return self._source_thumbnails
 
     @property
-    def download_reverse(self) -> bool:
+    def download_reverse(self) -> OverridesBooleanFormatterValidator:
         """
         Optional. Whether to download entries in the reverse order of the metadata downloaded.
         Defaults to True.
         """
-        return self._download_reverse.value
+        return self._download_reverse
+
+    @property
+    def ytdl_options(self) -> YTDLOptions:
+        """
+        Optional. ``ytdl_options`` that only apply to this URL. These take precedence
+        over the plugin ``ytdl_options``.
+        """
+        return self._ytdl_options
 
     @property
     def include_sibling_metadata(self) -> bool:
         """
         Optional. Whether to include sibling metadata as an entry variable, which comprises basic
         metadata from all other entries (including itself) that belong to the same playlist. For
         channels or large playlists, this becomes memory-intensive since you are storing
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/custom_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/custom_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/function_scripts.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/function_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict
 
 from ytdl_sub.entries.script.variable_definitions import VARIABLES
 from ytdl_sub.entries.script.variable_definitions import VariableDefinitions
 
 v: VariableDefinitions = VARIABLES
 
+# TODO: Make this a proper class with docstrings
 CUSTOM_FUNCTION_SCRIPTS: Dict[str, str] = {
     #############################################################################################
     # SIBLING GETTER
     "%extract_field_from_siblings": f"""{{
         %if(
             %bool({v.sibling_metadata.variable_name}),
             %array_apply_fixed(
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/variable_definitions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,14 +747,32 @@
         """
         :description:
           The input URL used in ytdl-sub to create this entry.
         """
         return StringVariable(variable_name="ytdl_sub_input_url", definition="{ %string('') }")
 
     @cached_property
+    def ytdl_sub_input_url_index(self: "VariableDefinitions") -> IntegerVariable:
+        """
+        :description:
+          The index of the input URL as defined in the subscription, top-most being the 0th index.
+        """
+        # init as -1 so if prior downloaded entries are known when they do not have this value
+        # in their .info.json
+        return IntegerVariable(variable_name="ytdl_sub_input_url_index", definition="{ %int(-1) }")
+
+    @cached_property
+    def ytdl_sub_input_url_count(self: "VariableDefinitions") -> IntegerVariable:
+        """
+        :description:
+          The total number of input URLs as defined in the subscription.
+        """
+        return IntegerVariable(variable_name="ytdl_sub_input_url_count", definition="{ %int(0) }")
+
+    @cached_property
     def download_index(self: "VariableDefinitions") -> IntegerVariable:
         """
         :description:
           The i'th entry downloaded. NOTE that this is fetched dynamically from the download
           archive.
         """
         return IntegerVariable(variable_name="download_index", definition="{ %int(1) }")
@@ -1096,14 +1114,16 @@
             self.download_index,
             self.upload_date_index,
             self.comments,
             self.requested_subtitles,
             self.chapters,
             self.sponsorblock_chapters,
             self.ytdl_sub_input_url,
+            self.ytdl_sub_input_url_index,
+            self.ytdl_sub_input_url_count,
         }
 
     @cache
     def required_entry_variables(self) -> Set[MetadataVariable]:
         """
         Returns variables that the entry requires to exist
         """
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/script/variable_types.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from ytdl_sub.script.types.array import Array
 from ytdl_sub.script.types.map import Map
+from ytdl_sub.script.types.resolvable import Boolean
 from ytdl_sub.script.types.resolvable import Integer
 from ytdl_sub.script.types.resolvable import String
 
 ENTRY_METADATA_VARIABLE_NAME = "entry_metadata"
 PLAYLIST_METADATA_VARIABLE_NAME = "playlist_metadata"
 SOURCE_METADATA_VARIABLE_NAME = "source_metadata"
 
@@ -60,14 +61,21 @@
     def human_readable_type(cls) -> str:
         """
         Script type of the variable, for documentation
         """
 
 
 @dataclass(frozen=True)
+class BooleanVariable(Variable):
+    @classmethod
+    def human_readable_type(cls) -> str:
+        return Boolean.__name__
+
+
+@dataclass(frozen=True)
 class StringVariable(Variable):
     @classmethod
     def human_readable_type(cls) -> str:
         return String.__name__
 
     def to_sanitized_plex(self, variable_name: str) -> "StringVariable":
         """
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/entries/variables/override_variables.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/override_variables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,84 @@
+from typing import Dict
+from typing import Set
+
 from ytdl_sub.entries.script.function_scripts import CUSTOM_FUNCTION_SCRIPTS
 from ytdl_sub.entries.script.variable_definitions import VARIABLE_SCRIPTS
+from ytdl_sub.entries.script.variable_types import BooleanVariable
+from ytdl_sub.entries.script.variable_types import MapVariable
+from ytdl_sub.entries.script.variable_types import StringVariable
+from ytdl_sub.entries.script.variable_types import Variable
 from ytdl_sub.script.functions import Functions
 from ytdl_sub.script.utils.name_validation import is_valid_name
 
 # TODO: use this
 SUBSCRIPTION_ARRAY = "subscription_array"
 
 
 class SubscriptionVariables:
     @staticmethod
-    def subscription_name() -> str:
+    def subscription_name() -> StringVariable:
         """
         Name of the subscription. For subscriptions types that use a prefix (``~``, ``+``),
         the prefix and all whitespace afterwards is stripped from the subscription name.
         """
-        return "subscription_name"
+        return StringVariable(variable_name="subscription_name", definition="{ %string('') }")
 
     @staticmethod
-    def subscription_value() -> str:
+    def subscription_value() -> StringVariable:
         """
         For subscriptions in the form of
 
         .. code-block:: yaml
 
            "Subscription Name": "https://..."
 
         ``subscription_value`` gets set to ``https://...``.
         """
-        return "subscription_value"
+        return StringVariable(variable_name="subscription_value", definition="{ %string('') }")
 
     @staticmethod
-    def subscription_indent_i(index: int) -> str:
+    def subscription_indent_i(index: int) -> StringVariable:
         """
         For subscriptions in the form of
 
         .. code-block:: yaml
 
            Preset | = Indent Value 1:
              = Indent Value 2:
                "Subscription Name": "https://..."
 
         ``subscription_indent_1`` and ``subscription_indent_2`` get set to
         ``Indent Value 1`` and ``Indent Value 2``.
         """
-        return f"subscription_indent_{index + 1}"
+        return StringVariable(
+            variable_name=f"subscription_indent_{index + 1}", definition="{ %string('') }"
+        )
 
     @staticmethod
-    def subscription_value_i(index: int) -> str:
+    def subscription_value_i(index: int) -> StringVariable:
         """
         For subscriptions in the form of
 
         .. code-block:: yaml
 
            "Subscription Name":
              - "https://url1.com/..."
              - "https://url2.com/..."
 
         ``subscription_value_1`` and ``subscription_value_2`` get set to ``https://url1.com/...``
         and ``https://url2.com/...``. Note that ``subscription_value_1`` also gets set to
         ``subscription_value``.
         """
-        return f"subscription_value_{index + 1}"
+        return StringVariable(
+            variable_name=f"subscription_value_{index + 1}", definition="{ %string('') }"
+        )
 
     @staticmethod
-    def subscription_map() -> str:
+    def subscription_map() -> MapVariable:
         """
         For subscriptions in the form of
 
         .. code-block:: yaml
 
            + Subscription Name:
              Music Videos:
@@ -85,15 +96,25 @@
                "https://url1.com/..."
              ],
              "Concerts: [
                "https://url2.com/..."
              ]
            }
         """
-        return "subscription_map"
+        return MapVariable(variable_name="subscription_map", definition="{ {} }")
+
+    @staticmethod
+    def subscription_has_download_archive() -> BooleanVariable:
+        """
+        Returns True if the subscription has any entries recorded in a download archive. False
+        otherwise.
+        """
+        return BooleanVariable(
+            variable_name="subscription_has_download_archive", definition="{ %bool(True) }"
+        )
 
 
 class OverrideHelpers:
     @classmethod
     def is_entry_variable_name(cls, name: str) -> bool:
         """
         Returns
@@ -120,7 +141,21 @@
         -------
         True if the override name itself is valid. False otherwise.
         """
         if name.startswith("%"):
             return is_valid_name(name=name[1:])
 
         return is_valid_name(name=name)
+
+
+REQUIRED_OVERRIDE_VARIABLES: Set[Variable] = {
+    SubscriptionVariables.subscription_name(),
+    SubscriptionVariables.subscription_has_download_archive(),
+}
+
+REQUIRED_OVERRIDE_VARIABLE_DEFINITIONS: Dict[str, str] = {
+    var.variable_name: var.definition for var in REQUIRED_OVERRIDE_VARIABLES
+}
+
+REQUIRED_OVERRIDE_VARIABLE_NAMES: Set[str] = {
+    var.variable_name for var in REQUIRED_OVERRIDE_VARIABLES
+}
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/main.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/filter_exclude.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_exclude.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/filter_include.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_include.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/format.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/format.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/throttle_protection.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/throttle_protection.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/helpers/players.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music/singles.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/singles.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -27,23 +27,14 @@
   _kodi_tv_show:
     preset:
       - "_kodi_base"
       - "_jellyfin_tv_show"
 
 ####################################################################################################
 
-  # TV show from one or more sources. Uses {url}'s avatar and banner as poster and fanart
-  _tv_show_by_date:
-    preset: "_multi_url"
-    overrides:
-      avatar_uncropped_thumbnail_file_name: "{tv_show_poster_file_name}"
-      banner_uncropped_thumbnail_file_name: "{tv_show_fanart_file_name}"
-
-####################################################################################################
-
   _episode_video_tags:
     video_tags:
       show: "{tv_show_name}"
       genre: "{tv_show_genre}"
       episode_id: "{episode_number}"
       title: "{episode_title}"
       synopsis: "{episode_plot}"
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -29,14 +29,23 @@
   "Plex TV Show by Date":
     preset:
       - "plex_tv_show_by_date"
       - "season_by_year__episode_by_month_day"
 
 ####################################################################################################
 
+  # TV show from one or more sources. Uses {url}'s avatar and banner as poster and fanart
+  _tv_show_by_date:
+    preset: "_multi_url_bilateral"
+    overrides:
+      avatar_uncropped_thumbnail_file_name: "{tv_show_poster_file_name}"
+      banner_uncropped_thumbnail_file_name: "{tv_show_fanart_file_name}"
+
+####################################################################################################
+
   _season_by_year:
     overrides:
       season_number: "{upload_year}"
       season_number_padded: "{season_number}"
 
   _season_by_year_month:
     overrides:
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     overrides:
       episode_number: "{playlist_index_reversed}"
       episode_number_padded: "{playlist_index_reversed_padded6}"
 
   ##############
 
   _tv_show_collection:
+    preset:
+      - "_tv_show_collection_bilateral"
+
     download:
       - url: "{collection_season_1_url}"
         variables:
           collection_season_number: "1"
           collection_season_name: "{collection_season_1_name}"
         playlist_thumbnails:
           # Use latest_entry first, then see if YT channel artwork exists
@@ -75,280 +78,319 @@
           - name: "{tv_show_fanart_file_name}"
             uid: "banner_uncropped"
         source_thumbnails:
           - name: "{tv_show_poster_file_name}"
             uid: "avatar_uncropped"
           - name: "{tv_show_fanart_file_name}"
             uid: "banner_uncropped"
+
       - url: "{collection_season_2_url}"
         variables:
           collection_season_number: "2"
           collection_season_name: "{collection_season_2_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_3_url}"
         variables:
           collection_season_number: "3"
           collection_season_name: "{collection_season_3_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_4_url}"
         variables:
           collection_season_number: "4"
           collection_season_name: "{collection_season_4_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_5_url}"
         variables:
           collection_season_number: "5"
           collection_season_name: "{collection_season_5_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_6_url}"
         variables:
           collection_season_number: "6"
           collection_season_name: "{collection_season_6_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_7_url}"
         variables:
           collection_season_number: "7"
           collection_season_name: "{collection_season_7_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_8_url}"
         variables:
           collection_season_number: "8"
           collection_season_name: "{collection_season_8_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_9_url}"
         variables:
           collection_season_number: "9"
           collection_season_name: "{collection_season_9_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_10_url}"
         variables:
           collection_season_number: "10"
           collection_season_name: "{collection_season_10_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_11_url}"
         variables:
           collection_season_number: "11"
           collection_season_name: "{collection_season_11_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_12_url}"
         variables:
           collection_season_number: "12"
           collection_season_name: "{collection_season_12_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_13_url}"
         variables:
           collection_season_number: "13"
           collection_season_name: "{collection_season_13_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_14_url}"
         variables:
           collection_season_number: "14"
           collection_season_name: "{collection_season_14_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_15_url}"
         variables:
           collection_season_number: "15"
           collection_season_name: "{collection_season_15_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_16_url}"
         variables:
           collection_season_number: "16"
           collection_season_name: "{collection_season_16_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_17_url}"
         variables:
           collection_season_number: "17"
           collection_season_name: "{collection_season_17_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_18_url}"
         variables:
           collection_season_number: "18"
           collection_season_name: "{collection_season_18_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_19_url}"
         variables:
           collection_season_number: "19"
           collection_season_name: "{collection_season_19_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_20_url}"
         variables:
           collection_season_number: "20"
           collection_season_name: "{collection_season_20_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_21_url}"
         variables:
           collection_season_number: "21"
           collection_season_name: "{collection_season_21_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_22_url}"
         variables:
           collection_season_number: "22"
           collection_season_name: "{collection_season_22_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_23_url}"
         variables:
           collection_season_number: "23"
           collection_season_name: "{collection_season_23_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_24_url}"
         variables:
           collection_season_number: "24"
           collection_season_name: "{collection_season_24_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_25_url}"
         variables:
           collection_season_number: "25"
           collection_season_name: "{collection_season_25_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_26_url}"
         variables:
           collection_season_number: "26"
           collection_season_name: "{collection_season_26_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_27_url}"
         variables:
           collection_season_number: "27"
           collection_season_name: "{collection_season_27_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_28_url}"
         variables:
           collection_season_number: "28"
           collection_season_name: "{collection_season_28_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_29_url}"
         variables:
           collection_season_number: "29"
           collection_season_name: "{collection_season_29_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_30_url}"
         variables:
           collection_season_number: "30"
           collection_season_name: "{collection_season_30_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_31_url}"
         variables:
           collection_season_number: "31"
           collection_season_name: "{collection_season_31_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_32_url}"
         variables:
           collection_season_number: "32"
           collection_season_name: "{collection_season_32_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_33_url}"
         variables:
           collection_season_number: "33"
           collection_season_name: "{collection_season_33_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_34_url}"
         variables:
           collection_season_number: "34"
           collection_season_name: "{collection_season_34_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_35_url}"
         variables:
           collection_season_number: "35"
           collection_season_name: "{collection_season_35_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_36_url}"
         variables:
           collection_season_number: "36"
           collection_season_name: "{collection_season_36_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_37_url}"
         variables:
           collection_season_number: "37"
           collection_season_name: "{collection_season_37_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_38_url}"
         variables:
           collection_season_number: "38"
           collection_season_name: "{collection_season_38_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_39_url}"
         variables:
           collection_season_number: "39"
           collection_season_name: "{collection_season_39_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
+
       - url: "{collection_season_40_url}"
         variables:
           collection_season_number: "40"
           collection_season_name: "{collection_season_40_name}"
         playlist_thumbnails:
           - name: "{season_poster_file_name}"
             uid: "latest_entry"
@@ -644,14 +686,340 @@
       s35_url: ""
       s36_url: ""
       s37_url: ""
       s38_url: ""
       s39_url: ""
       s40_url: ""
 
+  _tv_show_collection_bilateral:
+    preset:
+      - "_url_bilateral_overrides"
+
+    download:
+      - url: "{ %bilateral_url(collection_season_1_url) }"
+        variables:
+          collection_season_number: "1"
+          collection_season_name: "{collection_season_1_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_2_url) }"
+        variables:
+          collection_season_number: "2"
+          collection_season_name: "{collection_season_2_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_3_url) }"
+        variables:
+          collection_season_number: "3"
+          collection_season_name: "{collection_season_3_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_4_url) }"
+        variables:
+          collection_season_number: "4"
+          collection_season_name: "{collection_season_4_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_5_url) }"
+        variables:
+          collection_season_number: "5"
+          collection_season_name: "{collection_season_5_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_6_url) }"
+        variables:
+          collection_season_number: "6"
+          collection_season_name: "{collection_season_6_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_7_url) }"
+        variables:
+          collection_season_number: "7"
+          collection_season_name: "{collection_season_7_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_8_url) }"
+        variables:
+          collection_season_number: "8"
+          collection_season_name: "{collection_season_8_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_9_url) }"
+        variables:
+          collection_season_number: "9"
+          collection_season_name: "{collection_season_9_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_10_url) }"
+        variables:
+          collection_season_number: "10"
+          collection_season_name: "{collection_season_10_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_11_url) }"
+        variables:
+          collection_season_number: "11"
+          collection_season_name: "{collection_season_11_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_12_url) }"
+        variables:
+          collection_season_number: "12"
+          collection_season_name: "{collection_season_12_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_13_url) }"
+        variables:
+          collection_season_number: "13"
+          collection_season_name: "{collection_season_13_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_14_url) }"
+        variables:
+          collection_season_number: "14"
+          collection_season_name: "{collection_season_14_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_15_url) }"
+        variables:
+          collection_season_number: "15"
+          collection_season_name: "{collection_season_15_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_16_url) }"
+        variables:
+          collection_season_number: "16"
+          collection_season_name: "{collection_season_16_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_17_url) }"
+        variables:
+          collection_season_number: "17"
+          collection_season_name: "{collection_season_17_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_18_url) }"
+        variables:
+          collection_season_number: "18"
+          collection_season_name: "{collection_season_18_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_19_url) }"
+        variables:
+          collection_season_number: "19"
+          collection_season_name: "{collection_season_19_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_20_url) }"
+        variables:
+          collection_season_number: "20"
+          collection_season_name: "{collection_season_20_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_21_url) }"
+        variables:
+          collection_season_number: "21"
+          collection_season_name: "{collection_season_21_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_22_url) }"
+        variables:
+          collection_season_number: "22"
+          collection_season_name: "{collection_season_22_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_23_url) }"
+        variables:
+          collection_season_number: "23"
+          collection_season_name: "{collection_season_23_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_24_url) }"
+        variables:
+          collection_season_number: "24"
+          collection_season_name: "{collection_season_24_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_25_url) }"
+        variables:
+          collection_season_number: "25"
+          collection_season_name: "{collection_season_25_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_26_url) }"
+        variables:
+          collection_season_number: "26"
+          collection_season_name: "{collection_season_26_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_27_url) }"
+        variables:
+          collection_season_number: "27"
+          collection_season_name: "{collection_season_27_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_28_url) }"
+        variables:
+          collection_season_number: "28"
+          collection_season_name: "{collection_season_28_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_29_url) }"
+        variables:
+          collection_season_number: "29"
+          collection_season_name: "{collection_season_29_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_30_url) }"
+        variables:
+          collection_season_number: "30"
+          collection_season_name: "{collection_season_30_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_31_url) }"
+        variables:
+          collection_season_number: "31"
+          collection_season_name: "{collection_season_31_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_32_url) }"
+        variables:
+          collection_season_number: "32"
+          collection_season_name: "{collection_season_32_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_33_url) }"
+        variables:
+          collection_season_number: "33"
+          collection_season_name: "{collection_season_33_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_34_url) }"
+        variables:
+          collection_season_number: "34"
+          collection_season_name: "{collection_season_34_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_35_url) }"
+        variables:
+          collection_season_number: "35"
+          collection_season_name: "{collection_season_35_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_36_url) }"
+        variables:
+          collection_season_number: "36"
+          collection_season_name: "{collection_season_36_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_37_url) }"
+        variables:
+          collection_season_number: "37"
+          collection_season_name: "{collection_season_37_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_38_url) }"
+        variables:
+          collection_season_number: "38"
+          collection_season_name: "{collection_season_38_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_39_url) }"
+        variables:
+          collection_season_number: "39"
+          collection_season_name: "{collection_season_39_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+      - url: "{ %bilateral_url(collection_season_40_url) }"
+        variables:
+          collection_season_number: "40"
+          collection_season_name: "{collection_season_40_name}"
+        download_reverse: False
+        ytdl_options:
+          playlist_items: "-1:0:-1"
+
+
 ####################################################################################################
 # DEPRECATED SEASON PRESETS
 
   collection_season_1: {}
   collection_season_2: {}
   collection_season_3: {}
   collection_season_4: {}
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/__init__.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/array_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/array_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/boolean_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/boolean_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/conditional_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/conditional_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/error_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/error_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/json_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/json_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/map_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/map_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/numeric_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/regex_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/regex_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/functions/string_functions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/parser.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/script.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/script.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/script_output.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/script_output.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/array.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/array.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/function.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/function.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/map.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/map.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/resolvable.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/resolvable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/syntax_tree.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/variable.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/types/variable_dependency.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable_dependency.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/exception_formatters.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exception_formatters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/exceptions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/name_validation.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/name_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/script/utils/type_checking.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/type_checking.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,21 +5,40 @@
 from ytdl_sub.config.config_validator import ConfigOptions
 from ytdl_sub.config.overrides import Overrides
 from ytdl_sub.config.plugin.preset_plugins import PresetPlugins
 from ytdl_sub.config.preset import Preset
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import YTDLOptions
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
+from ytdl_sub.entries.variables.override_variables import SubscriptionVariables
 from ytdl_sub.utils.file_handler import FileHandlerTransactionLog
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 logger = Logger.get("subscription")
 
 
+def _initialize_download_archive(
+    output_options: OutputOptions,
+    overrides: Overrides,
+    working_directory: str,
+    output_directory: str,
+) -> EnhancedDownloadArchive:
+    migrated_file_name: Optional[str] = None
+    if migrated_file_name_option := output_options.migrated_download_archive_name:
+        migrated_file_name = overrides.apply_formatter(migrated_file_name_option)
+
+    return EnhancedDownloadArchive(
+        file_name=overrides.apply_formatter(output_options.download_archive_name),
+        working_directory=working_directory,
+        output_directory=output_directory,
+        migrated_file_name=migrated_file_name,
+    ).reinitialize(dry_run=True)
+
+
 class BaseSubscription(ABC):
     """
     Subscription classes are the 'controllers' that perform...
 
     -  Downloading via ytdlp
     -  Adding metadata
     -  Placing files in the output directory
@@ -44,29 +63,52 @@
         config_options: ConfigOptions
         preset_options: Preset
         """
         self.name = name
         self._config_options = config_options
         self._preset_options = preset_options
 
-        migrated_file_name: Optional[str] = None
-        if migrated_file_name_option := self.output_options.migrated_download_archive_name:
-            migrated_file_name = self.overrides.apply_formatter(migrated_file_name_option)
-
-        # TODO: Do not include this as part of the subscription
-        self._enhanced_download_archive = EnhancedDownloadArchive(
-            file_name=self.overrides.apply_formatter(self.output_options.download_archive_name),
+        # Add overrides pre-archive
+        self.overrides.add(
+            {
+                SubscriptionVariables.subscription_name(): self.name,
+            }
+        )
+
+        self._enhanced_download_archive: Optional[
+            EnhancedDownloadArchive
+        ] = _initialize_download_archive(
+            output_options=self.output_options,
+            overrides=self.overrides,
             working_directory=self.working_directory,
             output_directory=self.output_directory,
-            migrated_file_name=migrated_file_name,
+        )
+
+        # Add post-archive variables
+        self.overrides.add(
+            {
+                SubscriptionVariables.subscription_has_download_archive(): f"""{{
+                        %bool({self.download_archive.num_entries > 0})
+                    }}""",
+            }
         )
 
         self._exception: Optional[Exception] = None
 
     @property
+    def download_archive(self) -> EnhancedDownloadArchive:
+        """
+        Returns
+        -------
+        Initialized download archive
+        """
+        assert self._enhanced_download_archive is not None
+        return self._enhanced_download_archive
+
+    @property
     def downloader_options(self) -> MultiUrlValidator:
         """
         Returns
         -------
         The download options for this subscription's downloader
         """
         return self._preset_options.downloader_options
@@ -137,51 +179,51 @@
     @property
     def num_entries_added(self) -> int:
         """
         Returns
         -------
         Number of entries added
         """
-        return self._enhanced_download_archive.num_entries_added
+        return self.download_archive.num_entries_added
 
     @property
     def num_entries_modified(self) -> int:
         """
         Returns
         -------
         Number of entries modified
         """
-        return self._enhanced_download_archive.num_entries_modified
+        return self.download_archive.num_entries_modified
 
     @property
     def num_entries_removed(self) -> int:
         """
         Returns
         -------
         Number of entries removed
         """
-        return self._enhanced_download_archive.num_entries_removed
+        return self.download_archive.num_entries_removed
 
     @property
     def num_entries(self) -> int:
         """
         Returns
         -------
         The number of entries
         """
-        return self._enhanced_download_archive.num_entries
+        return self.download_archive.num_entries
 
     @property
     def transaction_log(self) -> FileHandlerTransactionLog:
         """
         Returns
         -------
         Transaction log from the subscription
         """
-        return self._enhanced_download_archive.get_file_handler_transaction_log()
+        return self.download_archive.get_file_handler_transaction_log()
 
     @property
     def exception(self) -> Optional[Exception]:
         """
         Returns
         -------
         An exception if one occurred while processing the subscription
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,29 +63,29 @@
         entry_metadata
             Optional. Metadata to record to the transaction log for this entry
         """
         # Move the file after all direct file modifications are complete
         output_file_name = self.overrides.apply_formatter(
             formatter=self.output_options.file_name, entry=entry
         )
-        self._enhanced_download_archive.save_file_to_output_directory(
+        self.download_archive.save_file_to_output_directory(
             file_name=entry.get_download_file_name(),
             file_metadata=entry_metadata,
             output_file_name=output_file_name,
             entry=entry,
         )
 
         # Always pretend to include the thumbnail in a dry-run
         if self.output_options.thumbnail_name and (dry_run or entry.is_thumbnail_downloaded()):
             output_thumbnail_name = self.overrides.apply_formatter(
                 formatter=self.output_options.thumbnail_name, entry=entry
             )
 
             # Copy the thumbnails since they could be used later for other things
-            self._enhanced_download_archive.save_file_to_output_directory(
+            self.download_archive.save_file_to_output_directory(
                 file_name=entry.get_download_thumbnail_name(),
                 output_file_name=output_thumbnail_name,
                 entry=entry,
                 copy_file=True,
             )
         elif not entry.is_thumbnail_downloaded():
             logger.warning(
@@ -97,15 +97,15 @@
                 formatter=self.output_options.info_json_name, entry=entry
             )
 
             # if not dry-run, write the info json
             if not dry_run:
                 entry.write_info_json()
 
-            self._enhanced_download_archive.save_file_to_output_directory(
+            self.download_archive.save_file_to_output_directory(
                 file_name=entry.get_download_info_json_name(),
                 output_file_name=output_info_json_name,
                 entry=entry,
             )
 
     def _delete_working_directory(self, is_error: bool = False) -> None:
         _ = is_error
@@ -131,15 +131,15 @@
 
     @contextlib.contextmanager
     def _maintain_archive_file(self):
         """
         Context manager to initialize the enhanced download archive
         """
         if self.maintain_download_archive:
-            self._enhanced_download_archive.prepare_download_archive()
+            self.download_archive.prepare_download_archive()
 
         yield
 
         # If output options maintains stale file deletion, perform the delete here prior to saving
         # the download archive
         if self.maintain_download_archive:
             date_range_to_keep = to_date_range(
@@ -152,27 +152,27 @@
             if self.output_options.keep_max_files:
                 # validated it can be cast to int within the validator
                 keep_max_files = int(
                     self.overrides.apply_formatter(self.output_options.keep_max_files)
                 )
 
             if date_range_to_keep or self.output_options.keep_max_files is not None:
-                self._enhanced_download_archive.remove_stale_files(
+                self.download_archive.remove_stale_files(
                     date_range=date_range_to_keep, keep_max_files=keep_max_files
                 )
 
-            self._enhanced_download_archive.save_download_mappings()
-            FileHandler.delete(self._enhanced_download_archive.working_file_path)
+            self.download_archive.save_download_mappings()
+            FileHandler.delete(self.download_archive.working_file_path)
 
     @contextlib.contextmanager
     def _remove_empty_directories_in_output_directory(self):
         try:
             yield
         finally:
-            if not self._enhanced_download_archive.is_dry_run:
+            if not self.download_archive.is_dry_run:
                 for root, dir_names, _ in os.walk(Path(self.output_directory), topdown=False):
                     for dir_name in dir_names:
                         dir_path = Path(root) / dir_name
                         if len(os.listdir(dir_path)) == 0:
                             os.rmdir(dir_path)
 
     @contextlib.contextmanager
@@ -190,15 +190,15 @@
         -------
         List of plugins defined in the subscription, initialized and ready to use.
         """
         plugins = [
             plugin_type(
                 options=plugin_options,
                 overrides=self.overrides,
-                enhanced_download_archive=self._enhanced_download_archive,
+                enhanced_download_archive=self.download_archive,
             )
             for plugin_type, plugin_options in self.plugins.zipped()
         ]
         return [plugin for plugin in plugins if plugin.is_enabled]
 
     @classmethod
     def _cleanup_entry_files(cls, entry: Entry):
@@ -229,15 +229,15 @@
         # Then, move it to the output directory
         self._move_entry_files_to_output_directory(
             dry_run=dry_run, entry=entry, entry_metadata=entry_metadata
         )
 
         # Re-save the download archive after each entry is moved to the output directory
         if self.maintain_download_archive:
-            self._enhanced_download_archive.save_download_mappings()
+            self.download_archive.save_download_mappings()
 
     def _process_entry(
         self, plugins: List[Plugin], dry_run: bool, entry: Entry, entry_metadata: FileMetadata
     ) -> None:
         entry_: Optional[Entry] = entry
 
         # First, modify the entry with all plugins
@@ -319,43 +319,43 @@
                     self._process_entry(
                         plugins=plugins, dry_run=dry_run, entry=entry, entry_metadata=entry_metadata
                     )
 
         for plugin in plugins:
             plugin.post_process_subscription()
 
-        return self._enhanced_download_archive.get_file_handler_transaction_log()
+        return self.download_archive.get_file_handler_transaction_log()
 
     def download(self, dry_run: bool = False) -> FileHandlerTransactionLog:
         """
         Performs the subscription download
 
         Parameters
         ----------
         dry_run
             If true, do not download any video/audio files or move anything to the output
             directory.
         """
         self._exception = None
-        self._enhanced_download_archive.reinitialize(dry_run=dry_run)
+        self.download_archive.reinitialize(dry_run=dry_run)
 
         plugins = self._initialize_plugins()
 
         subscription_ytdl_options = SubscriptionYTDLOptions(
             preset=self._preset_options,
             plugins=plugins,
-            enhanced_download_archive=self._enhanced_download_archive,
+            enhanced_download_archive=self.download_archive,
             overrides=self.overrides,
             working_directory=self.working_directory,
             dry_run=dry_run,
         )
 
         downloader = MultiUrlDownloader(
             options=self.downloader_options,
-            enhanced_download_archive=self._enhanced_download_archive,
+            enhanced_download_archive=self.download_archive,
             download_ytdl_options=subscription_ytdl_options.download_builder(),
             metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
             overrides=self.overrides,
         )
 
         plugins.extend(downloader.added_plugins())
 
@@ -385,41 +385,41 @@
 
         Parameters
         ----------
         dry_run
             If true, do not modify any video/audio files or move anything to the output directory.
         """
         self._exception = None
-        self._enhanced_download_archive.reinitialize(dry_run=dry_run)
+        self.download_archive.reinitialize(dry_run=dry_run)
 
         plugins = self._initialize_plugins()
 
         subscription_ytdl_options = SubscriptionYTDLOptions(
             preset=self._preset_options,
             plugins=plugins,
-            enhanced_download_archive=self._enhanced_download_archive,
+            enhanced_download_archive=self.download_archive,
             overrides=self.overrides,
             working_directory=self.working_directory,
             dry_run=dry_run,
         )
 
         # Re-add the original downloader class' plugins
         plugins.extend(
             MultiUrlDownloader(
                 options=self.downloader_options,
-                enhanced_download_archive=self._enhanced_download_archive,
+                enhanced_download_archive=self.download_archive,
                 download_ytdl_options=subscription_ytdl_options.download_builder(),
                 metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
                 overrides=self.overrides,
             ).added_plugins()
         )
 
         downloader = InfoJsonDownloader(
             options=InfoJsonDownloaderOptions(name="no-op", value={}),
-            enhanced_download_archive=self._enhanced_download_archive,
+            enhanced_download_archive=self.download_archive,
             download_ytdl_options=YTDLOptionsBuilder(),
             metadata_ytdl_options=YTDLOptionsBuilder(),
             overrides=self.overrides,
         )
 
         return self._process_subscription(
             plugins=plugins,
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription_validators.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def _indent_overrides_dict(self) -> Dict[str, str]:
         """
         Returns
         -------
         indent overrides to merge with the preset dict's overrides
         """
         return {
-            SubscriptionVariables.subscription_indent_i(i): self._indent_overrides[i]
+            SubscriptionVariables.subscription_indent_i(i).variable_name: self._indent_overrides[i]
             for i in range(len(self._indent_overrides))
         }
 
     @abstractmethod
     def subscription_dicts(self, global_presets_to_apply: List[str]) -> Dict[str, Dict]:
         """
         Parameters
@@ -139,15 +139,17 @@
             name=name,
             value=value,
             subscription_name=subscription_name,
             config=config,
             presets=presets,
             indent_overrides=indent_overrides,
         )
-        self._overrides_to_add[SubscriptionVariables.subscription_value()] = self.value
+        self._overrides_to_add[
+            SubscriptionVariables.subscription_value().variable_name
+        ] = self.value
 
 
 class SubscriptionListValuesValidator(SubscriptionLeafValidator, StringListValidator):
     def __init__(
         self,
         name,
         value,
@@ -165,19 +167,19 @@
             indent_overrides=indent_overrides,
         )
 
         for idx, list_value in enumerate(self.list):
             # Write the first list value into subscription_value as well
             if idx == 0:
                 self._overrides_to_add[
-                    SubscriptionVariables.subscription_value()
+                    SubscriptionVariables.subscription_value().variable_name
                 ] = list_value.value
 
             self._overrides_to_add[
-                SubscriptionVariables.subscription_value_i(index=idx)
+                SubscriptionVariables.subscription_value_i(index=idx).variable_name
             ] = list_value.value
 
 
 class SubscriptionWithOverridesValidator(SubscriptionLeafValidator, DictFormatterValidator):
     def __init__(
         self,
         name,
@@ -213,17 +215,17 @@
             name=name,
             value=value,
             subscription_name=subscription_name,
             config=config,
             presets=presets,
             indent_overrides=indent_overrides,
         )
-        self._overrides_to_add[SubscriptionVariables.subscription_map()] = ScriptUtils.to_script(
-            self.dict
-        )
+        self._overrides_to_add[
+            SubscriptionVariables.subscription_map().variable_name
+        ] = ScriptUtils.to_script(self.dict)
 
 
 class SubscriptionValidator(SubscriptionOutput):
     """
     Top-level subscription validator
     """
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/file_path.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_path.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/script.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/script.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/scriptable.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/scriptable.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 from typing import Optional
 from typing import Set
 
 from ytdl_sub.entries.script.function_scripts import CUSTOM_FUNCTION_SCRIPTS
 from ytdl_sub.entries.script.variable_definitions import UNRESOLVED_VARIABLES
 from ytdl_sub.entries.script.variable_definitions import VARIABLE_SCRIPTS
 from ytdl_sub.entries.script.variable_types import Variable
+from ytdl_sub.entries.variables.override_variables import REQUIRED_OVERRIDE_VARIABLE_DEFINITIONS
 from ytdl_sub.script.script import Script
 from ytdl_sub.script.utils.exceptions import RuntimeException
 from ytdl_sub.utils.exceptions import StringFormattingException
 from ytdl_sub.utils.script import ScriptUtils
 
 BASE_SCRIPT: Script = Script(
-    dict(ScriptUtils.add_sanitized_variables(VARIABLE_SCRIPTS), **CUSTOM_FUNCTION_SCRIPTS)
+    ScriptUtils.add_sanitized_variables(VARIABLE_SCRIPTS)
+    | ScriptUtils.add_sanitized_variables(REQUIRED_OVERRIDE_VARIABLE_DEFINITIONS)
+    | CUSTOM_FUNCTION_SCRIPTS
 )
 
 
 class Scriptable(ABC):
     """
     Shared class between Entry and Overrides to manage their underlying Script.
     """
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2024.3.31
+Version: 2024.4.1
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2024.3.31/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 src/ytdl_sub/plugins/internal/view.py
 src/ytdl_sub/prebuilt_presets/__init__.py
 src/ytdl_sub/prebuilt_presets/helpers/__init__.py
 src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
 src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
 src/ytdl_sub/prebuilt_presets/helpers/players.yaml
 src/ytdl_sub/prebuilt_presets/helpers/url.yaml
+src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
 src/ytdl_sub/prebuilt_presets/internal/__init__.py
 src/ytdl_sub/prebuilt_presets/internal/view.yaml
 src/ytdl_sub/prebuilt_presets/music/__init__.py
 src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
 src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
 src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
 src/ytdl_sub/prebuilt_presets/music/singles.yaml
```

