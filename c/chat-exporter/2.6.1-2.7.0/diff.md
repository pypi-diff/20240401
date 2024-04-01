# Comparing `tmp/chat_exporter-2.6.1.tar.gz` & `tmp/chat_exporter-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_exporter-2.6.1.tar", last modified: Tue Jul 11 20:52:24 2023, max compression
+gzip compressed data, was "chat_exporter-2.7.0.tar", last modified: Mon Apr  1 12:46:19 2024, max compression
```

## Comparing `chat_exporter-2.6.1.tar` & `chat_exporter-2.7.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.872674 chat_exporter-2.6.1/
--rw-rw-rw-   0        0        0    35803 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/LICENSE
--rw-rw-rw-   0        0        0       79 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11902 2023-07-11 20:52:24.871673 chat_exporter-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    10649 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.797063 chat_exporter-2.6.1/chat_exporter/
--rw-rw-rw-   0        0        0      212 2023-07-11 20:50:45.000000 chat_exporter-2.6.1/chat_exporter/__init__.py
--rw-rw-rw-   0        0        0     5862 2023-05-13 17:51:37.000000 chat_exporter-2.6.1/chat_exporter/chat_exporter.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.814084 chat_exporter-2.6.1/chat_exporter/construct/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.832591 chat_exporter-2.6.1/chat_exporter/construct/assets/
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-05-13 16:20:32.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/attachment.py
--rw-rw-rw-   0        0        0     3939 2023-01-09 20:42:18.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/component.py
--rw-rw-rw-   0        0        0     6239 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/embed.py
--rw-rw-rw-   0        0        0     1544 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/reaction.py
--rw-rw-rw-   0        0        0    20123 2023-07-11 20:45:29.000000 chat_exporter-2.6.1/chat_exporter/construct/message.py
--rw-rw-rw-   0        0        0     6837 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/construct/transcript.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.840812 chat_exporter-2.6.1/chat_exporter/ext/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/ext/__init__.py
--rw-rw-rw-   0        0        0     1285 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/ext/cache.py
--rw-rw-rw-   0        0        0      225 2023-07-11 18:47:19.000000 chat_exporter-2.6.1/chat_exporter/ext/discord_import.py
--rw-rw-rw-   0        0        0     2123 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/discord_utils.py
--rw-rw-rw-   0        0        0      146 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/discriminator.py
--rw-rw-rw-   0        0        0     4214 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/emoji_convert.py
--rw-rw-rw-   0        0        0     4304 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/html_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.841812 chat_exporter-2.6.1/chat_exporter/html/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.845322 chat_exporter-2.6.1/chat_exporter/html/attachment/
--rw-rw-rw-   0        0        0      774 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/audio.html
--rw-rw-rw-   0        0        0      140 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/image.html
--rw-rw-rw-   0        0        0      547 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/message.html
--rw-rw-rw-   0        0        0      127 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/video.html
--rw-rw-rw-   0        0        0    44009 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/base.html
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.848322 chat_exporter-2.6.1/chat_exporter/html/component/
--rw-rw-rw-   0        0        0      229 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_button.html
--rw-rw-rw-   0        0        0      254 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_menu.html
--rw-rw-rw-   0        0        0      159 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_menu_options.html
--rw-rw-rw-   0        0        0      508 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_menu_options_emoji.html
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.856108 chat_exporter-2.6.1/chat_exporter/html/embed/
--rw-rw-rw-   0        0        0      123 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/author.html
--rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/author_icon.html
--rw-rw-rw-   0        0        0      667 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/body.html
--rw-rw-rw-   0        0        0      116 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/description.html
--rw-rw-rw-   0        0        0      317 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/field-inline.html
--rw-rw-rw-   0        0        0      306 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/field.html
--rw-rw-rw-   0        0        0      113 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/footer.html
--rw-rw-rw-   0        0        0      183 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/footer_image.html
--rw-rw-rw-   0        0        0      186 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/image.html
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/thumbnail.html
--rw-rw-rw-   0        0        0       97 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/title.html
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.865616 chat_exporter-2.6.1/chat_exporter/html/message/
--rw-rw-rw-   0        0        0      239 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/bot-tag-verified.html
--rw-rw-rw-   0        0        0       43 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/bot-tag.html
--rw-rw-rw-   0        0        0       77 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/content.html
--rw-rw-rw-   0        0        0        6 2023-06-24 11:50:24.000000 chat_exporter-2.6.1/chat_exporter/html/message/end.html
--rw-rw-rw-   0        0        0      507 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/interaction.html
--rw-rw-rw-   0        0        0      961 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/message.html
--rw-rw-rw-   0        0        0     1108 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/meta.html
--rw-rw-rw-   0        0        0     1000 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/pin.html
--rw-rw-rw-   0        0        0      550 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/reference.html
--rw-rw-rw-   0        0        0      131 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/reference_unknown.html
--rw-rw-rw-   0        0        0     1254 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/start.html
--rw-rw-rw-   0        0        0      895 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/thread.html
--rw-rw-rw-   0        0        0      968 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/thread_add.html
--rw-rw-rw-   0        0        0      972 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/thread_remove.html
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.866616 chat_exporter-2.6.1/chat_exporter/html/reaction/
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/reaction/custom_emoji.html
--rw-rw-rw-   0        0        0      120 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/reaction/emoji.html
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.869668 chat_exporter-2.6.1/chat_exporter/html/script/
--rw-rw-rw-   0        0        0      112 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/script/channel_subject.html
--rw-rw-rw-   0        0        0       59 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/script/channel_topic.html
--rw-rw-rw-   0        0        0     1183 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/script/fancy_time.html
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.870674 chat_exporter-2.6.1/chat_exporter/parse/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/parse/__init__.py
--rw-rw-rw-   0        0        0    16229 2023-07-11 20:50:45.000000 chat_exporter-2.6.1/chat_exporter/parse/markdown.py
--rw-rw-rw-   0        0        0     6799 2023-07-11 20:44:33.000000 chat_exporter-2.6.1/chat_exporter/parse/mention.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.812080 chat_exporter-2.6.1/chat_exporter.egg-info/
--rw-rw-rw-   0        0        0    11902 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2610 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1348 2023-07-11 20:50:45.000000 chat_exporter-2.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 20:52:24.872674 chat_exporter-2.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.215108 chat_exporter-2.7.0/
+-rw-rw-rw-   0        0        0    35803 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0       79 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18346 2024-04-01 12:46:19.215108 chat_exporter-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17001 2024-04-01 12:43:15.000000 chat_exporter-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.159675 chat_exporter-2.7.0/chat_exporter/
+-rw-rw-rw-   0        0        0      446 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/__init__.py
+-rw-rw-rw-   0        0        0     6433 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/chat_exporter.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.174205 chat_exporter-2.7.0/chat_exporter/construct/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.178502 chat_exporter-2.7.0/chat_exporter/construct/assets/
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/construct/assets/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-05-13 16:20:32.000000 chat_exporter-2.7.0/chat_exporter/construct/assets/attachment.py
+-rw-rw-rw-   0        0        0     3939 2023-01-09 20:42:18.000000 chat_exporter-2.7.0/chat_exporter/construct/assets/component.py
+-rw-rw-rw-   0        0        0     6239 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/construct/assets/embed.py
+-rw-rw-rw-   0        0        0     1544 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/construct/assets/reaction.py
+-rw-rw-rw-   0        0        0     2426 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/construct/attachment_handler.py
+-rw-rw-rw-   0        0        0    20717 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/construct/message.py
+-rw-rw-rw-   0        0        0     7060 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/construct/transcript.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.182502 chat_exporter-2.7.0/chat_exporter/ext/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/ext/__init__.py
+-rw-rw-rw-   0        0        0     1693 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/ext/cache.py
+-rw-rw-rw-   0        0        0      225 2023-07-11 18:47:19.000000 chat_exporter-2.7.0/chat_exporter/ext/discord_import.py
+-rw-rw-rw-   0        0        0     2123 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/ext/discord_utils.py
+-rw-rw-rw-   0        0        0      146 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/ext/discriminator.py
+-rw-rw-rw-   0        0        0     4214 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/ext/emoji_convert.py
+-rw-rw-rw-   0        0        0     4304 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/ext/html_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.184006 chat_exporter-2.7.0/chat_exporter/html/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.187523 chat_exporter-2.7.0/chat_exporter/html/attachment/
+-rw-rw-rw-   0        0        0      774 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/attachment/audio.html
+-rw-rw-rw-   0        0        0      140 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/attachment/image.html
+-rw-rw-rw-   0        0        0      547 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/attachment/message.html
+-rw-rw-rw-   0        0        0      127 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/attachment/video.html
+-rw-rw-rw-   0        0        0    44049 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/html/base.html
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.190523 chat_exporter-2.7.0/chat_exporter/html/component/
+-rw-rw-rw-   0        0        0      229 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/component/component_button.html
+-rw-rw-rw-   0        0        0      254 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/component/component_menu.html
+-rw-rw-rw-   0        0        0      159 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/component/component_menu_options.html
+-rw-rw-rw-   0        0        0      508 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/component/component_menu_options_emoji.html
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.197564 chat_exporter-2.7.0/chat_exporter/html/embed/
+-rw-rw-rw-   0        0        0      123 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/author.html
+-rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/author_icon.html
+-rw-rw-rw-   0        0        0      667 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/body.html
+-rw-rw-rw-   0        0        0      116 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/description.html
+-rw-rw-rw-   0        0        0      317 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/field-inline.html
+-rw-rw-rw-   0        0        0      306 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/field.html
+-rw-rw-rw-   0        0        0      113 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/footer.html
+-rw-rw-rw-   0        0        0      183 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/footer_image.html
+-rw-rw-rw-   0        0        0      186 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/image.html
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/thumbnail.html
+-rw-rw-rw-   0        0        0       97 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/embed/title.html
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.207595 chat_exporter-2.7.0/chat_exporter/html/message/
+-rw-rw-rw-   0        0        0      239 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/bot-tag-verified.html
+-rw-rw-rw-   0        0        0       43 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/bot-tag.html
+-rw-rw-rw-   0        0        0       77 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/content.html
+-rw-rw-rw-   0        0        0        6 2023-06-24 11:50:24.000000 chat_exporter-2.7.0/chat_exporter/html/message/end.html
+-rw-rw-rw-   0        0        0      507 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/html/message/interaction.html
+-rw-rw-rw-   0        0        0      961 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/html/message/message.html
+-rw-rw-rw-   0        0        0     1108 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/meta.html
+-rw-rw-rw-   0        0        0      994 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/html/message/pin.html
+-rw-rw-rw-   0        0        0      550 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/html/message/reference.html
+-rw-rw-rw-   0        0        0      131 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/reference_unknown.html
+-rw-rw-rw-   0        0        0     1254 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/start.html
+-rw-rw-rw-   0        0        0      895 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/message/thread.html
+-rw-rw-rw-   0        0        0      968 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/html/message/thread_add.html
+-rw-rw-rw-   0        0        0      972 2023-07-11 19:11:19.000000 chat_exporter-2.7.0/chat_exporter/html/message/thread_remove.html
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.209589 chat_exporter-2.7.0/chat_exporter/html/reaction/
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/reaction/custom_emoji.html
+-rw-rw-rw-   0        0        0      120 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/reaction/emoji.html
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.211595 chat_exporter-2.7.0/chat_exporter/html/script/
+-rw-rw-rw-   0        0        0      112 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/script/channel_subject.html
+-rw-rw-rw-   0        0        0       59 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/script/channel_topic.html
+-rw-rw-rw-   0        0        0     1183 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/html/script/fancy_time.html
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.212596 chat_exporter-2.7.0/chat_exporter/parse/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.7.0/chat_exporter/parse/__init__.py
+-rw-rw-rw-   0        0        0    17168 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/parse/markdown.py
+-rw-rw-rw-   0        0        0     8801 2024-02-26 18:17:36.000000 chat_exporter-2.7.0/chat_exporter/parse/mention.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:46:19.214098 chat_exporter-2.7.0/chat_exporter.egg-info/
+-rw-rw-rw-   0        0        0    18346 2024-04-01 12:46:19.000000 chat_exporter-2.7.0/chat_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2656 2024-04-01 12:46:19.000000 chat_exporter-2.7.0/chat_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:46:19.000000 chat_exporter-2.7.0/chat_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-01 12:46:19.000000 chat_exporter-2.7.0/chat_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-01 12:46:19.000000 chat_exporter-2.7.0/chat_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1348 2024-04-01 12:44:07.000000 chat_exporter-2.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:46:19.215108 chat_exporter-2.7.0/setup.cfg
```

### Comparing `chat_exporter-2.6.1/LICENSE` & `chat_exporter-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/README.md` & `chat_exporter-2.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -90,21 +90,22 @@
 This would be the main function to use within chat-exporter.
 
 **Required Argument(s):**<br/>
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel you gather.
 
 **Optional Argument(s):**<br/>
 `limit`: Integer value to set the limit (amount of messages) the chat exporter gathers when grabbing the history (default=unlimited).<br/>
