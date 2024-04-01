# Comparing `tmp/langserve-0.0.9.tar.gz` & `tmp/langserve-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langserve-0.0.9.tar", max compression
+gzip compressed data, was "langserve-0.1.0rc1.tar", max compression
```

## Comparing `langserve-0.0.9.tar` & `langserve-0.1.0rc1.tar`

### file list

```diff
@@ -1,10 +1,145 @@
--rw-r--r--   0        0        0     3757 2023-10-17 01:32:14.505776 langserve-0.0.9/LICENSE
--rw-r--r--   0        0        0     6661 2023-10-17 01:32:14.505776 langserve-0.0.9/README.md
--rw-r--r--   0        0        0      222 2023-10-17 01:32:14.505776 langserve-0.0.9/langserve/__init__.py
--rw-r--r--   0        0        0    16014 2023-10-17 01:32:14.505776 langserve-0.0.9/langserve/client.py
--rw-r--r--   0        0        0     3019 2023-10-17 01:32:14.505776 langserve-0.0.9/langserve/serialization.py
--rw-r--r--   0        0        0    14549 2023-10-17 01:32:14.505776 langserve-0.0.9/langserve/server.py
--rw-r--r--   0        0        0     7176 2023-10-17 01:32:14.509775 langserve-0.0.9/langserve/validation.py
--rw-r--r--   0        0        0      307 2023-10-17 01:32:14.509775 langserve-0.0.9/langserve/version.py
--rw-r--r--   0        0        0     1780 2023-10-17 01:32:14.509775 langserve-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     7601 1970-01-01 00:00:00.000000 langserve-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     3757 2024-04-01 19:51:36.072289 langserve-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0    42394 2024-04-01 19:51:36.072289 langserve-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      505 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/__init__.py
+-rw-r--r--   0        0        0    63222 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/api_handler.py
+-rw-r--r--   0        0        0    14240 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/callbacks.py
+-rw-r--r--   0        0        0      436 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/.eslintrc.cjs
+-rw-r--r--   0        0        0      266 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/.gitignore
+-rw-r--r--   0        0        0     1263 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/README.md
+-rw-r--r--   0        0        0    23810 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/dist/assets/index-434ff580.css
+-rw-r--r--   0        0        0   494586 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/dist/assets/index-86d4d9c0.js
+-rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/dist/favicon.ico
+-rw-r--r--   0        0        0     1141 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/dist/index.html
+-rw-r--r--   0        0        0      981 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/index.html
+-rw-r--r--   0        0        0     1526 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/package.json
+-rw-r--r--   0        0        0       81 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/postcss.config.js
+-rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/public/favicon.ico
+-rw-r--r--   0        0        0     2554 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/App.css
+-rw-r--r--   0        0        0     2989 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/App.tsx
+-rw-r--r--   0        0        0      310 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ArrowUp.svg
+-rw-r--r--   0        0        0     2626 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ChatIcon.svg
+-rw-r--r--   0        0        0      789 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon.svg
+-rw-r--r--   0        0        0      328 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon2.svg
+-rw-r--r--   0        0        0      505 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ChevronRight.svg
+-rw-r--r--   0        0        0     1153 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CircleSpinIcon.svg
+-rw-r--r--   0        0        0      823 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CodeIcon.svg
+-rw-r--r--   0        0        0     1328 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CopyIcon.svg
+-rw-r--r--   0        0        0     1744 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/EmptyState.svg
+-rw-r--r--   0        0        0    11000 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/LangServeLogo.svg
+-rw-r--r--   0        0        0     2350 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/PadlockIcon.svg
+-rw-r--r--   0        0        0      670 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/PlusIcon.svg
+-rw-r--r--   0        0        0      400 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/RefreshCW.svg
+-rw-r--r--   0        0        0     1260 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/SendIcon.svg
+-rw-r--r--   0        0        0     1831 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ShareIcon.svg
+-rw-r--r--   0        0        0      374 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ThumbsDownIcon.svg
+-rw-r--r--   0        0        0      354 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ThumbsUpIcon.svg
+-rw-r--r--   0        0        0     1509 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/TrashIcon.svg
+-rw-r--r--   0        0        0      346 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/XCircle.svg
+-rw-r--r--   0        0        0     1578 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/AutosizeTextarea.tsx
+-rw-r--r--   0        0        0     4288 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/ChatMessage.tsx
+-rw-r--r--   0        0        0     7735 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/ChatWindow.tsx
+-rw-r--r--   0        0        0     5116 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/ShareDialog.tsx
+-rw-r--r--   0        0        0     3463 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx
+-rw-r--r--   0        0        0      308 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/main.tsx
+-rw-r--r--   0        0        0      368 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/types.tsx
+-rw-r--r--   0        0        0     3924 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/useSchemas.tsx
+-rw-r--r--   0        0        0     2345 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/useStreamCallback.tsx
+-rw-r--r--   0        0        0     3406 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/useStreamLog.tsx
+-rw-r--r--   0        0        0      183 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/cn.ts
+-rw-r--r--   0        0        0     5344 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/defaults.ts
+-rw-r--r--   0        0        0      140 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/json-refs.d.ts
+-rw-r--r--   0        0        0   367401 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/json-refs.js
+-rw-r--r--   0        0        0      227 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/messages.ts
+-rw-r--r--   0        0        0      726 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/path.ts
+-rw-r--r--   0        0        0      548 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/schema.ts
+-rw-r--r--   0        0        0      330 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/simplifySchema.ts
+-rw-r--r--   0        0        0      147 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/str.ts
+-rw-r--r--   0        0        0      958 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/url.ts
+-rw-r--r--   0        0        0       87 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/vite-env.d.ts
+-rw-r--r--   0        0        0      950 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/tailwind.config.js
+-rw-r--r--   0        0        0      605 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/tsconfig.node.json
+-rw-r--r--   0        0        0      571 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/vite.config.ts
+-rw-r--r--   0        0        0   134098 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/chat_playground/yarn.lock
+-rw-r--r--   0        0        0    31643 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/client.py
+-rw-r--r--   0        0        0    14983 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/lzstring.py
+-rw-r--r--   0        0        0      436 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/.eslintrc.cjs
+-rw-r--r--   0        0        0      266 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/.gitignore
+-rw-r--r--   0        0        0     1263 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/README.md
+-rw-r--r--   0        0        0    16476 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/dist/assets/index-52e8ab2f.css
+-rw-r--r--   0        0        0  1332675 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/dist/assets/index-dbc96538.js
+-rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/dist/favicon.ico
+-rw-r--r--   0        0        0      916 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/dist/index.html
+-rw-r--r--   0        0        0      756 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/index.html
+-rw-r--r--   0        0        0     1616 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/package.json
+-rw-r--r--   0        0        0       81 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/postcss.config.js
+-rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/public/favicon.ico
+-rw-r--r--   0        0        0     2081 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/src/App.css
+-rw-r--r--   0        0        0     7176 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/src/App.tsx
+-rw-r--r--   0        0        0     2626 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ChatIcon.svg
+-rw-r--r--   0        0        0      792 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CheckCircleIcon.svg
+-rw-r--r--   0        0        0      505 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ChevronRight.svg
+-rw-r--r--   0        0        0     1153 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CircleSpinIcon.svg
+-rw-r--r--   0        0        0      823 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CodeIcon.svg
+-rw-r--r--   0        0        0     1328 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CopyIcon.svg
+-rw-r--r--   0        0        0     2350 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/PadlockIcon.svg
+-rw-r--r--   0        0        0      670 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/PlusIcon.svg
+-rw-r--r--   0        0        0     1260 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/SendIcon.svg
+-rw-r--r--   0        0        0     1831 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ShareIcon.svg
+-rw-r--r--   0        0        0     1089 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ThumbsDownIcon.svg
+-rw-r--r--   0        0        0      549 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ThumbsUpIcon.svg
+-rw-r--r--   0        0        0     1509 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/TrashIcon.svg
+-rw-r--r--   0        0        0     1424 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/AutosizeTextarea.tsx
+-rw-r--r--   0        0        0     5541 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ChatMessageInput.tsx
+-rw-r--r--   0        0        0     5595 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx
+-rw-r--r--   0        0        0     5168 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx
+-rw-r--r--   0        0        0     1076 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomAnyOfRenderer.tsx
+-rw-r--r--   0        0        0     2519 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx
+-rw-r--r--   0        0        0    13357 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx
+-rw-r--r--   0        0        0     1562 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx
+-rw-r--r--   0        0        0     3182 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx
+-rw-r--r--   0        0        0     1819 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx
+-rw-r--r--   0        0        0     3680 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer.tsx
+-rw-r--r--   0        0        0     2617 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomTextAreaCell.tsx
+-rw-r--r--   0        0        0     1256 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/FileBase64Tester.tsx
+-rw-r--r--   0        0        0     2468 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/IntermediateSteps.tsx
+-rw-r--r--   0        0        0     2941 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/JsonTextAreaCell.tsx
+-rw-r--r--   0        0        0     5189 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ShareDialog.tsx
+-rw-r--r--   0        0        0     3320 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/StreamOutput.tsx
+-rw-r--r--   0        0        0     2347 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/SubmitButton.tsx
+-rw-r--r--   0        0        0     2910 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx
+-rw-r--r--   0        0        0      308 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/main.tsx
+-rw-r--r--   0        0        0     3372 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/renderers.tsx
+-rw-r--r--   0        0        0     1580 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/sections/SectionConfigure.tsx
+-rw-r--r--   0        0        0     2125 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/sections/SectionInputs.tsx
+-rw-r--r--   0        0        0      358 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/types.tsx
+-rw-r--r--   0        0        0     2633 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/useSchemas.tsx
+-rw-r--r--   0        0        0     2345 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/useStreamCallback.tsx
+-rw-r--r--   0        0        0     3401 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/useStreamLog.tsx
+-rw-r--r--   0        0        0      183 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/utils/cn.ts
+-rw-r--r--   0        0        0     5344 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/utils/defaults.ts
+-rw-r--r--   0        0        0      140 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/utils/json-refs.d.ts
+-rw-r--r--   0        0        0   367401 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/json-refs.js
+-rw-r--r--   0        0        0      227 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/messages.ts
+-rw-r--r--   0        0        0      726 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/path.ts
+-rw-r--r--   0        0        0      548 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/schema.ts
+-rw-r--r--   0        0        0      330 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/simplifySchema.ts
+-rw-r--r--   0        0        0      147 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/str.ts
+-rw-r--r--   0        0        0      958 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/url.ts
+-rw-r--r--   0        0        0       87 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/vite-env.d.ts
+-rw-r--r--   0        0        0      781 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/tailwind.config.js
+-rw-r--r--   0        0        0      605 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/tsconfig.node.json
+-rw-r--r--   0        0        0      539 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/vite.config.ts
+-rw-r--r--   0        0        0   135134 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/yarn.lock
+-rw-r--r--   0        0        0     3543 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/py.typed
+-rw-r--r--   0        0        0     1187 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/pydantic_v1.py
+-rw-r--r--   0        0        0     5337 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/schema.py
+-rw-r--r--   0        0        0     7004 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/serialization.py
+-rw-r--r--   0        0        0    46956 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/server.py
+-rw-r--r--   0        0        0     4089 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/server_sent_events.py
+-rw-r--r--   0        0        0    17233 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/validation.py
+-rw-r--r--   0        0        0      307 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/version.py
+-rw-r--r--   0        0        0     2539 2024-04-01 19:51:36.112289 langserve-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    43302 1970-01-01 00:00:00.000000 langserve-0.1.0rc1/PKG-INFO
```

### Comparing `langserve-0.0.9/LICENSE` & `langserve-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