-`tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List) to set a custom timezone for the exported messages (default=UTC)<br/>
-`guild`: `discord.Guild` object which can be passed in to solve bugs for certain forks<br/>
-`military_time`: Boolean value to set a 24h format for times within your exported chat (default=False | 12h format)<br/>
-`fancy_times`: Boolean value which toggles the 'fancy times' (Today|Yesterday|Day)<br/>
-`before`: `datetime.datetime` object which allows to gather messages from before a certain date
-`after`: `datetime.datetime` object which allows to gather messages from after a certain date
-`bot`: `commands.Bot` object to gather members who are no longer in your guild.
+`tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List) to set a custom timezone for the exported messages (default=UTC).<br/>
+`guild`: `discord.Guild` object which can be passed in to solve bugs for certain forks.<br/>
+`military_time`: Boolean value to set a 24h format for times within your exported chat (default=False | 12h format).<br/>
+`fancy_times`: Boolean value which toggles the 'fancy times' (Today|Yesterday|Day).<br/>
+`before`: `datetime.datetime` object which allows to gather messages from before a certain date.<br/>
+`after`: `datetime.datetime` object which allows to gather messages from after a certain date.<br/>
+`bot`: `commands.Bot` object to gather members who are no longer in your guild.<br/>
+`attachment_handler`: `chat_exporter.AttachmentHandler` object to export assets to in order to make them available after the `channel` got deleted.<br/>
 
 **Return Argument:**<br/>
 `transcript`: The HTML build-up for you to construct the HTML File with Discord.
 
 **Example:**
 ```python
 import io
@@ -145,14 +146,15 @@
 `messages`: A list of Message objects which you wish to export to an HTML file.
 
 **Optional Argument(s):**<br/>
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List) to set a custom timezone for the exported messages (default=UTC)<br/>
 `military_time`: Boolean value to set a 24h format for times within your exported chat (default=False | 12h format)<br/>
 `fancy_times`: Boolean value which toggles the 'fancy times' (Today|Yesterday|Day)<br/>
 `bot`: `commands.Bot` object to gather members who are no longer in your guild.
+`attachment_handler`: `chat_exporter.AttachmentHandler` object to export assets to in order to make them available after the `channel` got deleted.<br/>
 
 **Return Argument:**<br/>
 `transcript`: The HTML build-up for you to construct the HTML File with Discord.
 
 **Example:**
 ```python
 import io
@@ -179,14 +181,186 @@
         filename=f"transcript-{ctx.channel.name}.html",
     )
 
     await ctx.send(file=transcript_file)
 ```
 </details>
 
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+---
+## Attachment Handler
+
+Due to Discords newly introduced restrictions on to their CDN, we have introduced an Attachment Handler. This handler
+will assist you with circumventing the 'broken' and 'dead-assets' which arise when former attachments hosted by Discord
+reach their expiration date.
+
+The `AttachmentHandler` serves as a template for you to implement your own asset handler. Below are two basic examples on
+how to use the `AttachmentHandler`. One using the example of storing files on a local webserver, with the other being
+an example of storing them on Discord *(the latter merely just being an example, this will still obviously run in to
+the expiration issue)*.
+
+If you do not specify an attachment handler, chat-exporter will continue to use the (proxy) URLs for the assets.
+
+<details><summary><b>Concept</b></summary>
+
+The concept of implementing such an AttachmentHandler is very easy. In the following a short general procedure is 
+described to write your own AttachmentHandler fitting your storage solution. Here we will assume, that we store the 
+attachments in a cloud storage.
+
+1. Subclassing
+Start by subclassing `chat_exporter.AttachmentHandler` and implement the `__init__` method if needed. This should look 
+something like this:
+
+```python
+from chat_exporter import AttachmentHandler
+from cloud_wrapper import CloudClient
+
+
+class MyAttachmentHandler(AttachmentHandler):
+    def __init__(self, *args, **kwargs):
+        # Your initialization code here
+        # in your case we just create the cloud client
+        self.cloud_client = CloudClient()
+
+```
+
+2. Overwrite process_asset
+The `process_asset` method is the method that is called for each asset in the chat. Here we have to implement the 
+upload logic and the generation of the asset url from the uploaded asset.
+    
+```python
+import io
+import aiohttp
+from chat_exporter import AttachmentHandler
+from cloud_wrapper import CloudClient
+from discord import Attachment
+
+
+class MyAttachmentHandler(AttachmentHandler):
+    async def process_asset(self, attachment: Attachment):
+        # Your upload logic here, in our example we just upload the asset to the cloud
+        
+        # first we need to authorize the client
+        await self.cloud_client.authorize()
+        
+        # then we fetch the content of the attachment
+        async with aiohttp.ClientSession() as session:
+            async with session.get(attachment.url) as res:
+                if res.status != 200:
+                    res.raise_for_status()
+                data = io.BytesIO(await res.read())
+        data.seek(0)
+        
+        # and upload it to the cloud, back we get some sort of identifier for the uploaded file
+        asset_id = await self.cloud_client.upload(data)
+        
+        # now we can generate the asset url from the identifier
+        asset_url = await self.cloud_client.get_share_url(asset_id, shared_with="everyone")
+        
+        # and set the url attribute of the attachment to the generated url
+        attachment.url = asset_url
+        return attachment
+
+```
+
+Note
+1. The `process_asset` method should return the attachment object with the url attribute set to the generated url.
+2. The `process_asset` method should be an async method, as it is likely that you have to do some async operations 
+   like fetching the content of the attachment or uploading it to the cloud.
+3. You are free to add other methods in your class, and call them from `process_asset` if you need to do some 
+   operations before or after the upload of the asset. But the `process_asset` method is the only method that is 
+called from chat-exporter.
+
+</details>
+
+**Examples:**
+
+<ol>
+<details><summary>AttachmentToLocalFileHostHandler</summary>
+
+Assuming you have a file server running, which serves the content of the folder `/usr/share/assets/` 
+under `https://example.com/assets/`, you can easily use the `AttachmentToLocalFileHostHandler` like this:
+```python
+import io
+import discord
+from discord.ext import commands
+import chat_exporter
+from chat_exporter import AttachmentToLocalFileHostHandler
+
+...
+
+# Establish the file handler
+file_handler = AttachmentToLocalFileHostHandler(
+    base_path="/usr/share/assets",
+    url_base="https://example.com/assets/",
+)
+
+@bot.command()
+async def save(ctx: commands.Context):
+    transcript = await chat_exporter.export(
+        ctx.channel,
+        attachment_handler=file_handler,
+    )
+
+    if transcript is None:
+        return
+
+    transcript_file = discord.File(
+        io.BytesIO(transcript.encode()),
+        filename=f"transcript-{ctx.channel.name}.html",
+    )
+
+    await ctx.send(file=transcript_file)
+
+```
+</details>
+
+<details><summary>AttachmentToDiscordChannel</summary>
+
+Assuming you want to store your attachments in a discord channel, you can use the `AttachmentToDiscordChannel`. 
+Please note that discord recent changes regarding content links will result in the attachments links being broken 
+after 24 hours. While this is therefor not a recommended way to store your attachments, it should give you a good 
+idea how to perform asynchronous storing of the attachments.
+
+```python
+import io
+import discord
+from discord.ext import commands
+import chat_exporter
+from chat_exporter import AttachmentToDiscordChannel
+
+...
+
+# Establish the file handler
+channel_handler = AttachmentToDiscordChannel(
+    channel=bot.get_channel(CHANNEL_ID),
+)
+
+@bot.command()
+async def save(ctx: commands.Context):
+    transcript = await chat_exporter.export(
+        ctx.channel,
+        attachment_handler=channel_handler,
+    )
+
+    if transcript is None:
+        return
+
+    transcript_file = discord.File(
+        io.BytesIO(transcript.encode()),
+        filename=f"transcript-{ctx.channel.name}.html",
+    )
+
+    await ctx.send(file=transcript_file)
+
+```
+</details>
+</ol>
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ---
 ## Screenshots
 
 <details><summary><b>General</b></summary>
 <ol>
@@ -200,14 +374,15 @@
 </details>
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 
 ---
 ## Additional Functions
 
+
 <details><summary><b>Link Function</b></summary>
 Downloading exported chats can build up a bunch of unwanted files on your PC which can get annoying, additionally - not everyone wants to download content from Discord.
 
 Due to these pain, and many requests - I have built a fancy PHP script which will show the transcript file within a browser.<br/>
 <ol>
 <details><summary>quick_link</summary>
 Similar in design to `.quick_export()` this is a bit of a demo function to produce a link and to give you an embed.
@@ -270,14 +445,16 @@
 </ol>
 
 _Please note that the PHP script does NOT store any information.<br/>
 It simply makes a request to the given URL and echos (prints) the content for you to be able to view it._
 
 </details>
 
+
+
 ---
 ## Attributions
 
 *This project borrows CSS and HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/) repository.*
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -37,25 +37,29 @@
 exporter. **Required Argument(s):**
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel
 you gather. **Optional Argument(s):**
 `limit`: Integer value to set the limit (amount of messages) the chat exporter
 gathers when grabbing the history (default=unlimited).
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/
 List_of_tz_database_time_zones#List) to set a custom timezone for the exported
-messages (default=UTC)
+messages (default=UTC).
 `guild`: `discord.Guild` object which can be passed in to solve bugs for
-certain forks
+certain forks.
 `military_time`: Boolean value to set a 24h format for times within your
-exported chat (default=False | 12h format)
+exported chat (default=False | 12h format).
 `fancy_times`: Boolean value which toggles the 'fancy times'
-(Today|Yesterday|Day)
+(Today|Yesterday|Day).
 `before`: `datetime.datetime` object which allows to gather messages from
-before a certain date `after`: `datetime.datetime` object which allows to
-gather messages from after a certain date `bot`: `commands.Bot` object to
-gather members who are no longer in your guild. **Return Argument:**
+before a certain date.
+`after`: `datetime.datetime` object which allows to gather messages from after
+a certain date.
+`bot`: `commands.Bot` object to gather members who are no longer in your guild.
+`attachment_handler`: `chat_exporter.AttachmentHandler` object to export assets
+to in order to make them available after the `channel` got deleted.
+**Return Argument:**
 `transcript`: The HTML build-up for you to construct the HTML File with
 Discord. **Example:** ```python import io ... @bot.command() async def save
 (ctx: commands.Context, limit: int = 100, tz_info: str = "UTC", military_time:
 bool = True): transcript = await chat_exporter.export( ctx.channel,
 limit=limit, tz_info=tz_info, military_time=military_time, bot=bot, ) if
 transcript is None: return transcript_file = discord.File( io.BytesIO
 (transcript.encode()), filename=f"transcript-{ctx.channel.name}.html", ) await
@@ -73,25 +77,100 @@
 List_of_tz_database_time_zones#List) to set a custom timezone for the exported
 messages (default=UTC)
 `military_time`: Boolean value to set a 24h format for times within your
 exported chat (default=False | 12h format)
 `fancy_times`: Boolean value which toggles the 'fancy times'
 (Today|Yesterday|Day)
 `bot`: `commands.Bot` object to gather members who are no longer in your guild.
+`attachment_handler`: `chat_exporter.AttachmentHandler` object to export assets
+to in order to make them available after the `channel` got deleted.
 **Return Argument:**
 `transcript`: The HTML build-up for you to construct the HTML File with
 Discord. **Example:** ```python import io ... @bot.command() async def purge
 (ctx: commands.Context, tz_info: str, military_time: bool): deleted_messages =
 await ctx.channel.purge() transcript = await chat_exporter.raw_export
 ( ctx.channel, messages=deleted_messages, tz_info=tz_info,
 military_time=military_time, bot=bot, ) if transcript is None: return
 transcript_file = discord.File( io.BytesIO(transcript.encode()),
 filename=f"transcript-{ctx.channel.name}.html", ) await ctx.send
 (file=transcript_file) ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
+--- ## Attachment Handler Due to Discords newly introduced restrictions on to
+their CDN, we have introduced an Attachment Handler. This handler will assist
+you with circumventing the 'broken' and 'dead-assets' which arise when former
+attachments hosted by Discord reach their expiration date. The
+`AttachmentHandler` serves as a template for you to implement your own asset
+handler. Below are two basic examples on how to use the `AttachmentHandler`.
+One using the example of storing files on a local webserver, with the other
+being an example of storing them on Discord *(the latter merely just being an
+example, this will still obviously run in to the expiration issue)*. If you do
+not specify an attachment handler, chat-exporter will continue to use the
+(proxy) URLs for the assets. CCoonncceepptt The concept of implementing such an
+AttachmentHandler is very easy. In the following a short general procedure is
+described to write your own AttachmentHandler fitting your storage solution.
+Here we will assume, that we store the attachments in a cloud storage. 1.
+Subclassing Start by subclassing `chat_exporter.AttachmentHandler` and
+implement the `__init__` method if needed. This should look something like
+this: ```python from chat_exporter import AttachmentHandler from cloud_wrapper
+import CloudClient class MyAttachmentHandler(AttachmentHandler): def __init__
+(self, *args, **kwargs): # Your initialization code here # in your case we just
+create the cloud client self.cloud_client = CloudClient() ``` 2. Overwrite
+process_asset The `process_asset` method is the method that is called for each
+asset in the chat. Here we have to implement the upload logic and the
+generation of the asset url from the uploaded asset. ```python import io import
+aiohttp from chat_exporter import AttachmentHandler from cloud_wrapper import
+CloudClient from discord import Attachment class MyAttachmentHandler
+(AttachmentHandler): async def process_asset(self, attachment: Attachment): #
+Your upload logic here, in our example we just upload the asset to the cloud #
+first we need to authorize the client await self.cloud_client.authorize() #
+then we fetch the content of the attachment async with aiohttp.ClientSession()
+as session: async with session.get(attachment.url) as res: if res.status !=
+200: res.raise_for_status() data = io.BytesIO(await res.read()) data.seek(0) #
+and upload it to the cloud, back we get some sort of identifier for the
+uploaded file asset_id = await self.cloud_client.upload(data) # now we can
+generate the asset url from the identifier asset_url = await
+self.cloud_client.get_share_url(asset_id, shared_with="everyone") # and set the
+url attribute of the attachment to the generated url attachment.url = asset_url
+return attachment ``` Note 1. The `process_asset` method should return the
+attachment object with the url attribute set to the generated url. 2. The
+`process_asset` method should be an async method, as it is likely that you have
+to do some async operations like fetching the content of the attachment or
+uploading it to the cloud. 3. You are free to add other methods in your class,
+and call them from `process_asset` if you need to do some operations before or
+after the upload of the asset. But the `process_asset` method is the only
+method that is called from chat-exporter. **Examples:**
+   1. AttachmentToLocalFileHostHandler Assuming you have a file server running,
+      which serves the content of the folder `/usr/share/assets/` under `https:
+      //example.com/assets/`, you can easily use the
+      `AttachmentToLocalFileHostHandler` like this: ```python import io import
+      discord from discord.ext import commands import chat_exporter from
+      chat_exporter import AttachmentToLocalFileHostHandler ... # Establish the
+      file handler file_handler = AttachmentToLocalFileHostHandler
+      ( base_path="/usr/share/assets", url_base="https://example.com/assets/",
+      ) @bot.command() async def save(ctx: commands.Context): transcript =
+      await chat_exporter.export( ctx.channel, attachment_handler=file_handler,
+      ) if transcript is None: return transcript_file = discord.File
+      ( io.BytesIO(transcript.encode()), filename=f"transcript-
+      {ctx.channel.name}.html", ) await ctx.send(file=transcript_file) ```
+      AttachmentToDiscordChannel Assuming you want to store your attachments in
+      a discord channel, you can use the `AttachmentToDiscordChannel`. Please
+      note that discord recent changes regarding content links will result in
+      the attachments links being broken after 24 hours. While this is therefor
+      not a recommended way to store your attachments, it should give you a
+      good idea how to perform asynchronous storing of the attachments.
+      ```python import io import discord from discord.ext import commands
+      import chat_exporter from chat_exporter import AttachmentToDiscordChannel
+      ... # Establish the file handler channel_handler =
+      AttachmentToDiscordChannel( channel=bot.get_channel(CHANNEL_ID), )
+      @bot.command() async def save(ctx: commands.Context): transcript = await
+      chat_exporter.export( ctx.channel, attachment_handler=channel_handler, )
+      if transcript is None: return transcript_file = discord.File( io.BytesIO
+      (transcript.encode()), filename=f"transcript-{ctx.channel.name}.html", )
+      await ctx.send(file=transcript_file) ```
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 --- ## Screenshots GGeenneerraall
    1. Discord [https://raw.githubusercontent.com/mahtoid/DiscordChatExporterPy/
       master/.screenshots/channel_output.png]Chat-Exporter[https://
       raw.githubusercontent.com/mahtoid/DiscordChatExporterPy/
       master/.screenshots/html_output.png]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 --- ## Additional Functions LLiinnkk FFuunnccttiioonn Downloading exported chats can build
```

### Comparing `chat_exporter-2.6.1/chat_exporter/chat_exporter.py` & `chat_exporter-2.7.0/chat_exporter/chat_exporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import io
 from typing import List, Optional
 
 from chat_exporter.construct.transcript import Transcript
 from chat_exporter.ext.discord_import import discord
+from chat_exporter.construct.attachment_handler import AttachmentHandler, AttachmentToLocalFileHostHandler, AttachmentToDiscordChannelHandler
 
 
 async def quick_export(
     channel: discord.TextChannel,
     guild: Optional[discord.Guild] = None,
     bot: Optional[discord.Client] = None,
 ):
@@ -57,27 +58,29 @@
     guild: Optional[discord.Guild] = None,
     bot: Optional[discord.Client] = None,
     military_time: Optional[bool] = True,
     fancy_times: Optional[bool] = True,
     before: Optional[datetime.datetime] = None,
     after: Optional[datetime.datetime] = None,
     support_dev: Optional[bool] = True,
+    attachment_handler: Optional[AttachmentHandler] = None,
 ):
     """
     Create a customised transcript of your Discord channel.
     This function will return the transcript which you can then turn in to a file to post wherever.
     :param channel: discord.TextChannel - channel to Export
     :param limit: (optional) integer - limit of messages to capture
     :param tz_info: (optional) TZ Database Name - set the timezone of your transcript
     :param guild: (optional) discord.Guild - solution for edpy
     :param bot: (optional) discord.Client - set getting member role colour
     :param military_time: (optional) boolean - set military time (24hour clock)
     :param fancy_times: (optional) boolean - set javascript around time display
     :param before: (optional) datetime.datetime - allows before time for history
     :param after: (optional) datetime.datetime - allows after time for history
+    :param attachment_handler: (optional) attachment_handler.AttachmentHandler - allows custom asset handling
     :return: string - transcript file make up
     """
     if guild:
         channel.guild = guild
 
     return (
         await Transcript(
@@ -87,38 +90,41 @@
             pytz_timezone=tz_info,
             military_time=military_time,
             fancy_times=fancy_times,
             before=before,
             after=after,
             support_dev=support_dev,
             bot=bot,
+            attachment_handler=attachment_handler,
         ).export()
     ).html
 
 
 async def raw_export(
     channel: discord.TextChannel,
     messages: List[discord.Message],
     tz_info="UTC",
     guild: Optional[discord.Guild] = None,
     bot: Optional[discord.Client] = None,
     military_time: Optional[bool] = False,
     fancy_times: Optional[bool] = True,
     support_dev: Optional[bool] = True,
+    attachment_handler: Optional[AttachmentHandler] = None,
 ):
     """
     Create a customised transcript with your own captured Discord messages
     This function will return the transcript which you can then turn in to a file to post wherever.
     :param channel: discord.TextChannel - channel to Export
     :param messages: List[discord.Message] - list of Discord messages to export
     :param tz_info: (optional) TZ Database Name - set the timezone of your transcript
     :param guild: (optional) discord.Guild - solution for edpy
     :param bot: (optional) discord.Client - set getting member role colour
     :param military_time: (optional) boolean - set military time (24hour clock)
     :param fancy_times: (optional) boolean - set javascript around time display
+    :param attachment_handler: (optional) AttachmentHandler - allows custom asset handling
     :return: string - transcript file make up
     """
     if guild:
         channel.guild = guild
 
     return (
         await Transcript(
@@ -128,14 +134,15 @@
             pytz_timezone=tz_info,
             military_time=military_time,
             fancy_times=fancy_times,
             before=None,
             after=None,
             support_dev=support_dev,
             bot=bot,
+            attachment_handler=attachment_handler
         ).export()
     ).html
 
 
 async def quick_link(
     channel: discord.TextChannel,
     message: discord.Message
```

### Comparing `chat_exporter-2.6.1/chat_exporter/construct/assets/attachment.py` & `chat_exporter-2.7.0/chat_exporter/construct/assets/attachment.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/construct/assets/component.py` & `chat_exporter-2.7.0/chat_exporter/construct/assets/component.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/construct/assets/embed.py` & `chat_exporter-2.7.0/chat_exporter/construct/assets/embed.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/construct/assets/reaction.py` & `chat_exporter-2.7.0/chat_exporter/construct/assets/reaction.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/construct/message.py` & `chat_exporter-2.7.0/chat_exporter/construct/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import html
+import io
+import traceback
 from typing import List, Optional, Union
 
+import aiohttp
 from pytz import timezone
 from datetime import timedelta
 
+from chat_exporter.construct.attachment_handler import AttachmentHandler
 from chat_exporter.ext.discord_import import discord
 
 from chat_exporter.construct.assets import Attachment, Component, Embed, Reaction
 from chat_exporter.ext.discord_utils import DiscordUtils
 from chat_exporter.ext.discriminator import discriminator
+from chat_exporter.ext.cache import cache
 from chat_exporter.ext.html_generator import (
     fill_out,
     bot_tag,
     bot_tag_verified,
     message_body,
     message_pin,
     message_thread,
@@ -57,23 +62,24 @@
         self,
         message: discord.Message,
         previous_message: Optional[discord.Message],
         pytz_timezone,
         military_time: bool,
         guild: discord.Guild,
         meta_data: dict,
-        message_dict: dict
+        message_dict: dict,
+        attachment_handler: Optional[AttachmentHandler]
     ):
         self.message = message
         self.previous_message = previous_message
         self.pytz_timezone = pytz_timezone
         self.military_time = military_time
         self.guild = guild
         self.message_dict = message_dict
-
+        self.attachment_handler = attachment_handler
         self.time_format = "%A, %e %B %Y %I:%M %p"
         if self.military_time:
             self.time_format = "%A, %e %B %Y %H:%M"
 
         self.message_created_at, self.message_edited_at = self.set_time()
         self.meta_data = meta_data
 
@@ -242,14 +248,16 @@
         ])
 
     async def build_assets(self):
         for e in self.message.embeds:
             self.embeds += await Embed(e, self.guild).flow()
 
         for a in self.message.attachments:
+            if self.attachment_handler and isinstance(self.attachment_handler, AttachmentHandler):
+                a = await self.attachment_handler.process_asset(a)
             self.attachments += await Attachment(a, self.guild).flow()
 
         for c in self.message.components:
             self.components += await Component(c, self.guild).flow()
 
         for r in self.message.reactions:
             self.reactions += await Reaction(r, self.guild).flow()
@@ -332,15 +340,15 @@
     async def build_pin_template(self):
         self.message_html += await fill_out(self.guild, message_pin, [
             ("PIN_URL", DiscordUtils.pinned_message_icon, PARSE_MODE_NONE),
             ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
             ("NAME", str(html.escape(self.message.author.display_name))),
             ("NAME_TAG", await discriminator(self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
-            ("REF_MESSAGE_ID", str(self.message.reference.message_id), PARSE_MODE_NONE)
+            ("REF_MESSAGE_ID", str(self.message.reference.message_id) if self.message.reference else "", PARSE_MODE_NONE)
         ])
 
     async def build_thread_template(self):
         self.message_html += await fill_out(self.guild, message_thread, [
             ("THREAD_URL", DiscordUtils.thread_channel_icon,
              PARSE_MODE_NONE),
             ("THREAD_NAME", self.message.content, PARSE_MODE_NONE),
@@ -378,14 +386,15 @@
             ("RECIPIENT_USER_COLOUR", await self._gather_user_colour(removed_member)),
             ("RECIPIENT_NAME", str(html.escape(removed_member.display_name))),
             ("RECIPIENT_NAME_TAG", await discriminator(removed_member.name, removed_member.discriminator),
              PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
         ])
 
+    @cache()
     async def _gather_member(self, author: discord.Member):
         member = self.guild.get_member(author.id)
 
         if member:
             return member
 
         try:
@@ -430,22 +439,23 @@
 
 
 async def gather_messages(
     messages: List[discord.Message],
     guild: discord.Guild,
     pytz_timezone,
     military_time,
+    attachment_handler: Optional[AttachmentHandler],
 ) -> (str, dict):
     message_html: str = ""
     meta_data: dict = {}
     previous_message: Optional[discord.Message] = None
 
     message_dict = {message.id: message for message in messages}
 
-    if "thread" in str(messages[0].channel.type) and messages[0].reference:
+    if messages and "thread" in str(messages[0].channel.type) and messages[0].reference:
         channel = guild.get_channel(messages[0].reference.channel_id)
 
         if not channel:
             channel = await guild.fetch_channel(messages[0].reference.channel_id)
 
         message = await channel.fetch_message(messages[0].reference.message_id)
         messages[0] = message
@@ -456,13 +466,15 @@
             message,
             previous_message,
             pytz_timezone,
             military_time,
             guild,
             meta_data,
             message_dict,
-        ).construct_message()
+            attachment_handler,
+            ).construct_message()
+
         message_html += content_html
         previous_message = message
 
     message_html += "</div>"
     return message_html, meta_data
```

### Comparing `chat_exporter-2.6.1/chat_exporter/construct/transcript.py` & `chat_exporter-2.7.0/chat_exporter/construct/transcript.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import traceback
 
 import re
 from typing import List, Optional
 
 import pytz
 
+from chat_exporter.construct.attachment_handler import AttachmentHandler
 from chat_exporter.ext.discord_import import discord
 
 from chat_exporter.construct.message import gather_messages
 from chat_exporter.construct.assets.component import Component
 
 from chat_exporter.ext.cache import clear_cache
 from chat_exporter.parse.mention import pass_bot
@@ -31,37 +32,40 @@
         pytz_timezone,
         military_time: bool,
         fancy_times: bool,
         before: Optional[datetime.datetime],
         after: Optional[datetime.datetime],
         support_dev: bool,
         bot: Optional[discord.Client],
+        attachment_handler: Optional[AttachmentHandler],
     ):
         self.channel = channel
         self.messages = messages
         self.limit = int(limit) if limit else None
         self.military_time = military_time
         self.fancy_times = fancy_times
         self.before = before
         self.after = after
         self.support_dev = support_dev
         self.pytz_timezone = pytz_timezone
+        self.attachment_handler = attachment_handler
 
         # This is to pass timezone in to mention.py without rewriting
         setattr(discord.Guild, "timezone", self.pytz_timezone)
 
         if bot:
             pass_bot(bot)
 
     async def build_transcript(self):
         message_html, meta_data = await gather_messages(
             self.messages,
             self.channel.guild,
             self.pytz_timezone,
             self.military_time,
+            self.attachment_handler
         )
         await self.export_transcript(message_html, meta_data)
         clear_cache()
         Component.menu_div_id = 0
         return self
 
     async def export_transcript(self, message_html: str, meta_data: str):
```

### Comparing `chat_exporter-2.6.1/chat_exporter/ext/cache.py` & `chat_exporter-2.7.0/chat_exporter/ext/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import wraps
+from typing import Any
 
 _internal_cache: dict = {}
 
 
 def _wrap_and_store_coroutine(cache, key, coro):
     async def func():
         value = await coro
@@ -19,21 +20,27 @@
 
 def clear_cache():
     _internal_cache.clear()
 
 
 def cache():
     def decorator(func):
-        def _make_key(args, kwargs):
-            key = [f'{func.__module__}.{func.__name__}']
-            key.extend(repr(o) for o in args)
+        def _make_key(args: tuple[Any, ...], kwargs: dict[str, Any]) -> str:
+            def _true_repr(o):
+                if o.__class__.__repr__ is object.__repr__:
+                    # this is how MessageConstruct can retain
+                    # caching across multiple instances
+                    return f'<{o.__class__.__module__}.{o.__class__.__name__}>'
+                return repr(o)
 
+            key = [f'{func.__module__}.{func.__name__}']
+            key.extend(_true_repr(o) for o in args)
             for k, v in kwargs.items():
-                key.append(repr(k))
-                key.append(repr(v))
+                key.append(_true_repr(k))
+                key.append(_true_repr(v))
 
             return ':'.join(key)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             key = _make_key(args, kwargs)
             try:
```

### Comparing `chat_exporter-2.6.1/chat_exporter/ext/discord_utils.py` & `chat_exporter-2.7.0/chat_exporter/ext/discord_utils.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/ext/emoji_convert.py` & `chat_exporter-2.7.0/chat_exporter/ext/emoji_convert.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/ext/html_generator.py` & `chat_exporter-2.7.0/chat_exporter/ext/html_generator.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/attachment/audio.html` & `chat_exporter-2.7.0/chat_exporter/html/attachment/audio.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/attachment/message.html` & `chat_exporter-2.7.0/chat_exporter/html/attachment/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/base.html` & `chat_exporter-2.7.0/chat_exporter/html/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -657,21 +657,22 @@
         .markup ul ul {
             list-style-type: circle;
             margin-bottom: 0;
         }
 
         .markup li {
             margin: 0;
-            padding: 0;
             border: 0;
             font-weight: inherit;
             font-style: inherit;
             font-family: inherit;
             font-size: 100%;
             vertical-align: baseline;
+            padding-top: 5px;
+            padding-bottom: 5px;
         }
 
 
         .meta__details .chatlog__bot-tag {
             margin-left: 1ch;
         }
```

### Comparing `chat_exporter-2.6.1/chat_exporter/html/embed/body.html` & `chat_exporter-2.7.0/chat_exporter/html/embed/body.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/message.html` & `chat_exporter-2.7.0/chat_exporter/html/message/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/meta.html` & `chat_exporter-2.7.0/chat_exporter/html/message/meta.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/pin.html` & `chat_exporter-2.7.0/chat_exporter/html/message/pin.html`

 * *Files 8% similar despite different names*

```diff
@@ -14,8 +14,7 @@
                         a message
                     </a>
                     to this channel
                 </div>
             </div>
         </div>
     </div>
-</div>
```

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/reference.html` & `chat_exporter-2.7.0/chat_exporter/html/message/reference.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/start.html` & `chat_exporter-2.7.0/chat_exporter/html/message/start.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/thread.html` & `chat_exporter-2.7.0/chat_exporter/html/message/thread.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/thread_add.html` & `chat_exporter-2.7.0/chat_exporter/html/message/thread_add.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/message/thread_remove.html` & `chat_exporter-2.7.0/chat_exporter/html/message/thread_remove.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/html/script/fancy_time.html` & `chat_exporter-2.7.0/chat_exporter/html/script/fancy_time.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.1/chat_exporter/parse/markdown.py` & `chat_exporter-2.7.0/chat_exporter/parse/markdown.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,48 +2,54 @@
 import re
 from chat_exporter.ext.emoji_convert import convert_emoji
 
 
 class ParseMarkdown:
     def __init__(self, content):
         self.content = content
+        self.code_blocks_content = []
+
 
     async def standard_message_flow(self):
+        self.parse_code_block_markdown()
         self.https_http_links()
         self.parse_normal_markdown()
-        self.parse_code_block_markdown()
-        await self.parse_emoji()
 
+        await self.parse_emoji()
+        self.reverse_code_block_markdown()
         return self.content
 
     async def link_embed_flow(self):
         self.parse_embed_markdown()
         await self.parse_emoji()
 
     async def standard_embed_flow(self):
+        self.parse_code_block_markdown()
         self.https_http_links()
         self.parse_embed_markdown()
         self.parse_normal_markdown()
-        self.parse_code_block_markdown()
-        await self.parse_emoji()
 
+        await self.parse_emoji()
+        self.reverse_code_block_markdown()
         return self.content
 
     async def special_embed_flow(self):
         self.https_http_links()
-        self.parse_normal_markdown()
         self.parse_code_block_markdown()
-        await self.parse_emoji()
+        self.parse_normal_markdown()
 
+        await self.parse_emoji()
+        self.reverse_code_block_markdown()
         return self.content
 
     async def message_reference_flow(self):
         self.strip_preserve()
-        self.parse_normal_markdown()
         self.parse_code_block_markdown(reference=True)
+        self.parse_normal_markdown()
+        self.reverse_code_block_markdown()
         self.parse_br()
 
         return self.content
 
     async def special_emoji_flow(self):
         await self.parse_emoji()
         return self.content
@@ -91,15 +97,15 @@
         for line in lines:
             match = re.match(r'^(\s*)([-*])\s+(.+)$', line)
             if match:
                 indent, bullet, content = match.groups()
                 indent = len(indent)
 
                 if started:
-                    html += '<ul class="markup">\n'
+                    html += '<ul class="markup" style="padding-left: 20px;margin: 0 !important">\n'
                     started = False
                 if indent % 2 == 0:
                     while indent < indent_stack[-1]:
                         html += '</ul>\n'
                         indent_stack.pop()
                     if indent > indent_stack[-1]:
                         html += '<ul class="markup">\n'
@@ -110,41 +116,46 @@
                         indent_stack.pop()
                     if indent + 1 > indent_stack[-1]:
                         html += '<ul class="markup">\n'
                         indent_stack.append(indent + 1)
 
                 html += f'<li class="markup">{content.strip()}</li>\n'
             else:
-                html += line
+                while len(indent_stack) > 1:
+                    html += '</ul>'
+                    indent_stack.pop()
+                if not started:
+                    html += '</ul>'
+                    started = True
+                html += line + '\n'
 
         while len(indent_stack) > 1:
             html += '</ul>\n'
             indent_stack.pop()
 
-        if not started:
-            self.content = html
+        self.content = html
 
     def parse_normal_markdown(self):
-        # self.order_list_markdown_to_html()
+        self.order_list_markdown_to_html()
         holder = (
             [r"__(.*?)__", '<span style="text-decoration: underline">%s</span>'],
             [r"\*\*(.*?)\*\*", '<strong>%s</strong>'],
             [r"\*(.*?)\*", '<em>%s</em>'],
             [r"~~(.*?)~~", '<span style="text-decoration: line-through">%s</span>'],
-            # [r"###\s(.*?)\n", '<h3>%s</h1>'],
-            # [r"##\s(.*?)\n", '<h2>%s</h1>'],
-            # [r"#\s(.*?)\n", '<h1>%s</h1>'],
+            [r"^###\s(.*?)\n", '<h3>%s</h1>'],
+            [r"^##\s(.*?)\n", '<h2>%s</h1>'],
+            [r"^#\s(.*?)\n", '<h1>%s</h1>'],
             [r"\|\|(.*?)\|\|", '<span class="spoiler spoiler--hidden" onclick="showSpoiler(event, this)"> <span '
                                'class="spoiler-text">%s</span></span>'],
         )
 
         for x in holder:
             p, r = x
 
-            pattern = re.compile(p)
+            pattern = re.compile(p, re.M)
             match = re.search(pattern, self.content)
             while match is not None:
                 affected_text = match.group(1)
                 self.content = self.content.replace(self.content[match.start():match.end()], r % affected_text)
                 match = re.search(pattern, self.content)
 
         # > quote
@@ -201,49 +212,56 @@
             second_pattern = re.compile(r"^<br>|<br>$")
             second_match = re.search(second_pattern, affected_text)
             while second_match is not None:
                 affected_text = re.sub(r"^<br>|<br>$", '', affected_text)
                 second_match = re.search(second_pattern, affected_text)
             affected_text = re.sub("  ", "&nbsp;&nbsp;", affected_text)
 
+            self.code_blocks_content.append(affected_text)
             if not reference:
                 self.content = self.content.replace(
                     self.content[match.start():match.end()],
-                    '<div class="pre pre--multiline %s">%s</div>' % (language_class, affected_text)
+                    '<div class="pre pre--multiline %s">%s</div>' % (language_class, f'%s{len(self.code_blocks_content)}')
                 )
             else:
                 self.content = self.content.replace(
                     self.content[match.start():match.end()],
-                    '<span class="pre pre-inline">%s</span>' % affected_text
+                    '<span class="pre pre-inline">%s</span>' % f'%s{len(self.code_blocks_content)}'
                 )
 
             match = re.search(pattern, self.content)
 
         # ``code``
         pattern = re.compile(r"``(.*?)``")
         match = re.search(pattern, self.content)
         while match is not None:
             affected_text = match.group(1)
             affected_text = self.return_to_markdown(affected_text)
+            self.code_blocks_content.append(affected_text)
             self.content = self.content.replace(self.content[match.start():match.end()],
-                                                '<span class="pre pre-inline">%s</span>' % affected_text)
+                                                '<span class="pre pre-inline">%s</span>' % f'%s{len(self.code_blocks_content)}')
             match = re.search(pattern, self.content)
 
         # `code`
         pattern = re.compile(r"`(.*?)`")
         match = re.search(pattern, self.content)
         while match is not None:
             affected_text = match.group(1)
             affected_text = self.return_to_markdown(affected_text)
+            self.code_blocks_content.append(affected_text)
             self.content = self.content.replace(self.content[match.start():match.end()],
-                                                '<span class="pre pre-inline">%s</span>' % affected_text)
+                                                '<span class="pre pre-inline">%s</span>' % f'%s{len(self.code_blocks_content)}')
             match = re.search(pattern, self.content)
 
         self.content = re.sub(r"<br>", "\n", self.content)
 
+    def reverse_code_block_markdown(self):
+        for x in range(len(self.code_blocks_content)):
+            self.content = self.content.replace(f'%s{x + 1}', self.code_blocks_content[x])
+
     def parse_embed_markdown(self):
         # [Message](Link)
         pattern = re.compile(r"\[(.+?)]\((.+?)\)")
         match = re.search(pattern, self.content)
         while match is not None:
             affected_text = match.group(1)
             affected_url = match.group(2)
```

### Comparing `chat_exporter-2.6.1/chat_exporter/parse/mention.py` & `chat_exporter-2.7.0/chat_exporter/parse/mention.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 import re
 from typing import Optional
 
 import pytz
 import datetime
+import time
 
 from chat_exporter.ext.discord_import import discord
-
+from chat_exporter.parse.markdown import ParseMarkdown
 bot: Optional[discord.Client] = None
 
 
 def pass_bot(_bot):
     # Bot is used to fetch a user who is no longer inside a guild
     # This will stop the user from appearing as 'Unknown' which some people do not want
     global bot
     bot = _bot
 
 
 class ParseMention:
     REGEX_ROLES = r"&lt;@&amp;([0-9]+)&gt;"
     REGEX_ROLES_2 = r"<@&([0-9]+)>"
+    REGEX_EVERYONE = r"@(everyone)(?:[$\s\t\n\f\r\0]|$)"
+    REGEX_HERE = r"@(here)(?:[$\s\t\n\f\r\0]|$)"
     REGEX_MEMBERS = r"&lt;@!?([0-9]+)&gt;"
     REGEX_MEMBERS_2 = r"<@!?([0-9]+)>"
     REGEX_CHANNELS = r"&lt;#([0-9]+)&gt;"
     REGEX_CHANNELS_2 = r"<#([0-9]+)>"
     REGEX_EMOJIS = r"&lt;a?(:[^\n:]+:)[0-9]+&gt;"
     REGEX_EMOJIS_2 = r"<a?(:[^\n:]+:)[0-9]+>"
     REGEX_TIME_HOLDER = (
-        [r"&lt;t:([0-9]+):t&gt;", "%H:%M"],
-        [r"&lt;t:([0-9]+):T&gt;", "%T"],
-        [r"&lt;t:([0-9]+):d&gt;", "%d/%m/%Y"],
-        [r"&lt;t:([0-9]+):D&gt;", "%e %B %Y"],
-        [r"&lt;t:([0-9]+):f&gt;", "%e %B %Y %H:%M"],
-        [r"&lt;t:([0-9]+):F&gt;", "%A, %e %B %Y %H:%M"],
-        [r"&lt;t:([0-9]+):R&gt;", "%e %B %Y %H:%M"],
-        [r"&lt;t:([0-9]+)&gt;", "%e %B %Y %H:%M"]
+        [r"&lt;t:([0-9]{1,13}):t&gt;", "%H:%M"],
+        [r"&lt;t:([0-9]{1,13}):T&gt;", "%T"],
+        [r"&lt;t:([0-9]{1,13}):d&gt;", "%d/%m/%Y"],
+        [r"&lt;t:([0-9]{1,13}):D&gt;", "%e %B %Y"],
+        [r"&lt;t:([0-9]{1,13}):f&gt;", "%e %B %Y %H:%M"],
+        [r"&lt;t:([0-9]{1,13}):F&gt;", "%A, %e %B %Y %H:%M"],
+        [r"&lt;t:([0-9]{1,13}):R&gt;", "%e %B %Y %H:%M"],
+        [r"&lt;t:([0-9]{1,13})&gt;", "%e %B %Y %H:%M"]
     )
+    REGEX_SLASH_COMMAND = r"&lt;\/([\w]+ ?[\w]*):[0-9]+&gt;"
 
     ESCAPE_LT = "______lt______"
     ESCAPE_GT = "______gt______"
     ESCAPE_AMP = "______amp______"
 
     def __init__(self, content, guild):
         self.content = content
         self.guild = guild
+        self.code_blocks_content = []
 
     async def flow(self):
+        markdown = ParseMarkdown(self.content)
+        markdown.parse_code_block_markdown()
+        self.content = markdown.content
         await self.escape_mentions()
         await self.escape_mentions()
         await self.unescape_mentions()
         await self.channel_mention()
         await self.member_mention()
         await self.role_mention()
         await self.time_mention()
-
+        await self.slash_command_mention()
+        markdown.content = self.content
+        markdown.reverse_code_block_markdown()
+        self.content = markdown.content
         return self.content
 
+
     async def escape_mentions(self):
         for match in re.finditer("(%s|%s|%s|%s|%s|%s|%s|%s)"
                                  % (self.REGEX_ROLES, self.REGEX_MEMBERS, self.REGEX_CHANNELS, self.REGEX_EMOJIS,
                                     self.REGEX_ROLES_2, self.REGEX_MEMBERS_2, self.REGEX_CHANNELS_2,
                                     self.REGEX_EMOJIS_2), self.content):
             pre_content = self.content[:match.start()]
             post_content = self.content[match.end():]
@@ -90,34 +102,54 @@
                     replacement = '<span class="mention" title="%s">#%s</span>' \
                                   % (channel.id, channel.name)
                 self.content = self.content.replace(self.content[match.start():match.end()], replacement)
 
                 match = re.search(regex, self.content)
 
     async def role_mention(self):
+        holder = self.REGEX_EVERYONE, self.REGEX_HERE
+        for regex in holder:
+            match = re.search(regex, self.content)
+            while match is not None:
+                role_name = match.group(1)
+                replacement = '<span class="mention" title="%s">@%s</span>' % (str(role_name), str(role_name))
+
+                self.content = self.content.replace(self.content[match.start():match.end()],
+                                                    replacement)
+                match = re.search(regex, self.content)
         holder = self.REGEX_ROLES, self.REGEX_ROLES_2
         for regex in holder:
             match = re.search(regex, self.content)
             while match is not None:
                 role_id = int(match.group(1))
                 role = self.guild.get_role(role_id)
 
                 if role is None:
                     replacement = '@deleted-role'
                 else:
                     if role.color.r == 0 and role.color.g == 0 and role.color.b == 0:
                         colour = "#dee0fc"
                     else:
                         colour = "#%02x%02x%02x" % (role.color.r, role.color.g, role.color.b)
-                    replacement = '<span style="color: %s;">@%s</span>' \
-                                  % (colour, role.name)
+                    replacement = '<span style="color: %s;">@%s</span>' % (colour, role.name)
                 self.content = self.content.replace(self.content[match.start():match.end()], replacement)
-
                 match = re.search(regex, self.content)
 
+    async def slash_command_mention(self):
+        match = re.search(self.REGEX_SLASH_COMMAND, self.content)
+        while match is not None:
+            slash_command_name = match.group(1)
+            replacement = (
+                    '<span class="mention" title="%s">/%s</span>'
+                    % (slash_command_name, slash_command_name)
+            )
+            self.content = self.content.replace(self.content[match.start():match.end()], replacement)
+
+            match = re.search(self.REGEX_SLASH_COMMAND, self.content)
+
     async def member_mention(self):
         holder = self.REGEX_MEMBERS, self.REGEX_MEMBERS_2
         for regex in holder:
             match = re.search(regex, self.content)
             while match is not None:
                 member_id = int(match.group(1))
 
@@ -146,17 +178,21 @@
         if hasattr(self.guild, "timezone"):
             timezone = pytz.timezone(self.guild.timezone)
 
         for p in holder:
             regex, strf = p
             match = re.search(regex, self.content)
             while match is not None:
-                time = datetime.datetime.fromtimestamp(int(match.group(1)), timezone)
-                ui_time = time.strftime(strf)
-                tooltip_time = time.strftime("%A, %e %B %Y at %H:%M")
+                timestamp = int(match.group(1)) - 1
+                time_stamp = time.gmtime(timestamp)
+                datetime_stamp = datetime.datetime(2010, *time_stamp[1:6], tzinfo=pytz.utc)
+                ui_time = datetime_stamp.strftime(strf)
+                ui_time = ui_time.replace(str(datetime_stamp.year), str(time_stamp[0]))
+                tooltip_time = datetime_stamp.strftime("%A, %e %B %Y at %H:%M")
+                tooltip_time = tooltip_time.replace(str(datetime_stamp.year), str(time_stamp[0]))
                 original = match.group().replace("&lt;", "<").replace("&gt;", ">")
                 replacement = (
                     f'<span class="unix-timestamp" data-timestamp="{tooltip_time}" raw-content="{original}">'
                     f'{ui_time}</span>'
                 )
 
                 self.content = self.content.replace(self.content[match.start():match.end()],
```

### Comparing `chat_exporter-2.6.1/chat_exporter.egg-info/SOURCES.txt` & `chat_exporter-2.7.0/chat_exporter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 chat_exporter/chat_exporter.py
 chat_exporter.egg-info/PKG-INFO
 chat_exporter.egg-info/SOURCES.txt
 chat_exporter.egg-info/dependency_links.txt
 chat_exporter.egg-info/requires.txt
 chat_exporter.egg-info/top_level.txt
 chat_exporter/construct/__init__.py
+chat_exporter/construct/attachment_handler.py
 chat_exporter/construct/message.py
 chat_exporter/construct/transcript.py
 chat_exporter/construct/assets/__init__.py
 chat_exporter/construct/assets/attachment.py
 chat_exporter/construct/assets/component.py
 chat_exporter/construct/assets/embed.py
 chat_exporter/construct/assets/reaction.py
```

### Comparing `chat_exporter-2.6.1/pyproject.toml` & `chat_exporter-2.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chat_exporter"
 description = "A simple Discord chat exporter for Python Discord bots."
-version = "2.6.1"
+version = "2.7.0"
 readme = "README.md"
 authors = [
     { name="mahtoid", email="info@mahto.id" }
 ]
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-only" }
 classifiers = [
```

