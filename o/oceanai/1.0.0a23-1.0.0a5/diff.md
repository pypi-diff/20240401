# Comparing `tmp/oceanai-1.0.0a23.tar.gz` & `tmp/oceanai-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanai-1.0.0a23.tar", last modified: Mon Apr  1 10:00:55 2024, max compression
+gzip compressed data, was "oceanai-1.0.0a5.tar", last modified: Tue Jan  3 17:29:36 2023, max compression
```

## Comparing `oceanai-1.0.0a23.tar` & `oceanai-1.0.0a5.tar`

### file list

```diff
@@ -1,55 +1,46 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.164955 oceanai-1.0.0a23/
--rw-r--r--   0 dl         (501) staff       (20)     1628 2023-09-11 08:26:13.000000 oceanai-1.0.0a23/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      103 2023-09-11 08:26:13.000000 oceanai-1.0.0a23/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)    10753 2024-04-01 10:00:55.165287 oceanai-1.0.0a23/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     7971 2024-01-12 09:31:46.000000 oceanai-1.0.0a23/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.114568 oceanai-1.0.0a23/oceanai/
--rw-r--r--   0 dl         (501) staff       (20)      961 2024-04-01 09:59:17.000000 oceanai-1.0.0a23/oceanai/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.117217 oceanai-1.0.0a23/oceanai/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-09-11 08:26:13.000000 oceanai-1.0.0a23/oceanai/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.125571 oceanai-1.0.0a23/oceanai/modules/core/
--rw-rw-r--   0 dl         (501) staff       (20)        0 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/core/__init__.py
--rw-rw-r--   0 dl         (501) staff       (20)   152110 2024-04-01 09:58:25.000000 oceanai-1.0.0a23/oceanai/modules/core/core.py
--rw-rw-r--   0 dl         (501) staff       (20)     2394 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/core/exceptions.py
--rw-rw-r--   0 dl         (501) staff       (20)    15130 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/core/language.py
--rw-rw-r--   0 dl         (501) staff       (20)     7630 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/core/messages.py
--rw-rw-r--   0 dl         (501) staff       (20)    66035 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/core/settings.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.148045 oceanai-1.0.0a23/oceanai/modules/lab/
--rw-rw-r--   0 dl         (501) staff       (20)        0 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/__init__.py
--rw-rw-r--   0 dl         (501) staff       (20)   118703 2024-03-23 19:21:48.000000 oceanai-1.0.0a23/oceanai/modules/lab/audio.py
--rw-rw-r--   0 dl         (501) staff       (20)     2692 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/build.py
--rw-rw-r--   0 dl         (501) staff       (20)    28394 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/download.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.157025 oceanai-1.0.0a23/oceanai/modules/lab/keras_vggface/
--rw-rw-r--   0 dl         (501) staff       (20)        0 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/keras_vggface/__init__.py
--rw-rw-r--   0 dl         (501) staff       (20)     5234 2024-03-23 06:20:30.000000 oceanai-1.0.0a23/oceanai/modules/lab/keras_vggface/models.py
--rw-rw-r--   0 dl         (501) staff       (20)     1244 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/keras_vggface/utils.py
--rw-rw-r--   0 dl         (501) staff       (20)      687 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/keras_vggface/vggface.py
--rw-rw-r--   0 dl         (501) staff       (20)   130451 2024-03-23 17:14:00.000000 oceanai-1.0.0a23/oceanai/modules/lab/prediction.py
--rw-rw-r--   0 dl         (501) staff       (20)    87728 2024-03-23 19:26:18.000000 oceanai-1.0.0a23/oceanai/modules/lab/text.py
--rw-rw-r--   0 dl         (501) staff       (20)    17246 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/unzip.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.160206 oceanai-1.0.0a23/oceanai/modules/lab/utils/
--rw-rw-r--   0 dl         (501) staff       (20)        0 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/utils/__init__.py
--rw-rw-r--   0 dl         (501) staff       (20)     1856 2024-03-23 08:01:22.000000 oceanai-1.0.0a23/oceanai/modules/lab/utils/addition.py
--rw-rw-r--   0 dl         (501) staff       (20)     2253 2024-03-23 06:11:20.000000 oceanai-1.0.0a23/oceanai/modules/lab/utils/attention.py
--rw-rw-r--   0 dl         (501) staff       (20)     3459 2024-03-23 07:34:34.000000 oceanai-1.0.0a23/oceanai/modules/lab/utils/gfl.py
--rw-rw-r--   0 dl         (501) staff       (20)   178736 2024-03-28 18:54:17.000000 oceanai-1.0.0a23/oceanai/modules/lab/video.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.111008 oceanai-1.0.0a23/oceanai/modules/locales/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.110759 oceanai-1.0.0a23/oceanai/modules/locales/en/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.160881 oceanai-1.0.0a23/oceanai/modules/locales/en/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)    16103 2023-12-24 21:27:33.000000 oceanai-1.0.0a23/oceanai/modules/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.111130 oceanai-1.0.0a23/oceanai/modules/locales/ru/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.161568 oceanai-1.0.0a23/oceanai/modules/locales/ru/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)      407 2023-12-24 21:27:37.000000 oceanai-1.0.0a23/oceanai/modules/locales/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.116642 oceanai-1.0.0a23/oceanai.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)    10753 2024-04-01 10:00:54.000000 oceanai-1.0.0a23/oceanai.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1193 2024-04-01 10:00:55.000000 oceanai-1.0.0a23/oceanai.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-01 10:00:54.000000 oceanai-1.0.0a23/oceanai.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)      388 2024-04-01 10:00:54.000000 oceanai-1.0.0a23/oceanai.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)       13 2024-04-01 10:00:54.000000 oceanai-1.0.0a23/oceanai.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 oceanai-1.0.0a23/pyproject.toml
--rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-01 10:00:55.166009 oceanai-1.0.0a23/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     3741 2024-03-28 18:54:36.000000 oceanai-1.0.0a23/setup.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-01 10:00:55.164143 oceanai-1.0.0a23/test/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-09-11 08:26:13.000000 oceanai-1.0.0a23/test/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    10132 2023-12-16 16:53:39.000000 oceanai-1.0.0a23/test/unit_tests_fi_en.py
--rw-r--r--   0 dl         (501) staff       (20)     5199 2023-12-16 16:53:39.000000 oceanai-1.0.0a23/test/unit_tests_mupta_ru.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.866377 oceanai-1.0.0a5/
+-rw-r--r--   0 dl         (501) staff       (20)     1628 2022-11-16 12:52:28.000000 oceanai-1.0.0a5/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      103 2022-12-01 12:19:26.000000 oceanai-1.0.0a5/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     6966 2023-01-03 17:29:36.866564 oceanai-1.0.0a5/PKG-INFO
+-rw-------   0 dl         (501) staff       (20)     4186 2023-01-03 17:27:10.000000 oceanai-1.0.0a5/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.842095 oceanai-1.0.0a5/oceanai/
+-rw-r--r--   0 dl         (501) staff       (20)      914 2023-01-03 09:39:39.000000 oceanai-1.0.0a5/oceanai/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.844730 oceanai-1.0.0a5/oceanai/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-09-01 09:03:06.000000 oceanai-1.0.0a5/oceanai/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.850132 oceanai-1.0.0a5/oceanai/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-02 18:36:57.000000 oceanai-1.0.0a5/oceanai/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   126647 2023-01-03 11:14:50.000000 oceanai-1.0.0a5/oceanai/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     2388 2022-12-03 12:16:27.000000 oceanai-1.0.0a5/oceanai/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)    15095 2022-12-11 12:22:25.000000 oceanai-1.0.0a5/oceanai/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     8120 2022-12-11 09:15:29.000000 oceanai-1.0.0a5/oceanai/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    65557 2022-12-03 20:05:51.000000 oceanai-1.0.0a5/oceanai/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.858626 oceanai-1.0.0a5/oceanai/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-09-01 09:06:56.000000 oceanai-1.0.0a5/oceanai/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   112964 2022-12-30 15:03:42.000000 oceanai-1.0.0a5/oceanai/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)     2715 2022-12-01 14:38:15.000000 oceanai-1.0.0a5/oceanai/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)    27089 2022-12-30 14:06:40.000000 oceanai-1.0.0a5/oceanai/modules/lab/download.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.863336 oceanai-1.0.0a5/oceanai/modules/lab/keras_vggface/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-10-30 15:04:03.000000 oceanai-1.0.0a5/oceanai/modules/lab/keras_vggface/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    17683 2022-12-03 21:21:19.000000 oceanai-1.0.0a5/oceanai/modules/lab/keras_vggface/models.py
+-rw-r--r--   0 dl         (501) staff       (20)     3067 2022-10-30 15:20:51.000000 oceanai-1.0.0a5/oceanai/modules/lab/keras_vggface/utils.py
+-rw-r--r--   0 dl         (501) staff       (20)     1450 2022-12-03 21:21:38.000000 oceanai-1.0.0a5/oceanai/modules/lab/keras_vggface/vggface.py
+-rw-r--r--   0 dl         (501) staff       (20)    62643 2022-12-26 12:21:41.000000 oceanai-1.0.0a5/oceanai/modules/lab/prediction.py
+-rw-r--r--   0 dl         (501) staff       (20)   169215 2022-12-10 09:16:38.000000 oceanai-1.0.0a5/oceanai/modules/lab/video.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.839355 oceanai-1.0.0a5/oceanai/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.839175 oceanai-1.0.0a5/oceanai/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.864064 oceanai-1.0.0a5/oceanai/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)    12401 2022-12-11 12:47:58.000000 oceanai-1.0.0a5/oceanai/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.839465 oceanai-1.0.0a5/oceanai/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.864696 oceanai-1.0.0a5/oceanai/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      407 2022-12-11 12:48:11.000000 oceanai-1.0.0a5/oceanai/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.844379 oceanai-1.0.0a5/oceanai.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     6966 2023-01-03 17:29:36.000000 oceanai-1.0.0a5/oceanai.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)      939 2023-01-03 17:29:36.000000 oceanai-1.0.0a5/oceanai.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2023-01-03 17:29:36.000000 oceanai-1.0.0a5/oceanai.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      287 2023-01-03 17:29:36.000000 oceanai-1.0.0a5/oceanai.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)       13 2023-01-03 17:29:36.000000 oceanai-1.0.0a5/oceanai.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       79 2023-01-03 17:29:36.867095 oceanai-1.0.0a5/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     3559 2022-12-28 10:58:59.000000 oceanai-1.0.0a5/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2023-01-03 17:29:36.865626 oceanai-1.0.0a5/test/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-09-01 09:03:06.000000 oceanai-1.0.0a5/test/__init__.py
+-rw-------   0 dl         (501) staff       (20)     6899 2022-12-11 17:01:21.000000 oceanai-1.0.0a5/test/unit_tests.py
```

### Comparing `oceanai-1.0.0a23/LICENSE` & `oceanai-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanai-1.0.0a23/oceanai/modules/core/core.py` & `oceanai-1.0.0a5/oceanai/modules/core/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,66 +4,58 @@
 """
 Ядро
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
-import sys  # Доступ к некоторым переменным и функциям Python
-import re  # Регулярные выражения
-import time  # Работа со временем
-import numpy as np  # Научные вычисления
+import os                 # Взаимодействие с файловой системой
+import sys                # Доступ к некоторым переменным и функциям Python
+import re                 # Регулярные выражения
+import time               # Работа со временем
+import numpy as np        # Научные вычисления
 import scipy
-import pandas as pd  # Обработка и анализ данных
-import opensmile  # Анализ, обработка и классификация звука
-import jupyterlab as jlab  # Интерактивная среда разработки для работы с блокнотами, кодом и данными
-import requests  # Отправка HTTP запросов
-import librosa  # Обработка аудио
-import audioread  # Декодирование звука
-import sklearn  # Машинное обучение и интеллектуальный анализ данных
-import cv2  # Алгоритмы компьютерного зрения
-import mediapipe as mp  # Набор нейросетевых моделей и решений для компьютерного зрения
+import pandas as pd       # Обработка и анализ данных
+import opensmile          # Анализ, обработка и классификация звука
+import jupyterlab as jlab # Интерактивная среда разработки для работы с блокнотами, кодом и данными
+import requests           # Отправка HTTP запросов
+import librosa            # Обработка аудио
+import audioread          # Декодирование звука
+import sklearn            # Машинное обучение и интеллектуальный анализ данных
+import cv2                # Алгоритмы компьютерного зрения
+import mediapipe as mp    # Набор нейросетевых моделей и решений для компьютерного зрения
 import IPython
 import logging
-import urllib.error  # Обработка ошибок URL
+import pymediainfo        # Получение meta данных из медиафайлов
+import urllib.error       # Обработка ошибок URL
 import math
-import liwc  # Анализатор лингвистических запросов и подсчета слов
-import transformers  # Доступ к Hugging Face Transformers
-import sentencepiece  # Обработка и токенизация текста с использованием SentencePiece
-import torch  # Машинное обучение от Facebook
-import torchaudio  # Работа с аудио от Facebook
 
-from datetime import datetime  # Работа со временем
-from typing import List, Dict, Tuple, Union, Optional, Iterable  # Типы данных
+from datetime import datetime # Работа со временем
+from typing import List, Dict, Tuple, Union, Optional, Iterable # Типы данных
 
 from IPython import get_ipython
 from IPython.display import Markdown, display, clear_output
 
 # Персональные
-import oceanai  # oceanai - персональные качества личности человека
-from oceanai.modules.core.settings import Settings  # Глобальный файл настроек
+import oceanai                                     # oceanai - персональные качества личности человека
+from oceanai.modules.core.settings import Settings # Глобальный файл настроек
 
 # Порог регистрации сообщений TensorFlow
 logging.disable(logging.WARNING)
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
-import tensorflow as tf  # Машинное обучение от Google
+import tensorflow as tf # Машинное обучение от Google
 import keras
 
-
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class CoreMessages(Settings):
     """Класс для сообщений
 
@@ -79,96 +71,61 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._trac_file: str = self._("Файл")
-        self._trac_line: str = self._("Линия")
-        self._trac_method: str = self._("Метод")
-        self._trac_type_err: str = self._("Тип ошибки")
+        self._trac_file: str = self._('Файл')
+        self._trac_line: str = self._('Линия')
+        self._trac_method: str = self._('Метод')
+        self._trac_type_err: str = self._('Тип ошибки')
 
-        self._sec: str = self._("сек.")
+        self._sec: str = self._('сек.')
 
         self._folder_not_found: str = self._oh + self._('директория "{}" не найдена ...')
-        self._files_not_found: str = self._oh + self._("в указанной директории необходимые файлы не найдены ...")
+        self._files_not_found: str = self._oh + self._('в указанной директории необходимые файлы не найдены ...')
         self._file_not_found: str = self._oh + self._('файл "{}" не найден ...')
         self._directory_inst_file: str = self._oh + self._('вместо файла передана директория "{}" ...')
         self._no_acoustic_signal: str = self._oh + self._('файл "{}" не содержит акустического сигнала ...')
-        self._url_error_log: str = self._oh + self._("не удалось сохранить LOG файл{} ...")
-        self._url_error_code_log: str = self._(" (ошибка {})")
+        self._url_error_log: str = self._oh + self._('не удалось сохранить LOG файл{} ...')
+        self._url_error_code_log: str = self._(' (ошибка {})')
 
-        self._mul: str = "&#10005;"  # Знак умножения
+        self._mul: str = '&#10005;' # Знак умножения
 
-        self._get_acoustic_feature_stat: str = (
-            "{}" * 4
-            + self._(
-                "Статистика извлеченных признаков из акустического сигнала:"
-                "{}Общее количество сегментов с:"
-                "{}1. экспертными признаками: {}"
-                "{}2. лог мел-спектрограммами: {}"
-                "{}Размерность матрицы экспертных признаков одного сегмента: "
-                "{} "
-            )
-            + self._mul
-            + " {}"
-            + self._("{}Размерность тензора с лог мел-спектрограммами одного сегмента:")
-            + "{} "
-            + self._mul
-            + " {} "
-            + self._mul
-            + " {}"
-        )
+        self._get_acoustic_feature_stat: str = '{}' * 4 + self._(
+            'Статистика извлеченных признаков из акустического сигнала:'
+            '{}Общее количество сегментов с:'
+            '{}1. экспертными признаками: {}'
+            '{}2. лог мел-спектрограммами: {}'
+            '{}Размерность матрицы экспертных признаков одного сегмента: '
+            '{} ') + self._mul + ' {}' + \
+            self._('{}Размерность тензора с лог мел-спектрограммами одного сегмента:') + \
+            '{} ' + self._mul + ' {} ' + self._mul + ' {}'
+
+        self._get_visual_feature_stat: str = '{}' * 4 + self._(
+            'Статистика извлеченных признаков из визуального сигнала:'
+            '{}Общее количество сегментов с:'
+            '{}1. экспертными признаками: {}'
+            '{}2. нейросетевыми признаками: {}'
+            '{}Размерность матрицы экспертных признаков одного сегмента: '
+            '{} ') + self._mul + ' {}' + \
+            self._('{}Размерность тензора с нейросетевыми признаками одного сегмента:') + \
+            '{} ' + self._mul + ' {} ' + \
+            self._('{}Понижение кадровой частоты: с') + '{} ' + self._('до') + ' {} '
 
-        self._get_visual_feature_stat: str = (
-            "{}" * 4
-            + self._(
-                "Статистика извлеченных признаков из визуального сигнала:"
-                "{}Общее количество сегментов с:"
-                "{}1. экспертными признаками: {}"
-                "{}2. нейросетевыми признаками: {}"
-                "{}Размерность матрицы экспертных признаков одного сегмента: "
-                "{} "
-            )
-            + self._mul
-            + " {}"
-            + self._("{}Размерность матрицы с нейросетевыми признаками одного сегмента:")
-            + "{} "
-            + self._mul
-            + " {} "
-            + self._("{}Понижение кадровой частоты: с")
-            + "{} "
-            + self._("до")
-            + " {} "
-        )
-
-        self._get_text_feature_stat: str = (
-            "{}" * 4
-            + self._("Статистика извлеченных признаков из текста:" "{}Размерность матрицы экспертных признаков: " "{} ")
-            + self._mul
-            + " {}"
-            + self._("{}Размерность матрицы с нейросетевыми признаками:")
-            + "{} "
-            + self._mul
-            + " {} "
-        )
-
-        self._get_text_feature_stat_with_text: str = self._get_text_feature_stat + self._("{}Текст:") + "{}"
-
-        self._curr_progress_union_predictions: str = "{} " + self._from_precent + " {} ({}%) ... {} ..."
+        self._curr_progress_union_predictions: str = '{} ' + self._from_precent + ' {} ({}%) ... {} ...'
 
         self._sum_ranking_exceeded: str = self._oh + self._(
-            "сумма весов для ранжирования персональных качеств должна быть равна 100 ..."
+            'сумма весов для ранжирования персональных качеств должна быть равна 100 ...'
         )
 
-        self._dataframe_empty: str = self._oh + self._("DataFrame с данными пуст ...")
-
+        self._dataframe_empty: str = self._oh + self._('DataFrame с данными пуст ...')
 
 # ######################################################################################################################
 # Ядро модулей
 # ######################################################################################################################
 @dataclass
 class Core(CoreMessages):
     """Класс-ядро модулей
@@ -185,230 +142,138 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._start_time: Union[int, float] = -1  # Старт времени выполнения
-        self._runtime: Union[int, float] = -1  # Время выполнения
+        self._start_time: Union[int, float] = -1 # Старт времени выполнения
+        self._runtime: Union[int, float] = -1 # Время выполнения
 
-        self._notebook_history_output: List[str] = []  # История вывода сообщений в ячейке Jupyter
+        self._notebook_history_output: List[str] = [] # История вывода сообщений в ячейке Jupyter
 
-        self._df_pkgs: pd.DataFrame = pd.DataFrame()  # DataFrame c версиями установленных библиотек
+        self._df_pkgs: pd.DataFrame = pd.DataFrame() # DataFrame c версиями установленных библиотек
 
         # Персональные качества личности человека (Порядок только такой)
         self._b5: Dict[str, Tuple[str, ...]] = {
-            "en": ("openness", "conscientiousness", "extraversion", "agreeableness", "non-neuroticism"),
-            "ru": (
-                self._("открытость опыту"),
-                self._("добросовестность"),
-                self._("экстраверсия"),
-                self._("доброжелательность"),
-                self._("эмоциональная стабильность"),
-            ),
+            'en': ('openness', 'conscientiousness', 'extraversion', 'agreeableness', 'neuroticism'),
+            'ru': (self._('открытость опыту'), self._('добросовестность'), self._('экстраверсия'),
+                   self._('доброжелательность'), self._('нейротизм'))
         }
 
         # Веса для нейросетевых архитектур
         self._weights_for_big5: Dict[str, Dict] = {
-            "audio": {
-                "fi": {
-                    "hc": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/400635799?token=MMRrak8fMsyzxLE&filename=weights_2022-05-05_11-27-55.h5",
-                    },
-                    "nn": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/400635678?token=W6LCtD33FQHnYEz&filename=weights_2022-05-03_07-46-14.h5",
-                    },
-                    "b5": {
-                        "openness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/405035301?token=443WRA9MFWqWBAE&filename=weights_2022-06-15_16-16-20.h5",
-                        },
-                        "conscientiousness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/405034601?token=eDG28m3H6c8bWoE&filename=weights_2022-06-15_16-21-57.h5",
-                        },
-                        "extraversion": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/405034830?token=3daBSTYnmZaesee&filename=weights_2022-06-15_16-26-41.h5",
-                        },
-                        "agreeableness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/405034397?token=52ZPHMjb4CFmdYa&filename=weights_2022-06-15_16-32-51.h5",
-                        },
-                        "non_neuroticism": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/405035156?token=q8CZJ99rZqcNxkM&filename=weights_2022-06-15_16-37-46.h5",
-                        },
-                    },
+            'audio': {
+                'hc': {
+                    'sberdisk': 'https://download.sberdisk.ru/download/file/400635799?token=MMRrak8fMsyzxLE&filename=weights_2022-05-05_11-27-55.h5',
                 },
-                "mupta": {
-                    "hc": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962562?token=pFKAlXd8koEngHa&filename=ahc_mupta_2022-06-18_08-32-05.h5",
-                    },
-                    "nn": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962561?token=lPCiioXg7ZeNUK8&filename=ann_mupta_2022-06-18_09-57-06.h5",
-                    },
+                'nn': {
+                    'sberdisk': 'https://download.sberdisk.ru/download/file/400635678?token=W6LCtD33FQHnYEz&filename=weights_2022-05-03_07-46-14.h5',
                 },
-            },
-            "video": {
-                "fi": {
-                    "hc": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/412059444?token=JXerCfAjJZg6crD&filename=weights_2022-08-27_18-53-35.h5",
+                'b5': {
+                    'openness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/405035301?token=443WRA9MFWqWBAE&filename=weights_2022-06-15_16-16-20.h5',
                     },
-                    "nn": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/412059478?token=85KeW6q4QKy6kP8&filename=weights_2022-03-22_16-31-48.h5",
+                    'conscientiousness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/405034601?token=eDG28m3H6c8bWoE&filename=weights_2022-06-15_16-21-57.h5',
                     },
-                    "fe": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/414207833?token=ygzxWEkndjSMnEL&filename=weights_2022-11-01_12-27-07.h5"
+                    'extraversion': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/405034830?token=3daBSTYnmZaesee&filename=weights_2022-06-15_16-26-41.h5',
                     },
-                    "b5": {
-                        "openness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/415127050?token=rfpy9TLdbeXtiN7&filename=weights_2022-06-15_16-46-30.h5",
-                        },
-                        "conscientiousness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/415126986?token=PnjzaHaR3wPg2RT&filename=weights_2022-06-15_16-48-50.h5",
-                        },
-                        "extraversion": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/415127012?token=s5aTwbt8DBkt7G4&filename=weights_2022-06-15_16-54-06.h5",
-                        },
-                        "agreeableness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/415126845?token=joN7TMHk59Gffsf&filename=weights_2022-06-15_17-02-03.h5",
-                        },
-                        "non_neuroticism": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/415127032?token=NEBSsE7mjyjen3o&filename=weights_2022-06-15_17-06-15.h5",
-                        },
-                    },
-                },
-                "mupta": {
-                    "hc": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962567?token=oSMaqRe5xK8UBIP&filename=vhc_mupta_2022-07-22_10-02-37.h5",
+                    'agreeableness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/405034397?token=52ZPHMjb4CFmdYa&filename=weights_2022-06-15_16-32-51.h5',
                     },
-                    "nn": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962568?token=TZWoSGYW3LPoKg4&filename=vnn_mupta_2022-06-25_18-12-38.h5",
-                    },
-                    "fe": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/414207833?token=ygzxWEkndjSMnEL&filename=weights_2022-11-01_12-27-07.h5"
+                    'neuroticism': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/405035156?token=q8CZJ99rZqcNxkM&filename=weights_2022-06-15_16-37-46.h5',
                     },
                 },
             },
-            "text": {
-                "fi": {
-                    "hc": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/472034034?token=59eA6DXo6GXWV77&filename=weights_2023-07-15_10-52-15.h5",
-                    },
-                    "nn": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/472139570?token=LpndWNlovMhxU3O&filename=weights_2023-07-03_15-01-08.h5",
+            'video': {
+                'hc': {
+                    'sberdisk': 'https://download.sberdisk.ru/download/file/412059444?token=JXerCfAjJZg6crD&filename=weights_2022-08-27_18-53-35.h5',
+                },
+                'nn': {
+                    'sberdisk': 'https://download.sberdisk.ru/download/file/412059478?token=85KeW6q4QKy6kP8&filename=weights_2022-03-22_16-31-48.h5',
+                },
+                'fe': {
+                    'sberdisk': 'https://download.sberdisk.ru/download/file/414207833?token=ygzxWEkndjSMnEL&filename=weights_2022-11-01_12-27-07.h5'
+                },
+                'b5': {
+                    'openness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/415127050?token=rfpy9TLdbeXtiN7&filename=weights_2022-06-15_16-46-30.h5',
                     },
-                    "b5": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962564?token=3aCG3GRqbjkOBIK&filename=ft_fi_2023-12-09_14-25-13.h5",
+                    'conscientiousness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/415126986?token=PnjzaHaR3wPg2RT&filename=weights_2022-06-15_16-48-50.h5',
                     },
-                },
-                "mupta": {
-                    "hc": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/472042355?token=MUJ82JsJiRe6RIz&filename=weights_2023-07-15_10-53-38.h5",
+                    'extraversion': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/415127012?token=s5aTwbt8DBkt7G4&filename=weights_2022-06-15_16-54-06.h5',
                     },
-                    "nn": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/472139571?token=DvEzGThzqaMl2pp&filename=weights_2023-07-16_18-12-01.h5",
+                    'agreeableness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/415126845?token=joN7TMHk59Gffsf&filename=weights_2022-06-15_17-02-03.h5',
                     },
-                    "b5": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962566?token=sliTZG1OBMIrlwY&filename=ft_mupta_2023-12-09_14-25-13.h5",
+                    'neuroticism': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/415127032?token=NEBSsE7mjyjen3o&filename=weights_2022-06-15_17-06-15.h5',
                     },
                 },
             },
-            "av": {
-                "fi": {
-                    "b5": {
-                        "openness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/425515223?token=Btoo2flpzGewhry&filename=weights_2022-08-28_11-14-35.h5",
-                        },
-                        "conscientiousness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/425515311?token=bUjloqk32e4wasj&filename=weights_2022-08-28_11-08-10.h5",
-                        },
-                        "extraversion": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/425515337?token=IC44ovFFcnj4DZl&filename=weights_2022-08-28_11-17-57.h5",
-                        },
-                        "agreeableness": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/425515346?token=gFjvtM2HIabtsvc&filename=weights_2022-08-28_11-25-11.h5",
-                        },
-                        "non_neuroticism": {
-                            "sberdisk": "https://download.sberdisk.ru/download/file/425515375?token=pPpzOQC9z6WMzNt&filename=weights_2022-06-14_21-44-09.h5",
-                        },
+            'av': {
+                'b5': {
+                    'openness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/425515223?token=Btoo2flpzGewhry&filename=weights_2022-08-28_11-14-35.h5',
+                    },
+                    'conscientiousness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/425515311?token=bUjloqk32e4wasj&filename=weights_2022-08-28_11-08-10.h5',
                     },
-                },
-                "mupta": {
-                    "b5": {},
-                },
-            },
-            "avt": {
-                "fi": {
-                    "b5": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962565?token=YSTP75aNv8eVtxf&filename=avt_fi_2023-12-03_11-36-51.h5",
+                    'extraversion': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/425515337?token=IC44ovFFcnj4DZl&filename=weights_2022-08-28_11-17-57.h5',
                     },
-                },
-                "mupta": {
-                    "b5": {
-                        "sberdisk": "https://download.sberdisk.ru/download/file/477962563?token=v5hUmyJEbhyPqic&filename=avt_mupta_2023-12-09_14-25-13.h5",
+                    'agreeableness': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/425515346?token=gFjvtM2HIabtsvc&filename=weights_2022-08-28_11-25-11.h5',
+                    },
+                    'neuroticism': {
+                        'sberdisk': 'https://download.sberdisk.ru/download/file/425515375?token=pPpzOQC9z6WMzNt&filename=weights_2022-06-14_21-44-09.h5',
                     },
                 },
             },
         }
 
         # Верные предсказания для подсчета точности
         self._true_traits: Dict[str, str] = {
-            "fi": {
-                "sberdisk": "https://download.sberdisk.ru/download/file/478675810?token=anU8umMha1GiWPQ&filename=data_true_traits_fi.csv"
-            },
-            "mupta": {
-                "sberdisk": "https://download.sberdisk.ru/download/file/478675811?token=hUMsrUSKjSRrV5e&filename=data_true_traits_mupta.csv"
-            },
+            'sberdisk': 'https://download.sberdisk.ru/download/file/410305241?token=TFePK6w5CW6ADnq&filename=data_true_traits.csv',
         }
 
-        self._df_files: pd.DataFrame = pd.DataFrame()  # DataFrame с данными
-        self._df_files_ranking: pd.DataFrame = pd.DataFrame()  # DataFrame с ранжированными данными
+        self._df_files: pd.DataFrame = pd.DataFrame() # DataFrame с данными
+        self._df_files_ranking: pd.DataFrame = pd.DataFrame() # DataFrame с ранжированными данными
         # DataFrame с ранжированными предпочтениями на основе данных
         self._df_files_priority: pd.DataFrame = pd.DataFrame()
-        # DataFrame с ранжированными коллегами на основе данных
-        self._df_files_colleague: pd.DataFrame = pd.DataFrame()
-        self._df_files_priority_skill: pd.DataFrame = pd.DataFrame()
-        self._dict_of_files: Dict[str, List[Union[int, str, float]]] = {}  # Словарь для DataFrame с данными
+        self._dict_of_files: Dict[str, List[Union[int, str, float]]] = {} # Словарь для DataFrame с данными
 
-        self._df_accuracy: pd.DataFrame = pd.DataFrame()  # DataFrame с результатами вычисления точности
+        self._df_accuracy: pd.DataFrame = pd.DataFrame() # DataFrame с результатами вычисления точности
         # Словарь для DataFrame с результатами вычисления точности
         self._dict_of_accuracy: Dict[str, List[Union[int, float]]] = {}
 
-        self._keys_id: str = "Person ID"  # Идентификатор
-        self._keys_score: str = "Candidate score"  # Комплексная оценка кандидатов
-        self._keys_colleague: str = "Match"
-        self._keys_priority: str = "Priority"  # Приоритетные предпочтения
+        self._keys_id: str = 'ID' # Идентификатор
+        self._keys_score: str = 'Candidate score' # Комплексная оценка кандидатов
+        self._keys_priority: str = 'Priority' # Приоритетные предпочтения
         # Наиболее важные качества влияющие на приоритетные предпочтения
-        self._keys_trait_importance: str = "Trait importance"
+        self._keys_trait_importance: str = 'Trait importance'
 
-        self._ext_for_logs: str = ".csv"  # Расширение для сохранения lOG файлов
+        self._ext_for_logs: str = '.csv' # Расширение для сохранения lOG файлов
 
         # Тип файла с META информацией
         self._type_meta_info: Dict[str, List[str]] = {
-            "Video": [
-                "format",
-                "duration",
-                "other_width",
-                "other_height",
-                "other_display_aspect_ratio",
-                "minimum_frame_rate",
-                "frame_rate",
-                "maximum_frame_rate",
-                "other_bit_rate",
-                "encoded_date",
-            ]
+            'Video': ['format', 'duration', 'other_width', 'other_height', 'other_display_aspect_ratio',
+                      'minimum_frame_rate', 'frame_rate', 'maximum_frame_rate', 'other_bit_rate', 'encoded_date']
         }
 
-        self._device = "cuda:0" if torch.cuda.is_available() else "cpu"
-
-        self._colleague: List[str] = ["major", "minor"]
-
         # ----------------------- Только для внутреннего использования внутри класса
 
-        self.__tab: str = "&nbsp;" * 4  # Табуляция (в виде пробелов)
+        self.__tab: str = '&nbsp;' * 4 # Табуляция (в виде пробелов)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     @property
     def is_notebook_(self) -> bool:
@@ -611,14 +476,15 @@
                 | 6  | SciPy        | 1.9.3   |
                 | 7  | Pandas       | 1.5.2   |
                 | 8  | Scikit-learn | 1.1.3   |
                 | 9  | OpenSmile    | 2.4.1   |
                 | 10 | Librosa      | 0.9.2   |
                 | 11 | AudioRead    | 3.0.0   |
                 | 12 | IPython      | 8.7.0   |
+                | 13 | PyMediaInfo  | 6.0.1   |
                 | 14 | Requests     | 2.28.1  |
                 | 15 | JupyterLab   | 3.5.0   |
                 |----|--------------|---------|
         """
 
         return self._df_pkgs
 
@@ -706,34 +572,14 @@
 
                 0
         """
 
         return self._df_files_priority
 
     @property
-    def df_files_colleague_(self) -> pd.DataFrame:
-        """Получение DataFrame c ранжированными коллегами на основе данных
-
-        Returns:
-            pd.DataFrame: **DataFrame** c данными
-        """
-
-        return self._df_files_colleague
-
-    @property
-    def df_files_priority_skill_(self) -> pd.DataFrame:
-        """Получение DataFrame c ранжированными коллегами на основе данных
-
-        Returns:
-            pd.DataFrame: **DataFrame** c данными
-        """
-
-        return self._df_files_priority_skill
-
-    @property
     def df_accuracy_(self) -> pd.DataFrame:
         """Получение DataFrame с результатами вычисления точности
 
         Returns:
             pd.DataFrame: **DataFrame** с результатами вычисления точности
 
         .. dropdown:: Пример
@@ -802,15 +648,15 @@
                             },
                             'extraversion': {
                                 'sberdisk': 'https://download.sberdisk.ru/download/file/405034830?token=3daBSTYnmZaesee&filename=weights_2022-06-15_16-26-41.h5',
                             },
                             'agreeableness': {
                                 'sberdisk': 'https://download.sberdisk.ru/download/file/405034397?token=52ZPHMjb4CFmdYa&filename=weights_2022-06-15_16-32-51.h5',
                             },
-                            'non_neuroticism': {
+                            'neuroticism': {
                                 'sberdisk': 'https://download.sberdisk.ru/download/file/405035156?token=q8CZJ99rZqcNxkM&filename=weights_2022-06-15_16-37-46.h5',
                             },
                         },
                     },
                     'video': {
                         'hc': {
                             'sberdisk': 'https://download.sberdisk.ru/download/file/412059444?token=JXerCfAjJZg6crD&filename=weights_2022-08-27_18-53-35.h5',
@@ -830,15 +676,15 @@
                             },
                             'extraversion': {
                                 'sberdisk': 'https://download.sberdisk.ru/download/file/415127012?token=s5aTwbt8DBkt7G4&filename=weights_2022-06-15_16-54-06.h5',
                             },
                             'agreeableness': {
                                 'sberdisk': 'https://download.sberdisk.ru/download/file/415126845?token=joN7TMHk59Gffsf&filename=weights_2022-06-15_17-02-03.h5',
                             },
-                            'non_neuroticism': {
+                            'neuroticism': {
                                 'sberdisk': 'https://download.sberdisk.ru/download/file/415127032?token=NEBSsE7mjyjen3o&filename=weights_2022-06-15_17-06-15.h5',
                             }
                         }
                     }
                 }
         """
 
@@ -920,21 +766,21 @@
                     'filename': '/var/folders/gw/w3k5kxtx0s3_nqdqw94zr8yh0000gn/T/ipykernel_22253/4179594971.py',
                     'lineno': 6,
                     'name': '<cell line: 6>',
                     'type': 'Exception'
                 }
         """
 
-        exc_type, exc_value, exc_traceback = sys.exc_info()  # Получение информации об ошибке
+        exc_type, exc_value, exc_traceback = sys.exc_info() # Получение информации об ошибке
 
         _trac = {
-            "filename": exc_traceback.tb_frame.f_code.co_filename,
-            "lineno": exc_traceback.tb_lineno,
-            "name": exc_traceback.tb_frame.f_code.co_name,
-            "type": exc_type.__name__,
+            'filename': exc_traceback.tb_frame.f_code.co_filename,
+            'lineno': exc_traceback.tb_lineno,
+            'name': exc_traceback.tb_frame.f_code.co_name,
+            'type': exc_type.__name__
         }
 
         return _trac
 
     def _notebook_display_markdown(self, message: str, last: bool = False, out: bool = True) -> None:
         """Отображение сообщения
 
@@ -986,30 +832,25 @@
 
                 [2022-10-14 15:52:03] Неверные типы или значения аргументов в "Core._notebook_display_markdown" ...
         """
 
         if self.is_notebook_ is True:
             try:
                 # Проверка аргументов
-                if type(message) is not str or not message:
-                    raise TypeError
+                if type(message) is not str or not message: raise TypeError
             except TypeError:
-                self._inv_args(__class__.__name__, self._notebook_display_markdown.__name__, out=out)
-                return None
+                self._inv_args(__class__.__name__, self._notebook_display_markdown.__name__, out = out); return None
 
-            if type(last) is not bool:
-                last = False
+            if type(last) is not bool: last = False
 
-            self._add_notebook_history_output(message, last)  # Добавление истории вывода сообщений в ячейке Jupyter
+            self._add_notebook_history_output(message, last) # Добавление истории вывода сообщений в ячейке Jupyter
 
-            if type(out) is not bool:
-                out = True
+            if type(out) is not bool: out = True
 
-            if out is True:
-                display(Markdown(message))  # Отображение
+            if out is True: display(Markdown(message)) # Отображение
 
     def _metadata_info(self, last: bool = False, out: bool = True) -> None:
         """Информация об библиотеке
 
         .. note::
             protected (защищенный метод)
 
@@ -1076,51 +917,43 @@
                     Версия: 1.0.0-a7
                     Лицензия: GPLv3
         """
 
         if self.is_notebook_ is True:
             tab = self.__tab
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
             cr = self.color_simple_
 
-            generate_name_with_email = lambda list1, list2: "".join(
-                map(
-                    str,
-                    map(
-                        lambda l1, l2: f'<br /><span style="color:{cr}">{tab * 2}{l1} [<u>{l2}</u>]</span>',
-                        list1.split(", "),
-                        list2.split(", "),
-                    ),
-                )
+            generate_name_with_email = lambda list1, list2: ''.join(
+                map(str, map(
+                    lambda l1, l2: f'<br /><span style=\"color:{cr}\">{tab * 2}{l1} [<u>{l2}</u>]</span>',
+                    list1.split(', '), list2.split(', ')
+                ))
             )
 
             author = generate_name_with_email(
-                oceanai.__author__ru__ if self.lang_ == "ru" else oceanai.__author__en__, oceanai.__email__
+                oceanai.__author__ru__ if self.lang_ == 'ru' else oceanai.__author__en__, oceanai.__email__
             )
             maintainer = generate_name_with_email(
-                oceanai.__maintainer__ru__ if self.lang_ == "ru" else oceanai.__maintainer__en__,
-                oceanai.__maintainer_email__,
+                oceanai.__maintainer__ru__ \
+                    if self.lang_ == 'ru' else oceanai.__maintainer__en__, oceanai.__maintainer_email__
             )
 
             # Отображение сообщения
-            self._notebook_display_markdown(
-                ("{}" * 8).format(
-                    f'<span style="color:{self.color_simple_}">{b}[</span><span style="color:{self.color_info_}">',
-                    datetime.now().strftime(self._format_time),
-                    f'</span><span style="color:{self.color_simple_}">]</span> ',
-                    f'<span style="color:{self.color_simple_}">{self._metadata[0]}:</span>{b}',
-                    f'<br /><span style="color:{cr}">{tab}{self._metadata[1]}:</span>{author}',
-                    f'<br /><span style="color:{cr}">{tab}{self._metadata[2]}:</span>{maintainer}',
-                    f'<br /><span style="color:{cr}">{tab}{self._metadata[3]}: <u>{oceanai.__release__}</u></span>',
-                    f'<br /><span style="color:{cr}">{tab}{self._metadata[4]}: <u>{oceanai.__license__}</u></span></p>',
-                ),
-                last,
-                out,
-            )
+            self._notebook_display_markdown(('{}' * 8).format(
+                f'<span style=\"color:{self.color_simple_}\">{b}[</span><span style=\"color:{self.color_info_}\">',
+                datetime.now().strftime(self._format_time),
+                f'</span><span style=\"color:{self.color_simple_}\">]</span> ',
+                f'<span style=\"color:{self.color_simple_}\">{self._metadata[0]}:</span>{b}',
+                f'<br /><span style=\"color:{cr}\">{tab}{self._metadata[1]}:</span>{author}',
+                f'<br /><span style=\"color:{cr}\">{tab}{self._metadata[2]}:</span>{maintainer}',
+                f'<br /><span style=\"color:{cr}\">{tab}{self._metadata[3]}: <u>{oceanai.__release__}</u></span>',
+                f'<br /><span style=\"color:{cr}\">{tab}{self._metadata[4]}: <u>{oceanai.__license__}</u></span></p>'
+            ), last, out)
 
     def _inv_args(self, class_name: str, build_name: str, last: bool = False, out: bool = True) -> None:
         """Сообщение об указании неверных типов аргументов
 
         .. note::
             protected (защищенный метод)
 
@@ -1175,37 +1008,29 @@
         """
 
         if self.is_notebook_ is True:
             try:
                 # Проверка аргументов
                 if type(class_name) is not str or not class_name or type(build_name) is not str or not build_name:
                     raise TypeError
-            except TypeError:
-                class_name, build_name = __class__.__name__, self._inv_args.__name__
+            except TypeError: class_name, build_name = __class__.__name__, self._inv_args.__name__
 
-            inv_args = self._invalid_arguments.format(class_name + "." + build_name)
+            inv_args = self._invalid_arguments.format(class_name + '.' + build_name)
 
-            if len(inv_args) == 0:
-                inv_args = self._invalid_arguments_empty
+            if len(inv_args) == 0: inv_args = self._invalid_arguments_empty
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
 
             # Отображение сообщения
-            self._notebook_display_markdown(
-                "{}[{}{}{}] {}{}".format(
-                    f'<span style="color:{self.color_simple_}">{b}',
-                    f'</span><span style="color:{self.color_err_}">',
-                    datetime.now().strftime(self._format_time),
-                    f'</span><span style="color:{self.color_simple_}">',
-                    inv_args,
-                    f"{b}</span>",
-                ),
-                last,
-                out,
-            )
+            self._notebook_display_markdown('{}[{}{}{}] {}{}'.format(
+                f'<span style=\"color:{self.color_simple_}\">{b}',
+                f'</span><span style=\"color:{self.color_err_}\">',
+                datetime.now().strftime(self._format_time),
+                f'</span><span style=\"color:{self.color_simple_}\">', inv_args, f'{b}</span>'
+            ), last, out)
 
     def _info(self, message: str, last: bool = False, out: bool = True) -> None:
         """Информационное сообщение
 
         .. note::
             protected (защищенный метод)
 
@@ -1272,33 +1097,26 @@
 
                 [2022-10-14 11:43:00] Неверные типы или значения аргументов в "Core._info" ...
         """
 
         if self.is_notebook_ is True:
             try:
                 # Проверка аргументов
-                if type(message) is not str or not message:
-                    raise TypeError
-            except TypeError:
-                self._inv_args(__class__.__name__, self._info.__name__, out=out)
-                return None
+                if type(message) is not str or not message: raise TypeError
+            except TypeError: self._inv_args(__class__.__name__, self._info.__name__, out = out); return None
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
 
             # Отображение сообщения
-            self._notebook_display_markdown(
-                ("{}" * 4).format(
-                    f'<span style="color:{self.color_simple_}">{b}[</span><span style="color:{self.color_info_}">',
-                    datetime.now().strftime(self._format_time),
-                    f'</span><span style="color:{self.color_simple_}">]</span> ',
-                    f'<span style="color:{self.color_simple_}">{message}</span>{b} ',
-                ),
-                last,
-                out,
-            )
+            self._notebook_display_markdown(('{}' * 4).format(
+                f'<span style=\"color:{self.color_simple_}\">{b}[</span><span style=\"color:{self.color_info_}\">',
+                datetime.now().strftime(self._format_time),
+                f'</span><span style=\"color:{self.color_simple_}\">]</span> ',
+                f'<span style=\"color:{self.color_simple_}\">{message}</span>{b} '
+            ), last, out)
 
     def _info_wrapper(self, message: str) -> str:
         """Обернутое информационное сообщение
 
         .. note::
             protected (защищенный метод)
 
@@ -1330,15 +1148,15 @@
                 :linenos:
 
                 <span style="color:#1776D2">Обернутое информационное сообщение 1</span>
                 <span style="color:#0B45B9">Обернутое информационное сообщение 2</span>
         """
 
         if self.is_notebook_ is True:
-            return ("{}" * 3).format(f'<span style="color:{self.color_info_}">', message, f"</span>")
+            return ('{}' * 3).format(f'<span style=\"color:{self.color_info_}\">', message, f'</span>')
 
     # Положительная информация
     def _info_true(self, message: str, last: bool = False, out: bool = True) -> None:
         """Положительная информация
 
         .. note::
             protected (защищенный метод)
@@ -1406,26 +1224,22 @@
 
                 [2022-10-22 16:46:56] Неверные типы или значения аргументов в "Core._info_true" ...
         """
 
         if self.is_notebook_ is True:
             try:
                 # Проверка аргументов
-                if type(message) is not str or not message:
-                    raise TypeError
-            except TypeError:
-                self._inv_args(__class__.__name__, self._info_true.__name__, out=out)
-                return None
+                if type(message) is not str or not message: raise TypeError
+            except TypeError: self._inv_args(__class__.__name__, self._info_true.__name__, out = out); return None
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
 
             # Отображение сообщения
             self._notebook_display_markdown(
-                "{}".format(f'<span style="color:{self.color_true_}">{b}{message}{b}</span>'), last, out
-            )
+                '{}'.format(f'<span style=\"color:{self.color_true_}\">{b}{message}{b}</span>'), last, out)
 
     def _bold_wrapper(self, message: str) -> str:
         """Обернутое сообщение с жирным начертанием
 
         .. note::
             protected (защищенный метод)
 
@@ -1461,17 +1275,17 @@
                 :linenos:
 
                 <span style="color:#666">Обернутое сообщение без жирного начертания</span>
                 <span style="color:#666">**Обернутое сообщение с жирным начертанием**</span>
         """
 
         if self.is_notebook_ is True:
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
 
-            return ("{}" * 3).format(f'<span style="color:{self.color_simple_}">{b}', message, f"{b}</span>")
+            return ('{}' * 3).format(f'<span style=\"color:{self.color_simple_}\">{b}', message, f'{b}</span>')
 
     def _error(self, message: str, last: bool = False, out: bool = True) -> None:
         """Сообщение об ошибке
 
         .. note::
             protected (защищенный метод)
 
@@ -1538,35 +1352,26 @@
 
                 [2022-10-12 17:06:04] Неверные типы или значения аргументов в "Core._error" ...
         """
 
         if self.is_notebook_ is True:
             try:
                 # Проверка аргументов
-                if type(message) is not str or not message:
-                    raise TypeError
-            except TypeError:
-                self._inv_args(__class__.__name__, self._error.__name__, out=out)
-                return None
+                if type(message) is not str or not message: raise TypeError
+            except TypeError: self._inv_args(__class__.__name__, self._error.__name__, out = out); return None
 
-            b = "**" if self.bold_text_ is True else ""
+
+            b = '**' if self.bold_text_ is True else ''
 
             # Отображение сообщения
-            self._notebook_display_markdown(
-                "{}[{}{}{}] {}{}".format(
-                    f'<span style="color:{self.color_simple_}">{b}',
-                    f'</span><span style="color:{self.color_err_}">',
-                    datetime.now().strftime(self._format_time),
-                    f'</span><span style="color:{self.color_simple_}">',
-                    message,
-                    f"{b}</span>",
-                ),
-                last,
-                out,
-            )
+            self._notebook_display_markdown('{}[{}{}{}] {}{}'.format(
+                f'<span style=\"color:{self.color_simple_}\">{b}', f'</span><span style=\"color:{self.color_err_}\">',
+                datetime.now().strftime(self._format_time),
+                f'</span><span style=\"color:{self.color_simple_}\">', message, f'{b}</span>'
+            ), last, out)
 
     def _other_error(self, message: str, last: bool = False, out: bool = True) -> None:
         """Сообщение об прочей ошибке
 
         .. note::
             protected (защищенный метод)
 
@@ -1652,42 +1457,33 @@
 
                 [2022-10-14 16:25:11] Неверные типы или значения аргументов в "Core._other_error" ...
         """
 
         if self.is_notebook_ is True:
             try:
                 # Проверка аргументов
-                if type(message) is not str or not message:
-                    raise TypeError
-            except TypeError:
-                self._inv_args(__class__.__name__, self._other_error.__name__, out=out)
-                return None
+                if type(message) is not str or not message: raise TypeError
+            except TypeError: self._inv_args(__class__.__name__, self._other_error.__name__, out = out); return None
 
-            trac = self._traceback()  # Трассировка исключений
+            trac = self._traceback() # Трассировка исключений
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
             cr = self.color_simple_
 
             # Отображение сообщения
-            self._notebook_display_markdown(
-                ("{}" * 8).format(
-                    f'<span style="color:{cr}">{b}[</span><span style="color:{self.color_err_}">',
-                    datetime.now().strftime(self._format_time),
-                    f'</span><span style="color:{cr}">]</span> ',
-                    f'<span style="color:{cr}">{message}</span>{b}',
-                    f"<p>",
-                    f'<span style="color:{cr}">{self.__tab}{self._trac_file}: <u>{trac["filename"]}</u></span>',
-                    f'<br /><span style="color:{cr}">{self.__tab}{self._trac_line}: <u>{trac["lineno"]}</u></span>',
-                    f'<br /><span style="color:{cr}">{self.__tab}{self._trac_method}: <u>{trac["name"]}</u></span>',
-                    f'<br /><span style="color:{cr}">{self.__tab}{self._trac_type_err}: <u>{trac["type"]}</u></span>',
-                    f"</p>",
-                ),
-                last,
-                out,
-            )
+            self._notebook_display_markdown(('{}' * 8).format(
+                f'<span style=\"color:{cr}\">{b}[</span><span style=\"color:{self.color_err_}\">',
+                datetime.now().strftime(self._format_time),
+                f'</span><span style=\"color:{cr}\">]</span> ',
+                f'<span style=\"color:{cr}\">{message}</span>{b}',
+                f'<p><span style=\"color:{cr}\">{self.__tab}{self._trac_file}: <u>{trac["filename"]}</u></span>',
+                f'<br /><span style=\"color:{cr}\">{self.__tab}{self._trac_line}: <u>{trac["lineno"]}</u></span>',
+                f'<br /><span style=\"color:{cr}\">{self.__tab}{self._trac_method}: <u>{trac["name"]}</u></span>',
+                f'<br /><span style=\"color:{cr}\">{self.__tab}{self._trac_type_err}: <u>{trac["type"]}</u></span></p>'
+            ), last, out)
 
     def _error_wrapper(self, message: str) -> str:
         """Обернутое сообщение об ошибке
 
         .. note::
             protected (защищенный метод)
 
@@ -1722,19 +1518,18 @@
                 :linenos:
 
                 <span style="color:#FF0000">Обернутое сообщение об ошибке 1</span>
                 <span style="color:#FF4545">Обернутое сообщение об ошибке 2</span>
         """
 
         if self.is_notebook_ is True:
-            return ("{}" * 3).format(f'<span style="color:{self.color_err_}">', message, f"</span>")
+            return ('{}' * 3).format(f'<span style=\"color:{self.color_err_}\">', message, f'</span>')
 
-    def _stat_acoustic_features(
-        self, last: bool = False, out: bool = True, **kwargs: Union[int, Tuple[int], tf.TensorShape]
-    ) -> None:
+    def _stat_acoustic_features(self, last: bool = False, out: bool = True,
+                                **kwargs: Union[int, Tuple[int], tf.TensorShape]) -> None:
         """Сообщение со статистикой извлеченных признаков из акустического сигнала
 
         .. note::
             protected (защищенный метод)
 
         Args:
             last (bool): Замена последнего сообщения
@@ -1807,48 +1602,39 @@
 
                 [2022-10-14 17:59:21] Неверные типы или значения аргументов в "Core._stat_acoustic_features" ...
         """
 
         if self.is_notebook_ is True:
             tab = self.__tab
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
             cr = self.color_simple_
 
             try:
                 # Отображение сообщения
-                self._notebook_display_markdown(
-                    self._get_acoustic_feature_stat.format(
-                        f'<span style="color:{cr}">{b}[</span><span style="color:{self.color_info_}">',
-                        datetime.now().strftime(self._format_time),
-                        f'</span><span style="color:{cr}">]</span> ',
-                        f'<span style="color:{cr}">',
-                        f'</span>{b}<br /><span style="color:{cr}">{tab}',
-                        f'</span><br /><span style="color:{cr}">{tab * 2}',
-                        f'<u>{kwargs["len_hc_features"]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab * 2}',
-                        f'<u>{kwargs["len_melspectrogram_features"]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab}',
-                        f'<u>{kwargs["shape_hc_features"][0]}</u>',
-                        f'<u>{kwargs["shape_hc_features"][1]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab}',
-                        f' <u>{kwargs["shape_melspectrogram_features"][0]}</u>',
-                        f'<u>{kwargs["shape_melspectrogram_features"][1]}</u>',
-                        f'<u>{kwargs["shape_melspectrogram_features"][2]}</u></span>',
-                    ),
-                    last,
-                    out,
-                )
+                self._notebook_display_markdown(self._get_acoustic_feature_stat.format(
+                    f'<span style=\"color:{cr}\">{b}[</span><span style=\"color:{self.color_info_}\">',
+                    datetime.now().strftime(self._format_time),
+                    f'</span><span style=\"color:{cr}\">]</span> ', f'<span style=\"color:{cr}\">',
+                    f'</span>{b}<br /><span style=\"color:{cr}\">{tab}',
+                    f'</span><br /><span style=\"color:{cr}\">{tab * 2}', f'<u>{kwargs["len_hc_features"]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab * 2}',
+                    f'<u>{kwargs["len_melspectrogram_features"]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab}',
+                    f'<u>{kwargs["shape_hc_features"][0]}</u>', f'<u>{kwargs["shape_hc_features"][1]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab}',
+                    f' <u>{kwargs["shape_melspectrogram_features"][0]}</u>',
+                    f'<u>{kwargs["shape_melspectrogram_features"][1]}</u>',
+                    f'<u>{kwargs["shape_melspectrogram_features"][2]}</u></span>',
+                ), last, out)
             except KeyError:
-                self._inv_args(__class__.__name__, self._stat_acoustic_features.__name__, out=out)
-                return None
+                self._inv_args(__class__.__name__, self._stat_acoustic_features.__name__, out = out); return None
 
-    def _stat_visual_features(
-        self, last: bool = False, out: bool = True, **kwargs: Union[int, Tuple[int], tf.TensorShape]
-    ) -> None:
+    def _stat_visual_features(self, last: bool = False, out: bool = True,
+                              **kwargs: Union[int, Tuple[int], tf.TensorShape]) -> None:
         """Сообщение c статистикой извлеченных признаков из визуального сигнала
 
         .. note::
             protected (защищенный метод)
 
         Args:
             last (bool): Замена последнего сообщения
@@ -1924,110 +1710,36 @@
 
                 [2022-11-03 16:19:35] Неверные типы или значения аргументов в "Core._stat_visual_features" ...
         """
 
         if self.is_notebook_ is True:
             tab = self.__tab
 
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
             cr = self.color_simple_
 
             try:
                 # Отображение сообщения
-                self._notebook_display_markdown(
-                    self._get_visual_feature_stat.format(
-                        f'<span style="color:{cr}">{b}[</span><span style="color:{self.color_info_}">',
-                        datetime.now().strftime(self._format_time),
-                        f'</span><span style="color:{cr}">]</span> ',
-                        f'<span style="color:{cr}">',
-                        f'</span>{b}<br /><span style="color:{cr}">{tab}',
-                        f'</span><br /><span style="color:{cr}">{tab * 2}',
-                        f'<u>{kwargs["len_hc_features"]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab * 2}',
-                        f'<u>{kwargs["len_nn_features"]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab}',
-                        f'<u>{kwargs["shape_hc_features"][0]}</u>',
-                        f'<u>{kwargs["shape_hc_features"][1]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab}',
-                        f' <u>{kwargs["shape_nn_features"][0]}</u>',
-                        f'<u>{kwargs["shape_nn_features"][1]}</u></span>',
-                        f'<br /><span style="color:{cr}">{tab}',
-                        f' <u>{kwargs["fps_before"]}</u>',
-                        f'<u>{kwargs["fps_after"]}</u></span>',
-                    ),
-                    last,
-                    out,
-                )
-            except KeyError:
-                self._inv_args(__class__.__name__, self._stat_visual_features.__name__, out=out)
-                return None
-
-    def _stat_text_features(
-        self, last: bool = False, out: bool = True, **kwargs: Union[int, Tuple[int], tf.TensorShape]
-    ) -> None:
-        """Сообщение c статистикой извлеченных признаков из текста
-
-        .. note::
-            protected (защищенный метод)
-
-        Args:
-            last (bool): Замена последнего сообщения
-            out (bool): Отображение
-            **kwargs (Union[int, Tuple[int], tf.TensorShape]): Дополнительные именованные аргументы
-
-        Returns:
-            None
-        """
-
-        if self.is_notebook_ is True:
-            tab = self.__tab
-
-            b = "**" if self.bold_text_ is True else ""
-            cr = self.color_simple_
-
-            try:
-                if not kwargs["text"]:
-                    self._notebook_display_markdown(
-                        self._get_text_feature_stat.format(
-                            f'<span style="color:{cr}">{b}[</span><span style="color:{self.color_info_}">',
-                            datetime.now().strftime(self._format_time),
-                            f'</span><span style="color:{cr}">]</span> ',
-                            f'<span style="color:{cr}">',
-                            f'</span>{b}<br /><span style="color:{cr}">{tab}',
-                            f'<u>{kwargs["shape_hc_features"][0]}</u>',
-                            f'<u>{kwargs["shape_hc_features"][1]}</u></span>',
-                            f'<br /><span style="color:{cr}">{tab}',
-                            f' <u>{kwargs["shape_nn_features"][0]}</u>',
-                            f'<u>{kwargs["shape_nn_features"][1]}</u></span>',
-                        ),
-                        last,
-                        out,
-                    )
-                else:
-                    self._notebook_display_markdown(
-                        self._get_text_feature_stat_with_text.format(
-                            f'<span style="color:{cr}">{b}[</span><span style="color:{self.color_info_}">',
-                            datetime.now().strftime(self._format_time),
-                            f'</span><span style="color:{cr}">]</span> ',
-                            f'<span style="color:{cr}">',
-                            f'</span>{b}<br /><span style="color:{cr}">{tab}',
-                            f'<u>{kwargs["shape_hc_features"][0]}</u>',
-                            f'<u>{kwargs["shape_hc_features"][1]}</u></span>',
-                            f'<br /><span style="color:{cr}">{tab}',
-                            f' <u>{kwargs["shape_nn_features"][0]}</u>',
-                            f'<u>{kwargs["shape_nn_features"][1]}</u></span>',
-                            f'<br /><span style="color:{cr}">{tab}',
-                            f'<br />{tab * 2}{kwargs["text"]}</span>',
-                        ),
-                        last,
-                        out,
-                    )
+                self._notebook_display_markdown(self._get_visual_feature_stat.format(
+                    f'<span style=\"color:{cr}\">{b}[</span><span style=\"color:{self.color_info_}\">',
+                    datetime.now().strftime(self._format_time),
+                    f'</span><span style=\"color:{cr}\">]</span> ', f'<span style=\"color:{cr}\">',
+                    f'</span>{b}<br /><span style=\"color:{cr}\">{tab}',
+                    f'</span><br /><span style=\"color:{cr}\">{tab * 2}', f'<u>{kwargs["len_hc_features"]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab * 2}',
+                    f'<u>{kwargs["len_nn_features"]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab}',
+                    f'<u>{kwargs["shape_hc_features"][0]}</u>', f'<u>{kwargs["shape_hc_features"][1]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab}',
+                    f' <u>{kwargs["shape_nn_features"][0]}</u>', f'<u>{kwargs["shape_nn_features"][1]}</u></span>',
+                    f'<br /><span style=\"color:{cr}\">{tab}',
+                    f' <u>{kwargs["fps_before"]}</u>', f'<u>{kwargs["fps_after"]}</u></span>',
+                ), last, out)
             except KeyError:
-                self._inv_args(__class__.__name__, self._stat_text_features.__name__, out=out)
-                return None
+                self._inv_args(__class__.__name__, self._stat_visual_features.__name__, out = out); return None
 
     def _r_start(self) -> None:
         """Начало отсчета времени выполнения
 
         .. note::
             protected (защищенный метод)
 
@@ -2074,17 +1786,17 @@
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
                 --- Время выполнения: 1665756222.704 сек. ---
         """
 
-        self._runtime = self._start_time = -1  # Сброс значений
+        self._runtime = self._start_time = -1 # Сброс значений
 
-        self._start_time = time.time()  # Отсчет времени выполнения
+        self._start_time = time.time() # Отсчет времени выполнения
 
     def _r_end(self, last: bool = False, out: bool = True) -> None:
         """Конец отсчета времени выполнения
 
         .. note::
             protected (защищенный метод)
 
@@ -2135,28 +1847,27 @@
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
                 --- Время выполнения: 1665756222.704 сек. ---
         """
 
-        self._runtime = round(time.time() - self._start_time, 3)  # Время выполнения
+        self._runtime = round(time.time() - self._start_time, 3) # Время выполнения
 
-        t = "--- {}: {} {} ---".format(self.text_runtime_, self._runtime, self._sec)
+        t = '--- {}: {} {} ---'.format(self.text_runtime_, self._runtime, self._sec)
 
         if self.is_notebook_ is True:
-            b = "**" if self.bold_text_ is True else ""
+            b = '**' if self.bold_text_ is True else ''
 
             # Отображение сообщения
             self._notebook_display_markdown(
-                "{}".format(f'<span style="color:{self.color_simple_}">{b}{t}{b}</span>'), last, out
-            )
+                '{}'.format(f'<span style=\"color:{self.color_simple_}\">{b}{t}{b}</span>'), last, out)
 
     def _progressbar(
-        self, message: str, progress: str, clear_out: bool = True, last: bool = False, out: bool = True
+            self, message: str, progress: str, clear_out: bool = True, last: bool = False, out: bool = True
     ) -> None:
         """Индикатор выполнения
 
         .. note::
             protected (защищенный метод)
 
         Args:
@@ -2257,50 +1968,36 @@
                 :execution-count: 3
                 :linenos:
 
                 [2022-10-14 16:52:38] Неверные типы или значения аргументов в "Core._progressbar" ...
         """
 
         if self.is_notebook_ is True:
-            if clear_out is True:
-                clear_output(True)
+            if clear_out is True: clear_output(True)
 
             try:
                 # Проверка аргументов
-                if type(message) is not str or not message or type(progress) is not str or not progress:
-                    raise TypeError
-            except TypeError:
-                self._inv_args(__class__.__name__, self._progressbar.__name__, out=out)
-                return None
+                if type(message) is not str or not message or type(progress) is not str or not progress: raise TypeError
+            except TypeError: self._inv_args(__class__.__name__, self._progressbar.__name__, out = out); return None
 
-            b = "**" if self.bold_text is True else ""
+            b = '**' if self.bold_text is True else ''
             tab = self.__tab
 
             # Отображение сообщения
-            self._notebook_display_markdown(
-                ("{}" * 5).format(
-                    f'<span style="color:{self.color_simple_}">{b}[</span><span style="color:{self.color_info_}">',
-                    datetime.now().strftime(self._format_time),
-                    f'</span><span style="color:{self.color_simple_}">]</span> ',
-                    f'<span style="color:{self.color_simple_}">{message}</span>{b}',
-                    f'<p><span style="color:{self.color_simple_}">{tab}{progress}</span></p>',
-                ),
-                last,
-                out,
-            )
+            self._notebook_display_markdown(('{}' * 5).format(
+                f'<span style=\"color:{self.color_simple_}\">{b}[</span><span style=\"color:{self.color_info_}\">',
+                datetime.now().strftime(self._format_time),
+                f'</span><span style=\"color:{self.color_simple_}\">]</span> ',
+                f'<span style=\"color:{self.color_simple_}\">{message}</span>{b}',
+                f'<p><span style=\"color:{self.color_simple_}\">{tab}{progress}</span></p>'
+            ), last, out)
 
     def _progressbar_union_predictions(
-        self,
-        message: str,
-        item: int,
-        info: str,
-        len_paths: int,
-        clear_out: bool = True,
-        last: bool = False,
-        out: bool = True,
+        self, message: str, item: int, info: str, len_paths: int, clear_out: bool = True, last: bool = False,
+            out: bool = True
     ) -> None:
         """Индикатор выполнения получения прогнозов по аудио
 
         .. note::
             private (приватный метод)
 
         Args:
@@ -2415,45 +2112,35 @@
                 :execution-count: 3
                 :linenos:
 
                 [2022-10-20 16:55:15] Неверные типы или значения аргументов в "Audio._progressbar_union_predictions" ...
         """
 
         if self.is_notebook_ is True:
-            if clear_out is False and last is True:
-                clear_out, last = last, clear_out
-            elif clear_out is False and last is False:
-                clear_out = True
-            if clear_out is True:
-                clear_output(True)
+            if clear_out is False and last is True: clear_out, last = last, clear_out
+            elif clear_out is False and last is False: clear_out = True
+            if clear_out is True: clear_output(True)
 
             try:
                 # Проверка аргументов
-                if (
-                    type(message) is not str
-                    or not message
-                    or type(item) is not int
-                    or type(len_paths) is not int
-                    or type(info) is not str
-                    or not info
-                ):
-                    raise TypeError
+                if (type(message) is not str or not message or type(item) is not int or type(len_paths) is not int
+                    or type(info) is not str or not info): raise TypeError
             except TypeError:
-                self._inv_args(__class__.__name__, self._progressbar_union_predictions.__name__, out=out)
+                self._inv_args(__class__.__name__, self._progressbar_union_predictions.__name__, out = out)
                 return None
 
             self._progressbar(
                 message,
-                self._curr_progress_union_predictions.format(item, len_paths, round(item * 100 / len_paths, 2), info),
-                clear_out=clear_out,
-                last=last,
-                out=False,
+                self._curr_progress_union_predictions.format(
+                    item, len_paths, round(item * 100 / len_paths, 2), info
+                ),
+                clear_out = clear_out,
+                last = last, out = False
             )
-            if out:
-                self.show_notebook_history_output()
+            if out: self.show_notebook_history_output()
 
     def _clear_notebook_history_output(self) -> None:
         """Очистка истории вывода сообщений в ячейке Jupyter
 
         .. note::
             protected (защищенный метод)
 
@@ -2486,15 +2173,15 @@
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
 
         """
 
-        self._notebook_history_output.clear()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._notebook_history_output.clear() # Очистка истории вывода сообщений в ячейке Jupyter
 
     def _add_notebook_history_output(self, message: str, last: bool = False) -> None:
         """Добавление истории вывода сообщений в ячейке Jupyter
 
         .. note::
             protected (защищенный метод)
 
@@ -2566,20 +2253,17 @@
                 :linenos:
 
                 Сообщение 1
                 Замена последнего сообщения
         """
 
         if last is True:
-            try:
-                self._notebook_history_output[-1] = message
-            except Exception:
-                pass
-            else:
-                return None
+            try: self._notebook_history_output[-1] = message
+            except Exception: pass
+            else: return None
 
         self._notebook_history_output.append(message)
 
     def _del_last_el_notebook_history_output(self) -> None:
         """Удаление последнего сообщения из истории вывода сообщений в ячейке Jupyter
 
         .. note::
@@ -2614,18 +2298,16 @@
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
                 Сообщение 1
         """
 
-        try:
-            last_el = self._notebook_history_output.pop()
-        except Exception:
-            pass
+        try: last_el = self._notebook_history_output.pop()
+        except Exception: pass
 
     def _add_last_el_notebook_history_output(self, message: str) -> None:
         """Добавление текста к последнему сообщению из истории вывода сообщений в ячейке Jupyter
 
         .. note::
             protected (защищенный метод)
 
@@ -2660,18 +2342,16 @@
                 :execution-count: 1
                 :linenos:
 
                 ...
                 Сообщение 1 ...
         """
 
-        try:
-            self._notebook_history_output[-1] += " " + message
-        except Exception:
-            self._add_notebook_history_output(message=message, last=False)
+        try: self._notebook_history_output[-1] += ' ' + message
+        except Exception: self._add_notebook_history_output(message = message, last = False)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (приватные)
     # ------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def __is_notebook() -> bool:
@@ -2718,28 +2398,23 @@
 
                 True
         """
 
         try:
             # Определение режима запуска библиотеки
             shell = get_ipython().__class__.__name__
-        except (NameError, Exception):
-            return False  # Запуск в Python
+        except (NameError, Exception): return False # Запуск в Python
         else:
-            if shell == "ZMQInteractiveShell" or shell == "Shell":
-                return True
-            elif shell == "TerminalInteractiveShell":
-                return False
-            else:
-                return False
+            if shell == 'ZMQInteractiveShell' or shell == 'Shell': return True
+            elif shell == 'TerminalInteractiveShell': return False
+            else: return False
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (защищенные)
     # ------------------------------------------------------------------------------------------------------------------
-
     def _get_paths(self, path: Iterable, depth: int = 1, out: bool = True) -> Union[List[str], bool]:
         """Получение директорий где хранятся данные
 
         .. note::
             protected (защищенный метод)
 
         Args:
@@ -2822,123 +2497,46 @@
                     Тип ошибки: FileNotFoundError
 
                 False
         """
 
         try:
             # Проверка аргументов
-            if (
-                not isinstance(path, Iterable)
-                or not path
-                or type(depth) is not int
-                or depth < 1
-                or type(out) is not bool
-            ):
+            if (not isinstance(path, Iterable) or not path or type(depth) is not int or depth < 1
+                    or type(out) is not bool):
                 raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self._get_paths.__name__, out=out)
-            return False
+        except TypeError: self._inv_args(__class__.__name__, self._get_paths.__name__, out = out); return False
         else:
-            if type(path) is not list:
-                path = [path]
+            if type(path) is not list: path = [path]
 
-            new_path = []  # Список с директориями
+            new_path = [] # Список с директориями
 
             # Проход по всем директориям набора данных
             for curr_path in path:
-                try:
-                    scandir = os.scandir(os.path.normpath(str(curr_path)))
+                try: scandir = os.scandir(os.path.normpath(str(curr_path)))
                 except FileNotFoundError:
-                    self._other_error(self._folder_not_found.format(self._info_wrapper(str(curr_path))), out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
+                    self._other_error(self._folder_not_found.format(self._info_wrapper(str(curr_path))), out = out)
                     return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
                 else:
                     for f in scandir:
-                        if f.is_dir() and not f.name.startswith("."):
-                            ignore = False  # По умолчанию не игнорировать директорию
+                        if f.is_dir() and not f.name.startswith('.'):
+                            ignore = False # По умолчанию не игнорировать директорию
                             if depth == 1:
                                 for curr_dir in self.ignore_dirs_:
-                                    if type(curr_dir) is not str:
-                                        continue
+                                    if type(curr_dir) is not str: continue
                                     # Игнорировать директорию
-                                    if re.search("^" + curr_dir, f.name) is not None:
-                                        ignore = True
+                                    if re.search('^' + curr_dir, f.name) is not None: ignore = True
 
-                            if ignore is False:
-                                new_path.append(f.path)
+                            if ignore is False: new_path.append(f.path)
 
             # Рекурсивный переход на следующий уровень иерархии
-            if depth != 1 and len(new_path) > 0:
-                return self._get_paths(new_path, depth - 1)
-
-            return new_path  # Список с директориями
-
-    def _search_file(self, path_to_file: str, ext: str, create: bool = False, out: bool = True) -> bool:
-        """Поиск файла
-
-        .. note::
-            protected (защищенный метод)
-
-        Args:
-            path_to_file (str): Путь к файлу
-            ext (str): Расширение файла
-            create (bool): Создание файла в случае его отсутствия
-            out (bool): Печатать процесс выполнения
-
-        Returns:
-            bool: **True** если файл найден, в обратном случае **False**
-        """
-
-        # Проверка аргументов
-        if (
-            type(path_to_file) is not str
-            or type(ext) is not str
-            or not ext
-            or type(create) is not bool
-            or type(out) is not bool
-        ):
-            self.inv_args(__class__.__name__, self._search_file.__name__, out=out)
-            return False
-
-        # Файл не передан
-        if not path_to_file:
-            self._other_error(self._file_name.format(ext.lower()), out=out)
-            return False
+            if depth != 1 and len(new_path) > 0: return self._get_paths(new_path, depth - 1)
 
-        path_to_file = os.path.normpath(path_to_file)
-        ext = ext.replace(".", "")
-
-        # Передана директория
-        if os.path.isdir(path_to_file) is True:
-            self._other_error(self._dir_found, out=out)
-            return False
-
-        self._file_load = self._file_find_hide  # Установка сообщения в исходное состояние
-
-        _, extension = os.path.splitext(path_to_file)  # Расширение файла
-
-        if ext != extension.replace(".", ""):
-            self._other_error(self._wrong_extension.format(ext), out=out)
-            return False
-
-        # Файл не найден
-        if os.path.isfile(path_to_file) is False:
-            # Создание файла
-            if create is True:
-                open(path_to_file, "a", encoding="utf-8").close()
-
-                self._other_error(self._file_not_found_create.format(os.path.basename(path_to_file)), out=out)
-                return False
-
-            self._other_error(self._file_not_found.format(os.path.basename(path_to_file)), out=out)
-            return False
-
-        return True  # Результат
+            return new_path # Список с директориями
 
     def _append_to_list_of_files(self, path: str, preds: List[Optional[float]], out: bool = True) -> bool:
         """Добавление значений в словарь для DataFrame c данными
 
         .. note::
             protected (защищенный метод)
 
@@ -3046,24 +2644,18 @@
         try:
             if len(self._dict_of_files.keys()) != len(self.keys_dataset_):
                 # Словарь для DataFrame набора данных с данными
                 self._dict_of_files = dict(zip(self.keys_dataset_, [[] for _ in range(0, len(self.keys_dataset_))]))
 
             self._dict_of_files[self.keys_dataset_[0]].append(path)
 
-            for i in range(len(preds)):
-                self._dict_of_files[self.keys_dataset_[i + 1]].append(preds[i])
-        except (IndexError, KeyError):
-            self._other_error(self._som_ww, out=out)
-            return False
-        except Exception:
-            self._other_error(self._unknown_err, out=out)
-            return False
-        else:
-            return True
+            for i in range(len(preds)): self._dict_of_files[self.keys_dataset_[i + 1]].append(preds[i])
+        except (IndexError, KeyError): self._other_error(self._som_ww, out = out); return False
+        except Exception: self._other_error(self._unknown_err, out = out); return False
+        else: return True
 
     def _append_to_list_of_accuracy(self, preds: List[Optional[float]], out: bool = True) -> bool:
         """Добавление значений в словарь для DataFrame с результатами вычисления точности
 
         .. note::
             protected (защищенный метод)
 
@@ -3164,24 +2756,18 @@
         try:
             if len(self._dict_of_accuracy.keys()) != len(self.keys_dataset_[1:]):
                 # Словарь для DataFrame набора данных с результатами вычисления точности
                 self._dict_of_accuracy = dict(
                     zip(self.keys_dataset_[1:], [[] for _ in range(0, len(self.keys_dataset_[1:]))])
                 )
 
-            for i in range(len(preds)):
-                self._dict_of_accuracy[self.keys_dataset_[i + 1]].append(preds[i])
-        except (IndexError, KeyError):
-            self._other_error(self._som_ww, out=out)
-            return False
-        except Exception:
-            self._other_error(self._unknown_err, out=out)
-            return False
-        else:
-            return True
+            for i in range(len(preds)): self._dict_of_accuracy[self.keys_dataset_[i + 1]].append(preds[i])
+        except (IndexError, KeyError): self._other_error(self._som_ww, out = out); return False
+        except Exception: self._other_error(self._unknown_err, out = out); return False
+        else: return True
 
     def _create_folder_for_logs(self, out: bool = True):
         """Создание директории для сохранения LOG файлов
 
         .. note::
             protected (защищенный метод)
 
@@ -3211,28 +2797,21 @@
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
                 true
         """
 
-        if type(out) is not bool:
-            out = True
+        if type(out) is not bool: out = True
 
         try:
-            if not os.path.exists(self.path_to_logs_):
-                os.makedirs(self.path_to_logs_)
-        except (FileNotFoundError, TypeError):
-            self._other_error(self._som_ww, out=out)
-            return False
-        except Exception:
-            self._other_error(self._unknown_err, out=out)
-            return False
-        else:
-            return True
+            if not os.path.exists(self.path_to_logs_): os.makedirs(self.path_to_logs_)
+        except (FileNotFoundError, TypeError): self._other_error(self._som_ww, out = out); return False
+        except Exception: self._other_error(self._unknown_err, out = out); return False
+        else: return True
 
     def _save_logs(self, df: pd.DataFrame, name: str, out: bool = True) -> bool:
         """Сохранение LOG файла
 
         .. note::
             protected (защищенный метод)
 
@@ -3275,35 +2854,27 @@
                 True
         """
 
         try:
             # Проверка аргументов
             if type(df) is not pd.DataFrame or type(name) is not str or not name or type(out) is not bool:
                 raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self._save_logs.__name__, out=out)
-            return False
+        except TypeError: self._inv_args(__class__.__name__, self._save_logs.__name__, out = out); return False
         else:
             # Создание директории для сохранения LOG файлов
             if self._create_folder_for_logs() is True:
                 # Сохранение LOG файла
                 try:
                     df.to_csv(os.path.join(self.path_to_logs_, name + self._ext_for_logs))
                 except urllib.error.HTTPError as e:
-                    self._other_error(
-                        self._url_error_log.format(self._url_error_code_log.format(self._error_wrapper(str(e.code)))),
-                        out=out,
-                    )
-                except urllib.error.URLError:
-                    self._other_error(self._url_error_log.format(""), out=out)
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    return True
+                    self._other_error(self._url_error_log.format(self._url_error_code_log.format(
+                        self._error_wrapper(str(e.code)))), out = out)
+                except urllib.error.URLError: self._other_error(self._url_error_log.format(''), out = out)
+                except Exception: self._other_error(self._unknown_err, out = out); return False
+                else: return True
 
             return False
 
     def _round_math(self, val: Union[int, float], out: bool = True) -> Union[int, bool]:
         """Округление чисел по математическому закону
 
         .. note::
@@ -3375,149 +2946,100 @@
                 [2022-11-03 15:52:30] Неверные типы или значения аргументов в "Core._round_math" ...
 
                 False
         """
 
         try:
             # Проверка аргументов
-            if (type(val) is not int and type(val) is not float and type(val) is not np.float64) or type(
-                out
-            ) is not bool:
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self._round_math.__name__, out=out)
-            return False
+            if ((type(val) is not int and type(val) is not float and type(val) is not np.float64)
+                or type(out) is not bool): raise TypeError
+        except TypeError: self._inv_args(__class__.__name__, self._round_math.__name__, out = out); return False
         else:
             modf = math.modf(val)
 
-            if modf[0] >= 0.5:
-                res = modf[1] + 1
+            if modf[0] >= 0.5: res = modf[1] + 1
             else:
-                if modf[0] <= -0.5:
-                    res = modf[1] - 1
-                else:
-                    res = math.ceil(modf[1])
+                if modf[0] <= -0.5: res = modf[1] - 1
+                else: res = math.ceil(modf[1])
 
             return int(res)
 
     def _candidate_ranking(
-        self,
-        weigths_openness: int = 0,
-        weigths_conscientiousness: int = 0,
-        weigths_extraversion: int = 0,
-        weigths_agreeableness: int = 0,
-        weigths_non_neuroticism: int = 0,
-        out: bool = True,
+        self, weigths_openness: int = 0, weigths_conscientiousness: int = 0, weigths_extraversion: int = 0,
+        weigths_agreeableness: int = 0, weigths_neuroticism: int = 0, out: bool = True
     ) -> pd.DataFrame:
-        """Ранжирование кандидатов по профессиональным обязанностям
+        """Ранжирование кандидатов
 
         .. note::
             protected (защищенный метод)
 
         Args:
             weigths_openness (int): Вес для ранжирования персонального качества (открытость опыту)
             weigths_conscientiousness (int): Вес для ранжирования персонального качества (добросовестность)
             weigths_extraversion (int): Вес для ранжирования персонального качества (экстраверсия)
             weigths_agreeableness (int): Вес для ранжирования персонального качества (доброжелательность)
-            weigths_non_neuroticism (int): Вес для ранжирования персонального качества (эмоциональная стабильность)
+            weigths_neuroticism (int): Вес для ранжирования персонального качества (нейротизм)
             out (bool): Отображение
 
         Returns:
              pd.DataFrame: **DataFrame** c ранжированными данными
         """
 
         # Сброс
-        self._df_files_ranking = pd.DataFrame()  # Пустой DataFrame с ранжированными данными
+        self._df_files_ranking = pd.DataFrame() # Пустой DataFrame с ранжированными данными
 
         try:
             # Проверка аргументов
-            if (
-                type(weigths_openness) is not int
-                or not (0 <= weigths_openness <= 100)
-                or type(weigths_conscientiousness) is not int
-                or not (0 <= weigths_conscientiousness <= 100)
-                or type(weigths_extraversion) is not int
-                or not (0 <= weigths_extraversion <= 100)
-                or type(weigths_agreeableness) is not int
-                or not (0 <= weigths_agreeableness <= 100)
-                or type(weigths_non_neuroticism) is not int
-                or not (0 <= weigths_non_neuroticism <= 100)
-                or type(out) is not bool
-            ):
-                raise TypeError
+            if (type(weigths_openness) is not int or not (0 <= weigths_openness <= 100)
+                or type(weigths_conscientiousness) is not int or not (0 <= weigths_conscientiousness <= 100)
+                or type(weigths_extraversion) is not int or not (0 <= weigths_extraversion <= 100)
+                or type(weigths_agreeableness) is not int or not (0 <= weigths_agreeableness <= 100)
+                or type(weigths_neuroticism) is not int or not (0 <= weigths_neuroticism <= 100)
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self._candidate_ranking.__name__, out=out)
+            self._inv_args(__class__.__name__, self._candidate_ranking.__name__, out = out)
             return self._df_files_ranking
         else:
             try:
-                if (
-                    sum(
-                        [
-                            weigths_openness,
-                            weigths_conscientiousness,
-                            weigths_extraversion,
-                            weigths_agreeableness,
-                            weigths_non_neuroticism,
-                        ]
-                    )
-                    != 100
-                ):
-                    raise TypeError
-            except TypeError:
-                self._other_error(self._sum_ranking_exceeded, out=out)
-                return self._df_files_ranking
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return self._df_files_ranking
+                if sum([
+                    weigths_openness, weigths_conscientiousness, weigths_extraversion,
+                    weigths_agreeableness, weigths_neuroticism
+                ]) != 100: raise TypeError
+            except TypeError: self._other_error(self._sum_ranking_exceeded, out = out); return self._df_files_ranking
+            except Exception: self._other_error(self._unknown_err, out = out); return self._df_files_ranking
             else:
                 try:
-                    if len(self._df_files) == 0:
-                        raise TypeError
-                except TypeError:
-                    self._other_error(self._dataframe_empty, out=out)
-                    return self._df_files_ranking
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return self._df_files_ranking
+                    if len(self._df_files) == 0: raise TypeError
+                except TypeError: self._other_error(self._dataframe_empty, out = out); return self._df_files_ranking
+                except Exception: self._other_error(self._unknown_err, out = out); return self._df_files_ranking
                 else:
                     try:
                         self._df_files_ranking = self._df_files.copy()
 
-                        df_files_ranking = self._df_files_ranking[self.keys_dataset_[1:]]
-
-                        traits_sum = np.sum(
-                            df_files_ranking.values
-                            * [
-                                weigths_openness,
-                                weigths_conscientiousness,
-                                weigths_extraversion,
-                                weigths_agreeableness,
-                                weigths_non_neuroticism,
-                            ],
-                            axis=1,
-                        )
+                        df_files_ranking_neuroticism = 1 - self._df_files_ranking[self.keys_dataset_[5]]
+                        df_files_ranking = pd.concat([
+                            self._df_files_ranking[self.keys_dataset_[1:5]],
+                            df_files_ranking_neuroticism
+                        ], axis = 1, ignore_index = False)
+
+                        traits_sum = np.sum(df_files_ranking.values * [
+                            weigths_openness, weigths_conscientiousness, weigths_extraversion,
+                            weigths_agreeableness, weigths_neuroticism
+                        ], axis = 1)
 
                         self._df_files_ranking[self._keys_score] = traits_sum
                         self._df_files_ranking = self._df_files_ranking.sort_values(
-                            by=self._keys_score, ascending=False
+                            by = self._keys_score, ascending = False
                         )
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return self._df_files_ranking
-                    else:
-                        return self._df_files_ranking
+                    except Exception: self._other_error(self._unknown_err, out = out); return self._df_files_ranking
+                    else: return self._df_files_ranking
 
     def _priority_calculation(
-        self,
-        correlation_coefficients: Optional[pd.DataFrame] = None,
-        col_name_ocean: str = "Trait",
-        threshold: float = 0.55,
-        number_priority: int = 1,
-        number_importance_traits: int = 1,
-        out: bool = True,
+        self, correlation_coefficients: Optional[pd.DataFrame] = None, col_name_ocean: str = 'Trait',
+        threshold: float = 0.55, number_priority: int = 1, number_importance_traits: int = 1, out: bool = True
     ) -> pd.DataFrame:
         """Ранжирование предпочтений
 
         .. note::
             protected (защищенный метод)
 
         Args:
@@ -3529,284 +3051,79 @@
             out (bool): Отображение
 
         Returns:
              pd.DataFrame: **DataFrame** c ранжированными предпочтениями
         """
 
         # Сброс
-        self._df_files_priority = pd.DataFrame()  # Пустой DataFrame с ранжированными предпочтениями
+        self._df_files_priority = pd.DataFrame() # Пустой DataFrame с ранжированными предпочтениями
 
         try:
             # Проверка аргументов
-            if (
-                type(correlation_coefficients) is not pd.DataFrame
-                or type(col_name_ocean) is not str
-                or not col_name_ocean
-                or type(threshold) is not float
-                or not (0.0 <= threshold <= 1.0)
-                or type(number_priority) is not int
-                or number_priority < 1
-                or type(number_importance_traits) is not int
-                or number_importance_traits < 1
-                or type(out) is not bool
-            ):
-                raise TypeError
+            if (type(correlation_coefficients) is not pd.DataFrame
+                or type(col_name_ocean) is not str or not col_name_ocean or type(threshold) is not float
+                or not (0.0 <= threshold <= 1.0) or type(number_priority) is not int or number_priority < 1
+                or type(number_importance_traits) is not int or number_importance_traits < 1
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self._priority_calculation.__name__, out=out)
+            self._inv_args(__class__.__name__, self._priority_calculation.__name__, out = out)
             return self._df_files_priority
         else:
-            try:
-                matrix = pd.DataFrame(correlation_coefficients.drop([col_name_ocean], axis=1)).values
-            except KeyError:
-                self._other_error(self._som_ww, out=out)
-                return self._df_files_priority
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return self._df_files_priority
+            try: matrix = pd.DataFrame(correlation_coefficients.drop([col_name_ocean], axis = 1)).values
+            except KeyError: self._other_error(self._som_ww, out = out); return self._df_files_priority
+            except Exception: self._other_error(self._unknown_err, out = out); return self._df_files_priority
             else:
                 try:
-                    if len(self._df_files) == 0:
-                        raise TypeError
-                except TypeError:
-                    self._other_error(self._dataframe_empty, out=out)
-                    return self._df_files_priority
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return self._df_files_priority
+                    if len(self._df_files) == 0: raise TypeError
+                except TypeError: self._other_error(self._dataframe_empty, out = out); return self._df_files_priority
+                except Exception: self._other_error(self._unknown_err, out = out); return self._df_files_priority
                 else:
                     try:
+                        name_priority = correlation_coefficients.columns[1:]
 
                         self._df_files_priority = self._df_files.copy()
-                        df_files_priority = self._df_files.copy()
 
-                        name_priority = correlation_coefficients.columns[1:]
+                        df_files_priority_neuroticism = 1 - self._df_files_priority[self.keys_dataset_[5]]
+                        df_files_priority = pd.concat([
+                            self._df_files_priority[self.keys_dataset_[:5]],
+                            df_files_priority_neuroticism
+                        ], axis = 1, ignore_index = False)
 
                         name_traits = correlation_coefficients[col_name_ocean].values
+                        df_files_priority = df_files_priority[[self.keys_dataset_[0]] + name_traits.tolist()]
 
                         for path in range(len(df_files_priority)):
                             curr_traits = df_files_priority.iloc[path].values[1:]
-
                             curr_traits = np.where(curr_traits < threshold, -1 * curr_traits, curr_traits).reshape(5, 1)
 
                             curr_traits_matrix = curr_traits * matrix
 
-                            curr_weights = np.sum(curr_traits_matrix, axis=0)
+                            curr_weights = np.sum(curr_traits_matrix, axis = 0)
 
                             idx_max_values = np.argsort(-np.asarray(curr_weights))[:number_priority]
                             priority = name_priority[idx_max_values]
 
                             slice_traits_matrix = curr_traits_matrix[:, idx_max_values]
-                            sum_slice_traits_matrix = np.sum(slice_traits_matrix, axis=1)
+                            sum_slice_traits_matrix = np.sum(slice_traits_matrix, axis = 1)
 
-                            id_traits = np.argsort(-sum_slice_traits_matrix, axis=0)[:number_importance_traits]
+                            id_traits = np.argsort(-sum_slice_traits_matrix, axis = 0)[:number_importance_traits]
                             importance_traits = name_traits[id_traits]
 
                             self._df_files_priority.loc[
                                 str(path + 1),
-                                [(self._keys_priority + " {}").format(i + 1) for i in range(number_priority)],
+                                [(self._keys_priority + ' {}').format(i + 1) for i in range(number_priority)]
                             ] = priority
 
                             self._df_files_priority.loc[
                                 str(path + 1),
-                                [
-                                    (self._keys_trait_importance + " {}").format(i + 1)
-                                    for i in range(number_importance_traits)
-                                ],
+                                [(self._keys_trait_importance + ' {}').format(i + 1)
+                                    for i in range(number_importance_traits)]
                             ] = importance_traits
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return self._df_files_priority
-                    else:
-                        return self._df_files_priority
-
-    def _colleague_ranking(
-        self,
-        correlation_coefficients: Optional[pd.DataFrame] = None,
-        target_scores: List[float] = [0.47, 0.63, 0.35, 0.58, 0.51],
-        colleague: str = "major",
-        equal_coefficients: float = 0.5,
-        out: bool = True,
-    ) -> pd.DataFrame:
-        """Поиск подходящего коллеги
-
-        .. note::
-            protected (защищенный метод)
-
-        Args:
-            correlation_coefficients (pd.DataFrame): **DataFrame** c коэффициентами корреляции
-            target_scores (List[float]): Список оценок персональных качеств личности целевого человека
-            colleague (str): Ранг коллеги по совместимости
-            equal_coefficients (float): Коэффициент применяемый к оценкам в случае равенства оценок двух человек
-            out (bool): Отображение
-
-        Returns:
-             pd.DataFrame: **DataFrame** c ранжированными коллегами
-        """
-
-        # Сброс
-        self._df_files_colleague = pd.DataFrame()  # Пустой DataFrame с ранжированными коллегами
-
-        try:
-            # Проверка аргументов
-            if (
-                type(correlation_coefficients) is not pd.DataFrame
-                or not isinstance(target_scores, list)
-                or not all(isinstance(score, float) for score in target_scores)
-                or len(target_scores) != 5
-                or not isinstance(colleague, str)
-                or colleague not in self._colleague
-                or type(equal_coefficients) is not float
-                or not (0.0 <= equal_coefficients <= 1.0)
-                or type(out) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self._colleague_ranking.__name__, out=out)
-            return self._df_files_colleague
-        else:
-            try:
-                if len(self._df_files) == 0:
-                    raise TypeError
-            except TypeError:
-                self._other_error(self._dataframe_empty, out=out)
-                return self._df_files_colleague
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return self._df_files_colleague
-            else:
-                try:
-                    self._df_files_colleague = self._df_files.copy()
-
-                    correlation_coefficients = correlation_coefficients[self.keys_dataset_[1:]].values
-
-                    score_colleague = self._df_files_colleague[self.keys_dataset_[1:]].values.tolist()
-
-                    score_target_colleague = np.round(target_scores, 4).astype("float16")
-                    score_colleague = np.round(score_colleague, 4).astype("float16")
-
-                    intermediate_scores = np.zeros((len(score_colleague), 5))
-
-                    if colleague == self._colleague[0]:
-                        for i, curr_score in enumerate(score_colleague):
-                            for j in range(5):
-                                if score_target_colleague[j] > curr_score[j]:
-                                    intermediate_scores[i, j] = curr_score[j] * correlation_coefficients[1][j]
-                                elif score_target_colleague[j] == curr_score[j]:
-                                    intermediate_scores[i, j] = curr_score[j] * equal_coefficients
-                                else:
-                                    intermediate_scores[i, j] = curr_score[j] * correlation_coefficients[0][j]
-                    elif colleague == self._colleague[1]:
-                        for i, curr_score in enumerate(score_colleague):
-                            for j in range(5):
-                                if score_target_colleague[j] > curr_score[j]:
-                                    intermediate_scores[i, j] = curr_score[j] * correlation_coefficients[0][j]
-                                elif score_target_colleague[j] == curr_score[j]:
-                                    intermediate_scores[i, j] = curr_score[j] * equal_coefficients
-                                else:
-                                    intermediate_scores[i, j] = curr_score[j] * correlation_coefficients[1][j]
-
-                    self._df_files_colleague[self._keys_colleague] = np.sum(intermediate_scores, axis=1)
-                    self._df_files_colleague = self._df_files_colleague.sort_values(
-                        by=self._keys_colleague, ascending=False
-                    )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return self._df_files_colleague
-                else:
-                    return self._df_files_colleague
-
-    def _priority_skill_calculation(
-        self,
-        df_files: Optional[pd.DataFrame] = None,
-        correlation_coefficients: Optional[pd.DataFrame] = None,
-        threshold: float = 0.55,
-        out: bool = True,
-    ) -> pd.DataFrame:
-        """Ранжирование кандидатов по профессиональным навыкам
-
-        .. note::
-            protected (защищенный метод)
-
-        Args:
-            df_files (pd.DataFrame): **DataFrame** c данными
-            correlation_coefficients (pd.DataFrame): **DataFrame** c коэффициентами корреляции
-            threshold (float): Порог для оценок полярности качеств (например, интроверт < 0.55, экстраверт > 0.55)
-            out (bool): Отображение
-
-        Returns:
-             pd.DataFrame: **DataFrame** c ранжированными кандидатами
-        """
-
-        # Сброс
-        self._df_files_priority_skill = pd.DataFrame()  # Пустой DataFrame с ранжированными кандидатами
-
-        if df_files is not None:
-            self._df_files = df_files
-
-        try:
-            # Проверка аргументов
-            if (
-                type(correlation_coefficients) is not pd.DataFrame
-                or type(threshold) is not float
-                or not (0.0 <= threshold <= 1.0)
-                or type(out) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self._priority_skill_calculation.__name__, out=out)
-            return self._df_files_priority_skill
-        else:
-            try:
-                if len(self._df_files) == 0:
-                    raise TypeError
-            except TypeError:
-                self._other_error(self._dataframe_empty, out=out)
-                return self._df_files_priority_skill
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return self._df_files_priority_skill
-            else:
-                try:
-                    self._df_files_priority_skill = self._df_files.copy()
-                    skills_name = correlation_coefficients.columns[2:].tolist()
-                    score_level = ["high", "low"]
-                    traits = self.keys_dataset_[1:]
-                    pred_list = self._df_files_priority_skill[traits].values.tolist()
-                    new_list = []
-
-                    for index_person, curr_scores in enumerate(pred_list):
-                        result = np.zeros((len(traits), len(skills_name)))
-
-                        for index_traits, score in enumerate(curr_scores):
-                            trait = traits[index_traits]
-                            category = score_level[0] if score >= threshold else score_level[1]
-                            coefficient = correlation_coefficients[correlation_coefficients.Trait == trait].values[
-                                score_level.index(category)
-                            ][2:]
-                            result[index_traits] = score * coefficient
-
-                        new_list.append(
-                            np.hstack((self._df_files_priority_skill.iloc[index_person], np.mean(result, axis=0)))
-                        )
-
-                    self._df_files_priority_skill = pd.DataFrame(
-                        data=new_list, columns=self.keys_dataset_ + skills_name
-                    )
-                    self._df_files_priority_skill = self._df_files_priority_skill.sort_values(
-                        by=skills_name, ascending=False
-                    )
-                    self._df_files_priority_skill.index.name = self._keys_id
-                    self._df_files_priority_skill.index += 1
-                    self._df_files_priority_skill.index = self._df_files_priority_skill.index.map(str)
-
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return self._df_files_priority_skill
-                else:
-                    return self._df_files_priority_skill
+                    except Exception: self._other_error(self._unknown_err, out = out); return self._df_files_priority
+                    else: return self._df_files_priority
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внешние методы
     # ------------------------------------------------------------------------------------------------------------------
 
     def show_notebook_history_output(self) -> None:
         """Отображение истории вывода сообщений в ячейке Jupyter
@@ -3837,16 +3154,15 @@
                 :linenos:
 
                 [2022-10-15 18:27:46] Информационное сообщение
         """
 
         if self.is_notebook_ is True and len(self._notebook_history_output) > 0:
             # Отображение
-            for e in self._notebook_history_output:
-                display(e if isinstance(e, pd.DataFrame) else Markdown(e))
+            for e in self._notebook_history_output: display(e if isinstance(e, pd.DataFrame) else Markdown(e))
 
     def libs_vers(self, out: bool = True, runtime: bool = True, run: bool = True) -> None:
         """Получение и отображение версий установленных библиотек
 
         Args:
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
@@ -3869,37 +3185,33 @@
                 core = Core()
                 core.libs_vers(out = True, runtime = True, run = True)
 
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
-                |----|---------------|---------|
-                |    | Package       | Version |
-                |----|---------------|---------|
-                | 1  | TensorFlow    | 2.11.0  |
-                | 2  | Keras         | 2.11.0  |
-                | 3  | OpenCV        | 4.6.0   |
-                | 4  | MediaPipe     | 0.9.0   |
-                | 5  | NumPy         | 1.23.5  |
-                | 6  | SciPy         | 1.9.3   |
-                | 7  | Pandas        | 1.5.2   |
-                | 8  | Scikit-learn  | 1.1.3   |
-                | 9  | OpenSmile     | 2.4.1   |
-                | 10 | Librosa       | 0.9.2   |
-                | 11 | AudioRead     | 3.0.0   |
-                | 12 | IPython       | 8.7.0   |
-                | 14 | Requests      | 2.28.1  |
-                | 15 | JupyterLab    | 3.5.0   |
-                | 16 | LIWC          | 0.5.0   |
-                | 17 | Transformers  | 4.24.0  |
-                | 18 | Sentencepiece | 0.1.99  |
-                | 19 | Torch         | 1.12.1  |
-                | 20 | Torchaudio    | 0.12.1  |
-                |----|---------------|---------|
+                |----|--------------|---------|
+                |    | Package      | Version |
+                |----|--------------|---------|
+                | 1  | TensorFlow   | 2.11.0  |
+                | 2  | Keras        | 2.11.0  |
+                | 3  | OpenCV       | 4.6.0   |
+                | 4  | MediaPipe    | 0.9.0   |
+                | 5  | NumPy        | 1.23.5  |
+                | 6  | SciPy        | 1.9.3   |
+                | 7  | Pandas       | 1.5.2   |
+                | 8  | Scikit-learn | 1.1.3   |
+                | 9  | OpenSmile    | 2.4.1   |
+                | 10 | Librosa      | 0.9.2   |
+                | 11 | AudioRead    | 3.0.0   |
+                | 12 | IPython      | 8.7.0   |
+                | 13 | PyMediaInfo  | 6.0.1   |
+                | 14 | Requests     | 2.28.1  |
+                | 15 | JupyterLab   | 3.5.0   |
+                |----|--------------|---------|
                 --- Время выполнения: 0.005 сек. ---
 
             :bdg-light:`-- 2 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
@@ -3929,87 +3241,42 @@
             .. output-cell::
                 :execution-count: 3
                 :linenos:
 
                 [2022-10-15 18:18:51] Неверные типы или значения аргументов в "Core.libs_vers" ...
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         # Сброс
-        self._df_pkgs = pd.DataFrame()  # Пустой DataFrame
+        self._df_pkgs = pd.DataFrame() # Пустой DataFrame
 
-        if type(out) is not bool:
-            out = True
+        if type(out) is not bool: out = True
 
         try:
             # Проверка аргументов
-            if type(runtime) is not bool or type(run) is not bool:
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.libs_vers.__name__, out=out)
+            if type(runtime) is not bool or type(run) is not bool: raise TypeError
+        except TypeError: self._inv_args(__class__.__name__, self.libs_vers.__name__, out = out)
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return None
+            if run is False: self._error(self._lock_user, out = out); return None
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             pkgs = {
-                "Package": [
-                    "TensorFlow",
-                    "Keras",
-                    "OpenCV",
-                    "MediaPipe",
-                    "NumPy",
-                    "SciPy",
-                    "Pandas",
-                    "Scikit-learn",
-                    "OpenSmile",
-                    "Librosa",
-                    "AudioRead",
-                    "IPython",
-                    "Requests",
-                    "JupyterLab",
-                    "LIWC",
-                    "Transformers",
-                    "Sentencepiece",
-                    "Torch",
-                    "Torchaudio",
-                ],
-                "Version": [
-                    i.__version__
-                    for i in [
-                        tf,
-                        keras,
-                        cv2,
-                        mp,
-                        np,
-                        scipy,
-                        pd,
-                        sklearn,
-                        opensmile,
-                        librosa,
-                        audioread,
-                        IPython,
-                        requests,
-                        jlab,
-                        liwc,
-                        transformers,
-                        sentencepiece,
-                        torch,
-                        torchaudio,
-                    ]
+                'Package': [
+                    'TensorFlow', 'Keras', 'OpenCV', 'MediaPipe', 'NumPy', 'SciPy', 'Pandas', 'Scikit-learn',
+                    'OpenSmile', 'Librosa', 'AudioRead', 'IPython', 'PyMediaInfo', 'Requests', 'JupyterLab'
                 ],
+                'Version': [i.__version__ for i in [
+                    tf, keras, cv2, mp, np, scipy, pd, sklearn, opensmile, librosa, audioread, IPython, pymediainfo,
+                    requests, jlab
+                ]]
             }
 
-            self._df_pkgs = pd.DataFrame(data=pkgs)  # Версии используемых библиотек
+            self._df_pkgs = pd.DataFrame(data = pkgs) # Версии используемых библиотек
             self._df_pkgs.index += 1
 
             # Отображение
-            if self.is_notebook_ is True and out is True:
-                display(self._df_pkgs)
+            if self.is_notebook_ is True and out is True: display(self._df_pkgs)
 
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/core/exceptions.py` & `oceanai-1.0.0a5/oceanai/modules/core/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-
 class CustomException(Exception):
     """Класс для всех пользовательских исключений
 
     .. dropdown:: Пример
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
@@ -22,18 +21,16 @@
 
         .. output-cell::
             :execution-count: 1
             :linenos:
 
             Пользовательское исключение
     """
-
     pass
 
-
 class IsSmallWindowSizeError(CustomException):
     """Указан слишком маленький размер окна сегмента сигнала
 
     .. dropdown:: Пример
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
@@ -51,18 +48,16 @@
         .. output-cell::
             :execution-count: 1
             :linenos:
 
             Указан слишком маленький размер окна сегмента сигнала
 
     """
-
     pass
 
-
 class InvalidContentLength(CustomException):
     """Не определен размер файла для загрузки
 
     .. dropdown:: Пример
 
         :bdg-success:`верно` :bdg-light:`-- 1 --`
 
@@ -80,9 +75,8 @@
         .. output-cell::
             :execution-count: 1
             :linenos:
 
             Не определен размер файла для загрузки
 
     """
-
     pass
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/core/language.py` & `oceanai-1.0.0a5/oceanai/modules/core/language.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,43 +9,39 @@
 # Импорт необходимых инструментов
 # ######################################################################################################################
 # Интернационализация (I18N) и локализация (L10N) (см. https://www.loc.gov/standards/iso639-2/php/code_list.php)
 #     - brew install gettext (Если не установлен)
 #     - brew link gettext --force
 #     1. gettext --help
 #     2. locate pygettext.py
-#     3. /Library/Frameworks/Python.framework/Versions/3.9/share/doc/python3.9/examples/Tools/i18n/pygettext.py
-#        -d oceanai -o oceanai/modules/locales/base.pot oceanai
+#     3. /usr/local/Cellar/python@3.9/3.9.7/Frameworks/Python.framework/Versions/3.9/share/doc/python3.9/examples/Tools/
+#        i18n/pygettext.py -d oceanai -o oceanai/modules/locales/base.pot oceanai
 #     4. msgfmt --help
 #     5. locate msgfmt.py
-#     6. /Library/Frameworks/Python.framework/Versions/3.9/share/doc/python3.9/examples/Tools/i18n/msgfmt.py
-#        oceanai/modules/locales/en/LC_MESSAGES/base.po oceanai/modules/locales/en/LC_MESSAGES/base
-
-import warnings
-
+#     6. /usr/local/Cellar/python@3.9/3.9.7/Frameworks/Python.framework/Versions/3.9/share/doc/python3.9/examples/Tools/
+#        i18n/msgfmt.py oceanai/modules/locales/en/LC_MESSAGES/base.po oceanai/modules/locales/en/LC_MESSAGES/base
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
-import gettext  # Формирование языковых пакетов
-import inspect  # Инспектор
+import os      # Взаимодействие с файловой системой
+import gettext # Формирование языковых пакетов
+import inspect # Инспектор
 
 # Типы данных
 from typing import List, Dict, Optional
 from types import MethodType
 
 # ######################################################################################################################
 # Константы
 # ######################################################################################################################
 
-LANG: str = "ru"  # Язык
-
+LANG: str = 'ru' # Язык
 
 # ######################################################################################################################
 # Интернационализация (I18N) и локализация (L10N)
 # ######################################################################################################################
 @dataclass
 class Language:
     """Класс для интернационализации (I18N) и локализации (L10N)
@@ -60,15 +56,15 @@
 
     lang: str = LANG
     """
     str: Язык, доступные варианты:
 
         * ``"ru"`` - Русский язык (``по умолчанию``)
         * ``"en"`` - Английский язык
-
+        
     .. dropdown:: Примеры
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
         .. code-cell:: python
             :execution-count: 1
             :linenos:
@@ -151,22 +147,23 @@
             :linenos:
 
             1 ru
     """
 
     def __post_init__(self):
         # Директория с поддерживаемыми языками
-        self.__path_to_locales: str = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "locales"))
-        self.__locales: List[str] = self.__get_languages()  # Поддерживаемые языки
+        self.__path_to_locales: str = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'locales'))
+        self.__locales: List[str] = self.__get_languages() # Поддерживаемые языки
+
+        self.__lang: str = self.lang # Язык
 
-        self.__lang: str = self.lang  # Язык
+        self.__i18n: Dict[str, MethodType] = self.__get_locales() # Получение языковых пакетов
 
-        self.__i18n: Dict[str, MethodType] = self.__get_locales()  # Получение языковых пакетов
+        self._: MethodType = self.__set_locale(self.lang_) # Установка языка
 
-        self._: MethodType = self.__set_locale(self.lang_)  # Установка языка
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     @property
     def lang_(self) -> str:
@@ -263,18 +260,16 @@
                 ru
         """
 
         try:
             # Проверка аргументов
             if type(self.__lang) is not str or not self.__lang or (self.__lang in self.locales_) is False:
                 raise TypeError
-        except TypeError:
-            return LANG
-        else:
-            return self.__lang
+        except TypeError: return LANG
+        else: return self.__lang
 
     @property
     def path_to_locales_(self) -> str:
         """Получение директории с языковыми пакетами
 
         Returns:
             str: Директория с языковыми пакетами
@@ -296,15 +291,15 @@
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
                 /Users/dl/GitHub/OCEANAI/oceanai/modules/locales
         """
 
-        return os.path.normpath(self.__path_to_locales)  # Нормализация пути
+        return os.path.normpath(self.__path_to_locales) # Нормализация пути
 
     @property
     def locales_(self) -> List[str]:
         """Получение поддерживаемых языков
 
         Returns:
             List[str]: Список поддерживаемых языков
@@ -374,15 +369,15 @@
     def __get_locales(self) -> Dict[str, MethodType]:
         """Получение языковых пакетов
 
         .. note::
             private (приватный метод)
 
         Returns:
-            Dict[str, MethodType]: Словарь с языковыми пакетами
+             Dict[str, MethodType]: Словарь с языковыми пакетами
 
         .. dropdown:: Пример
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
@@ -400,38 +395,38 @@
 
                 {
                     'ru': <bound method GNUTranslations.gettext of <gettext.GNUTranslations object at 0x14680ce50>>,
                     'en': <bound method GNUTranslations.gettext of <gettext.GNUTranslations object at 0x1460ddbb0>>
                 }
         """
 
-        trs_base = {}  # Языки
+        trs_base = {} # Языки
 
         # Проход по всем языкам
         for curr_lang in self.locales_:
             trs_base[curr_lang] = gettext.translation(
-                "base",  # Домен
-                localedir=self.path_to_locales_,  # Директория с поддерживаемыми языками
-                languages=[curr_lang],  # Язык
-                fallback=True,  # Отключение ошибки
+                'base', # Домен
+                localedir = self.path_to_locales_, # Директория с поддерживаемыми языками
+                languages = [curr_lang], # Язык
+                fallback = True # Отключение ошибки
             ).gettext
 
         return trs_base
 
-    def __set_locale(self, lang: str = "") -> MethodType:
+    def __set_locale(self, lang: str = '') -> MethodType:
         """Установка языка
 
         .. note::
             private (приватный метод)
 
         Args:
             lang (str): Язык
 
         Returns:
-            MethodType: MethodType перевода строк на один из поддерживаемых языков если метод запущен через конструктор
+             MethodType: MethodType перевода строк на один из поддерживаемых языков если метод запущен через конструктор
 
         .. dropdown:: Примеры
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 1
@@ -465,25 +460,21 @@
                 :linenos:
 
                 en
         """
 
         try:
             # Проверка аргументов
-            if type(lang) is not str:
-                raise TypeError
-        except TypeError:
-            pass
+            if type(lang) is not str: raise TypeError
+        except TypeError: pass
         else:
             # Проход по всем поддерживаемым языкам
             for curr_lang in self.locales_:
                 # В аргументах метода не найден язык
-                if lang != curr_lang:
-                    continue
+                if lang != curr_lang: continue
 
-                self.__lang = curr_lang  # Изменение языка
+                self.__lang = curr_lang # Изменение языка
 
             # Метод запущен в конструкторе
             if inspect.stack()[1].function == "__init__" or inspect.stack()[1].function == "__post_init__":
                 return self.__i18n[self.lang_]
-            else:
-                self._ = self.__i18n[self.lang_]  # Установка языка
+            else: self._ = self.__i18n[self.lang_] # Установка языка
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/core/messages.py` & `oceanai-1.0.0a5/oceanai/modules/core/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,24 @@
 """
 Сообщения
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-from typing import List  # Типы данных
+from typing import List # Типы данных
 
 # Персональные
-from oceanai.modules.core.language import Language  # Определение языка
-
+from oceanai.modules.core.language import Language # Определение языка
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class Messages(Language):
     """Класс для сообщений
@@ -35,103 +31,84 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
         self._metadata: List[str] = [
-            self._("OCEANAI - персональные качества личности человека"),
-            self._("Авторы"),
-            self._("Сопровождающие"),
-            self._("Версия"),
-            self._("Лицензия"),
+            self._('OCEANAI - персональные качества личности человека'),
+            self._('Авторы'), self._('Сопровождающие'), self._('Версия'), self._('Лицензия')
         ]
 
-        self._format_time: str = "%Y-%m-%d %H:%M:%S"  # Формат времени
+        self._format_time: str = '%Y-%m-%d %H:%M:%S' # Формат времени
 
         self._invalid_arguments: str = self._('Неверные типы или значения аргументов в "{}" ...')
-        self._invalid_arguments_empty: str = self._("Неверные типы или значения аргументов ...")
+        self._invalid_arguments_empty: str = self._('Неверные типы или значения аргументов ...')
+
+        self._oh: str = self._('Что-то пошло не так ... ')
+        self._trouble: str = self._('Прям беда! ')
 
-        self._oh: str = self._("Что-то пошло не так ... ")
-        self._trouble: str = self._("Прям беда! ")
+        self._unknown_err: str = self._trouble + self._('Не обработанную ошибку необходимо проанализировать и выявить '
+                                                        'причину ...')
 
-        self._unknown_err: str = self._trouble + self._(
-            "Не обработанную ошибку необходимо проанализировать и выявить " "причину ..."
-        )
-
-        self._som_ww: str = self._oh + self._("смотрите настройки ядра и цепочку выполнения действий ...")
-
-        self._lock_user: str = self._("Выполнение заблокировано пользователем ...")
-
-        self._text_runtime: str = self._("Время выполнения")
-
-        self._download_precent: str = " ({}%) ..."
-
-        self._from_precent: str = self._("из")
-
-        self._logs_save_true: str = self._("Лог файл успешно сохранен ...")
-        self._logs_saves_true: str = self._("Лог файлы успешно сохранены ...")
-
-        self._formation_model_hc: str = self._(
-            "Формирование нейросетевой архитектуры модели для получения оценок по " "экспертным признакам"
-        )
-        self._load_model_weights_hc: str = self._(
-            "Загрузка весов нейросетевой модели для получения оценок по " "экспертным признакам"
-        )
-        self._load_model_weights_error: str = self._oh + self._("не удалось загрузить веса нейросетевой модели ...")
-        self._model_hc_not_formation: str = self._oh + self._(
-            "нейросетевая архитектура модели для получения " "оценок по экспертным признакам не сформирована"
-        )
-        self._model_nn_not_formation: str = self._oh + self._(
-            "нейросетевая архитектура модели для получения " "оценок по нейросетевым признакам не сформирована"
-        )
-        self._models_not_formation: str = self._oh + self._(
-            "нейросетевые архитектуры моделей для получения "
-            "оценок по экспертным и нейросетевым признакам не "
-            "сформированы"
-        )
-        self._formation_model_nn: str = self._(
-            "Формирование нейросетевой архитектуры для получения оценок по " "нейросетевым признакам"
-        )
-        self._load_model_weights_nn: str = self._(
-            "Загрузка весов нейросетевой модели для получения оценок по " "нейросетевым признакам"
-        )
-        self._formation_models_b5: str = self._(
-            "Формирование нейросетевых архитектур моделей для получения результатов" " оценки персональных качеств"
-        )
-        self._load_models_weights_b5: str = self._(
-            "Загрузка весов нейросетевых моделей для получения результатов " "оценки персональных качеств"
-        )
-
-        self._concat_pred_error: str = self._oh + self._(
-            "конкатенация оценок по экспертным и нейросетевым признакам " "не произведена"
-        )
-        self._norm_pred_error: str = self._oh + self._(
-            "нормализация оценок по экспертным и нейросетевым признакам " "не произведена"
-        )
-
-        self._get_union_predictions_info: str = self._("Получение прогнозов")
-        self._get_accuracy_info: str = self._(" и вычисление точности")
-
-        self._load_data_true_traits_error: str = self._oh + self._(
-            "не удалось загрузить файл с верными " "предсказаниями для подсчета точности ..."
-        )
-
-        self._wrong_ext: str = self._oh + self._("не указано минимум одно расширение искомых файлов ...")
-
-        self._expert_values_not_found: str = self._oh + self._("отсутствуют экспертные оценки ...")
-
-        self._get_union_predictions_result: str = self._(
-            "Точность по отдельным персональным качествам личности " "человека ..."
-        )
-        self._get_union_predictions_results_mean: str = self._(
-            "Средняя средних абсолютных ошибок: {}, " "средняя точность: {} ..."
-        )
+        self._som_ww: str = self._oh + self._('смотрите настройки ядра и цепочку выполнения действий ...')
+
+        self._lock_user: str = self._('Выполнение заблокировано пользователем ...')
+
+        self._text_runtime: str = self._('Время выполнения')
+
+        self._download_precent: str = ' ({}%) ...'
+
+        self._from_precent: str = self._('из')
+
+        self._logs_save_true: str = self._('Лог файл успешно сохранен ...')
+        self._logs_saves_true: str = self._('Лог файлы успешно сохранены ...')
+
+        self._formation_model_hc: str = self._('Формирование нейросетевой архитектуры модели для получения оценок по '
+                                               'экспертным признакам')
+        self._load_model_weights_hc: str = self._('Загрузка весов нейросетевой модели для получения оценок по '
+                                                  'экспертным признакам')
+        self._load_model_weights_error: str = self._oh + self._('не удалось загрузить веса нейросетевой модели ...')
+        self._model_hc_not_formation: str = self._oh + self._('нейросетевая архитектура модели для получения '
+                                                              'оценок по экспертным признакам не сформирована')
+        self._model_nn_not_formation: str = self._oh + self._('нейросетевая архитектура модели для получения '
+                                                              'оценок по нейросетевым признакам не сформирована')
+        self._models_not_formation: str = self._oh + self._('нейросетевые архитектуры моделей для получения '
+                                                            'оценок по экспертным и нейросетевым признакам не '
+                                                            'сформированы')
+        self._formation_model_nn: str = self._('Формирование нейросетевой архитектуры для получения оценок по '
+                                               'нейросетевым признакам')
+        self._load_model_weights_nn: str = self._('Загрузка весов нейросетевой модели для получения оценок по '
+                                                  'нейросетевым признакам')
+        self._formation_models_b5: str = self._('Формирование нейросетевых архитектур моделей для получения результатов'
+                                                ' оценки персональных качеств')
+        self._load_models_weights_b5: str = self._('Загрузка весов нейросетевых моделей для получения результатов '
+                                                   'оценки персональных качеств')
+
+        self._concat_pred_error: str = self._oh + self._('конкатенация оценок по экспертным и нейросетевым признакам '
+                                                         'не произведена')
+        self._norm_pred_error: str = self._oh + self._('нормализация оценок по экспертным и нейросетевым признакам '
+                                                       'не произведена')
+
+        self._get_union_predictions_info: str = self._('Получение прогнозов')
+        self._get_accuracy_info: str = self._(' и вычисление точности')
+
+        self._load_data_true_traits_error: str = self._oh + self._('не удалось загрузить файл с верными '
+                                                                   'предсказаниями для подсчета точности ...')
+
+        self._wrong_ext: str = self._oh + self._('не указано минимум одно расширение искомых файлов ...')
+
+        self._expert_values_not_found: str = self._oh + self._('отсутствуют экспертные оценки ...')
+
+        self._get_union_predictions_result: str = self._('Точность по отдельным персональным качествам личности '
+                                                         'человека ...')
+        self._get_union_predictions_results_mean: str = self._('Средняя средних абсолютных ошибок: {}, '
+                                                               'средняя точность: {} ...')
 
     # ------------------------------------------------------------------------------------------------------------------
     # Документация
     # ------------------------------------------------------------------------------------------------------------------
 
-    # __doc__ = Language.__doc__
+    # __doc__ = Language.__doc__
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/core/settings.py` & `oceanai-1.0.0a5/oceanai/modules/core/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,51 +4,47 @@
 """
 Настройки
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
-import re  # Регулярные выражения
+import os # Взаимодействие с файловой системой
+import re # Регулярные выражения
 
 from typing import List
 
 # Персональные
-from oceanai.modules.core.messages import Messages  # Сообщения
+from oceanai.modules.core.messages import Messages # Сообщения
 
 # ######################################################################################################################
 # Константы
 # ######################################################################################################################
 
-COLOR_INFO: str = "#1776D2"  # Цвет текста содержащего информацию (шестнадцатеричный код)
-COLOR_SIMPLE: str = "#666"  # Цвет обычного текста (шестнадцатеричный код)
-COLOR_ERR: str = "#FF0000"  # Цвет текста содержащего ошибку (шестнадцатеричный код)
-COLOR_TRUE: str = "#008001"  # Цвет текста содержащего положительную информацию (шестнадцатеричный код)
-BOLD_TEXT: bool = True  # Жирное начертание текста
-CHUNK_SIZE: int = 1000000  # Размер загрузки файла из сети за 1 шаг
-EXT: List[str] = []  # Расширения искомых файлов
-IGNORE_DIRS: List[str] = []  # Директории не входящие в выборку
+COLOR_INFO: str = '#1776D2' # Цвет текста содержащего информацию (шестнадцатеричный код)
+COLOR_SIMPLE: str = '#666'  # Цвет обычного текста (шестнадцатеричный код)
+COLOR_ERR: str = '#FF0000'  # Цвет текста содержащего ошибку (шестнадцатеричный код)
+COLOR_TRUE: str = '#008001' # Цвет текста содержащего положительную информацию (шестнадцатеричный код)
+BOLD_TEXT: bool = True      # Жирное начертание текста
+CHUNK_SIZE: int = 1000000   # Размер загрузки файла из сети за 1 шаг
+EXT: List[str] = []         # Расширения искомых файлов
+IGNORE_DIRS: List[str] = [] # Директории не входящие в выборку
 # Названия ключей для DataFrame набора данных
-KEYS_DATASET: List[str] = ["Path", "Openness", "Conscientiousness", "Extraversion", "Agreeableness", "Non-Neuroticism"]
-NUM_TO_DF_DISPLAY: int = 30  # Количество строк для отображения в таблицах
-PATH_TO_DATASET: str = ""  # Директория набора данных
-PATH_TO_SAVE: str = "./models"  # Директория для сохранения данных
-PATH_TO_LOGS: str = "./logs"  # Директория для сохранения LOG файлов
-TEXT_RUNTIME: str = ""  # Текст времени выполнения
-
+KEYS_DATASET: List[str] = ['Path', 'Openness', 'Conscientiousness', 'Extraversion', 'Agreeableness', 'Neuroticism']
+NUM_TO_DF_DISPLAY: int = 30 # Количество строк для отображения в таблицах
+PATH_TO_DATASET: str = '' # Директория набора данных
+PATH_TO_SAVE: str = './models' # Директория для сохранения данных
+PATH_TO_LOGS: str = './logs' # Директория для сохранения LOG файлов
+TEXT_RUNTIME: str = '' # Текст времени выполнения
 
 # ######################################################################################################################
 # Настройки
 # ######################################################################################################################
 @dataclass
 class Settings(Messages):
     """Класс для настроек
@@ -160,15 +156,15 @@
 
             #666 #666
     """
 
     color_info: str = COLOR_INFO
     """
     str: Цвет текста содержащего информацию (шестнадцатеричный код)
-
+    
     .. dropdown:: Примеры
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
         .. code-cell:: python
             :execution-count: 1
             :linenos:
@@ -252,15 +248,15 @@
 
             #1776D2 #1776D2
     """
 
     color_err: str = COLOR_ERR
     """
     str: Цвет текста содержащего ошибку (шестнадцатеричный код)
-
+    
     .. dropdown:: Примеры
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
         .. code-cell:: python
             :execution-count: 1
             :linenos:
@@ -436,15 +432,15 @@
 
             #008001 #008001
     """
 
     bold_text: bool = BOLD_TEXT
     """
     bool: Жирное начертание текста
-
+    
     .. dropdown:: Примеры
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
         .. code-cell:: python
             :execution-count: 1
             :linenos:
@@ -528,15 +524,15 @@
 
             True True
     """
 
     text_runtime: str = TEXT_RUNTIME
     """
     str: Текст времени выполнения
-
+    
     .. dropdown:: Примеры
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
         .. code-cell:: python
             :execution-count: 1
             :linenos:
@@ -620,15 +616,15 @@
 
             Время выполнения Время выполнения
     """
 
     num_to_df_display: int = NUM_TO_DF_DISPLAY
     """
     int: Количество строк для отображения в таблицах
-
+    
     .. dropdown:: Примеры
 
         :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
         .. code-cell:: python
             :execution-count: 1
             :linenos:
@@ -710,51 +706,51 @@
             :execution-count: 5
             :linenos:
 
             30 30
     """
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self.__re_search_color: str = r"^#(?:[0-9a-fA-F]{3}){1,2}$"  # Регулярное выражение для корректности ввода цвета
+        self.__re_search_color: str = r'^#(?:[0-9a-fA-F]{3}){1,2}$' # Регулярное выражение для корректности ввода цвета
 
         # Цвет текстов
-        self.__color_simple_true: int = 0  # Счетчик изменения текста
-        self.color_simple_: str = self.color_simple  # Обычный текст
+        self.__color_simple_true: int = 0 # Счетчик изменения текста
+        self.color_simple_: str = self.color_simple # Обычный текст
 
         self.__color_info_true: int = 0  # Счетчик изменения текста
-        self.color_info_: str = self.color_info  # Цвет текста содержащего информацию
+        self.color_info_: str = self.color_info # Цвет текста содержащего информацию
 
         self.__color_true_true: int = 0  # Счетчик изменения текста
         self.color_true_: str = self.color_true  # Цвет текста содержащего положительную информацию
 
-        self.__color_err_true: int = 0  # Счетчик изменения текста
-        self.color_err_: str = self.color_err  # Цвет текста содержащего ошибку
+        self.__color_err_true: int = 0 # Счетчик изменения текста
+        self.color_err_: str = self.color_err # Цвет текста содержащего ошибку
 
-        self.__bold_text_true: int = 0  # Счетчик изменения начертания текста
-        self.bold_text_: bool = self.bold_text  # Жирное начертание текста
+        self.__bold_text_true: int = 0 # Счетчик изменения начертания текста
+        self.bold_text_: bool = self.bold_text # Жирное начертание текста
 
-        self.__text_runtime_true: int = 0  # Счетчик изменения текста
-        self.text_runtime_: str = self.text_runtime  # Текст времени выполнения
+        self.__text_runtime_true: int = 0 # Счетчик изменения текста
+        self.text_runtime_: str = self.text_runtime # Текст времени выполнения
 
-        self.__num_to_df_display_true: int = 0  # Счетчик изменения количества строк для отображения в таблицах
-        self.num_to_df_display_: int = self.num_to_df_display  # Количество строк для отображения в таблицах
+        self.__num_to_df_display_true: int = 0 # Счетчик изменения количества строк для отображения в таблицах
+        self.num_to_df_display_: int = self.num_to_df_display # Количество строк для отображения в таблицах
 
-        self.chunk_size_: int = CHUNK_SIZE  # Размер загрузки файла из сети за 1 шаг
+        self.chunk_size_: int = CHUNK_SIZE # Размер загрузки файла из сети за 1 шаг
 
-        self.path_to_save_: str = PATH_TO_SAVE  # Директория для сохранения данных
-        self.path_to_dataset_: str = PATH_TO_DATASET  # Директория набора данных
-        self.path_to_logs_: str = PATH_TO_LOGS  # Директория для сохранения LOG файлов
+        self.path_to_save_: str = PATH_TO_SAVE # Директория для сохранения данных
+        self.path_to_dataset_: str = PATH_TO_DATASET # Директория набора данных
+        self.path_to_logs_: str = PATH_TO_LOGS # Директория для сохранения LOG файлов
 
-        self.ext_: List[str] = EXT  # Расширения искомых файлов
+        self.ext_: List[str] = EXT # Расширения искомых файлов
 
-        self.ignore_dirs_: List[str] = IGNORE_DIRS  # Директории не входящие в выборку
+        self.ignore_dirs_: List[str] = IGNORE_DIRS # Директории не входящие в выборку
 
-        self.keys_dataset_: List[str] = KEYS_DATASET  # Названия ключей для DataFrame набора данных
+        self.keys_dataset_: List[str] = KEYS_DATASET # Названия ключей для DataFrame набора данных
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     @property
     def color_simple_(self) -> str:
@@ -845,22 +841,20 @@
     @color_simple_.setter
     def color_simple_(self, color: str) -> None:
         """Установка цвета обычного текста"""
 
         try:
             # Проверка аргументов
             match = re.search(self.__re_search_color, color)
-            if not match:
-                raise TypeError
+            if not match: raise TypeError
         except TypeError:
-            if self.__color_simple_true == 0:
-                self.color_simple = COLOR_SIMPLE
+            if self.__color_simple_true == 0: self.color_simple = COLOR_SIMPLE
         else:
             self.color_simple = color
-            self.__color_simple_true += 1  # Увеличение счетчика изменения цвета текста
+            self.__color_simple_true += 1 # Увеличение счетчика изменения цвета текста
 
     @property
     def color_info_(self) -> str:
         """Получение/установка цвета текста содержащего информацию
 
         Args:
             (str): Шестнадцатеричный код
@@ -947,22 +941,20 @@
     @color_info_.setter
     def color_info_(self, color: str) -> None:
         """Установка цвета текста содержащего информацию"""
 
         try:
             # Проверка аргументов
             match = re.search(self.__re_search_color, color)
-            if not match:
-                raise TypeError
+            if not match: raise TypeError
         except TypeError:
-            if self.__color_info_true == 0:
-                self.color_info = COLOR_INFO
+            if self.__color_info_true == 0: self.color_info = COLOR_INFO
         else:
             self.color_info = color
-            self.__color_info_true += 1  # Увеличение счетчика изменения цвета текста
+            self.__color_info_true += 1 # Увеличение счетчика изменения цвета текста
 
     @property
     def color_true_(self) -> str:
         """Получение/установка цвета текста содержащего положительную информацию
 
         Args:
             (str): Шестнадцатеричный код
@@ -1049,22 +1041,20 @@
     @color_true_.setter
     def color_true_(self, color: str) -> None:
         """Установка цвета текста содержащего положительную информацию"""
 
         try:
             # Проверка аргументов
             match = re.search(self.__re_search_color, color)
-            if not match:
-                raise TypeError
+            if not match: raise TypeError
         except TypeError:
-            if self.__color_true_true == 0:
-                self.color_true = COLOR_TRUE
+            if self.__color_true_true == 0: self.color_true = COLOR_TRUE
         else:
             self.color_true = color
-            self.__color_true_true += 1  # Увеличение счетчика изменения цвета текста
+            self.__color_true_true += 1 # Увеличение счетчика изменения цвета текста
 
     @property
     def color_err_(self) -> str:
         """Получение/установка цвета текста содержащего ошибку
 
         Args:
             (str): Шестнадцатеричный код
@@ -1151,22 +1141,20 @@
     @color_err_.setter
     def color_err_(self, color: str) -> None:
         """Установка цвета текста содержащего ошибку"""
 
         try:
             # Проверка аргументов
             match = re.search(self.__re_search_color, color)
-            if not match:
-                raise TypeError
+            if not match: raise TypeError
         except TypeError:
-            if self.__color_err_true == 0:
-                self.color_err = COLOR_ERR
+            if self.__color_err_true == 0: self.color_err = COLOR_ERR
         else:
             self.color_err = color
-            self.__color_err_true += 1  # Увеличение счетчика изменения цвета текста
+            self.__color_err_true += 1 # Увеличение счетчика изменения цвета текста
 
     @property
     def bold_text_(self) -> bool:
         """Получение/установка жирного начертания текста
 
         Args:
             (bool): **True** или **False**
@@ -1252,22 +1240,20 @@
 
     @bold_text_.setter
     def bold_text_(self, bold: bool) -> None:
         """Установка жирного начертания текста"""
 
         try:
             # Проверка аргументов
-            if type(bold) is not bool:
-                raise TypeError
+            if type(bold) is not bool: raise TypeError
         except TypeError:
-            if self.__bold_text_true == 0:
-                self.bold_text = BOLD_TEXT
+            if self.__bold_text_true == 0: self.bold_text = BOLD_TEXT
         else:
             self.bold_text = bold
-            self.__bold_text_true += 1  # Увеличение счетчика изменения начертания текста
+            self.__bold_text_true += 1 # Увеличение счетчика изменения начертания текста
 
     @property
     def text_runtime_(self) -> str:
         """Получение/установка текста времени выполнения
 
         Args:
             (str): Текст
@@ -1353,22 +1339,20 @@
 
     @text_runtime_.setter
     def text_runtime_(self, text: str) -> None:
         """Установка текста времени выполнения"""
 
         try:
             # Проверка аргументов
-            if type(text) is not str or len(text) < 1:
-                raise TypeError
+            if type(text) is not str or len(text) < 1: raise TypeError
         except TypeError:
-            if self.__text_runtime_true == 0:
-                self.text_runtime = self._text_runtime
+            if self.__text_runtime_true == 0: self.text_runtime = self._text_runtime
         else:
             self.text_runtime = text
-            self.__text_runtime_true += 1  # Увеличение счетчика изменения текста времени выполнения
+            self.__text_runtime_true += 1 # Увеличение счетчика изменения текста времени выполнения
 
     @property
     def num_to_df_display_(self) -> int:
         """Получение/установка количества строк для отображения в таблицах
 
         Args:
             (int): Количество строк
@@ -1455,19 +1439,17 @@
     # Установка количества строк для отображения в таблицах
     @num_to_df_display_.setter
     def num_to_df_display_(self, num: int) -> None:
         """Установка количества строк для отображения в таблицах"""
 
         try:
             # Проверка аргументов
-            if type(num) is not int or num < 1 or num > 50:
-                raise TypeError
+            if type(num) is not int or num < 1 or num > 50: raise TypeError
         except TypeError:
-            if self.__num_to_df_display_true == 0:
-                self.num_to_df_display = NUM_TO_DF_DISPLAY
+            if self.__num_to_df_display_true == 0: self.num_to_df_display = NUM_TO_DF_DISPLAY
         else:
             self.num_to_df_display = num
             # Увеличение счетчика изменения количества строк для отображения в таблицах
             self.__num_to_df_display_true += 1
 
     @property
     def path_to_save_(self) -> str:
@@ -1573,16 +1555,15 @@
 
         return self._path_to_save
 
     @path_to_save_.setter
     def path_to_save_(self, path: str) -> None:
         """Установка директории для сохранения данных"""
 
-        if type(path) is str:
-            self._path_to_save = os.path.normpath(path)
+        if type(path) is str: self._path_to_save = os.path.normpath(path)
 
     @property
     def path_to_logs_(self) -> str:
         """Получение/установка директории для сохранения LOG файлов
 
         Args:
             (str): Директория для сохранения LOG файлов
@@ -1684,16 +1665,15 @@
 
         return self._path_to_logs
 
     @path_to_logs_.setter
     def path_to_logs_(self, path: str) -> None:
         """Установка директории для сохранения LOG файлов"""
 
-        if type(path) is str:
-            self._path_to_logs = os.path.normpath(path)
+        if type(path) is str: self._path_to_logs = os.path.normpath(path)
 
     @property
     def chunk_size_(self) -> int:
         """Получение/установка размера загрузки файла из сети за 1 шаг
 
         Args:
             (int): Размер загрузки файла из сети за 1 шаг
@@ -1795,16 +1775,15 @@
 
         return self._chunk_size
 
     @chunk_size_.setter
     def chunk_size_(self, size: int) -> None:
         """Установка директории для сохранения данных"""
 
-        if type(size) is int and size > 0:
-            self._chunk_size = size
+        if type(size) is int and size > 0: self._chunk_size = size
 
     @property
     def path_to_dataset_(self) -> str:
         """Получение/установка директории набора данных
 
         Args:
             (str): Директория набора данных
@@ -1906,16 +1885,15 @@
 
         return self._path_to_dataset
 
     @path_to_dataset_.setter
     def path_to_dataset_(self, path: str) -> None:
         """Установка директории набора данных"""
 
-        if type(path) is str:
-            self._path_to_dataset = os.path.normpath(path)
+        if type(path) is str: self._path_to_dataset = os.path.normpath(path)
 
     @property
     def keys_dataset_(self):
         """Получение/установка названий ключей набора данных
 
         Args:
             (List[str]): Список с названиями ключей набора данных
@@ -1942,15 +1920,15 @@
 
                 [
                     'Path',
                     'Openness',
                     'Conscientiousness',
                     'Extraversion',
                     'Agreeableness',
-                    'Non-Neuroticism'
+                    'Neuroticism'
                 ]
 
             :bdg-light:`-- 2 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
@@ -1985,15 +1963,15 @@
 
                 [
                     'Path',
                     'Openness',
                     'Conscientiousness',
                     'Extraversion',
                     'Agreeableness',
-                    'Non-Neuroticism'
+                    'Neuroticism'
                 ]
 
             :bdg-light:`-- 2 --`
 
             .. code-cell:: python
                 :execution-count: 4
                 :linenos:
@@ -2010,15 +1988,15 @@
 
                 [
                     'Path',
                     'Openness',
                     'Conscientiousness',
                     'Extraversion',
                     'Agreeableness',
-                    'Non-Neuroticism'
+                    'Neuroticism'
                 ]
 
             :bdg-light:`-- 3 --`
 
             .. code-cell:: python
                 :execution-count: 5
                 :linenos:
@@ -2035,41 +2013,35 @@
 
                 [
                     'Path',
                     'Openness',
                     'Conscientiousness',
                     'Extraversion',
                     'Agreeableness',
-                    'Non-Neuroticism'
+                    'Neuroticism'
                 ]
         """
 
         return self._keys_dataset
 
     # Установка названий ключей набора данных
     @keys_dataset_.setter
     def keys_dataset_(self, keys: List[str]) -> None:
         """Установка названий ключей набора данных"""
 
         if type(keys) is list and len(keys) == len(KEYS_DATASET):
-            try:
-                # .capitalize()
-                self._keys_dataset = [x for x in keys]
-            except Exception:
-                pass
+            try: self._keys_dataset = [x.capitalize() for x in keys]
+            except Exception: pass
 
         if type(keys) is list and len(keys) == len(KEYS_DATASET) - 1:
             try:
                 for x in keys:
-                    if type(x) is not str or not x:
-                        raise TypeError
-                # .capitalize()
-                self._keys_dataset[1:] = [x for x in keys]
-            except Exception:
-                pass
+                    if type(x) is not str or not x: raise TypeError
+                self._keys_dataset[1:] = [x.capitalize() for x in keys]
+            except Exception: pass
 
     @property
     def ignore_dirs_(self) -> List[str]:
         """Получение/установка списка с директориями не входящими в выборку
 
         Args:
             (List[str]): Список с директориями
@@ -2172,18 +2144,16 @@
         return self._ignore_dirs
 
     @ignore_dirs_.setter
     def ignore_dirs_(self, l: List[str]) -> None:
         """Установка списка с директориями не входящими в выборку"""
 
         if type(l) is list:
-            try:
-                self._ignore_dirs = [x.lower() for x in l]
-            except Exception:
-                pass
+            try: self._ignore_dirs = [x.lower() for x in l]
+            except Exception: pass
 
     @property
     def ext_(self) -> List[str]:
         """Получение/установка расширений искомых файлов
 
         Args:
             (List[str]): Список с расширениями искомых файлов
@@ -2286,11 +2256,9 @@
         return self._ext
 
     @ext_.setter
     def ext_(self, ext: List[str]) -> None:
         """Установка расширений искомых файлов"""
 
         if type(ext) is list:
-            try:
-                self._ext = [x.lower() for x in ext]
-            except Exception:
-                pass
+            try: self._ext = [x.lower() for x in ext]
+            except Exception: pass
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/lab/audio.py` & `oceanai-1.0.0a5/oceanai/modules/lab/audio.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,65 +4,59 @@
 """
 Аудио
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
+import os           # Взаимодействие с файловой системой
 import logging
-import requests  # Отправка HTTP запросов
+import requests     # Отправка HTTP запросов
 import numpy as np  # Научные вычисления
-import pandas as pd  # Обработка и анализ данных
-import opensmile  # Анализ, обработка и классификация звука
-import librosa  # Обработка аудио
-import audioread  # Декодирование звука
+import pandas as pd # Обработка и анализ данных
+import opensmile    # Анализ, обработка и классификация звука
+import librosa      # Обработка аудио
+import audioread    # Декодирование звука
 import math
-import gradio
 
 from urllib.parse import urlparse
 from urllib.error import URLError
-from pathlib import Path  # Работа с путями в файловой системе
+from pathlib import Path # Работа с путями в файловой системе
 from sklearn import preprocessing
 from sklearn.metrics import mean_absolute_error
-from datetime import datetime  # Работа со временем
-import subprocess
+from datetime import datetime # Работа со временем
 
-from typing import Dict, List, Tuple, Union, Optional, Callable  # Типы данных
+from typing import Dict, List, Tuple, Union, Optional, Callable # Типы данных
 
 from IPython.display import clear_output
 
 # Персональные
-from oceanai.modules.lab.download import Download  # Загрузка файлов
+from oceanai.modules.lab.download import Download # Загрузка файлов
 from oceanai.modules.core.exceptions import IsSmallWindowSizeError
 
 # Порог регистрации сообщений TensorFlow
 logging.disable(logging.WARNING)
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
-import tensorflow as tf  # Машинное обучение от Google
+import tensorflow as tf # Машинное обучение от Google
 import keras
 
 from tensorflow.keras.applications import VGG16
 
 # ######################################################################################################################
 # Настройки необходимых инструментов
 # ######################################################################################################################
-pd.set_option("display.max_columns", None)  # Максимальное количество отображаемых столбцов
-pd.set_option("display.max_rows", None)  # Максимальное количество отображаемых строк
-
+pd.set_option('display.max_columns', None) # Максимальное количество отображаемых столбцов
+pd.set_option('display.max_rows', None)    # Максимальное количество отображаемых строк
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class AudioMessages(Download):
     """Класс для сообщений
@@ -79,47 +73,42 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._audio_modality: str = self._(" (аудио модальность) ...")
+        self._audio_modality: str = self._(' (аудио модальность) ...')
         self._formation_audio_model_hc: str = self._formation_model_hc + self._audio_modality
         self._formation_audio_model_nn: str = self._formation_model_nn + self._audio_modality
         self._formation_audio_models_b5: str = self._formation_models_b5 + self._audio_modality
 
         self._load_audio_model_weights_hc: str = self._load_model_weights_hc + self._audio_modality
         self._load_audio_model_weights_nn: str = self._load_model_weights_nn + self._audio_modality
         self._load_audio_models_weights_b5: str = self._load_models_weights_b5 + self._audio_modality
 
-        self._get_acoustic_feature_info: str = self._(
-            "Извлечение признаков (экспертных и лог мел-спектрограмм) из " "акустического сигнала ..."
-        )
-        self._get_acoustic_feature_hc_error: str = self._oh + self._(
-            "экспертные признаки из акустического сигнала не " "извлечены ..."
-        )
-        self._get_acoustic_feature_spec_error: str = self._oh + self._(
-            "лог мел-спектрограммы из акустического сигнала " "не извлечены ..."
-        )
+        self._get_acoustic_feature_info: str = self._('Извлечение признаков (экспертных и лог мел-спектрограмм) из '
+                                                      'акустического сигнала ...')
+        self._get_acoustic_feature_hc_error: str = self._oh + self._('экспертные признаки из акустического сигнала не '
+                                                                     'извлечены ...')
+        self._get_acoustic_feature_spec_error: str = self._oh + self._('лог мел-спектрограммы из акустического сигнала '
+                                                                       'не извлечены ...')
 
-        self._window_small_size_error: str = self._oh + self._(
-            "указан слишком маленький размер ({}) окна сегмента " "сигнала ..."
-        )
+        self._window_small_size_error: str = self._oh + self._('указан слишком маленький размер ({}) окна сегмента '
+                                                               'сигнала ...')
 
         self._model_audio_hc_not_formation: str = self._model_hc_not_formation + self._audio_modality
         self._model_audio_nn_not_formation: str = self._model_nn_not_formation + self._audio_modality
         self._models_audio_not_formation: str = self._models_not_formation + self._audio_modality
 
         self._concat_audio_pred_error: str = self._concat_pred_error + self._audio_modality
         self._norm_audio_pred_error: str = self._norm_pred_error + self._audio_modality
 
-
 # ######################################################################################################################
 # Аудио
 # ######################################################################################################################
 @dataclass
 class Audio(AudioMessages):
     """Класс для обработки аудио
 
@@ -135,60 +124,51 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
         # Нейросетевая модель **tf.keras.Model** для получения оценок по экспертным признакам
-        self._audio_model_hc: Optional[tf.keras.Model] = None
+        self._audio_model_hc: Optional[keras.engine.functional.Functional] = None
         # Нейросетевая модель **tf.keras.Model** для получения оценок по нейросетевым признакам
-        self._audio_model_nn: Optional[tf.keras.Model] = None
+        self._audio_model_nn: Optional[keras.engine.functional.Functional] = None
         # Нейросетевые модели **tf.keras.Model** для получения результатов оценки персональных качеств
-        self._audio_models_b5: Dict[str, Optional[tf.keras.Model]] = dict(
-            zip(self._b5["en"], [None] * len(self._b5["en"]))
-        )
+        self._audio_models_b5: Dict[str, Optional[keras.engine.functional.Functional]] = dict(zip(
+            self._b5['en'], [None] * len(self._b5['en'])
+        ))
 
-        self._smile: opensmile.core.smile.Smile = self.__smile()  # Извлечение функций OpenSmile
+        self._smile: opensmile.core.smile.Smile = self.__smile() # Извлечение функций OpenSmile
 
         # ----------------------- Только для внутреннего использования внутри класса
 
         # Настройки для спектрограммы
         self.__pl: List[Union[int, str, bool, float, None]] = [
-            2048,
-            512,
-            None,
-            True,
-            "reflect",
-            2.0,
-            128,
-            "slaney",
-            True,
-            None,
+            2048, 512, None, True, 'reflect', 2.0, 128, 'slaney', True, None
         ]
-        self.__len_paths: int = 0  # Количество искомых файлов
-        self.__local_path: Union[Callable[[str], str], None] = None  # Локальный путь
+        self.__len_paths: int = 0 # Количество искомых файлов
+        self.__local_path: Union[Callable[[str], str], None] = None # Локальный путь
 
         # Ключи для точности
-        self.__df_accuracy_index: List[str] = ["MAE", "Accuracy"]
-        self.__df_accuracy_index_name: str = "Metrics"
-        self.__df_accuracy_mean: str = "Mean"
+        self.__df_accuracy_index: List[str] = ['MAE', 'Accuracy']
+        self.__df_accuracy_index_name: str = 'Metrics'
+        self.__df_accuracy_mean: str = 'Mean'
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     @property
-    def audio_model_hc_(self) -> Optional[tf.keras.Model]:
+    def audio_model_hc_(self) -> Optional[keras.engine.functional.Functional]:
         """Получение нейросетевой модели **tf.keras.Model** для получения оценок по экспертным признакам
 
         Returns:
-            Optional[tf.keras.Model]: Нейросетевая модель **tf.keras.Model** или None
+            Optional[keras.engine.functional.Functional]: Нейросетевая модель **tf.keras.Model** или None
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
@@ -211,15 +191,15 @@
                 :execution-count: 1
                 :linenos:
 
                 [2022-10-17 13:54:35] Формирование нейросетевой архитектуры модели для получения оценок по экспертным признакам (аудио модальность) ...
 
                 --- Время выполнения: 0.509 сек. ---
 
-                <tf.keras.Model at 0x13dd600a0>
+                <keras.engine.functional.Functional at 0x13dd600a0>
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
@@ -236,19 +216,19 @@
 
 
         """
 
         return self._audio_model_hc
 
     @property
-    def audio_model_nn_(self) -> Optional[tf.keras.Model]:
+    def audio_model_nn_(self) -> Optional[keras.engine.functional.Functional]:
         """Получение нейросетевой модели **tf.keras.Model** для получения оценок по нейросетевым признакам
 
         Returns:
-            Optional[tf.keras.Model]: Нейросетевая модель **tf.keras.Model** или None
+            Optional[keras.engine.functional.Functional]: Нейросетевая модель **tf.keras.Model** или None
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
@@ -271,15 +251,15 @@
                 :execution-count: 1
                 :linenos:
 
                 [2022-10-17 13:58:29] Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам ...
 
                 --- Время выполнения: 0.444 сек. ---
 
-                <tf.keras.Model at 0x13db97760>
+                <keras.engine.functional.Functional at 0x13db97760>
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
@@ -296,15 +276,15 @@
 
 
         """
 
         return self._audio_model_nn
 
     @property
-    def audio_models_b5_(self) -> Dict[str, Optional[tf.keras.Model]]:
+    def audio_models_b5_(self) -> Dict[str, Optional[keras.engine.functional.Functional]]:
         """Получение нейросетевых моделей **tf.keras.Model** для получения результатов оценки персональных качеств
 
         Returns:
             Dict: Словарь с нейросетевыми моделями **tf.keras.Model**
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
@@ -333,19 +313,19 @@
 
                 [2022-10-19 15:45:35] Формирование нейросетевых архитектур моделей для получения результатов оценки
                 персональных качеств (аудио модальность) ...
 
                 --- Время выполнения: 0.07 сек. ---
 
                 {
-                    'openness': <tf.keras.Model at 0x1481e03a0>,
-                    'conscientiousness': <tf.keras.Model at 0x147d13520>,
-                    'extraversion': <tf.keras.Model at 0x1481edfa0>,
-                    'agreeableness': <tf.keras.Model at 0x1481cfc40>,
-                    'non_neuroticism': <tf.keras.Model at 0x1481cffd0>
+                    'openness': <keras.engine.functional.Functional at 0x1481e03a0>,
+                    'conscientiousness': <keras.engine.functional.Functional at 0x147d13520>,
+                    'extraversion': <keras.engine.functional.Functional at 0x1481edfa0>,
+                    'agreeableness': <keras.engine.functional.Functional at 0x1481cfc40>,
+                    'neuroticism': <keras.engine.functional.Functional at 0x1481cffd0>
                 }
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
@@ -363,15 +343,15 @@
                 :tab-width: 8
 
                 {
                     'openness': None,
                     'conscientiousness': None,
                     'extraversion': None,
                     'agreeableness': None,
-                    'non_neuroticism': None
+                    'neuroticism': None
                 }
         """
 
         return self._audio_models_b5
 
     @property
     def smile_(self) -> opensmile.core.smile.Smile:
@@ -416,21 +396,16 @@
         return self._smile
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (приватные)
     # ------------------------------------------------------------------------------------------------------------------
 
     def __load_model_weights(
-        self,
-        url: str,
-        force_reload: bool = True,
-        info_text: str = "",
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+        self, url: str, force_reload: bool = True, info_text: str = '',
+        out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
         """Загрузка весов нейросетевой модели
 
         .. note::
             private (приватный метод)
 
         Args:
@@ -536,85 +511,60 @@
                 :linenos:
 
                 [2022-10-17 12:21:57] Неверные типы или значения аргументов в "Audio.__load_model_weights" ...
 
                 False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(url) is not str
-                or not url
-                or type(force_reload) is not bool
-                or type(info_text) is not str
-                or not info_text
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(url) is not str or not url or type(force_reload) is not bool
+                or type(info_text) is not str or not info_text or type(out) is not bool
+                or type(runtime) is not bool or type(run) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__load_model_weights.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.__load_model_weights.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(info_text, last=False, out=out)
+            self._info(info_text, last = False, out = out)
 
-            sections = urlparse(url)  # Парсинг URL адреса
+            sections = urlparse(url) # Парсинг URL адреса
 
             try:
                 # URL файл невалидный
-                if sections.scheme == "":
-                    raise requests.exceptions.InvalidURL
+                if sections.scheme == '': raise requests.exceptions.InvalidURL
             except requests.exceptions.InvalidURL:
                 url = os.path.normpath(url)
 
                 try:
-                    if os.path.isfile(url) is False:
-                        raise FileNotFoundError  # Не файл
-                except FileNotFoundError:
-                    self._other_error(self._load_model_weights_error, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    self._url_last_filename = url
-                    return True
+                    if os.path.isfile(url) is False: raise FileNotFoundError # Не файл
+                except FileNotFoundError: self._other_error(self._load_model_weights_error, out = out); return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
+                else: self._url_last_filename = url; return True
             else:
                 try:
-                    if force_reload is False:
-                        clear_output(True)
+                    if force_reload is False: clear_output(True)
                     # Загрузка файла из URL
                     res_download_file_from_url = self._download_file_from_url(
-                        url=url, force_reload=force_reload, runtime=False, out=out, run=True
+                        url = url, force_reload = force_reload, runtime = False, out = out, run = True
                     )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
                 else:
                     # Файл загружен
-                    if res_download_file_from_url != 200:
-                        return False
+                    if res_download_file_from_url != 200: return False
 
                     return True
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
 
     @staticmethod
     def __smile() -> opensmile.core.smile.Smile:
         """Извлечение функций OpenSmile
 
         .. note::
             private (приватный метод)
@@ -652,16 +602,16 @@
                         'mixdown': False,
                         'resample': False
                     }
                 }
         """
 
         return opensmile.Smile(
-            feature_set=opensmile.FeatureSet.eGeMAPSv02,
-            feature_level=opensmile.FeatureLevel.LowLevelDescriptors,
+            feature_set = opensmile.FeatureSet.eGeMAPSv02,
+            feature_level = opensmile.FeatureLevel.LowLevelDescriptors,
         )
 
     def __norm_pred(self, pred_data: np.ndarray, len_spec: int = 16, out: bool = True) -> np.ndarray:
         """Нормализация оценок по экспертным и нейросетевым признакам
 
         .. note::
             private (приватный метод)
@@ -739,36 +689,26 @@
                 [2022-10-20 22:03:17] Неверные типы или значения аргументов в "Audio.__norm_pred" ...
 
                 array([], dtype=float64)
         """
 
         try:
             # Проверка аргументов
-            if (
-                type(pred_data) is not np.ndarray
-                or len(pred_data) < 1
-                or type(len_spec) is not int
-                or len_spec < 1
-                or type(out) is not bool
-            ):
-                raise TypeError
+            if (type(pred_data) is not np.ndarray or len(pred_data) < 1 or type(len_spec) is not int or len_spec < 1
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__norm_pred.__name__, out=out)
-            return np.array([])
+            self._inv_args(__class__.__name__, self.__norm_pred.__name__, out = out); return np.array([])
         else:
             try:
                 if pred_data.shape[0] < len_spec:
-                    return np.pad(pred_data, ((0, len_spec - pred_data.shape[0]), (0, 0)), "mean")
+                    return np.pad(pred_data, ((0, len_spec - pred_data.shape[0]), (0, 0)), 'mean')
                 return pred_data[:len_spec]
             except ValueError:
-                self._other_error(self._norm_audio_pred_error, last=False, out=out)
-                return np.array([])
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return np.array([])
+                self._other_error(self._norm_audio_pred_error, last = False, out = out); return np.array([])
+            except Exception: self._other_error(self._unknown_err, out = out); return np.array([])
 
     def __concat_pred(
         self, pred_hc: np.ndarray, pred_melspectrogram: np.ndarray, out: bool = True
     ) -> List[Optional[np.ndarray]]:
         """Конкатенация оценок по экспертным и нейросетевым признакам
 
         .. note::
@@ -902,65 +842,54 @@
                 признакам не произведена (аудио модальность) ...
 
                 []
         """
 
         try:
             # Проверка аргументов
-            if (
-                type(pred_hc) is not np.ndarray
-                or len(pred_hc) < 1
-                or type(pred_melspectrogram) is not np.ndarray
-                or len(pred_melspectrogram) < 1
-                or type(out) is not bool
-            ):
-                raise TypeError
+            if (type(pred_hc) is not np.ndarray or len(pred_hc) < 1
+                or type(pred_melspectrogram) is not np.ndarray or len(pred_melspectrogram) < 1
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__concat_pred.__name__, out=out)
-            return []
+            self._inv_args(__class__.__name__, self.__concat_pred.__name__, out = out); return []
         else:
             # Нормализация оценок по экспертным и нейросетевым признакам
-            pred_hc_norm = self.__norm_pred(pred_hc, out=False)
-            pred_melspectrogram_norm = self.__norm_pred(pred_melspectrogram, out=False)
+            pred_hc_norm = self.__norm_pred(pred_hc, out = False)
+            pred_melspectrogram_norm = self.__norm_pred(pred_melspectrogram, out = False)
 
             if len(pred_hc_norm) == 0 or len(pred_melspectrogram_norm) == 0:
-                self._error(self._concat_audio_pred_error, out=out)
-                return []
+                self._error(self._concat_audio_pred_error, out = out); return []
 
             concat = []
 
             try:
                 # Проход по всем персональным качествам личности человека
-                for i in range(len(self._b5["en"])):
+                for i in range(len(self._b5['en'])):
                     concat.append(
                         np.hstack((np.asarray(pred_hc_norm)[:, i], np.asarray(pred_melspectrogram_norm)[:, i]))
                     )
-            except IndexError:
-                self._other_error(self._concat_audio_pred_error, last=False, out=out)
-                return []
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return []
+            except IndexError: self._other_error(self._concat_audio_pred_error, last = False, out = out); return []
+            except Exception: self._other_error(self._unknown_err, out = out); return []
 
             return concat
 
     def __load_audio_model_b5(
         self, show_summary: bool = False, out: bool = True
-    ) -> Optional[tf.keras.Model]:
+    ) -> Optional[keras.engine.functional.Functional]:
         """Формирование нейросетевой архитектуры модели для получения результата оценки персонального качества
 
         .. note::
             private (приватный метод)
 
         Args:
             show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
             out (bool): Отображение
 
         Returns:
-            Optional[tf.keras.Model]:
+            Optional[keras.engine.functional.Functional]:
                 **None** если неверные типы или значения аргументов, в обратном случае нейросетевая модель
                 **tf.keras.Model** для получения результата оценки персонального качества
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
@@ -993,15 +922,15 @@
                  activ_1 (Activation)        (None, 1)                 0
 
                 =================================================================
                 Total params: 33
                 Trainable params: 33
                 Non-trainable params: 0
                 _________________________________________________________________
-                <tf.keras.Model at 0x13d442940>
+                <keras.engine.functional.Functional at 0x13d442940>
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
@@ -1019,45 +948,36 @@
                 :linenos:
 
                 [2022-10-17 10:53:03] Неверные типы или значения аргументов в "Audio.__load_audio_model_b5" ...
         """
 
         try:
             # Проверка аргументов
-            if type(show_summary) is not bool or type(out) is not bool:
-                raise TypeError
+            if type(show_summary) is not bool or type(out) is not bool: raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__load_audio_model_b5.__name__, out=out)
-            return None
+            self._inv_args(__class__.__name__, self.__load_audio_model_b5.__name__, out = out); return None
         else:
-            input_1 = tf.keras.Input(shape=(32,), name="input_1")
-            x = tf.keras.layers.Dense(units=1, name="dense_1")(input_1)
-            x = tf.keras.layers.Activation("sigmoid", name="activ_1")(x)
+            input_1 = tf.keras.Input(shape = (32,), name = 'input_1')
+            x = tf.keras.layers.Dense(units = 1, name = 'dense_1')(input_1)
+            x = tf.keras.layers.Activation('sigmoid', name = 'activ_1')(x)
 
-            model = tf.keras.Model(inputs=input_1, outputs=x)
+            model = tf.keras.Model(inputs = input_1, outputs = x)
 
-            if show_summary and out:
-                model.summary()
+            if show_summary and out: model.summary()
 
             return model
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (защищенные)
     # ------------------------------------------------------------------------------------------------------------------
 
     def _get_acoustic_features(
-        self,
-        path: str,
-        sr: int = 44100,
-        window: Union[int, float] = 2.0,
-        step: Union[int, float] = 1.0,
-        last: bool = False,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+        self, path: str, sr: int = 44100, window: Union[int, float] = 2.0,
+        step: Union[int, float] = 1.0, last: bool = False, out: bool = True, runtime: bool = True,
+        run: bool = True
     ) -> Tuple[List[Optional[np.ndarray]], List[Optional[np.ndarray]]]:
         """Извлечение признаков из акустического сигнала (без очистки истории вывода сообщений в ячейке Jupyter)
 
         .. note::
             protected (защищенный метод)
 
         Args:
@@ -1177,171 +1097,129 @@
                     Тип ошибки: IsSmallWindowSizeError
 
                 --- Время выполнения: 0.049 сек. ---
         """
 
         try:
             # Проверка аргументов
-            if (
-                (type(path) is not str or not path) and (type(path) is not gradio.utils.NamedString)
-                or type(sr) is not int
-                or sr < 1
+            if (type(path) is not str or not path or type(sr) is not int or sr < 1
                 or ((type(window) is not int or window < 1) and (type(window) is not float or window <= 0))
                 or ((type(step) is not int or step < 1) and (type(step) is not float or step <= 0))
-                or type(last) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+                or type(last) is not bool or type(out) is not bool or type(runtime) is not bool
+                or type(run) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self._get_acoustic_features.__name__, last=last, out=out)
+            self._inv_args(__class__.__name__, self._get_acoustic_features.__name__, last = last, out = out)
             return [], []
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, last=last, out=out)
-                return [], []
+            if run is False: self._error(self._lock_user, last = last, out = out); return [], []
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             if last is False:
                 # Информационное сообщение
-                self._info(self._get_acoustic_feature_info, out=False)
-                if out:
-                    self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+                self._info(self._get_acoustic_feature_info, out = False)
+                if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
             try:
                 # Считывание аудио или видеофайла
-                path_to_wav = os.path.join(str(Path(path).parent), Path(path).stem + "." + "wav")
-
-                if not Path(path_to_wav).is_file():
-                    if Path(path).suffix not in ["mp3", "wav"]:
-                        ff_audio = "ffmpeg -loglevel quiet -i {} -vn -acodec pcm_s16le -ar 44100 -ac 2 {}".format(
-                            path, path_to_wav
-                        )
-                        call_audio = subprocess.call(ff_audio, shell=True)
-
-                        try:
-                            if call_audio == 1:
-                                raise OSError
-                        except OSError:
-                            self._other_error(self._unknown_err, last=last, out=out)
-                            return np.empty([]), np.empty([])
-                        except Exception:
-                            self._other_error(self._unknown_err, last=last, out=out)
-                            return np.empty([]), np.empty([])
-                        else:
-                            audio, sr = librosa.load(path=path_to_wav, sr=sr)
-                else:
-                    audio, sr = librosa.load(path=path_to_wav, sr=sr)
+                audio, sr = librosa.load(path = path, sr = sr)
             except FileNotFoundError:
-                self._other_error(self._file_not_found.format(self._info_wrapper(path)), last=last, out=out)
+                self._other_error(self._file_not_found.format(self._info_wrapper(path)), last = last, out = out)
                 return [], []
             except IsADirectoryError:
-                self._other_error(self._directory_inst_file.format(self._info_wrapper(path)), last=last, out=out)
+                self._other_error(self._directory_inst_file.format(self._info_wrapper(path)), last = last, out = out)
                 return [], []
             except audioread.NoBackendError:
-                self._other_error(self._no_acoustic_signal.format(self._info_wrapper(path)), last=last, out=out)
-                return [], []
-            except Exception:
-                self._other_error(self._unknown_err, last=last, out=out)
+                self._other_error(self._no_acoustic_signal.format(self._info_wrapper(path)), last = last, out = out)
                 return [], []
+            except Exception: self._other_error(self._unknown_err, last = last, out = out); return [], []
             else:
-                hc_features = []  # Список с экспертными признаками
-                melspectrogram_features = []  # Список с лог мел-спектрограммами
+                hc_features = [] # Список с экспертными признаками
+                melspectrogram_features = [] # Список с лог мел-спектрограммами
 
                 try:
                     lhcf = int((window * 1000 - 40) / 10)
 
-                    if lhcf < 2:
-                        raise IsSmallWindowSizeError
+                    if lhcf < 2: raise IsSmallWindowSizeError
                 except IsSmallWindowSizeError:
-                    self._other_error(
-                        self._window_small_size_error.format(self._info_wrapper(str(window))), last=last, out=out
-                    )
-                    return [], []
-                except Exception:
-                    self._other_error(self._unknown_err, last=last, out=out)
+                    self._other_error(self._window_small_size_error.format(self._info_wrapper(str(window))),
+                                      last = last, out = out)
                     return [], []
+                except Exception: self._other_error(self._unknown_err, last = last, out = out); return [], []
                 else:
                     window_local = int(sr * window)
 
                     len_spec = window_local / self.__pl[1]
-                    if math.modf(len_spec)[0] == 0:
-                        len_spec += 1
+                    if math.modf(len_spec)[0] == 0: len_spec += 1
                     len_spec = math.ceil(len_spec)
 
                     for cnt, val in enumerate(range(0, audio.shape[0] + 1, int(sr * step))):
                         val_end = val + window_local
 
-                        curr_audio = audio[val:val_end]  # Часть аудио
+                        curr_audio = audio[val:val_end] # Часть аудио
 
                         # Формирование экспертных признаков
                         hc_feature = self.smile_.process_signal(curr_audio, sr).to_numpy()
 
                         try:
                             # Нормализация экспертных признаков
-                            hc_feature = preprocessing.normalize(hc_feature, norm="l2", axis=0)
-                        except Exception:
-                            pass
+                            hc_feature = preprocessing.normalize(hc_feature, norm = 'l2', axis = 0)
+                        except Exception: pass
                         else:
                             # Дополнение экспертных признаков нулями
                             hc_feature = np.pad(hc_feature, ((0, lhcf - hc_feature.shape[0]), (0, 0)))
-                            hc_features.append(hc_feature)  # Добавление экспертных признаков в список
+                            hc_features.append(hc_feature) # Добавление экспертных признаков в список
 
                         # Получение лог мел-спектрограмм
                         if len(curr_audio) > self.__pl[0]:
                             melspectrogram = librosa.feature.melspectrogram(
-                                y=curr_audio,
-                                sr=sr,
-                                n_fft=self.__pl[0],
-                                hop_length=self.__pl[1],
-                                win_length=self.__pl[2],
-                                center=self.__pl[3],
-                                pad_mode=self.__pl[4],
-                                power=self.__pl[5],
-                                n_mels=self.__pl[6],
-                                norm=self.__pl[7],
-                                htk=self.__pl[8],
-                                fmax=self.__pl[9],
+                                y          = curr_audio,
+                                sr         = sr,
+                                n_fft      = self.__pl[0],
+                                hop_length = self.__pl[1],
+                                win_length = self.__pl[2],
+                                center     = self.__pl[3],
+                                pad_mode   = self.__pl[4],
+                                power      = self.__pl[5],
+                                n_mels     = self.__pl[6],
+                                norm       = self.__pl[7],
+                                htk        = self.__pl[8],
+                                fmax       = self.__pl[9]
                             )
 
                             # Преобразование спектрограммы из мощности (квадрат амплитуды) в децибелы (дБ)
-                            melspectrogram_to_db = librosa.power_to_db(melspectrogram, top_db=80)
+                            melspectrogram_to_db = librosa.power_to_db(melspectrogram, top_db = 80)
 
                             if melspectrogram_to_db.shape[1] < len_spec:
                                 melspectrogram_to_db = np.pad(
                                     melspectrogram_to_db,
                                     ((0, 0), (0, len_spec - melspectrogram_to_db.shape[1])),
-                                    "mean",
+                                    'mean'
                                 )
-                            melspectrogram_to_db /= 255  # Линейная нормализация
-                            melspectrogram_to_db = np.expand_dims(melspectrogram_to_db, axis=-1)
-                            melspectrogram_to_db = tf.image.resize(melspectrogram_to_db, (224, 224))  # Масштабирование
-                            melspectrogram_to_db = tf.repeat(melspectrogram_to_db, 3, axis=-1)  # GRAY -> RGB
+                            melspectrogram_to_db /= 255 # Линейная нормализация
+                            melspectrogram_to_db = np.expand_dims(melspectrogram_to_db, axis = -1)
+                            melspectrogram_to_db = tf.image.resize(melspectrogram_to_db, (224, 224)) # Масштабирование
+                            melspectrogram_to_db = tf.repeat(melspectrogram_to_db, 3, axis = -1) # GRAY -> RGB
                             # Добавление лог мел-спектрограммы в список
                             melspectrogram_features.append(melspectrogram_to_db)
 
                     if last is False:
                         # Статистика извлеченных признаков из акустического сигнала
                         self._stat_acoustic_features(
-                            last=last,
-                            out=out,
-                            len_hc_features=len(hc_features),
-                            len_melspectrogram_features=len(melspectrogram_features),
-                            shape_hc_features=hc_features[0].shape,
-                            shape_melspectrogram_features=melspectrogram_features[0].shape,
+                            last = last, out = out,
+                            len_hc_features = len(hc_features),
+                            len_melspectrogram_features = len(melspectrogram_features),
+                            shape_hc_features = hc_features[0].shape,
+                            shape_melspectrogram_features = melspectrogram_features[0].shape
                         )
 
                     return hc_features, melspectrogram_features
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внешние методы
     # ------------------------------------------------------------------------------------------------------------------
 
     def load_audio_model_hc(
         self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
@@ -1405,57 +1283,44 @@
                 :linenos:
 
                 [2022-10-17 13:20:04] Неверные типы или значения аргументов в "Audio.load_audio_model_hc" ...
 
                 False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.load_audio_model_hc.__name__, out=out)
-            return False
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
+        except TypeError: self._inv_args(__class__.__name__, self.load_audio_model_hc.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(self._formation_audio_model_hc, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            self._info(self._formation_audio_model_hc, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
-            input_lstm = tf.keras.Input(shape=(196, 25))
+            input_lstm = tf.keras.Input(shape = (196, 25))
 
-            x = tf.keras.layers.LSTM(64, return_sequences=True)(input_lstm)
-            x = tf.keras.layers.Dropout(rate=0.2)(x)
-            x = tf.keras.layers.LSTM(128, return_sequences=False, name="lstm_128_a_hc")(x)
-            x = tf.keras.layers.Dropout(rate=0.2)(x)
-            x = tf.keras.layers.Dense(5, activation="linear")(x)
+            x = tf.keras.layers.LSTM(64, return_sequences = True)(input_lstm)
+            x = tf.keras.layers.Dropout(rate = 0.2)(x)
+            x = tf.keras.layers.LSTM(128, return_sequences = False)(x)
+            x = tf.keras.layers.Dropout(rate = 0.2)(x)
+            x = tf.keras.layers.Dense(5, activation = 'linear')(x)
 
-            self._audio_model_hc = tf.keras.Model(inputs=input_lstm, outputs=x)
+            self._audio_model_hc = tf.keras.Model(inputs = input_lstm, outputs = x)
 
-            if show_summary and out:
-                self._audio_model_hc.summary()
+            if show_summary and out: self._audio_model_hc.summary()
 
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
             return True
 
     def load_audio_model_nn(
         self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
         """Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам
@@ -1574,58 +1439,46 @@
                 :linenos:
 
                 [2022-10-17 13:25:40] Неверные типы или значения аргументов в "Audio.load_audio_model_nn" ...
 
                 False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.load_audio_model_nn.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_audio_model_nn.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(self._formation_audio_model_nn, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            self._info(self._formation_audio_model_nn, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
-            vgg_model = VGG16(weights=None, include_top=False, input_shape=(224, 224, 3))
+            vgg_model = VGG16(weights = None, include_top = False, input_shape = (224, 224, 3))
 
             x = vgg_model.output
             x = tf.keras.layers.Flatten()(x)
-            x = tf.keras.layers.Dense(512, activation="relu")(x)
+            x = tf.keras.layers.Dense(512, activation = 'relu')(x)
             x = tf.keras.layers.Dropout(0.5)(x)
-            x = tf.keras.layers.Dense(256, activation="relu", name="dense_256")(x)
-            x = tf.keras.layers.Dense(5, activation="linear")(x)
+            x = tf.keras.layers.Dense(256, activation = 'relu')(x)
+            x = tf.keras.layers.Dense(5, activation = 'linear')(x)
 
-            self._audio_model_nn = tf.keras.models.Model(inputs=vgg_model.input, outputs=x)
+            self._audio_model_nn = tf.keras.models.Model(inputs = vgg_model.input, outputs = x)
 
-            if show_summary and out:
-                self._audio_model_nn.summary()
+            if show_summary and out: self._audio_model_nn.summary()
 
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
             return True
 
     def load_audio_models_b5(
         self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
         """Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств
@@ -1703,50 +1556,38 @@
                 :linenos:
 
                 [2022-10-18 13:47:36] Неверные типы или значения аргументов в "Audio.load_audio_models_b5" ...
 
                 False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.load_audio_models_b5.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_audio_models_b5.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(self._formation_audio_models_b5, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            self._info(self._formation_audio_models_b5, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
             for key, _ in self._audio_models_b5.items():
                 self._audio_models_b5[key] = self.__load_audio_model_b5()
 
-            if show_summary and out:
-                self._audio_models_b5[key].summary()
+            if show_summary and out: self._audio_models_b5[key].summary()
 
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
             return True
 
     def load_audio_model_weights_hc(
         self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
         """Загрузка весов нейросетевой модели для получения оценок по экспертным признакам
@@ -1855,32 +1696,22 @@
                 [2022-10-17 15:21:14] Что-то пошло не так ... нейросетевая архитектура модели для получения оценок по экспертным признакам не сформирована (аудио модальность) ...
 
                 --- Время выполнения: 0.364 сек. ---
 
                 False
         """
 
-        if runtime:
-            self._r_start()
+        if runtime: self._r_start()
 
         if self.__load_model_weights(url, force_reload, self._load_audio_model_weights_hc, out, False, run) is True:
-            try:
-                self._audio_model_hc.load_weights(self._url_last_filename)
-                self._audio_model_hc = tf.keras.models.Model(
-                    inputs=self._audio_model_hc.input,
-                    outputs=[self._audio_model_hc.output, self._audio_model_hc.get_layer("lstm_128_a_hc").output],
-                )
-            except Exception:
-                self._error(self._model_audio_hc_not_formation, out=out)
-                return False
-            else:
-                return True
+            try: self._audio_model_hc.load_weights(self._url_last_filename)
+            except Exception: self._error(self._model_audio_hc_not_formation, out = out); return False
+            else: return True
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
 
         return False
 
     def load_audio_model_weights_nn(
         self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
         """Загрузка весов нейросетевой модели для получения оценок по нейросетевым признакам
@@ -1991,55 +1822,37 @@
                 [2022-10-17 15:50:04] Что-то пошло не так ... нейросетевая архитектура модели для получения оценок по нейросетевым признакам не сформирована (аудио модальность) ...
 
                 --- Время выполнения: 6.786 сек. ---
 
                 False
         """
 
-        if runtime:
-            self._r_start()
+        if runtime: self._r_start()
 
         if self.__load_model_weights(url, force_reload, self._load_audio_model_weights_nn, out, False, run) is True:
-            try:
-                self._audio_model_nn.load_weights(self._url_last_filename)
-                self._audio_model_nn = tf.keras.models.Model(
-                    inputs=self._audio_model_nn.input,
-                    outputs=[self._audio_model_nn.output, self._audio_model_nn.get_layer("dense_256").output],
-                )
-            except Exception:
-                self._error(self._model_audio_nn_not_formation, out=out)
-                return False
-            else:
-                return True
+            try: self._audio_model_nn.load_weights(self._url_last_filename)
+            except Exception: self._error(self._model_audio_nn_not_formation, out = out); return False
+            else: return True
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
 
         return False
 
     def load_audio_models_weights_b5(
-        self,
-        url_openness: str,
-        url_conscientiousness: str,
-        url_extraversion: str,
-        url_agreeableness: str,
-        url_non_neuroticism: str,
-        force_reload: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+        self, url_openness: str, url_conscientiousness: str, url_extraversion: str, url_agreeableness: str,
+        url_neuroticism: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
         """Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств
 
         Args:
             url_openness (str): Полный путь к файлу с весами нейросетевой модели (открытость опыту)
             url_conscientiousness (str): Полный путь к файлу с весами нейросетевой модели (добросовестность)
             url_extraversion (str): Полный путь к файлу с весами нейросетевой модели (экстраверсия)
             url_agreeableness (str): Полный путь к файлу с весами нейросетевой модели (доброжелательность)
-            url_non_neuroticism (str): Полный путь к файлу с весами нейросетевой модели (эмоциональная стабильность)
+            url_neuroticism (str): Полный путь к файлу с весами нейросетевой модели (нейротизм)
             force_reload (bool): Принудительная загрузка файлов с весами нейросетевых моделей из сети
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
             bool: **True** если веса нейросетевых моделей загружены, в обратном случае **False**
@@ -2082,22 +1895,22 @@
                 audio.path_to_save_ = './models'
                 audio.chunk_size_ = 2000000
 
                 url_openness = audio.weights_for_big5_['audio']['b5']['openness']['sberdisk']
                 url_conscientiousness = audio.weights_for_big5_['audio']['b5']['conscientiousness']['sberdisk']
                 url_extraversion = audio.weights_for_big5_['audio']['b5']['extraversion']['sberdisk']
                 url_agreeableness = audio.weights_for_big5_['audio']['b5']['agreeableness']['sberdisk']
-                url_non_neuroticism = audio.weights_for_big5_['audio']['b5']['non_neuroticism']['sberdisk']
+                url_neuroticism = audio.weights_for_big5_['audio']['b5']['neuroticism']['sberdisk']
 
                 audio.load_audio_models_weights_b5(
                     url_openness = url_openness,
                     url_conscientiousness = url_conscientiousness,
                     url_extraversion = url_extraversion,
                     url_agreeableness = url_agreeableness,
-                    url_non_neuroticism = url_non_neuroticism,
+                    url_neuroticism = url_neuroticism,
                     force_reload = True,
                     out = True,
                     runtime = True,
                     run = True
                 )
 
             .. output-cell::
@@ -2111,15 +1924,15 @@
 
                 [2022-10-18 23:08:38] Загрузка файла "weights_2022-06-15_16-21-57.h5" (100.0%) ... Добросовестность
 
                 [2022-10-18 23:08:38] Загрузка файла "weights_2022-06-15_16-26-41.h5" (100.0%) ... Экстраверсия
 
                 [2022-10-18 23:08:38] Загрузка файла "weights_2022-06-15_16-32-51.h5" (100.0%) ... Доброжелательность
 
-                [2022-10-18 23:08:39] Загрузка файла "weights_2022-06-15_16-37-46.h5" (100.0%) ... Эмоциональная стабильность
+                [2022-10-18 23:08:39] Загрузка файла "weights_2022-06-15_16-37-46.h5" (100.0%) ... Нейротизм
 
                 --- Время выполнения: 1.611 сек. ---
 
                 True
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
@@ -2135,22 +1948,22 @@
                 audio.path_to_save_ = './models'
                 audio.chunk_size_ = 2000000
 
                 url_openness = audio.weights_for_big5_['audio']['b5']['openness']['sberdisk']
                 url_conscientiousness = audio.weights_for_big5_['audio']['b5']['conscientiousness']['sberdisk']
                 url_extraversion = audio.weights_for_big5_['audio']['b5']['extraversion']['sberdisk']
                 url_agreeableness = audio.weights_for_big5_['audio']['b5']['agreeableness']['sberdisk']
-                url_non_neuroticism = audio.weights_for_big5_['audio']['b5']['non_neuroticism']['sberdisk']
+                url_neuroticism = audio.weights_for_big5_['audio']['b5']['neuroticism']['sberdisk']
 
                 audio.load_audio_models_weights_b5(
                     url_openness = url_openness,
                     url_conscientiousness = url_conscientiousness,
                     url_extraversion = url_extraversion,
                     url_agreeableness = url_agreeableness,
-                    url_non_neuroticism = url_non_neuroticism,
+                    url_neuroticism = url_neuroticism,
                     force_reload = True,
                     out = True,
                     runtime = True,
                     run = True
                 )
 
             .. output-cell::
@@ -2199,149 +2012,113 @@
                     Линия: 1764
                     Метод: load_audio_models_weights_b5
                     Тип ошибки: AttributeError
 
                 [2022-10-18 23:09:42] Загрузка файла "weights_2022-06-15_16-37-46.h5" (100.0%) ...
 
                 [2022-10-18 23:09:42] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ...
-                Эмоциональная стабильность
+                Нейротизм
 
                     Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/audio.py
                     Линия: 1764
                     Метод: load_audio_models_weights_b5
                     Тип ошибки: AttributeError
 
                 --- Время выполнения: 1.573 сек. ---
 
                 False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(url_openness) is not str
-                or not url_openness
-                or type(url_conscientiousness) is not str
-                or not url_conscientiousness
-                or type(url_extraversion) is not str
-                or not url_extraversion
-                or type(url_agreeableness) is not str
-                or not url_agreeableness
-                or type(url_non_neuroticism) is not str
-                or not url_non_neuroticism
+            if (type(url_openness) is not str or not url_openness
+                or type(url_conscientiousness) is not str or not url_conscientiousness
+                or type(url_extraversion) is not str or not url_extraversion
+                or type(url_agreeableness) is not str or not url_agreeableness
+                or type(url_neuroticism) is not str or not url_neuroticism
                 or type(force_reload) is not bool
                 or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+                or type(runtime) is not bool or type(run) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.load_audio_models_weights_b5.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_audio_models_weights_b5.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
-            result_download_models = 0  # Все веса нейросетевых моделей по умолчанию загружены
+            result_download_models = 0 # Все веса нейросетевых моделей по умолчанию загружены
 
             # Информационное сообщение
-            self._info(self._load_audio_models_weights_b5, last=False, out=out)
+            self._info(self._load_audio_models_weights_b5, last = False, out = out)
 
             # Проход по всем URL с весами нейросетевых моделей
-            for cnt, url in enumerate(
-                [
-                    (url_openness, self._b5["ru"][0]),
-                    (url_conscientiousness, self._b5["ru"][1]),
-                    (url_extraversion, self._b5["ru"][2]),
-                    (url_agreeableness, self._b5["ru"][3]),
-                    (url_non_neuroticism, self._b5["ru"][4]),
-                ]
-            ):
-                sections = urlparse(url[0])  # Парсинг URL адреса
+            for cnt, url in enumerate([
+                (url_openness, self._b5['ru'][0]),
+                (url_conscientiousness, self._b5['ru'][1]),
+                (url_extraversion, self._b5['ru'][2]),
+                (url_agreeableness, self._b5['ru'][3]),
+                (url_neuroticism, self._b5['ru'][4]),
+            ]):
+                sections = urlparse(url[0]) # Парсинг URL адреса
 
                 try:
                     # URL файл невалидный
-                    if sections.scheme == "":
-                        raise requests.exceptions.InvalidURL
+                    if sections.scheme == '': raise requests.exceptions.InvalidURL
                 except requests.exceptions.InvalidURL:
                     url_norm = os.path.normpath(url[0])
 
                     try:
-                        if os.path.isfile(url_norm) is False:
-                            raise FileNotFoundError  # Не файл
-                    except FileNotFoundError:
-                        self._other_error(
-                            self._load_model_weights_error + " " + self._bold_wrapper(url[1].capitalize()), out=out
-                        )
-                        continue
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        continue
+                        if os.path.isfile(url_norm) is False: raise FileNotFoundError # Не файл
+                    except FileNotFoundError: self._other_error(
+                            self._load_model_weights_error + ' ' + self._bold_wrapper(url[1].capitalize()), out = out
+                        ); continue
+                    except Exception: self._other_error(self._unknown_err, out = out); continue
                     else:
                         self._url_last_filename = url_norm
 
                         # Отображение истории вывода сообщений в ячейке Jupyter
-                        if out:
-                            self.show_notebook_history_output()
+                        if out: self.show_notebook_history_output()
                 else:
                     try:
-                        if force_reload is False:
-                            clear_output(True)
+                        if force_reload is False: clear_output(True)
                         # Загрузка файла из URL
                         res_download_file_from_url = self._download_file_from_url(
-                            url=url[0], force_reload=force_reload, runtime=False, out=out, run=True
+                            url = url[0], force_reload = force_reload, runtime = False, out = out, run = True
                         )
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        continue
+                    except Exception: self._other_error(self._unknown_err, out = out); continue
                     else:
                         # Файл загружен
-                        if res_download_file_from_url != 200:
-                            continue
+                        if res_download_file_from_url != 200: continue
 
                         try:
-                            self._audio_models_b5[self._b5["en"][cnt]].load_weights(self._url_last_filename)
-                        except Exception:
-                            self._other_error(
-                                self._load_model_weights_error + " " + self._bold_wrapper(url[1].capitalize()), out=out
-                            )
-                            continue
+                            self._audio_models_b5[self._b5['en'][cnt]].load_weights(self._url_last_filename)
+                        except Exception: self._other_error(
+                                self._load_model_weights_error + ' ' + self._bold_wrapper(url[1].capitalize()),
+                                out = out
+                            ); continue
                         else:
                             self._add_last_el_notebook_history_output(self._bold_wrapper(url[1].capitalize()))
 
                             result_download_models += 1
 
             clear_output(True)
             # Отображение истории вывода сообщений в ячейке Jupyter
-            if out:
-                self.show_notebook_history_output()
+            if out: self.show_notebook_history_output()
 
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
-            if result_download_models != len(self._b5["ru"]):
-                return False
+            if result_download_models != len(self._b5['ru']): return False
             return True
 
     def get_acoustic_features(
-        self,
-        path: str,
-        sr: int = 44100,
-        window: Union[int, float] = 2.0,
-        step: Union[int, float] = 1.0,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+        self, path: str, sr: int = 44100, window: Union[int, float] = 2.0,
+        step: Union[int, float] = 1.0, out: bool = True, runtime: bool = True, run: bool = True
     ) -> Tuple[List[Optional[np.ndarray]], List[Optional[np.ndarray]]]:
         """Извлечение признаков из акустического сигнала
 
         Args:
             path (str): Путь к аудио или видеофайлу
             sr (int): Частота дискретизации
             window (Union[int, float]): Размер окна сегмента сигнала (в секундах)
@@ -2355,33 +2132,24 @@
 
                 1. Список с экспертными признаками
                 2. Список с лог мел-спектрограммами
 
         :bdg-link-light:`Пример <../../user_guide/notebooks/Audio-get_acoustic_features.ipynb>`
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
-        return self._get_acoustic_features(
-            path=path, sr=sr, window=window, step=step, last=False, out=out, runtime=runtime, run=run
-        )
+        return self._get_acoustic_features(path = path, sr = sr, window = window, step = step, last = False, out = out,
+                                           runtime = runtime, run = run)
 
     def get_audio_union_predictions(
-        self,
-        depth: int = 1,
-        recursive: bool = False,
-        sr: int = 44100,
-        window: Union[int, float] = 2.0,
-        step: Union[int, float] = 1.0,
-        accuracy=True,
-        url_accuracy: str = "",
-        logs: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+        self, depth: int = 1, recursive: bool = False, sr: int = 44100,
+        window: Union[int, float] = 2.0, step: Union[int, float] = 1.0,
+        accuracy = True, url_accuracy: str = '', logs: bool = True, out: bool = True, runtime: bool = True,
+        run: bool = True
     ) -> bool:
         """Получения прогнозов по аудио
 
         Args:
             depth (int): Глубина иерархии для получения данных
             recursive (bool): Рекурсивный поиск данных
             sr (int): Частота дискретизации
@@ -2391,362 +2159,290 @@
             url_accuracy (str): Полный путь к файлу с верными предсказаниями для подсчета точности
             logs (bool): При необходимости формировать LOG файл
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если прогнозы успешно получены, в обратном случае **False**
+            bool: **True** если веса прогнозы успешно получены, в обратном случае **False**
 
         :bdg-link-light:`Пример <../../user_guide/notebooks/Audio-get_audio_union_predictions.ipynb>`
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         # Сброс
-        self._df_files = pd.DataFrame()  # Пустой DataFrame с данными
-        self._df_accuracy = pd.DataFrame()  # Пустой DataFrame с результатами вычисления точности
+        self._df_files = pd.DataFrame() # Пустой DataFrame с данными
+        self._df_accuracy = pd.DataFrame() # Пустой DataFrame с результатами вычисления точности
 
         try:
             # Проверка аргументов
-            if (
-                type(depth) is not int
-                or depth < 1
-                or type(out) is not bool
-                or type(recursive) is not bool
-                or type(sr) is not int
-                or sr < 1
-                or ((type(window) is not int or window < 1) and (type(window) is not float or window <= 0))
-                or ((type(step) is not int or step < 1) and (type(step) is not float or step <= 0))
-                or type(accuracy) is not bool
-                or type(url_accuracy) is not str
-                or type(logs) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
+            if (type(depth) is not int or depth < 1 or type(out) is not bool or type(recursive) is not bool
+                    or type(sr) is not int or sr < 1
+                    or ((type(window) is not int or window < 1) and (type(window) is not float or window <= 0))
+                    or ((type(step) is not int or step < 1) and (type(step) is not float or step <= 0))
+                    or type(accuracy) is not bool or type(url_accuracy) is not str
+                    or type(logs) is not bool or type(runtime) is not bool or type(run) is not bool):
                 raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.get_audio_union_predictions.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.get_audio_union_predictions.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             try:
                 # Получение директорий, где хранятся данные
-                path_to_data = self._get_paths(self.path_to_dataset_, depth, out=out)
-                if type(path_to_data) is bool:
-                    return False
+                path_to_data = self._get_paths(self.path_to_dataset_, depth, out = out)
+                if type(path_to_data) is bool: return False
 
-                if type(self.keys_dataset_) is not list:
-                    raise TypeError
+                if type(self.keys_dataset_) is not list: raise TypeError
 
                 # Словарь для DataFrame набора данных с данными
                 self._dict_of_files = dict(zip(self.keys_dataset_, [[] for _ in range(0, len(self.keys_dataset_))]))
                 # Словарь для DataFrame набора данных с результатами вычисления точности
                 self._dict_of_accuracy = dict(
                     zip(self.keys_dataset_[1:], [[] for _ in range(0, len(self.keys_dataset_[1:]))])
                 )
             except (TypeError, FileNotFoundError):
-                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out=out)
-                return False
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
+                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out = out)
                 return False
+            except Exception: self._other_error(self._unknown_err, out = out); return False
             else:
                 # Вычисление точности
                 if accuracy is True:
                     get_audio_union_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
-                else:
-                    get_audio_union_predictions_info = self._get_union_predictions_info
+                else: get_audio_union_predictions_info = self._get_union_predictions_info
 
                 get_audio_union_predictions_info += self._audio_modality
 
                 # Вычисление точности
                 if accuracy is True:
                     # Информационное сообщение
-                    self._info(get_audio_union_predictions_info, out=out)
+                    self._info(get_audio_union_predictions_info, out = out)
 
-                    if not url_accuracy:
-                        url_accuracy = self._true_traits["sberdisk"]
+                    if not url_accuracy: url_accuracy = self._true_traits['sberdisk']
 
                     try:
                         # Загрузка верных предсказаний
                         data_true_traits = pd.read_csv(url_accuracy)
                     except (FileNotFoundError, URLError, UnicodeDecodeError):
-                        self._other_error(self._load_data_true_traits_error, out=out)
-                        return False
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return False
+                        self._other_error(self._load_data_true_traits_error, out = out); return False
+                    except Exception: self._other_error(self._unknown_err, out = out); return False
                     else:
                         true_traits = []
                         self._del_last_el_notebook_history_output()
 
-                paths = []  # Пути до искомых файлов
+                paths = [] # Пути до искомых файлов
 
                 # Проход по всем директориям
                 for curr_path in path_to_data:
-                    empty = True  # По умолчанию директория пустая
+                    empty = True # По умолчанию директория пустая
 
                     # Рекурсивный поиск данных
-                    if recursive is True:
-                        g = Path(curr_path).rglob("*")
-                    else:
-                        g = Path(curr_path).glob("*")
+                    if recursive is True: g = Path(curr_path).rglob('*')
+                    else: g = Path(curr_path).glob('*')
 
                     # Формирование словаря для DataFrame
                     for p in g:
                         try:
-                            if type(self.ext_) is not list or len(self.ext_) < 1:
-                                raise TypeError
+                            if type(self.ext_) is not list or len(self.ext_) < 1: raise TypeError
 
                             self.ext_ = [x.lower() for x in self.ext_]
-                        except TypeError:
-                            self._other_error(self._wrong_ext, out=out)
-                            return False
-                        except Exception:
-                            self._other_error(self._unknown_err, out=out)
-                            return False
+                        except TypeError: self._other_error(self._wrong_ext, out = out); return False
+                        except Exception: self._other_error(self._unknown_err, out = out); return False
                         else:
                             # Расширение файла соответствует расширению искомых файлов
                             if p.suffix.lower() in self.ext_:
-                                if empty is True:
-                                    empty = False  # Каталог не пустой
+                                if empty is True: empty = False # Каталог не пустой
 
                                 paths.append(p.resolve())
 
                 try:
-                    self.__len_paths = len(paths)  # Количество искомых файлов
+                    self.__len_paths = len(paths) # Количество искомых файлов
 
-                    if self.__len_paths == 0:
-                        raise TypeError
-                except TypeError:
-                    self._other_error(self._files_not_found, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
+                    if self.__len_paths == 0: raise TypeError
+                except TypeError: self._other_error(self._files_not_found, out = out); return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
                 else:
                     # Локальный путь
                     self.__local_path = lambda path: os.path.join(
-                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))) :]
+                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))):]
                     )
 
-                    last = False  # Замена последнего сообщения
+                    last = False # Замена последнего сообщения
 
                     # Проход по всем искомым файлов
                     for i, curr_path in enumerate(paths):
-                        if i != 0:
-                            last = True
+                        if i != 0: last = True
 
                         # Индикатор выполнения
                         self._progressbar_union_predictions(
-                            get_audio_union_predictions_info,
-                            i,
-                            self.__local_path(curr_path),
-                            self.__len_paths,
-                            True,
-                            last,
-                            out,
+                            get_audio_union_predictions_info, i, self.__local_path(curr_path), self.__len_paths,
+                            True, last, out
                         )
 
                         # Извлечение признаков из акустического сигнала
                         hc_features, melspectrogram_features = self._get_acoustic_features(
-                            path=str(curr_path.resolve()),
-                            sr=sr,
-                            window=window,
-                            step=step,
-                            last=True,
-                            out=False,
-                            runtime=False,
-                            run=run,
+                            path = str(curr_path.resolve()),
+                            sr = sr,
+                            window = window,
+                            step = step,
+                            last = True, out = False, runtime = False, run = run
                         )
 
                         # Признаки из акустического сигнала извлечены
                         if len(hc_features) > 0 and len(melspectrogram_features) > 0:
                             # Коды ошибок нейросетевых моделей
                             code_error_pred_hc = -1
                             code_error_pred_melspectrogram = -1
 
                             try:
                                 # Оправка экспертных признаков в нейросетевую модель
-                                pred_hc, _ = self.audio_model_hc_(np.array(hc_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_hc = 1
-                            except Exception:
-                                code_error_pred_hc = 2
+                                pred_hc = self.audio_model_hc_(np.array(hc_features, dtype = np.float16)).numpy()
+                            except TypeError: code_error_pred_hc = 1
+                            except Exception: code_error_pred_hc = 2
 
                             try:
                                 # Отправка нейросетевых признаков в нейросетевую модель
-                                pred_melspectrogram, _ = self.audio_model_nn_(
-                                    np.array(melspectrogram_features, dtype=np.float16)
-                                )
-                            except TypeError:
-                                code_error_pred_melspectrogram = 1
-                            except Exception:
-                                code_error_pred_melspectrogram = 2
+                                pred_melspectrogram = self.audio_model_nn_(
+                                    np.array(melspectrogram_features, dtype = np.float16)
+                                ).numpy()
+                            except TypeError: code_error_pred_melspectrogram = 1
+                            except Exception: code_error_pred_melspectrogram = 2
 
                             if code_error_pred_hc != -1 and code_error_pred_melspectrogram != -1:
-                                self._error(self._models_audio_not_formation, out=out)
-                                return False
+                                self._error(self._models_audio_not_formation, out = out); return False
 
                             if code_error_pred_hc != -1:
-                                self._error(self._model_audio_hc_not_formation, out=out)
-                                return False
+                                self._error(self._model_audio_hc_not_formation, out = out); return False
 
                             if code_error_pred_melspectrogram != -1:
-                                self._error(self._model_audio_nn_not_formation, out=out)
-                                return False
+                                self._error(self._model_audio_nn_not_formation, out = out); return False
 
                             # Конкатенация оценок по экспертным и нейросетевым признакам
-                            union_pred = self.__concat_pred(pred_hc.numpy(), pred_melspectrogram.numpy(), out=out)
+                            union_pred = self.__concat_pred(pred_hc, pred_melspectrogram, out = out)
 
-                            if len(union_pred) == 0:
-                                return False
+                            if len(union_pred) == 0: return False
 
                             final_pred = []
 
                             for cnt, (name_b5, model) in enumerate(self.audio_models_b5_.items()):
-                                result = model(np.expand_dims(union_pred[cnt], axis=0)).numpy()[0][0]
+                                result = model(np.expand_dims(union_pred[cnt], axis = 0)).numpy()[0][0]
 
                                 final_pred.append(result)
 
                             # Добавление данных в словарь для DataFrame
                             if self._append_to_list_of_files(str(curr_path.resolve()), final_pred, out) is False:
                                 return False
 
                             # Вычисление точности
                             if accuracy is True:
                                 try:
-                                    true_trait = (
-                                        data_true_traits[data_true_traits.NAME_VIDEO == curr_path.name][
-                                            list(self._b5["en"])
-                                        ]
-                                        .values[0]
-                                        .tolist()
-                                    )
+                                    true_trait = data_true_traits[
+                                        data_true_traits.NAME_VIDEO == curr_path.name
+                                    ][list(self._b5['en'])].values[0].tolist()
                                 except IndexError:
-                                    self._other_error(self._expert_values_not_found, out=out)
-                                    return False
-                                except Exception:
-                                    self._other_error(self._unknown_err, out=out)
-                                    return False
-                                else:
-                                    true_traits.append(true_trait)
+                                    self._other_error(self._expert_values_not_found, out = out); return False
+                                except Exception: self._other_error(self._unknown_err, out = out); return False
+                                else: true_traits.append(true_trait)
                         else:
                             # Добавление данных в словарь для DataFrame
-                            if (
-                                self._append_to_list_of_files(
-                                    str(curr_path.resolve()), [None] * len(self._b5["en"]), out
-                                )
-                                is False
-                            ):
-                                return False
+                            if self._append_to_list_of_files(
+                                str(curr_path.resolve()), [None] * len(self._b5['en']), out
+                            ) is False: return False
 
                     # Индикатор выполнения
                     self._progressbar_union_predictions(
-                        get_audio_union_predictions_info,
-                        self.__len_paths,
-                        self.__local_path(paths[-1]),
-                        self.__len_paths,
-                        True,
-                        last,
-                        out,
+                        get_audio_union_predictions_info, self.__len_paths, self.__local_path(paths[-1]),
+                        self.__len_paths, True, last, out
                     )
 
                     # Отображение в DataFrame с данными
-                    self._df_files = pd.DataFrame.from_dict(data=self._dict_of_files, orient="index").transpose()
+                    self._df_files = pd.DataFrame.from_dict(data = self._dict_of_files, orient = 'index').transpose()
                     self._df_files.index.name = self._keys_id
                     self._df_files.index += 1
 
                     self._df_files.index = self._df_files.index.map(str)
 
-                    self._df_files.Path = [os.path.basename(i) for i in self._df_files.Path]
-
                     # Отображение
                     if out is True:
-                        self._add_notebook_history_output(self._df_files.iloc[0 : self.num_to_df_display_, :])
+                        self._add_notebook_history_output(self._df_files.iloc[0:self.num_to_df_display_, :])
 
                     # Подсчет точности
                     if accuracy is True:
                         mae_curr = []
 
                         for cnt, name_b5 in enumerate(self._df_files.keys().tolist()[1:]):
                             mae_curr.append(
-                                mean_absolute_error(np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list())
+                                mean_absolute_error(
+                                    np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list()
+                                )
                             )
 
                         mae_curr = [round(float(i), 4) for i in mae_curr]
                         mae_mean = round(float(np.mean(mae_curr)), 4)
                         accuracy_curr = [round(float(i), 4) for i in 1 - np.asarray(mae_curr)]
                         accuracy_mean = round(float(np.mean(accuracy_curr)), 4)
 
                         for curr_acc in [mae_curr, accuracy_curr]:
                             # Добавление данных в словарь для DataFrame с результатами вычисления точности
-                            if self._append_to_list_of_accuracy(curr_acc, out) is False:
-                                return False
+                            if self._append_to_list_of_accuracy(curr_acc, out) is False: return False
 
-                        self._dict_of_accuracy.update({self.__df_accuracy_mean: [mae_mean, accuracy_mean]})
+                        self._dict_of_accuracy.update({
+                            self.__df_accuracy_mean: [mae_mean, accuracy_mean]
+                        })
                         # Отображение в DataFrame с данными
-                        self._df_accuracy = pd.DataFrame.from_dict(
-                            data=self._dict_of_accuracy, orient="index"
-                        ).transpose()
+                        self._df_accuracy = pd.DataFrame.from_dict(data = self._dict_of_accuracy,
+                                                                   orient = 'index').transpose()
                         self._df_accuracy.index = self.__df_accuracy_index
                         self._df_accuracy.index.name = self.__df_accuracy_index_name
 
                         # Информационное сообщение
-                        self._info(self._get_union_predictions_result, out=False)
+                        self._info(self._get_union_predictions_result, out = False)
 
                         # Отображение
                         if out is True:
-                            self._add_notebook_history_output(self._df_accuracy.iloc[0 : self.num_to_df_display_, :])
+                            self._add_notebook_history_output(self._df_accuracy.iloc[0:self.num_to_df_display_, :])
 
                         self._info(
                             self._get_union_predictions_results_mean.format(
-                                self._info_wrapper(str(mae_mean)), self._info_wrapper(str(accuracy_mean))
+                                self._info_wrapper(str(mae_mean)),
+                                self._info_wrapper(str(accuracy_mean))
                             ),
-                            out=False,
+                            out = False
                         )
 
                     clear_output(True)
                     # Отображение истории вывода сообщений в ячейке Jupyter
-                    if out is True:
-                        self.show_notebook_history_output()
+                    if out is True: self.show_notebook_history_output()
 
                     if logs is True:
                         # Текущее время для лог-файла
                         # см. datetime.fromtimestamp()
-                        curr_ts = str(datetime.now().timestamp()).replace(".", "_")
+                        curr_ts = str(datetime.now().timestamp()).replace('.', '_')
 
                         name_logs_file = self.get_audio_union_predictions.__name__
 
                         # Сохранение LOG
                         res_save_logs_df_files = self._save_logs(
-                            self._df_files, name_logs_file + "_df_files_" + curr_ts
+                            self._df_files, name_logs_file + '_df_files_' + curr_ts
                         )
 
                         # Подсчет точности
                         if accuracy is True:
                             # Сохранение LOG
                             res_save_logs_df_accuracy = self._save_logs(
-                                self._df_accuracy, name_logs_file + "_df_accuracy_" + curr_ts
+                                self._df_accuracy, name_logs_file + '_df_accuracy_' + curr_ts
                             )
 
                         if res_save_logs_df_files is True:
                             # Сохранение LOG файла/файлов
-                            if accuracy is True and res_save_logs_df_accuracy is True:
-                                logs_s = self._logs_saves_true
-                            else:
-                                logs_s = self._logs_save_true
+                            if accuracy is True and res_save_logs_df_accuracy is True: logs_s = self._logs_saves_true
+                            else: logs_s = self._logs_save_true
 
-                            self._info_true(logs_s, out=out)
+                            self._info_true(logs_s, out = out)
 
                     return True
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/lab/build.py` & `oceanai-1.0.0a5/oceanai/modules/lab/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,53 +4,48 @@
 """
 Сборка
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
 # Персональные
-from oceanai.modules.lab.prediction import Prediction  # Объединение аудио и видео
-
+from oceanai.modules.lab.prediction import Prediction # Объединение аудио и видео
 
 # ######################################################################################################################
 # Сборка
 # ######################################################################################################################
 @dataclass
 class Run(Prediction):
     """Класс для сборки
 
-    Args:
-        lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
-        color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
-        color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
-        color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
-        color_true (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_true`
-        bold_text (bool): Смотреть :attr:`~oceanai.modules.core.settings.Settings.bold_text`
-        num_to_df_display (int): Смотреть :attr:`~oceanai.modules.core.settings.Settings.num_to_df_display`
-        text_runtime (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.text_runtime`
-        metadata (bool): Отображение информации о библиотеке
-    """
+        Args:
+            lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
+            color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
+            color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
+            color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
+            color_true (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_true`
+            bold_text (bool): Смотреть :attr:`~oceanai.modules.core.settings.Settings.bold_text`
+            num_to_df_display (int): Смотреть :attr:`~oceanai.modules.core.settings.Settings.num_to_df_display`
+            text_runtime (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.text_runtime`
+            metadata (bool): Отображение информации о библиотеке
+        """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
-    metadata: bool = True  # Информация об библиотеке
+    metadata: bool = True # Информация об библиотеке
     """
     bool: Отображение информации о библиотеке
     """
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        if self.is_notebook_ is True and type(self.metadata) is bool and self.metadata is True:
-            self._metadata_info()
+        if self.is_notebook_ is True and type(self.metadata) is bool and self.metadata is True: self._metadata_info()
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/lab/download.py` & `oceanai-1.0.0a5/oceanai/modules/lab/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,43 +4,39 @@
 """
 Загрузка файлов
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
-import numpy as np  # Научные вычисления
-import requests  # Отправка HTTP запросов
-import re  # Регулярные выражения
-import shutil  # Набор функций высокого уровня для обработки файлов, групп файлов, и папок
+import os          # Взаимодействие с файловой системой
+import numpy as np # Научные вычисления
+import requests    # Отправка HTTP запросов
+import re          # Регулярные выражения
+import shutil      # Набор функций высокого уровня для обработки файлов, групп файлов, и папок
 
-from pathlib import Path  # Работа с путями в файловой системе
+from pathlib import Path # Работа с путями в файловой системе
 
 from IPython.display import clear_output
 
 # Персональные
-from oceanai.modules.lab.unzip import Unzip  # Обработка архивов
+from oceanai.modules.core.core import Core # Ядро
 from oceanai.modules.core.exceptions import InvalidContentLength
 
-
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
-class DownloadMessages(Unzip):
+class DownloadMessages(Core):
     """Класс для сообщений
 
     Args:
         lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
         color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
         color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
         color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
@@ -51,24 +47,23 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._could_not_process_url = self._oh + self._("не удалось обработать указанный URL ...")
-        self._url_incorrect = self._oh + self._("URL указан некорректно ...")
-        self._url_incorrect_content_length = self._oh + self._("Не определен размер файла для загрузки ...")
+        self._could_not_process_url = self._oh + self._('не удалось обработать указанный URL ...')
+        self._url_incorrect = self._oh + self._('URL указан некорректно ...')
+        self._url_incorrect_content_length = self._oh + self._('Не определен размер файла для загрузки ...')
         self._automatic_download: str = self._('Загрузка файла "{}"')
-        self._url_error_code_http: str = self._(" (ошибка {})")
+        self._url_error_code_http: str = self._(' (ошибка {})')
         self._url_error_http: str = self._oh + self._('не удалось скачать файл "{}"{} ...')
 
-
 # ######################################################################################################################
 # Загрузка файлов
 # ######################################################################################################################
 class Download(DownloadMessages):
     """Класс для загрузки файлов
 
     Args:
@@ -85,20 +80,18 @@
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
         super().__post_init__()  # Выполнение конструктора из суперкласса
 
-        self._headers: str = (
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) "
-            "Chrome/89.0.4389.90 Safari/537.36"
-        )  # User-Agent
+        self._headers: str = ('Mozilla/5.0 (Macintosh; Intel Mac OS X 11_2_3) AppleWebKit/537.36 (KHTML, like Gecko) '
+                              'Chrome/89.0.4389.90 Safari/537.36') # User-Agent
 
-        self._url_last_filename: str = ""  # Имя последнего загруженного файла
+        self._url_last_filename: str = '' # Имя последнего загруженного файла
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (приватные)
     # ------------------------------------------------------------------------------------------------------------------
 
     def __progressbar_download_file_from_url(
         self, url_filename: str, progress: float, clear_out: bool = True, last: bool = False, out: bool = True
@@ -204,50 +197,40 @@
             .. output-cell::
                 :execution-count: 3
                 :linenos:
 
                 [2022-10-16 17:00:11] Неверные типы или значения аргументов в "Download.__progressbar_download_file_from_url" ...
         """
 
-        if clear_out is False and last is True:
-            clear_out, last = last, clear_out
-        elif clear_out is False and last is False:
-            clear_out = True
+        if clear_out is False and last is True: clear_out, last = last, clear_out
+        elif clear_out is False and last is False: clear_out = True
 
-        if clear_out is True:
-            clear_output(True)
+        if clear_out is True: clear_output(True)
 
         try:
             # Проверка аргументов
-            if (
-                type(url_filename) is not str
-                or not url_filename
-                or type(progress) is not float
-                or not (0 <= progress <= 100)
-            ):
+            if (type(url_filename) is not str or not url_filename or type(progress) is not float
+                    or not (0 <= progress <= 100)):
                 raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__progressbar_download_file_from_url.__name__, out=out)
+            self._inv_args(__class__.__name__, self.__progressbar_download_file_from_url.__name__, out = out)
             return None
 
         self._info(
-            self._automatic_download.format(self._info_wrapper(url_filename)) + self._download_precent.format(progress),
-            last=last,
-            out=False,
+            self._automatic_download.format(self._info_wrapper(url_filename))
+            + self._download_precent.format(progress), last = last, out = False
         )
-        if out:
-            self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+        if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (защищенные)
     # ------------------------------------------------------------------------------------------------------------------
 
-    def _download_file_from_url(
-        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> int:
+    def _download_file_from_url(self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True,
+                                run: bool = True) -> int:
         """Загрузка файла из URL (без очистки истории вывода сообщений в ячейке Jupyter)
 
         .. note::
             protected (защищенный метод)
 
         Args:
             url (str): Полный путь к файлу
@@ -438,188 +421,138 @@
                 --- Время выполнения: 0.386 сек. ---
 
                 404
         """
 
         try:
             # Проверка аргументов
-            if (
-                type(url) is not str
-                or not url
-                or type(force_reload) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(url) is not str or not url or type(force_reload) is not bool or type(out) is not bool
+                or type(runtime) is not bool or type(run) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self._download_file_from_url.__name__, out=out)
-            return 400
+            self._inv_args(__class__.__name__, self._download_file_from_url.__name__, out = out); return 400
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return 403
+            if run is False: self._error(self._lock_user, out = out); return 403
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             try:
                 # Отправка GET запроса для получения файла
-                r = requests.get(url, headers={"user-agent": self._headers}, stream=True)
+                r = requests.get(url, headers = {'user-agent': self._headers}, stream = True)
             except (
                 # https://requests.readthedocs.io/en/master/_modules/requests/exceptions/
-                requests.exceptions.MissingSchema,
-                requests.exceptions.InvalidSchema,
-                requests.exceptions.ConnectionError,
-                requests.exceptions.InvalidURL,
-            ):
-                self._other_error(self._could_not_process_url, out=out)
-                return 404
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return 404
+                requests.exceptions.MissingSchema, requests.exceptions.InvalidSchema,
+                requests.exceptions.ConnectionError, requests.exceptions.InvalidURL
+            ): self._other_error(self._could_not_process_url, out = out); return 404
+            except Exception: self._other_error(self._unknown_err, out = out); return 404
             else:
                 # Имя файла
-                if "Content-Disposition" in r.headers.keys():
+                if 'Content-Disposition' in r.headers.keys():
                     try:
-                        url_filename = re.findall('(?<=[\(\{\["]).+(?=[\)\}\]"])', r.headers["Content-Disposition"])[0]
+                        url_filename = re.findall('(?<=[\(\{\["]).+(?=[\)\}\]"])', r.headers['Content-Disposition'])[0]
                     except IndexError:
                         url_filename = re.findall(
                             r'filename\*?=[\'"]?(?:UTF-\d[\'"]*)?([^;\r\n"\']*)[\'"]?;?',
-                            r.headers["Content-Disposition"],
+                            r.headers['Content-Disposition']
                         )[0]
-                else:
-                    url_filename = url.split("/")[-1]
+                else: url_filename = url.split('/')[-1]
 
                 try:
                     # URL файл невалидный
                     if not url_filename or not Path(url_filename).suffix:
-                        if not Path(url_filename).stem.lower():
-                            raise requests.exceptions.InvalidURL
+                        if not Path(url_filename).stem.lower(): raise requests.exceptions.InvalidURL
 
-                        if r.headers["Content-Type"] == "image/jpeg":
-                            ext = "jpg"
-                        elif r.headers["Content-Type"] == "image/png":
-                            ext = "png"
-                        elif r.headers["Content-Type"] == "text/plain":
-                            ext = "txt"
-                        elif r.headers["Content-Type"] == "text/csv":
-                            ext = "csv"
-                        elif r.headers["Content-Type"] == "video/mp4":
-                            ext = "mp4"
-                        else:
-                            raise requests.exceptions.InvalidHeader
+                        if r.headers['Content-Type'] == 'image/jpeg': ext = 'jpg'
+                        elif r.headers['Content-Type'] == 'image/png': ext = 'png'
+                        elif r.headers['Content-Type'] == 'text/plain': ext = 'txt'
+                        elif r.headers['Content-Type'] == 'text/csv': ext = 'csv'
+                        elif r.headers['Content-Type'] == 'video/mp4': ext = 'mp4'
+                        else: raise requests.exceptions.InvalidHeader
 
-                        url_filename = Path(url_filename).stem + "." + ext
+                        url_filename = Path(url_filename).stem + '.' + ext
                 except (requests.exceptions.InvalidURL, requests.exceptions.InvalidHeader):
-                    self._other_error(self._url_incorrect, out=out)
-                    return 404
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return 404
+                    self._other_error(self._url_incorrect, out = out); return 404
+                except Exception: self._other_error(self._unknown_err, out = out); return 404
                 else:
                     # Информационное сообщение
-                    self._info(self._automatic_download.format(self._info_wrapper(url_filename)), out=False)
-                    if out:
-                        self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+                    self._info(self._automatic_download.format(self._info_wrapper(url_filename)), out = False)
+                    if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
                     # Директория для сохранения файла
-                    if not os.path.exists(self.path_to_save_):
-                        os.makedirs(self.path_to_save_)
+                    if not os.path.exists(self.path_to_save_): os.makedirs(self.path_to_save_)
 
-                    local_file = os.path.join(self.path_to_save_, url_filename)  # Путь к файлу
+                    local_file = os.path.join(self.path_to_save_, url_filename) # Путь к файлу
 
                     try:
                         # Принудительная загрузка файла из сети
                         if force_reload is True:
                             # Файл найден
                             if os.path.isfile(local_file) is True:
                                 # Удаление файла
-                                try:
-                                    shutil.rmtree(local_file)
-                                except OSError:
-                                    os.remove(local_file)
-                                except Exception:
-                                    raise Exception
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return 404
+                                try: shutil.rmtree(local_file)
+                                except OSError: os.remove(local_file)
+                                except Exception: raise Exception
+                    except Exception: self._other_error(self._unknown_err, out = out); return 404
                     else:
                         # Файл с указанным именем найден локально и принудительная загрузка файла из сети не указана
                         if Path(local_file).is_file() is True and force_reload is False:
-                            self._url_last_filename = local_file
-                            return 200
+                            self._url_last_filename = local_file; return 200
                         else:
                             # Ответ получен
                             if r.status_code == 200:
-                                total_length = int(r.headers.get("content-length", 0))  # Длина файла
+                                total_length = int(r.headers.get('content-length', 0)) # Длина файла
 
                                 try:
-                                    if total_length == 0:
-                                        raise InvalidContentLength
+                                    if total_length == 0: raise InvalidContentLength
                                 except InvalidContentLength:
-                                    self._other_error(self._url_incorrect_content_length, out=out)
-                                    return 404
+                                    self._other_error(self._url_incorrect_content_length, out = out); return 404
                                 else:
-                                    num_bars = int(np.ceil(total_length / self.chunk_size_))  # Количество загрузок
+                                    num_bars = int(np.ceil(total_length / self.chunk_size_)) # Количество загрузок
 
                                     try:
                                         # Открытие файла для записи
-                                        with open(local_file, "wb") as f:
+                                        with open(local_file, 'wb') as f:
                                             # Индикатор выполнения
                                             self.__progressbar_download_file_from_url(
-                                                url_filename, 0.0, clear_out=True, last=True, out=out
+                                                url_filename, 0.0, clear_out = True, last = True, out = out
                                             )
 
                                             # Сохранение файла по частям
-                                            for i, chunk in enumerate(r.iter_content(chunk_size=self.chunk_size_)):
-                                                f.write(chunk)  # Запись в файл
+                                            for i, chunk in enumerate(r.iter_content(chunk_size = self.chunk_size_)):
+                                                f.write(chunk) # Запись в файл
                                                 f.flush()
 
                                                 # Индикатор выполнения
                                                 self.__progressbar_download_file_from_url(
-                                                    url_filename,
-                                                    round(i * 100 / num_bars, 2),
-                                                    clear_out=True,
-                                                    last=True,
-                                                    out=out,
+                                                    url_filename, round(i * 100 / num_bars, 2),
+                                                    clear_out = True, last = True, out = out
                                                 )
 
                                             # Индикатор выполнения
                                             self.__progressbar_download_file_from_url(
-                                                url_filename, 100.0, clear_out=True, last=True, out=out
+                                                url_filename, 100., clear_out = True, last = True, out = out
                                             )
-                                    except Exception:
-                                        self._other_error(self._unknown_err, out=out)
-                                        return 404
-                                    else:
-                                        self._url_last_filename = local_file
-                                        return 200
+                                    except Exception: self._other_error(self._unknown_err, out = out); return 404
+                                    else: self._url_last_filename = local_file; return 200
                             else:
-                                self._error(
-                                    self._url_error_http.format(
-                                        self._info_wrapper(url_filename),
-                                        self._url_error_code_http.format(self._error_wrapper(str(r.status_code))),
-                                    ),
-                                    out=out,
-                                )
+                                self._error(self._url_error_http.format(
+                                    self._info_wrapper(url_filename),
+                                    self._url_error_code_http.format(self._error_wrapper(str(r.status_code)))
+                                ), out = out)
 
                                 return 404
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внешние методы
     # ------------------------------------------------------------------------------------------------------------------
 
-    def download_file_from_url(
-        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> int:
+    def download_file_from_url(self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True,
+                               run: bool = True) -> int:
         """Загрузка файла из URL
 
         Args:
             url (str): Полный путь к файлу
             force_reload (bool): Принудительная загрузка файла из сети
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
@@ -632,10 +565,11 @@
                 * ``400`` - Ошибка при проверке аргументов
                 * ``403`` - Выполнение заблокировано пользователем
                 * ``404`` - Не удалось скачать файл
 
         :bdg-link-light:`Пример <../../user_guide/notebooks/Download-download_file_from_url.ipynb>`
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
-        return self._download_file_from_url(url=url, force_reload=force_reload, out=out, runtime=runtime, run=run)
+        return self._download_file_from_url(url = url, force_reload = force_reload, out = out, runtime = runtime,
+                                            run = run)
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/lab/prediction.py` & `oceanai-1.0.0a5/oceanai/modules/lab/video.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
-Мультимодальное объединение информации
+Видео
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
+import os           # Взаимодействие с файловой системой
 import logging
-import requests  # Отправка HTTP запросов
+import requests     # Отправка HTTP запросов
 import numpy as np  # Научные вычисления
-import pandas as pd  # Обработка и анализ данных
+import pandas as pd # Обработка и анализ данных
+import math
 
 from urllib.parse import urlparse
 from urllib.error import URLError
-from pathlib import Path  # Работа с путями в файловой системе
+from pathlib import Path # Работа с путями в файловой системе
+from scipy.spatial import distance
+from scipy import stats
+from pymediainfo import MediaInfo # Получение meta данных из медиафайлов
+from datetime import datetime # Работа со временем
 from sklearn.metrics import mean_absolute_error
-from datetime import datetime  # Работа со временем
 
 # Типы данных
-from typing import List, Dict, Union, Optional, Callable
+from typing import Dict, List, Tuple, Union, Optional, Callable
+from types import ModuleType
 
 from IPython.display import clear_output
 
 # Персональные
-from oceanai.modules.lab.audio import Audio  # Аудио
-from oceanai.modules.lab.video import Video  # Видео
-from oceanai.modules.lab.text import Text  # Текст
+from oceanai.modules.lab.download import Download # Загрузка файлов
 
 # Порог регистрации сообщений TensorFlow
 logging.disable(logging.WARNING)
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
-import tensorflow as tf  # Машинное обучение от Google
+import tensorflow as tf # Машинное обучение от Google
 import keras
+import cv2
+import mediapipe as mp # Набор нейросетевых моделей и решений для компьютерного зрения
 
-from oceanai.modules.lab.utils.gfl import GFL  # Модуль внимания
-from oceanai.modules.lab.utils.addition import Concat
+# Исправленная версия Keras_VGGFace
+from oceanai.modules.lab.keras_vggface import utils
+from oceanai.modules.lab.keras_vggface.vggface import VGGFace
 
+mp.solutions.face_mesh.FaceMesh() # Удаление сообщения: INFO: Created TensorFlow Lite XNNPACK delegate for CPU)
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
-class PredictionMessages(Audio, Video, Text):
+class  VideoMessages(Download):
     """Класс для сообщений
 
     Args:
         lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
         color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
         color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
         color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
@@ -69,49 +73,55 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._av_modality: str = self._(" (мультимодальное объединение) ...")
+        self._video_modality: str = self._(' (видео модальность) ...')
+        self._formation_video_model_hc: str = self._formation_model_hc + self._video_modality
+        self._formation_video_model_nn: str = self._formation_model_nn + self._video_modality
+        self._formation_video_deep_fe: str = self._('Формирование нейросетевой архитектуры для получения нейросетевых '
+                                                    'признаков') + self._video_modality
+        self._formation_video_models_b5: str = self._formation_models_b5 + self._video_modality
+
+        self._load_video_model_weights_hc: str = self._load_model_weights_hc + self._video_modality
+        self._load_video_model_weights_nn: str = self._load_model_weights_nn + self._video_modality
+        self._load_video_model_weights_deep_fe: str = self._('Загрузка весов нейросетевой модели для получения '
+                                                             'нейросетевых признаков') + self._video_modality
+        self._load_video_models_weights_b5: str = self._load_models_weights_b5 + self._video_modality
+
+        self._model_video_hc_not_formation: str = self._model_hc_not_formation + self._video_modality
+        self._model_video_nn_not_formation: str = self._model_nn_not_formation + self._video_modality
+        self._model_video_deep_fe_not_formation: str = self._oh + self._('нейросетевая архитектура модели для '
+                                                                         'получения нейросетевых признаков не '
+                                                                         'сформирована') + self._video_modality
+        self._models_video_not_formation: str = self._models_not_formation + self._video_modality
+
+        self._get_visual_feature_info: str = self._('Извлечение признаков (экспертных и нейросетевых) из визуального '
+                                                    'сигнала ...')
+
+        self._wrong_extension_video_formats = self._oh + self._('расширение видеофайла должно быть одним из: "{}"')
+        self._all_frames_is_zero: str = self._oh + self._('общее количество кадров в видеопотоке: {} ...')
+        self._calc_reshape_img_coef_error: str = self._oh + self._('вычисление коэффициента изменения размера '
+                                                                   'изображения не произведено ...')
 
-        self._formation_av_models_b5: str = self._formation_models_b5 + self._av_modality
-
-        self._formation_avt_model_b5: str = (
-            self._("Формирование нейросетевой архитектуры модели для получения " " оценок персональных качеств")
-            + self._av_modality
-        )
-        self._load_avt_model_weights_b5: str = (
-            self._("Загрузка весов нейросетевой модели для получения " "оценок персональных качеств")
-            + self._av_modality
-        )
-
-        self._model_avt_not_formation: str = (
-            self._oh
-            + self._(
-                "нейросетевая архитектура модели для получения " "оценок по мультимодальным данным не " "сформирована"
-            )
-            + self._av_modality
-        )
-
-        self._load_av_models_weights_b5: str = self._load_models_weights_b5 + self._av_modality
-
-        self._concat_av_pred_error: str = self._concat_pred_error + self._av_modality
-        self._norm_av_pred_error: str = self._norm_pred_error + self._av_modality
+        self._faces_not_found: str = self._oh + self._('не на одном кадре видеопотока лицо не найдено ...')
 
+        self._concat_video_pred_error: str = self._concat_pred_error + self._video_modality
+        self._norm_video_pred_error: str = self._norm_pred_error + self._video_modality
 
 # ######################################################################################################################
-# Мультимодальное объединение
+# Аудио
 # ######################################################################################################################
 @dataclass
-class Prediction(PredictionMessages):
-    """Класс для мультимодального объединения информации
+class Video(VideoMessages):
+    """Класс для обработки видео
 
     Args:
         lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
         color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
         color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
         color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
         color_true (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_true`
@@ -121,41 +131,246 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
+        # Нейросетевая модель **tf.keras.Model** для получения оценок по экспертным признакам
+        self._video_model_hc: Optional[keras.engine.functional.Functional] = None
+        # Нейросетевая модель **tf.keras.Model** для получения нейросетевых признаков
+        self._video_model_deep_fe: Optional[keras.engine.functional.Functional] = None
+        # Нейросетевая модель **tf.keras.Model** для получения оценок по нейросетевым признакам
+        self._video_model_nn: Optional[keras.engine.functional.Functional] = None
         # Нейросетевые модели **tf.keras.Model** для получения результатов оценки персональных качеств
-        self._av_models_b5: Dict[str, Optional[tf.keras.Model]] = dict(
-            zip(self._b5["en"], [None] * len(self._b5["en"]))
-        )
-
-        self._avt_model_b5: Optional[tf.keras.Model] = None
+        self._video_models_b5: Dict[str, Optional[keras.engine.functional.Functional]] = dict(zip(
+            self._b5['en'], [None] * len(self._b5['en'])
+        ))
 
         # ----------------------- Только для внутреннего использования внутри класса
 
-        self.__len_paths: int = 0  # Количество искомых файлов
-        self.__local_path: Union[Callable[[str], str], None] = None  # Локальный путь
+        # Поддерживаемые видео форматы
+        self.__supported_video_formats: List[str] = ['mp4']
+
+        self.__mp_face_mesh: ModuleType = mp.solutions.face_mesh # 468 3D-ориентиров лица
+        self.__mp_drawing: ModuleType = mp.solutions.drawing_utils # Утилиты MediaPipe
+
+        self.__bndbox_face_size: List[int] = [224, 224] # Размер изображения с лицом
+
+        # Используемые координаты ориентиров лица
+        self.__coords_face_mesh: List[int] = [
+            0, 1, 386, 133, 6, 8, 267, 13, 14, 17, 145, 276, 152, 282, 411, 285, 159, 291, 37,
+            299, 46, 52, 55, 187, 61, 69, 331, 334, 336, 102, 105, 362, 107, 374, 33, 263
+        ]
+
+        self.__couples_face_mesh: List[List[int]] = [
+            [133, 46], [133, 52], [133, 55], [362, 285], [362, 282], [362, 276], [55, 285], [1, 6], [8, 6], [0, 1],
+            [0, 17], [61, 291], [0, 13], [61, 291], [37, 13], [267, 13], [13, 14], [17, 152], [102, 331], [102, 133],
+            [331, 362], [291, 362], [61, 133], [386, 374], [159, 145], [69, 105], [69, 107], [299, 336], [299, 334],
+            [187, 133], [411, 362]
+        ]
+
+        self.__len_paths: int = 0 # Количество искомых файлов
+        self.__local_path: Union[Callable[[str], str], None] = None # Локальный путь
 
         # Ключи для точности
-        self.__df_accuracy_index: List[str] = ["MAE", "Accuracy"]
-        self.__df_accuracy_index_name: str = "Metrics"
-        self.__df_accuracy_mean: str = "Mean"
+        self.__df_accuracy_index: List[str] = ['MAE', 'Accuracy']
+        self.__df_accuracy_index_name: str = 'Metrics'
+        self.__df_accuracy_mean: str = 'Mean'
 
-        clear_output(False)  # Удаление сообщения: INFO: Created TensorFlow Lite XNNPACK delegate for CPU)
+        clear_output(False) # Удаление сообщения: INFO: Created TensorFlow Lite XNNPACK delegate for CPU)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     @property
-    def av_models_b5_(self) -> Dict[str, Optional[tf.keras.Model]]:
+    def video_model_hc_(self) -> Optional[keras.engine.functional.Functional]:
+        """Получение нейросетевой модели **tf.keras.Model** для получения оценок по экспертным признакам
+
+        Returns:
+            Optional[keras.engine.functional.Functional]: Нейросетевая модель **tf.keras.Model** или None
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.load_video_model_hc(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
+
+                video.video_model_hc_
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-10-26 12:37:42] Формирование нейросетевой архитектуры модели для получения оценок по экспертным признакам (видео модальность) ...
+
+                --- Время выполнения: 1.112 сек. ---
+
+                <keras.engine.functional.Functional at 0x1434eb1f0>
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.video_model_hc_
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+
+        """
+
+        return self._video_model_hc
+
+    @property
+    def video_model_nn_(self) -> Optional[keras.engine.functional.Functional]:
+        """Получение нейросетевой модели **tf.keras.Model** для получения оценок по нейросетевым признакам
+
+        Returns:
+            Optional[keras.engine.functional.Functional]: Нейросетевая модель **tf.keras.Model** или None
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.load_video_model_nn(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
+
+                video.video_model_nn_
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-10-27 14:49:00] Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам (видео модальность) ...
+
+                --- Время выполнения: 1.986 сек. ---
+
+                <keras.engine.functional.Functional at 0x13d5295b0>
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.video_model_nn_
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+
+        """
+
+        return self._video_model_nn
+
+    @property
+    def video_model_deep_fe_(self) -> Optional[keras.engine.functional.Functional]:
+        """Получение нейросетевой модели **tf.keras.Model** для получения нейросетевых признаков
+
+        Returns:
+            Optional[keras.engine.functional.Functional]: Нейросетевая модель **tf.keras.Model** или None
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.load_video_model_deep_fe(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
+
+                video.video_model_deep_fe_
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-11-01 12:12:35] Формирование нейросетевой архитектуры для получения нейросетевых признаков (видео модальность) ...
+
+                --- Время выполнения: 1.468 сек. ---
+
+                <keras.engine.functional.Functional at 0x14e138100>
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.video_model_deep_fe_
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+
+        """
+
+        return self._video_model_deep_fe
+
+    @property
+    def video_models_b5_(self) -> Dict[str, Optional[keras.engine.functional.Functional]]:
         """Получение нейросетевых моделей **tf.keras.Model** для получения результатов оценки персональных качеств
 
         Returns:
             Dict: Словарь с нейросетевыми моделями **tf.keras.Model**
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
@@ -163,119 +378,389 @@
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 1
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
-                pred.load_av_models_b5(
+                video.load_video_models_b5(
                     show_summary = False, out = True,
                     runtime = True, run = True
                 )
 
-                pred.av_models_b5_
+                video.video_models_b5_
 
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
-                [2022-12-08 15:21:22] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
+                [2022-10-19 15:45:35] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств ...
 
-                --- Время выполнения: 0.305 сек. ---
+                --- Время выполнения: 0.07 сек. ---
 
                 {
-                    'openness': <tf.keras.Model at 0x14eee5790>,
-                    'conscientiousness': <tf.keras.Model at 0x14f2d9d00>,
-                    'extraversion': <tf.keras.Model at 0x14f2fb190>,
-                    'agreeableness': <tf.keras.Model at 0x14f2c7fd0>,
-                    'non_neuroticism': <tf.keras.Model at 0x14f2ef940>
+                    'openness': <keras.engine.functional.Functional at 0x1481e03a0>,
+                    'conscientiousness': <keras.engine.functional.Functional at 0x147d13520>,
+                    'extraversion': <keras.engine.functional.Functional at 0x1481edfa0>,
+                    'agreeableness': <keras.engine.functional.Functional at 0x1481cfc40>,
+                    'neuroticism': <keras.engine.functional.Functional at 0x1481cffd0>
                 }
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
-                pred.av_models_b5_
+                video.video_models_b5_
 
             .. output-cell::
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
 
                 {
                     'openness': None,
                     'conscientiousness': None,
                     'extraversion': None,
                     'agreeableness': None,
-                    'non_neuroticism': None
+                    'neuroticism': None
                 }
         """
 
-        return self._av_models_b5
+        return self._video_models_b5
 
-    @property
-    def avt_model_b5_(self) -> Optional[tf.keras.Model]:
-        """Получение нейросетевой модели **tf.keras.Model** для получения оценок персональных качеств
+    # ------------------------------------------------------------------------------------------------------------------
+    # Внутренние методы (приватные)
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def __load_model_weights(
+        self, url: str, force_reload: bool = True, info_text: str = '',
+        out: bool = True, runtime: bool = True, run: bool = True
+    ) -> bool:
+        """Загрузка весов нейросетевой модели
+
+        .. note::
+            private (приватный метод)
+
+        Args:
+            url (str): Полный путь к файлу с весами нейросетевой модели
+            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
+            info_text (str): Текст для информационного сообщения
+            out (bool): Отображение
+            runtime (bool): Подсчет времени выполнения
+            run (bool): Блокировка выполнения
 
         Returns:
-            Dict: Нейроаетевая модель **tf.keras.Model**
+            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
+
+                video._Video__load_model_weights(
+                    url = 'https://download.sberdisk.ru/download/file/412059444?token=JXerCfAjJZg6crD&filename=weights_2022-08-27_18-53-35.h5',
+                    force_reload = True,
+                    info_text = 'Загрузка весов нейросетевой модели',
+                    out = True, runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-10-27 12:46:55] Загрузка весов нейросетевой модели
+
+                [2022-10-27 12:46:55] Загрузка файла "weights_2022-08-27_18-53-35.h5" (100.0%) ...
+
+                --- Время выполнения: 0.626 сек. ---
+
+                True
+
+            :bdg-light:`-- 2 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
+
+                video._Video__load_model_weights(
+                    url = './models/weights_2022-08-27_18-53-35.h5',
+                    force_reload = True,
+                    info_text = 'Загрузка весов нейросетевой модели',
+                    out = True, runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+                [2022-10-27 12:47:52] Загрузка весов нейросетевой модели
+
+                --- Время выполнения: 0.002 сек. ---
+
+                True
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
+
+                video._Video__load_model_weights(
+                    url = 'https://download.sberdisk.ru/download/file/412059444?token=JXerCfAjJZg6crD&filename=weights_2022-08-27_18-53-35.h5',
+                    force_reload = True, info_text = '',
+                    out = True, runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-10-27 12:48:24] Неверные типы или значения аргументов в "Video.__load_model_weights" ...
+
+                False
         """
 
-        return self._avt_model_b5
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
-    # ------------------------------------------------------------------------------------------------------------------
-    # Внутренние методы (приватные)
-    # ------------------------------------------------------------------------------------------------------------------
+        try:
+            # Проверка аргументов
+            if (type(url) is not str or not url or type(force_reload) is not bool
+                or type(info_text) is not str or not info_text or type(out) is not bool
+                or type(runtime) is not bool or type(run) is not bool): raise TypeError
+        except TypeError:
+            self._inv_args(__class__.__name__, self.__load_model_weights.__name__, out = out); return False
+        else:
+            # Блокировка выполнения
+            if run is False: self._error(self._lock_user, out = out); return False
+
+            if runtime: self._r_start()
+
+            # Информационное сообщение
+            self._info(info_text, last = False, out = out)
+
+            sections = urlparse(url) # Парсинг URL адреса
+
+            try:
+                # URL файл невалидный
+                if sections.scheme == '': raise requests.exceptions.InvalidURL
+            except requests.exceptions.InvalidURL:
+                url = os.path.normpath(url)
+
+                try:
+                    if os.path.isfile(url) is False: raise FileNotFoundError # Не файл
+                except FileNotFoundError: self._other_error(self._load_model_weights_error, out = out); return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
+                else: self._url_last_filename = url; return True
+            else:
+                try:
+                    if force_reload is False: clear_output(True)
+                    # Загрузка файла из URL
+                    res_download_file_from_url = self._download_file_from_url(
+                        url = url, force_reload = force_reload, runtime = False, out = out, run = True
+                    )
+                except Exception: self._other_error(self._unknown_err, out = out); return False
+                else:
+                    # Файл загружен
+                    if res_download_file_from_url != 200: return False
+
+                    return True
+            finally:
+                if runtime: self._r_end(out = out)
+
+    def __calc_reshape_img_coef(
+        self, shape: Union[Tuple[int], List[int]], new_shape: Union[int, Tuple[int], List[int]], out: bool = True
+    ) -> float:
+        """Вычисление коэффициента изменения размера изображения
+
+        .. note::
+            private (приватный метод)
+
+        Args:
+            shape (Union[Tuple[int], List[int]]): Текущий размер изображения (ширина, высота)
+            new_shape (Union[int, Tuple[int], List[int]]): Желаемый размер изображения
+            out (bool): Отображение
+
+        Returns:
+            float: Коэффициент изменения размера изображения
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video._Video__calc_reshape_img_coef(
+                    shape = (1280, 720),
+                    new_shape = 224,
+                    out = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                0.175
+
+            :bdg-success:`Верно` :bdg-light:`-- 2 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video._Video__calc_reshape_img_coef(
+                    shape = (1280, 720),
+                    new_shape = (1920, 1080),
+                    out = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                1.5
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video._Video__calc_reshape_img_coef(
+                    shape = (1280, 720),
+                    new_shape = '',
+                    out = True
+                )
+
+            .. output-cell::
+                :execution-count: 4
+                :linenos:
+
+                [2022-10-29 13:24:27] Неверные типы или значения аргументов в "Video.__calc_reshape_img_coef" ...
+
+                -1.0
+        """
+
+        try:
+            # Проверка аргументов
+            if (
+                (isinstance(shape, list) is False and isinstance(shape, tuple) is False) or len(shape) != 2
+                or (isinstance(new_shape, list) is False and isinstance(new_shape, tuple) is False
+                    and type(new_shape) is not int) or type(out) is not bool
+            ): raise TypeError
+
+            if type(shape[0]) is not int or type(shape[1]) is not int: raise TypeError
+
+            if shape[0] < 1 or shape[1] < 1: raise ValueError
+
+            if isinstance(new_shape, list) is True or isinstance(new_shape, tuple) is True:
+                if len(new_shape) != 2: raise TypeError
+
+                if type(new_shape[0]) is not int or type(new_shape[1]) is not int: raise TypeError
+
+                if new_shape[0] < 1 or new_shape[1] < 1: raise ValueError
+            else:
+                if new_shape < 1: raise ValueError
+        except (TypeError, ValueError):
+            self._inv_args(__class__.__name__, self.__calc_reshape_img_coef.__name__, out = out); return -1.0
+        else:
+            if isinstance(new_shape, list) is False and isinstance(new_shape, tuple) is False:
+                new_shape = (new_shape, new_shape)
+            return min(new_shape[0] / shape[0], new_shape[1] / shape[1])
 
     def __norm_pred(self, pred_data: np.ndarray, len_nn: int = 16, out: bool = True) -> np.ndarray:
-        """Нормализация оценок по экспертным и нейросетевым признакам (мультимодальная)
+        """Нормализация оценок по экспертным и нейросетевым признакам
 
         .. note::
             private (приватный метод)
 
         Args:
             pred_data (np.ndarray): Оценки
             len_nn (int): Максимальный размер вектора оценок
             out (bool): Отображение
 
         Returns:
-            np.ndarray: Нормализованные оценки по экспертным и нейросетевым признакам (мультимодальная)
+            np.ndarray: Нормализованные оценки по экспертным и нейросетевым признакам
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 1
                 :linenos:
                 :tab-width: 8
 
                 import numpy as np
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
                 arr = np.array([
                     [0.64113516, 0.6217892, 0.54451424, 0.6144415, 0.59334993],
                     [0.6652424, 0.63606125, 0.572305, 0.63169795, 0.612515]
                 ])
 
-                pred._Prediction__norm_pred(
+                video._Video__norm_pred(
                     pred_data = arr,
                     len_nn = 4,
                     out = True
                 )
 
             .. output-cell::
                 :execution-count: 1
@@ -293,78 +778,61 @@
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
 
                 import numpy as np
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
                 arr = np.array([])
 
-                pred._Prediction__norm_pred(
+                video._Video__norm_pred(
                     pred_data = arr,
                     len_nn = 4,
                     out = True
                 )
 
             .. output-cell::
                 :execution-count: 3
                 :linenos:
 
-                [2022-10-20 22:03:17] Неверные типы или значения аргументов в "Prediction.__norm_pred" ...
+                [2022-10-20 22:03:17] Неверные типы или значения аргументов в "Video.__norm_pred" ...
 
                 array([], dtype=float64)
         """
 
         try:
             # Проверка аргументов
-            if (
-                type(pred_data) is not np.ndarray
-                or len(pred_data) < 1
-                or type(len_nn) is not int
-                or len_nn < 1
-                or type(out) is not bool
-            ):
-                raise TypeError
+            if (type(pred_data) is not np.ndarray or len(pred_data) < 1 or type(len_nn) is not int or len_nn < 1
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__norm_pred.__name__, out=out)
-            return np.array([])
+            self._inv_args(__class__.__name__, self.__norm_pred.__name__, out = out); return np.array([])
         else:
             try:
                 if pred_data.shape[0] < len_nn:
-                    return np.pad(pred_data, ((0, len_nn - pred_data.shape[0]), (0, 0)), "mean")
+                    return np.pad(pred_data, ((0, len_nn - pred_data.shape[0]), (0, 0)), 'mean')
                 return pred_data[:len_nn]
             except ValueError:
-                self._other_error(self._norm_av_pred_error, last=False, out=out)
-                return np.array([])
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return np.array([])
+                self._other_error(self._norm_video_pred_error, last = False, out = out); return np.array([])
+            except Exception: self._other_error(self._unknown_err, out = out); return np.array([])
 
-    def __concat_pred_av(
-        self,
-        pred_hc_audio: np.ndarray,
-        pred_nn_audio: np.ndarray,
-        pred_hc_video: np.ndarray,
-        pred_nn_video: np.ndarray,
-        out: bool = True,
+    def __concat_pred(
+        self, pred_hc: np.ndarray, pred_nn: np.ndarray, out: bool = True
     ) -> List[Optional[np.ndarray]]:
-        """Конкатенация оценок по экспертным и нейросетевым признакам (мультимодальная)
+        """Конкатенация оценок по экспертным и нейросетевым признакам
 
         .. note::
             private (приватный метод)
 
         Args:
-            pred_hc_audio (np.ndarray): Оценки по экспертным признакам (аудио модальность)
-            pred_nn_audio (np.ndarray): Оценки по нейросетевым признакам (аудио модальность)
-            pred_hc_video (np.ndarray): Оценки по экспертным признакам (видео модальность)
-            pred_nn_video (np.ndarray): Оценки по нейросетевым признакам (видео модальность)
+            pred_hc (np.ndarray): Оценки по экспертным признакам
+            pred_nn (np.ndarray): Оценки по нейросетевым признакам
             out (bool): Отображение
 
         Returns:
             List[Optional[np.ndarray]]: Конкатенированные оценки по экспертным и нейросетевым признакам
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
@@ -373,2368 +841,2619 @@
 
             .. code-cell:: python
                 :execution-count: 1
                 :linenos:
                 :tab-width: 8
 
                 import numpy as np
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
-                arr_hc_audio = np.array([
+                arr_hc = np.array([
                     [0.64113516, 0.6217892, 0.54451424, 0.6144415, 0.59334993],
                     [0.6652424, 0.63606125, 0.572305, 0.63169795, 0.612515]
                 ])
 
-                arr_nn_audio = np.array([
+                arr_nn = np.array([
                     [0.56030345, 0.7488746, 0.44648764, 0.59893465, 0.5701077],
                     [0.5900006, 0.7652722, 0.4795154, 0.6409055, 0.6088242]
                 ])
-                arr_hc_video = np.array([
-                    [0.67113516, 0.6517892, 0.59451424, 0.6344415, 0.53334993],
-                    [0.6852424, 0.62606125, 0.562305, 0.67169795, 0.672515]
+
+                video._Video__concat_pred(
+                    pred_hc = arr_hc,
+                    pred_nn = arr_nn,
+                    out = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+                :tab-width: 12
+
+                [
+                    array([
+                        0.64113516, 0.6652424, 0.65318878, 0.65318878, 0.65318878,
+                        0.65318878, 0.65318878, 0.65318878, 0.65318878, 0.65318878,
+                        0.65318878, 0.65318878, 0.65318878, 0.65318878, 0.65318878,
+                        0.65318878, 0.56030345, 0.5900006, 0.57515202, 0.57515202,
+                        0.57515202, 0.57515202, 0.57515202, 0.57515202, 0.57515202,
+                        0.57515202, 0.57515202, 0.57515202, 0.57515202, 0.57515202,
+                        0.57515202, 0.57515202
+                    ]),
+                    array([
+                        0.6217892, 0.63606125, 0.62892523, 0.62892523, 0.62892523,
+                        0.62892523, 0.62892523, 0.62892523, 0.62892523, 0.62892523,
+                        0.62892523, 0.62892523, 0.62892523, 0.62892523, 0.62892523,
+                        0.62892523, 0.7488746, 0.7652722, 0.7570734, 0.7570734,
+                        0.7570734, 0.7570734, 0.7570734, 0.7570734, 0.7570734,
+                        0.7570734, 0.7570734, 0.7570734, 0.7570734, 0.7570734,
+                        0.7570734, 0.7570734
+                    ]),
+                    array([
+                        0.54451424, 0.572305, 0.55840962, 0.55840962, 0.55840962,
+                        0.55840962, 0.55840962, 0.55840962, 0.55840962, 0.55840962,
+                        0.55840962, 0.55840962, 0.55840962, 0.55840962, 0.55840962,
+                        0.55840962, 0.44648764, 0.4795154, 0.46300152, 0.46300152,
+                        0.46300152, 0.46300152, 0.46300152, 0.46300152, 0.46300152,
+                        0.46300152, 0.46300152, 0.46300152, 0.46300152, 0.46300152,
+                        0.46300152, 0.46300152
+                    ]),
+                    array([
+                        0.6144415, 0.63169795, 0.62306972, 0.62306972, 0.62306972,
+                        0.62306972, 0.62306972, 0.62306972, 0.62306972, 0.62306972,
+                        0.62306972, 0.62306972, 0.62306972, 0.62306972, 0.62306972,
+                        0.62306972, 0.59893465, 0.6409055, 0.61992008, 0.61992008,
+                        0.61992008, 0.61992008, 0.61992008, 0.61992008, 0.61992008,
+                        0.61992008, 0.61992008, 0.61992008, 0.61992008, 0.61992008,
+                        0.61992008, 0.61992008
+                    ]),
+                    array([
+                        0.59334993, 0.612515, 0.60293247, 0.60293247, 0.60293247,
+                        0.60293247, 0.60293247, 0.60293247, 0.60293247, 0.60293247,
+                        0.60293247, 0.60293247, 0.60293247, 0.60293247, 0.60293247,
+                        0.60293247, 0.5701077, 0.6088242, 0.58946595, 0.58946595,
+                        0.58946595, 0.58946595, 0.58946595, 0.58946595, 0.58946595,
+                        0.58946595, 0.58946595, 0.58946595, 0.58946595, 0.58946595,
+                        0.58946595, 0.58946595
+                    ])
+                ]
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                import numpy as np
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                arr_hc = np.array([
+                    [0.64113516, 0.6217892, 0.54451424, 0.6144415],
+                    [0.6652424, 0.63606125, 0.572305, 0.63169795, 0.612515]
                 ])
 
-                arr_nn_video = np.array([
-                    [0.58030345, 0.7788746, 0.47648764, 0.53893465, 0.5901077],
-                    [0.5100006, 0.7452722, 0.4495154, 0.6909055, 0.6488242]
+                arr_nn = np.array([
+                    [0.56030345, 0.7488746, 0.44648764, 0.59893465, 0.5701077],
+                    [0.5900006, 0.7652722, 0.4795154, 0.6409055, 0.6088242]
                 ])
 
-                pred._Prediction__concat_pred_av(
-                    pred_hc_audio = arr_hc_audio,
-                    pred_nn_audio = arr_nn_audio,
-                    pred_hc_video = arr_hc_video,
-                    pred_nn_video = arr_nn_video,
+                video._Video__concat_pred(
+                    pred_hc = arr_hc,
+                    pred_nn = arr_nn,
                     out = True
                 )
+
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-10-20 22:33:31] Ой! Что-то пошло не так ... конкатенация оценок по экспертным и нейросетевым
+                признакам не произведена (видео модальность) ...
+
+                []
         """
 
         try:
             # Проверка аргументов
-            if (
-                type(pred_hc_audio) is not np.ndarray
-                or len(pred_hc_audio) < 1
-                or type(pred_nn_audio) is not np.ndarray
-                or len(pred_nn_audio) < 1
-                or type(pred_hc_video) is not np.ndarray
-                or len(pred_hc_video) < 1
-                or type(pred_nn_video) is not np.ndarray
-                or len(pred_nn_video) < 1
-                or type(out) is not bool
-            ):
-                raise TypeError
+            if (type(pred_hc) is not np.ndarray or len(pred_hc) < 1
+                or type(pred_nn) is not np.ndarray or len(pred_nn) < 1
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__concat_pred_av.__name__, out=out)
-            return []
+            self._inv_args(__class__.__name__, self.__concat_pred.__name__, out = out); return []
         else:
-            # Нормализация оценок по экспертным и нейросетевым признакам (аудио модальность)
-            pred_hc_audio_norm = self.__norm_pred(pred_hc_audio, out=False)
-            pred_nn_audio_norm = self.__norm_pred(pred_nn_audio, out=False)
-
-            # Нормализация оценок по экспертным и нейросетевым признакам (видео модальность)
-            pred_hc_video_norm = self.__norm_pred(pred_hc_video, out=False)
-            pred_nn_video_norm = self.__norm_pred(pred_nn_video, out=False)
+            # Нормализация оценок по экспертным и нейросетевым признакам
+            pred_hc_norm = self.__norm_pred(pred_hc, out = False)
+            pred_nn_norm = self.__norm_pred(pred_nn, out = False)
 
-            if (
-                len(pred_hc_audio_norm) == 0
-                or len(pred_nn_audio_norm) == 0
-                or len(pred_hc_video_norm) == 0
-                or len(pred_nn_video_norm) == 0
-            ):
-                self._error(self._concat_av_pred_error, out=out)
-                return []
+            if len(pred_hc_norm) == 0 or len(pred_nn_norm) == 0:
+                self._error(self._concat_video_pred_error, out = out); return []
 
             concat = []
 
             try:
                 # Проход по всем персональным качествам личности человека
-                for i in range(len(self._b5["en"])):
+                for i in range(len(self._b5['en'])):
                     concat.append(
-                        np.hstack(
-                            (
-                                np.asarray(pred_hc_audio_norm)[:, i],
-                                np.asarray(pred_nn_audio_norm)[:, i],
-                                np.asarray(pred_hc_video_norm)[:, i],
-                                np.asarray(pred_nn_video_norm)[:, i],
-                            )
-                        )
+                        np.hstack((np.asarray(pred_hc_norm)[:, i], np.asarray(pred_nn_norm)[:, i]))
                     )
-            except IndexError:
-                self._other_error(self._concat_av_pred_error, last=False, out=out)
-                return []
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return []
+            except IndexError: self._other_error(self._concat_video_pred_error, last = False, out = out); return []
+            except Exception: self._other_error(self._unknown_err, out = out); return []
 
             return concat
 
-    def __load_model_weights(
-        self,
-        url: str,
-        force_reload: bool = True,
-        info_text: str = "",
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Загрузка весов нейросетевой модели
+    def __load_video_model_b5(
+        self, show_summary: bool = False, out: bool = True
+    ) -> Optional[keras.engine.functional.Functional]:
+        """Формирование нейросетевой архитектуры модели для получения результата оценки персонального качества
 
         .. note::
             private (приватный метод)
 
         Args:
-            url (str): Полный путь к файлу с весами нейросетевой модели
-            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
-            info_text (str): Текст для информационного сообщения
+            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
+            out (bool): Отображение
+
+        Returns:
+            Optional[keras.engine.functional.Functional]:
+                **None** если неверные типы или значения аргументов, в обратном случае нейросетевая модель
+                **tf.keras.Model** для получения результата оценки персонального качества
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video._Video__load_video_model_b5(
+                    show_summary = True, out = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                Model: "model"
+                _________________________________________________________________
+                 Layer (type)                Output Shape              Param #
+                =================================================================
+                 input_1 (InputLayer)        [(None, 32)]              0
+
+                 dense_1 (Dense)             (None, 1)                 33
+
+                 activ_1 (Activation)        (None, 1)                 0
+
+                =================================================================
+                Total params: 33
+                Trainable params: 33
+                Non-trainable params: 0
+                _________________________________________________________________
+                <keras.engine.functional.Functional at 0x13d442940>
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video._Video__load_video_model_b5(
+                    show_summary = True, out = []
+                )
+
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-10-17 10:53:03] Неверные типы или значения аргументов в "Video.__load_video_model_b5" ...
+        """
+
+        try:
+            # Проверка аргументов
+            if type(show_summary) is not bool or type(out) is not bool: raise TypeError
+        except TypeError:
+            self._inv_args(__class__.__name__, self.__load_video_model_b5.__name__, out = out); return None
+        else:
+            input_1 = tf.keras.Input(shape = (32,), name = 'input_1')
+            x = tf.keras.layers.Dense(units = 1, name = 'dense_1')(input_1)
+            x = tf.keras.layers.Activation('sigmoid', name = 'activ_1')(x)
+
+            model = tf.keras.Model(inputs = input_1, outputs = x)
+
+            if show_summary and out: model.summary()
+
+            return model
+
+    # ------------------------------------------------------------------------------------------------------------------
+    # Внутренние методы (защищенные)
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def _get_visual_features(
+        self, path: str, reduction_fps: int = 5, window: int = 10, step: int = 5,
+        last: bool = False, out: bool = True, runtime: bool = True, run: bool = True
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Извлечение признаков из визуального сигнала (без очистки истории вывода сообщений в ячейке Jupyter)
+
+        .. note::
+            protected (защищенный метод)
+
+        Args:
+            path (str): Путь к видеофайлу
+            reduction_fps (int): Понижение кадровой частоты
+            window (int): Размер окна сегмента сигнала (в кадрах)
+            step (int): Шаг сдвига окна сегмента сигнала (в кадрах)
+            last (bool): Замена последнего сообщения
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
-        """
+            Tuple[np.ndarray, np.ndarray]: Кортеж с двумя np.ndarray:
+
+                1. np.ndarray с экспертными признаками
+                2. np.ndarray с нейросетевыми признаками
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                res_load_model_deep_fe = video.load_video_model_deep_fe(
+                    show_summary = False,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-11-03 16:37:12] Формирование нейросетевой архитектуры для получения нейросетевых признаков (видео модальность) ...
+
+                --- Время выполнения: 1.564 сек. ---
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
+
+                url = video.weights_for_big5_['video']['fe']['sberdisk']
+
+                res_load_video_model_weights_deep_fe = video.load_video_model_weights_deep_fe(
+                    url = url,
+                    force_reload = True, out = True,
+                    runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+                [2022-11-03 16:39:10] Загрузка весов нейросетевой модели для получения нейросетевых признаков (видео модальность) ...
+
+                [2022-11-03 16:39:14] Загрузка файла "weights_2022-11-01_12-27-07.h5" (100.0%) ...
+
+                --- Время выполнения: 4.874 сек. ---
+
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+                :tab-width: 8
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+                path = '/Users/dl/GitHub/oceanai/oceanai/dataset/test80_01/glgfB3vFewc.004.mp4'
+
+                hc_features, nn_features = video.get_visual_features(
+                    path = path, reduction_fps = 5,
+                    window = 10, step = 5,
+                    out = True, runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-11-03 16:56:52] Извлечение признаков (экспертных и нейросетевых) из визуального сигнала ...
+
+                [2022-11-03 16:56:58] Статистика извлеченных признаков из визуального сигнала:
+                    Общее количество сегментов с:
+                        1. экспертными признаками: 12
+                        2. нейросетевыми признаками: 12
+                    Размерность матрицы экспертных признаков одного сегмента: 10 ✕ 115
+                    Размерность тензора с нейросетевыми признаками одного сегмента: 10 ✕ 512
+                    Понижение кадровой частоты: с 30 до 5
+
+                --- Время выполнения: 6.109 сек. ---
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 4
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                path = '/Users/dl/GitHub/oceanai/oceanai/dataset/test80_01/glgfB3vFewc.004.mp4'
+
+                hc_features, nn_features = video.get_visual_features(
+                    path = path, reduction_fps = 5,
+                    window = 10, step = 5,
+                    out = True, runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 4
+                :linenos:
+
+                [2022-11-03 16:59:45] Извлечение признаков (экспертных и нейросетевых) из визуального сигнала ...
+
+                [2022-11-03 16:59:46] Ой! Что-то пошло не так ... нейросетевая архитектура модели для получения нейросетевых признаков не сформирована (видео модальность) ...
+
+                --- Время выполнения: 1.358 сек. ---
+        """
 
         try:
             # Проверка аргументов
-            if (
-                type(url) is not str
-                or not url
-                or type(force_reload) is not bool
-                or type(info_text) is not str
-                or not info_text
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(path) is not str or not path or type(reduction_fps) is not int or reduction_fps < 1
+                or type(window) is not int or window < 1 or type(step) is not int or step < 1
+                or type(last) is not bool or type(out) is not bool or type(runtime) is not bool
+                or type(run) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__load_model_weights.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self._get_visual_features.__name__, last = last, out = out)
+            return np.empty([]), np.empty([])
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, last = last, out = out); return np.empty([]), np.empty([])
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
-            # Информационное сообщение
-            self._info(info_text, last=False, out=out)
-
-            sections = urlparse(url)  # Парсинг URL адреса
+            if last is False:
+                # Информационное сообщение
+                self._info(self._get_visual_feature_info, out = False)
+                if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
             try:
-                # URL файл невалидный
-                if sections.scheme == "":
-                    raise requests.exceptions.InvalidURL
-            except requests.exceptions.InvalidURL:
-                url = os.path.normpath(url)
-
-                try:
-                    if os.path.isfile(url) is False:
-                        raise FileNotFoundError  # Не файл
-                except FileNotFoundError:
-                    self._other_error(self._load_model_weights_error, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    self._url_last_filename = url
-                    return True
+                if os.path.isfile(path) is False: raise FileNotFoundError # Не файл
+            except FileNotFoundError:
+                self._other_error(self._file_not_found.format(self._info_wrapper(path)), last = last, out = out)
+                return np.empty([]), np.empty([])
+            except Exception:
+                self._other_error(self._unknown_err, last = last, out = out)
+                return np.empty([]), np.empty([])
             else:
                 try:
-                    if force_reload is False:
-                        clear_output(True)
-                    # Загрузка файла из URL
-                    res_download_file_from_url = self._download_file_from_url(
-                        url=url, force_reload=force_reload, runtime=False, out=out, run=True
-                    )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
+                    # Расширение файла не соответствует расширению искомых файлов
+                    if Path(path).suffix[1:].lower() not in self.__supported_video_formats: raise TypeError
+                except TypeError: self._other_error(
+                    self._wrong_extension_video_formats.format(
+                        self._info_wrapper(', '.join(x for x in self.__supported_video_formats))
+                    ), out = out
+                ); return np.empty([]), np.empty([])
+                except Exception: self._other_error(self._unknown_err, out = out); return np.empty([]), np.empty([])
                 else:
-                    # Файл загружен
-                    if res_download_file_from_url != 200:
-                        return False
+                    metadata = MediaInfo.parse(path).to_data() # Meta данные
 
-                    return True
+                    media_info = {} # Словарь для meta данных
+
+                    # Проход по всем meta словарям
+                    for track in metadata['tracks']:
+                        # Извлечение meta данных
+                        if track['track_type'] in [*self._type_meta_info]:
+                            media_info[track['track_type']] = {} # Словарь для meta данных определенного формата
+
+                            # Проход по всем необходимым meta данным
+                            for i, curr_necessary in enumerate(self._type_meta_info[track['track_type']]):
+                                try: val = track[curr_necessary] # Текущее значение
+                                except Exception: continue
+                                else:
+                                    try:
+                                        if curr_necessary == 'encoded_date':
+                                            val = datetime.strptime(val.replace('UTC ', ''), '%Y-%m-%d %H:%M:%S')
+                                        if (curr_necessary == 'frame_rate' or curr_necessary == 'minimum_frame_rate'
+                                            or curr_necessary == 'maximum_frame_rate'): val = float(val)
+                                    except Exception: continue
+
+                                    # Список в строку
+                                    if type(val) is list:
+                                        if len(val) < 2: val = val[0]
+                                        else: val = ', '.join([str(elem) for elem in val])
+
+                                    media_info[track['track_type']][curr_necessary] = val
+
+                    try:
+                        # Всего кадров в видеопотоке
+                        all_frames = int(media_info['Video']['duration'] / 1000 * media_info['Video']['frame_rate'])
+                    except Exception: all_frames = 0
+
+                    try:
+                        if all_frames == 0: raise ValueError
+                    except ValueError: self._other_error(
+                        self._all_frames_is_zero.format(self._info_wrapper(str(all_frames))), out = out
+                    ); return np.empty([]), np.empty([])
+                    except Exception: self._other_error(self._unknown_err, out = out); return np.empty([]), np.empty([])
+                    else:
+                        cap = cv2.VideoCapture(path) # Захват видеофайла для чтения
+                        width_video = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH)) # Ширина кадров в видеопотоке
+                        height_video = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)) # Высота кадров в видеопотоке
+                        all_frames_cv2 = int(cap.get(cv2.CAP_PROP_FRAME_COUNT)) # # Всего кадров в видеопотоке
+
+                        fps_cv2 = np.round(cap.get(cv2.CAP_PROP_FPS)) # Частота кадров (FPS)
+
+                        # Вычисление коэффициента изменения размера изображения
+                        reshape_img_coef = self.__calc_reshape_img_coef(
+                            shape = [width_video, height_video], new_shape = self.__bndbox_face_size, out = False
+                        )
+
+                        try:
+                            if reshape_img_coef == -1: raise ValueError
+                        except ValueError:
+                            self._other_error(self._calc_reshape_img_coef_error, out = out)
+                            return np.empty([]), np.empty([])
+                        else:
+                            # Прореживание кадров
+                            if reduction_fps > fps_cv2: reduction_fps = fps_cv2
+                            # Всего кадров после прореживания
+                            all_frms_reduct = all_frames_cv2 / (fps_cv2 / reduction_fps)
+
+                            # Индексы кадров, которые останутся после прореживания
+                            idx_reduction_frames = list(map(
+                                self._round_math,
+                                np.arange(0, all_frames_cv2, all_frames_cv2 / all_frms_reduct, dtype = float)
+                            ))
+
+                            def alignment_procedure(left_eye: List[int], right_eye: List[int]) -> float:
+                                """Выравнивание угла наклона головы относительно центров глаз
+
+                                .. note::
+                                    внутренняя функция
+
+                                Args:
+                                    left_eye (List[int]): Координаты центра левого глаза
+                                    right_eye (List[int]): Координаты центра правого глаза
+
+                                Returns:
+                                    float: Градус расхождения центров глаз
+                                """
+
+                                left_eye_x, left_eye_y = left_eye
+                                right_eye_x, right_eye_y = right_eye
+
+                                if left_eye_y > right_eye_y: point_3rd = (right_eye_x, left_eye_y); direction = -1
+                                else: point_3rd = (left_eye_x, right_eye_y); direction = 1
+
+                                a = distance.euclidean(np.array(left_eye), np.array(point_3rd))
+                                b = distance.euclidean(np.array(right_eye), np.array(point_3rd))
+                                c = distance.euclidean(np.array(right_eye), np.array(left_eye))
+
+                                if b != 0 and c != 0:
+                                    cos_a = (b * b + c * c - a * a) / (2 * b * c)
+                                    angle = np.arccos(cos_a)
+                                    angle = (angle * 180) / math.pi
+
+                                    if direction == -1: angle = 90 - angle
+                                else: angle = 0
+
+                                return angle
+
+                            cnt_frame = 0  # Счетчик кадров
+                            vt, pt = self.__mp_drawing._VISIBILITY_THRESHOLD, self.__mp_drawing._PRESENCE_THRESHOLD
+
+                            hcs = [] # Набор экспертных признаков
+                            bndbox_faces = [] # Области с лицами
+
+                            # Получение 468 3D-ориентиров лица
+                            with self.__mp_face_mesh.FaceMesh(
+                                max_num_faces = 1, # Максимальное количество лиц для обнаружения
+                                # Необходимо ли дополнительно уточнять координаты ориентиров вокруг глаз и губ
+                                # и выводить дополнительные ориентиры вокруг радужной оболочки
+                                refine_landmarks = True,
+                                # Минимальное значение достоверности из модели обнаружения лиц,
+                                # при котором обнаружение считается успешным
+                                min_detection_confidence = 0.5,
+                                # Минимальное значение достоверности из модели отслеживания ориентиров для того,
+                                # чтобы ориентиры лиц считались успешно отслеженными
+                                min_tracking_confidence = 0.5
+                            ) as face_mesh:
+                                # Проход по всем кадрам видеопотока
+                                while cap.isOpened():
+                                    _, frame = cap.read() # Захват, декодирование и возврат кадра
+
+                                    if frame is None: break # Кадр не найден
+
+                                    if cnt_frame in idx_reduction_frames:
+                                        # Запись недоступна (увеличение производительности)
+                                        frame.flags.writeable = False
+                                        frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                                        results = face_mesh.process(frame)
+                                        # Запись доступна
+                                        frame.flags.writeable = True
+
+                                        # Найдены 468 3D-ориентиров лица
+                                        if results.multi_face_landmarks:
+                                            # Проход по всем лицам
+                                            for idx_face, face_landmarks in enumerate(results.multi_face_landmarks):
+                                                idx_to_coors = {} # Координаты всех ориентиров лица
+
+                                                # Проход по всем ориентирам лица
+                                                for idx_landmark, lmk in enumerate(face_landmarks.landmark):
+                                                    if ((lmk.HasField('visibility') and lmk.visibility < vt)
+                                                            or (lmk.HasField('presence') and lmk.presence < pt)):
+                                                        continue
+
+                                                    # Нормализация координат
+                                                    norm_x = min(math.floor(lmk.x * width_video), width_video - 1)
+                                                    norm_y = min(math.floor(lmk.y * height_video), height_video - 1)
+
+                                                    norm_x = int(norm_x * reshape_img_coef)
+                                                    norm_y = int(norm_y * reshape_img_coef)
+
+                                                    # Добавление нормализованных координат ориентиров лица в словарь
+                                                    idx_to_coors[idx_landmark] = (norm_x, norm_y)
+
+                                                # Вычисление ограничивающей рамки из ориентиров лица
+                                                x_min = np.min(np.asarray(list(idx_to_coors.values()))[:, 0])
+                                                y_min = np.min(np.asarray(list(idx_to_coors.values()))[:, 1])
+                                                x_max = np.max(np.asarray(list(idx_to_coors.values()))[:, 0])
+                                                y_max = np.max(np.asarray(list(idx_to_coors.values()))[:, 1])
+
+                                                # Коррекция ограничивающей рамки
+                                                start_x, start_y = (max(0, x_min), max(0, y_min))
+                                                end_x, end_y = (
+                                                    min(width_video - 1, x_max),
+                                                    min(height_video - 1, y_max)
+                                                )
+
+                                                # Область с лицом
+                                                bndbox_face = frame[
+                                                    int(start_y / reshape_img_coef) : int(end_y / reshape_img_coef),
+                                                    int(start_x / reshape_img_coef) : int(end_x / reshape_img_coef)
+                                                ]
+                                                # Приведение изображения с лицом в нужному размеру
+                                                bndbox_face = cv2.resize(
+                                                    bndbox_face, self.__bndbox_face_size, interpolation = cv2.INTER_AREA
+                                                )
+
+                                                bndbox_face = tf.keras.preprocessing.image.img_to_array(bndbox_face)
+                                                bndbox_face = utils.preprocess_input(bndbox_face)
+
+                                                bndbox_face = bndbox_face.reshape(
+                                                    -1, self.__bndbox_face_size[0], self.__bndbox_face_size[1], 3
+                                                )
+
+                                                # 1) Координаты центра глаз
+                                                # 2) Текущие экспертные признаки
+                                                point_eyes, curr_seq_hc = [], []
+
+                                                # Вычисление центра глаз
+                                                for i in [[474, 476], [469, 471]]:
+                                                    eye_x_min = min(idx_to_coors[i[0]][0], idx_to_coors[i[1]][0])
+                                                    eye_y_min = min(idx_to_coors[i[0]][1], idx_to_coors[i[1]][1])
+                                                    # Разница между yголками глаза
+                                                    eye_x_diff = int(abs(
+                                                        idx_to_coors[i[0]][0] - idx_to_coors[i[1]][0]
+                                                    ) / 2)
+                                                    eye_y_diff = int(abs(
+                                                        idx_to_coors[i[0]][1] - idx_to_coors[i[1]][1]
+                                                    ) / 2)
+
+                                                    point_eyes.append([
+                                                        eye_x_min + eye_x_diff - x_min,
+                                                        eye_y_min + eye_y_diff - y_min
+                                                    ])
+                                                    curr_seq_hc.extend([
+                                                        eye_x_min + eye_x_diff - x_min,
+                                                        eye_y_min + eye_y_diff - y_min
+                                                    ])
+
+                                                coords_left_eye = point_eyes[0] # Координата центра левого глаза
+                                                coords_right_eye = point_eyes[1] # Координата центра правого глаза
+
+                                                # Вычисление расстояния между центрами глаз
+                                                curr_seq_hc.append(distance.euclidean(coords_left_eye, coords_right_eye))
+                                                # Вычисление угла наклона головы
+                                                curr_seq_hc.append(alignment_procedure(coords_left_eye, coords_right_eye))
+                                                # Вычисление расстояния между центром левого глаза и его левым углом
+                                                curr_seq_hc.append(distance.euclidean(
+                                                    coords_left_eye,
+                                                    np.asarray(idx_to_coors[263]) - np.asarray([x_min, y_min])
+                                                ))
+                                                # Вычисление расстояния между центром левого глаза и его правым углом
+                                                curr_seq_hc.append(distance.euclidean(
+                                                    coords_left_eye,
+                                                    np.asarray(idx_to_coors[362]) - np.asarray([x_min, y_min])
+                                                ))
+                                                # Вычисление расстояния между центром правого глаза и его левым углом
+                                                curr_seq_hc.append(distance.euclidean(
+                                                    coords_right_eye,
+                                                    np.asarray(idx_to_coors[133]) - np.asarray([x_min, y_min])
+                                                ))
+                                                # Вычисление расстояния между центром правого глаза и его правым углом
+                                                curr_seq_hc.append(distance.euclidean(
+                                                    coords_right_eye,
+                                                    np.asarray(idx_to_coors[33]) - np.asarray([x_min, y_min])))
+                                                # Вычисление угла наклона уголков рта
+                                                curr_seq_hc.append(alignment_procedure(
+                                                    np.asarray(idx_to_coors[105]) - np.asarray([x_min, y_min]),
+                                                    np.asarray(idx_to_coors[334]) - np.asarray([x_min, y_min])
+                                                ))
+                                                # Вычисление угла наклона бровей
+                                                curr_seq_hc.append(alignment_procedure(
+                                                    np.asarray(idx_to_coors[61]) - np.asarray([x_min, y_min]),
+                                                    np.asarray(idx_to_coors[291]) - np.asarray([x_min, y_min])
+                                                ))
+
+                                                for coord in self.__coords_face_mesh:
+                                                    curr_seq_hc.extend((
+                                                        np.asarray(idx_to_coors[coord]) - np.asarray([x_min, y_min])
+                                                    ).tolist())
+
+                                                for cpl in self.__couples_face_mesh:
+                                                    curr_seq_hc.append(distance.euclidean(
+                                                        np.asarray(idx_to_coors[cpl[0]]) - np.asarray([x_min, y_min]),
+                                                        np.asarray(idx_to_coors[cpl[1]]) - np.asarray([x_min, y_min])
+                                                    ))
+
+                                            bndbox_faces.append(bndbox_face)
+                                            hcs.append(curr_seq_hc)
+                                    cnt_frame += 1
+
+                                cap.release()
+
+                            # Лицо не найдено не на одном кадре
+                            if len(bndbox_faces) == 0:
+                                self._error(self._faces_not_found, out = out); return np.empty([]), np.empty([])
+
+                            hcs = np.asarray(hcs)
+
+                            # Коды ошибок нейросетевой модели
+                            code_error_pred_deep_fe = -1
+
+                            try:
+                                # Отправка областей с лицами в нейросетевую модель для получения нейросетевых признаков
+                                extract_deep_fe = self._video_model_deep_fe(np.vstack(bndbox_faces))
+                            except TypeError: code_error_pred_deep_fe = 1
+                            except Exception: code_error_pred_deep_fe = 2
+
+                            if code_error_pred_deep_fe != -1:
+                                self._error(self._model_video_deep_fe_not_formation, out = out)
+                                return np.empty([]), np.empty([])
+
+                            # 1. Список с экспертными признаками
+                            # 2. Список с нейросетевыми признаками
+                            hc_features, nn_features = [], []
+
+                            # Проход по всему набору экспертных и нейросетевых признаков
+                            for idx_hc_nn in range(0, len(hcs) + 1, step):
+                                last_idx__hc_nn = idx_hc_nn + window # ID последнего элемента в подвыборке
+
+                                # Текущие подвыборки
+                                curr_seq_nn = extract_deep_fe[idx_hc_nn:last_idx__hc_nn].numpy().tolist()
+                                curr_seq_hc = hcs[idx_hc_nn:last_idx__hc_nn].tolist()
+                                if len(curr_seq_nn) < window and len(curr_seq_nn) != 0:
+                                    curr_seq_hc.extend([curr_seq_hc[-1]] * (window - len(curr_seq_hc)))
+                                    curr_seq_nn.extend([curr_seq_nn[-1]] * (window - len(curr_seq_nn)))
+                                if len(curr_seq_nn) != 0:
+                                    hc_features.append(curr_seq_hc)
+                                    nn_features.append(curr_seq_nn)
+
+                            hc_features = stats.zscore(hc_features, axis = -1)
+
+                            if last is False:
+                                # Статистика извлеченных признаков из визуального сигнала
+                                self._stat_visual_features(
+                                    last = last, out = out,
+                                    len_hc_features = len(hc_features),
+                                    len_nn_features = len(nn_features),
+                                    shape_hc_features = np.array(hc_features[0]).shape,
+                                    shape_nn_features = np.array(nn_features[0]).shape,
+                                    fps_before = self._round_math(fps_cv2, out),
+                                    fps_after = self._round_math(reduction_fps, out),
+                                )
+
+                            return hc_features, np.asarray(nn_features)
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
 
-    def __load_avt_model_b5(self, show_summary: bool = False, out: bool = True) -> Optional[tf.keras.Model]:
-        """Формирование нейросетевой архитектуры модели для получения оценок персональных качеств
+    # ------------------------------------------------------------------------------------------------------------------
+    # Внешние методы
+    # ------------------------------------------------------------------------------------------------------------------
 
-        .. note::
-            private (приватный метод)
+    def load_video_model_hc(
+        self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
+    ) -> bool:
+        """Формирование нейросетевой архитектуры модели для получения оценок по экспертным признакам
 
         Args:
             show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
             out (bool): Отображение
+            runtime (bool): Подсчет времени выполнения
+            run (bool): Блокировка выполнения
 
         Returns:
-            Optional[tf.keras.Model]:
-                **None** если неверные типы или значения аргументов, в обратном случае нейросетевая модель
-                **tf.keras.Model** для получения оценок персональных качеств
+            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+                video.load_video_model_hc(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-10-25 16:37:43] Формирование нейросетевой архитектуры модели для получения оценок по экспертным признакам (видео модальность) ...
+
+                --- Время выполнения: 0.659 сек. ---
+
+                True
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+                video.load_video_model_hc(
+                    show_summary = 1, out = True,
+                    runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+                [2022-10-26 12:27:41] Неверные типы или значения аргументов в "Video.load_video_model_hc" ...
+
+                False
         """
 
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
+
         try:
             # Проверка аргументов
-            if type(show_summary) is not bool or type(out) is not bool:
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.__load_av_model_b5.__name__, out=out)
-            return None
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
+        except TypeError: self._inv_args(__class__.__name__, self.load_video_model_hc.__name__, out = out); return False
         else:
-            i_hc_t_1 = tf.keras.Input(shape=(128,), name="hc_t")
-            i_nn_t_1 = tf.keras.Input(shape=(128,), name="nn_t")
-            i_hc_a_1 = tf.keras.Input(shape=(256,), name="hc_a")
-            i_nn_a_1 = tf.keras.Input(shape=(512,), name="nn_a")
-            i_hc_v_1 = tf.keras.Input(shape=(256,), name="hc_v")
-            i_nn_v_1 = tf.keras.Input(shape=(2048,), name="nn_v")
-
-            i_hc_t_1_n = tf.keras.layers.LayerNormalization(axis=1, name="ln_hc_t")(i_hc_t_1)
-            i_nn_t_1_n = tf.keras.layers.LayerNormalization(axis=1, name="ln_nn_t")(i_nn_t_1)
-            i_hc_a_1_n = tf.keras.layers.LayerNormalization(axis=1, name="ln_hc_a")(i_hc_a_1)
-            i_nn_a_1_n = tf.keras.layers.LayerNormalization(axis=1, name="ln_nn_a")(i_nn_a_1)
-            i_hc_v_1_n = tf.keras.layers.LayerNormalization(axis=1, name="ln_hc_v")(i_hc_v_1)
-            i_nn_v_1_n = tf.keras.layers.LayerNormalization(axis=1, name="ln_nn_v")(i_nn_v_1)
-
-            gf_ta = GFL(output_dim=64, kernel_initializer=tf.keras.initializers.TruncatedNormal(seed=42), name="gata")
-            gf_tv = GFL(output_dim=64, kernel_initializer=tf.keras.initializers.TruncatedNormal(seed=42), name="gatv")
-            gf_av = GFL(output_dim=64, kernel_initializer=tf.keras.initializers.TruncatedNormal(seed=42), name="gaav")
-
-            gf_ta_1 = gf_ta([i_hc_t_1_n, i_hc_a_1_n, i_nn_t_1_n, i_nn_a_1_n])
-            gf_tv_1 = gf_tv([i_hc_t_1_n, i_hc_v_1_n, i_nn_t_1_n, i_nn_v_1_n])
-            gf_av_1 = gf_av([i_hc_a_1_n, i_hc_v_1_n, i_nn_a_1_n, i_nn_v_1_n])
-
-            concat_1 = Concat()((gf_ta_1, gf_tv_1, gf_av_1))
+            # Блокировка выполнения
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            dense = tf.keras.layers.Dense(50, activation="relu", name="dense")(concat_1)
+            if runtime: self._r_start()
 
-            dense = tf.keras.layers.Dense(5, activation="sigmoid", name="dence_cl")(dense)
+            # Информационное сообщение
+            self._info(self._formation_video_model_hc, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
-            model = tf.keras.Model(inputs=[i_hc_t_1, i_nn_t_1, i_hc_a_1, i_nn_a_1, i_hc_v_1, i_nn_v_1], outputs=dense)
+            input_lstm = tf.keras.Input(shape = (10, 115))
 
-            if show_summary and out:
-                model.summary()
+            x = tf.keras.layers.LSTM(64, return_sequences = True)(input_lstm)
+            x = tf.keras.layers.Dropout(rate = 0.2)(x)
+            x = tf.keras.layers.LSTM(128, return_sequences = False)(x)
+            x = tf.keras.layers.Dropout(rate = 0.2)(x)
+            x = tf.keras.layers.Dense(5, activation = 'linear')(x)
 
-            return model
+            self._video_model_hc = tf.keras.Model(inputs = input_lstm, outputs = x)
 
-    def __load_av_model_b5(self, show_summary: bool = False, out: bool = True) -> Optional[tf.keras.Model]:
-        """Формирование нейросетевой архитектуры модели для получения результата оценки персонального качества
+            if show_summary and out: self._video_model_hc.summary()
 
-        .. note::
-            private (приватный метод)
+            if runtime: self._r_end(out = out)
+
+            return True
+
+    def load_video_model_deep_fe(
+        self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
+    ) -> bool:
+        """Формирование нейросетевой архитектуры для получения нейросетевых признаков
 
         Args:
             show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
             out (bool): Отображение
+            runtime (bool): Подсчет времени выполнения
+            run (bool): Блокировка выполнения
 
         Returns:
-            Optional[tf.keras.Model]:
-                **None** если неверные типы или значения аргументов, в обратном случае нейросетевая модель
-                **tf.keras.Model** для получения результата оценки персонального качества
+            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 1
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
-
-                pred._Prediction__load_av_model_b5(
-                    show_summary = True, out = True
+                video = Video()
+                video.load_video_model_deep_fe(
+                    show_summary = True, out = True,
+                    runtime = True, run = True
                 )
 
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
-                Model: "model"
-                _________________________________________________________________
-                 Layer (type)                Output Shape              Param #
-                =================================================================
-                 input_1 (InputLayer)        [(None, 64)]              0
+                [2022-11-01 12:18:14] Формирование нейросетевой архитектуры для получения нейросетевых признаков (видео модальность) ...
 
-                 dense_1 (Dense)             (None, 1)                 65
+                Model: "model_1"
+                __________________________________________________________________________________________________
+                 Layer (type)                   Output Shape         Param #     Connected to
+                ==================================================================================================
+                 input_2 (InputLayer)           [(None, 224, 224, 3  0           []
+                                                )]
 
-                 activ_1 (Activation)        (None, 1)                 0
+                 conv1/7x7_s2 (Conv2D)          (None, 112, 112, 64  9408        ['input_2[0][0]']
+                                                )
 
-                =================================================================
-                Total params: 65
-                Trainable params: 65
-                Non-trainable params: 0
-                _________________________________________________________________
-                <tf.keras.Model at 0x147892ee0>
+                 conv1/7x7_s2/bn (BatchNormaliz  (None, 112, 112, 64  256        ['conv1/7x7_s2[0][0]']
+                 ation)                         )
+
+                 activation_49 (Activation)     (None, 112, 112, 64  0           ['conv1/7x7_s2/bn[0][0]']
+                                                )
+
+                 max_pooling2d_1 (MaxPooling2D)  (None, 55, 55, 64)  0           ['activation_49[0][0]']
+
+                 conv2_1_1x1_reduce (Conv2D)    (None, 55, 55, 64)   4096        ['max_pooling2d_1[0][0]']
+
+                 conv2_1_1x1_reduce/bn (BatchNo  (None, 55, 55, 64)  256         ['conv2_1_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_50 (Activation)     (None, 55, 55, 64)   0           ['conv2_1_1x1_reduce/bn[0][0]']
+
+                 conv2_1_3x3 (Conv2D)           (None, 55, 55, 64)   36864       ['activation_50[0][0]']
+
+                 conv2_1_3x3/bn (BatchNormaliza  (None, 55, 55, 64)  256         ['conv2_1_3x3[0][0]']
+                 tion)
+
+                 activation_51 (Activation)     (None, 55, 55, 64)   0           ['conv2_1_3x3/bn[0][0]']
+
+                 conv2_1_1x1_increase (Conv2D)  (None, 55, 55, 256)  16384       ['activation_51[0][0]']
+
+                 conv2_1_1x1_proj (Conv2D)      (None, 55, 55, 256)  16384       ['max_pooling2d_1[0][0]']
+
+                 conv2_1_1x1_increase/bn (Batch  (None, 55, 55, 256)  1024       ['conv2_1_1x1_increase[0][0]']
+                 Normalization)
+
+                 conv2_1_1x1_proj/bn (BatchNorm  (None, 55, 55, 256)  1024       ['conv2_1_1x1_proj[0][0]']
+                 alization)
+
+                 add_16 (Add)                   (None, 55, 55, 256)  0           ['conv2_1_1x1_increase/bn[0][0]',
+                                                                                  'conv2_1_1x1_proj/bn[0][0]']
+
+                 activation_52 (Activation)     (None, 55, 55, 256)  0           ['add_16[0][0]']
+
+                 conv2_2_1x1_reduce (Conv2D)    (None, 55, 55, 64)   16384       ['activation_52[0][0]']
+
+                 conv2_2_1x1_reduce/bn (BatchNo  (None, 55, 55, 64)  256         ['conv2_2_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_53 (Activation)     (None, 55, 55, 64)   0           ['conv2_2_1x1_reduce/bn[0][0]']
+
+                 conv2_2_3x3 (Conv2D)           (None, 55, 55, 64)   36864       ['activation_53[0][0]']
+
+                 conv2_2_3x3/bn (BatchNormaliza  (None, 55, 55, 64)  256         ['conv2_2_3x3[0][0]']
+                 tion)
+
+                 activation_54 (Activation)     (None, 55, 55, 64)   0           ['conv2_2_3x3/bn[0][0]']
+
+                 conv2_2_1x1_increase (Conv2D)  (None, 55, 55, 256)  16384       ['activation_54[0][0]']
+
+                 conv2_2_1x1_increase/bn (Batch  (None, 55, 55, 256)  1024       ['conv2_2_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_17 (Add)                   (None, 55, 55, 256)  0           ['conv2_2_1x1_increase/bn[0][0]',
+                                                                                  'activation_52[0][0]']
+
+                 activation_55 (Activation)     (None, 55, 55, 256)  0           ['add_17[0][0]']
+
+                 conv2_3_1x1_reduce (Conv2D)    (None, 55, 55, 64)   16384       ['activation_55[0][0]']
+
+                 conv2_3_1x1_reduce/bn (BatchNo  (None, 55, 55, 64)  256         ['conv2_3_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_56 (Activation)     (None, 55, 55, 64)   0           ['conv2_3_1x1_reduce/bn[0][0]']
+
+                 conv2_3_3x3 (Conv2D)           (None, 55, 55, 64)   36864       ['activation_56[0][0]']
+
+                 conv2_3_3x3/bn (BatchNormaliza  (None, 55, 55, 64)  256         ['conv2_3_3x3[0][0]']
+                 tion)
+
+                 activation_57 (Activation)     (None, 55, 55, 64)   0           ['conv2_3_3x3/bn[0][0]']
+
+                 conv2_3_1x1_increase (Conv2D)  (None, 55, 55, 256)  16384       ['activation_57[0][0]']
+
+                 conv2_3_1x1_increase/bn (Batch  (None, 55, 55, 256)  1024       ['conv2_3_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_18 (Add)                   (None, 55, 55, 256)  0           ['conv2_3_1x1_increase/bn[0][0]',
+                                                                                  'activation_55[0][0]']
+
+                 activation_58 (Activation)     (None, 55, 55, 256)  0           ['add_18[0][0]']
+
+                 conv3_1_1x1_reduce (Conv2D)    (None, 28, 28, 128)  32768       ['activation_58[0][0]']
+
+                 conv3_1_1x1_reduce/bn (BatchNo  (None, 28, 28, 128)  512        ['conv3_1_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_59 (Activation)     (None, 28, 28, 128)  0           ['conv3_1_1x1_reduce/bn[0][0]']
+
+                 conv3_1_3x3 (Conv2D)           (None, 28, 28, 128)  147456      ['activation_59[0][0]']
+
+                 conv3_1_3x3/bn (BatchNormaliza  (None, 28, 28, 128)  512        ['conv3_1_3x3[0][0]']
+                 tion)
+
+                 activation_60 (Activation)     (None, 28, 28, 128)  0           ['conv3_1_3x3/bn[0][0]']
+
+                 conv3_1_1x1_increase (Conv2D)  (None, 28, 28, 512)  65536       ['activation_60[0][0]']
+
+                 conv3_1_1x1_proj (Conv2D)      (None, 28, 28, 512)  131072      ['activation_58[0][0]']
+
+                 conv3_1_1x1_increase/bn (Batch  (None, 28, 28, 512)  2048       ['conv3_1_1x1_increase[0][0]']
+                 Normalization)
+
+                 conv3_1_1x1_proj/bn (BatchNorm  (None, 28, 28, 512)  2048       ['conv3_1_1x1_proj[0][0]']
+                 alization)
+
+                 add_19 (Add)                   (None, 28, 28, 512)  0           ['conv3_1_1x1_increase/bn[0][0]',
+                                                                                  'conv3_1_1x1_proj/bn[0][0]']
+
+                 activation_61 (Activation)     (None, 28, 28, 512)  0           ['add_19[0][0]']
+
+                 conv3_2_1x1_reduce (Conv2D)    (None, 28, 28, 128)  65536       ['activation_61[0][0]']
+
+                 conv3_2_1x1_reduce/bn (BatchNo  (None, 28, 28, 128)  512        ['conv3_2_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_62 (Activation)     (None, 28, 28, 128)  0           ['conv3_2_1x1_reduce/bn[0][0]']
+
+                 conv3_2_3x3 (Conv2D)           (None, 28, 28, 128)  147456      ['activation_62[0][0]']
+
+                 conv3_2_3x3/bn (BatchNormaliza  (None, 28, 28, 128)  512        ['conv3_2_3x3[0][0]']
+                 tion)
+
+                 activation_63 (Activation)     (None, 28, 28, 128)  0           ['conv3_2_3x3/bn[0][0]']
+
+                 conv3_2_1x1_increase (Conv2D)  (None, 28, 28, 512)  65536       ['activation_63[0][0]']
+
+                 conv3_2_1x1_increase/bn (Batch  (None, 28, 28, 512)  2048       ['conv3_2_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_20 (Add)                   (None, 28, 28, 512)  0           ['conv3_2_1x1_increase/bn[0][0]',
+                                                                                  'activation_61[0][0]']
+
+                 activation_64 (Activation)     (None, 28, 28, 512)  0           ['add_20[0][0]']
+
+                 conv3_3_1x1_reduce (Conv2D)    (None, 28, 28, 128)  65536       ['activation_64[0][0]']
+
+                 conv3_3_1x1_reduce/bn (BatchNo  (None, 28, 28, 128)  512        ['conv3_3_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_65 (Activation)     (None, 28, 28, 128)  0           ['conv3_3_1x1_reduce/bn[0][0]']
+
+                 conv3_3_3x3 (Conv2D)           (None, 28, 28, 128)  147456      ['activation_65[0][0]']
+
+                 conv3_3_3x3/bn (BatchNormaliza  (None, 28, 28, 128)  512        ['conv3_3_3x3[0][0]']
+                 tion)
+
+                 activation_66 (Activation)     (None, 28, 28, 128)  0           ['conv3_3_3x3/bn[0][0]']
+
+                 conv3_3_1x1_increase (Conv2D)  (None, 28, 28, 512)  65536       ['activation_66[0][0]']
+
+                 conv3_3_1x1_increase/bn (Batch  (None, 28, 28, 512)  2048       ['conv3_3_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_21 (Add)                   (None, 28, 28, 512)  0           ['conv3_3_1x1_increase/bn[0][0]',
+                                                                                  'activation_64[0][0]']
+
+                 activation_67 (Activation)     (None, 28, 28, 512)  0           ['add_21[0][0]']
+
+                 conv3_4_1x1_reduce (Conv2D)    (None, 28, 28, 128)  65536       ['activation_67[0][0]']
+
+                 conv3_4_1x1_reduce/bn (BatchNo  (None, 28, 28, 128)  512        ['conv3_4_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_68 (Activation)     (None, 28, 28, 128)  0           ['conv3_4_1x1_reduce/bn[0][0]']
+
+                 conv3_4_3x3 (Conv2D)           (None, 28, 28, 128)  147456      ['activation_68[0][0]']
+
+                 conv3_4_3x3/bn (BatchNormaliza  (None, 28, 28, 128)  512        ['conv3_4_3x3[0][0]']
+                 tion)
+
+                 activation_69 (Activation)     (None, 28, 28, 128)  0           ['conv3_4_3x3/bn[0][0]']
+
+                 conv3_4_1x1_increase (Conv2D)  (None, 28, 28, 512)  65536       ['activation_69[0][0]']
+
+                 conv3_4_1x1_increase/bn (Batch  (None, 28, 28, 512)  2048       ['conv3_4_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_22 (Add)                   (None, 28, 28, 512)  0           ['conv3_4_1x1_increase/bn[0][0]',
+                                                                                  'activation_67[0][0]']
+
+                 activation_70 (Activation)     (None, 28, 28, 512)  0           ['add_22[0][0]']
+
+                 conv4_1_1x1_reduce (Conv2D)    (None, 14, 14, 256)  131072      ['activation_70[0][0]']
+
+                 conv4_1_1x1_reduce/bn (BatchNo  (None, 14, 14, 256)  1024       ['conv4_1_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_71 (Activation)     (None, 14, 14, 256)  0           ['conv4_1_1x1_reduce/bn[0][0]']
+
+                 conv4_1_3x3 (Conv2D)           (None, 14, 14, 256)  589824      ['activation_71[0][0]']
+
+                 conv4_1_3x3/bn (BatchNormaliza  (None, 14, 14, 256)  1024       ['conv4_1_3x3[0][0]']
+                 tion)
+
+                 activation_72 (Activation)     (None, 14, 14, 256)  0           ['conv4_1_3x3/bn[0][0]']
+
+                 conv4_1_1x1_increase (Conv2D)  (None, 14, 14, 1024  262144      ['activation_72[0][0]']
+                                                )
+
+                 conv4_1_1x1_proj (Conv2D)      (None, 14, 14, 1024  524288      ['activation_70[0][0]']
+                                                )
+
+                 conv4_1_1x1_increase/bn (Batch  (None, 14, 14, 1024  4096       ['conv4_1_1x1_increase[0][0]']
+                 Normalization)                 )
+
+                 conv4_1_1x1_proj/bn (BatchNorm  (None, 14, 14, 1024  4096       ['conv4_1_1x1_proj[0][0]']
+                 alization)                     )
+
+                 add_23 (Add)                   (None, 14, 14, 1024  0           ['conv4_1_1x1_increase/bn[0][0]',
+                                                )                                 'conv4_1_1x1_proj/bn[0][0]']
+
+                 activation_73 (Activation)     (None, 14, 14, 1024  0           ['add_23[0][0]']
+                                                )
+
+                 conv4_2_1x1_reduce (Conv2D)    (None, 14, 14, 256)  262144      ['activation_73[0][0]']
+
+                 conv4_2_1x1_reduce/bn (BatchNo  (None, 14, 14, 256)  1024       ['conv4_2_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_74 (Activation)     (None, 14, 14, 256)  0           ['conv4_2_1x1_reduce/bn[0][0]']
+
+                 conv4_2_3x3 (Conv2D)           (None, 14, 14, 256)  589824      ['activation_74[0][0]']
+
+                 conv4_2_3x3/bn (BatchNormaliza  (None, 14, 14, 256)  1024       ['conv4_2_3x3[0][0]']
+                 tion)
+
+                 activation_75 (Activation)     (None, 14, 14, 256)  0           ['conv4_2_3x3/bn[0][0]']
+
+                 conv4_2_1x1_increase (Conv2D)  (None, 14, 14, 1024  262144      ['activation_75[0][0]']
+                                                )
+
+                 conv4_2_1x1_increase/bn (Batch  (None, 14, 14, 1024  4096       ['conv4_2_1x1_increase[0][0]']
+                 Normalization)                 )
+
+                 add_24 (Add)                   (None, 14, 14, 1024  0           ['conv4_2_1x1_increase/bn[0][0]',
+                                                )                                 'activation_73[0][0]']
+
+                 activation_76 (Activation)     (None, 14, 14, 1024  0           ['add_24[0][0]']
+                                                )
+
+                 conv4_3_1x1_reduce (Conv2D)    (None, 14, 14, 256)  262144      ['activation_76[0][0]']
+
+                 conv4_3_1x1_reduce/bn (BatchNo  (None, 14, 14, 256)  1024       ['conv4_3_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_77 (Activation)     (None, 14, 14, 256)  0           ['conv4_3_1x1_reduce/bn[0][0]']
+
+                 conv4_3_3x3 (Conv2D)           (None, 14, 14, 256)  589824      ['activation_77[0][0]']
+
+                 conv4_3_3x3/bn (BatchNormaliza  (None, 14, 14, 256)  1024       ['conv4_3_3x3[0][0]']
+                 tion)
+
+                 activation_78 (Activation)     (None, 14, 14, 256)  0           ['conv4_3_3x3/bn[0][0]']
+
+                 conv4_3_1x1_increase (Conv2D)  (None, 14, 14, 1024  262144      ['activation_78[0][0]']
+                                                )
+
+                 conv4_3_1x1_increase/bn (Batch  (None, 14, 14, 1024  4096       ['conv4_3_1x1_increase[0][0]']
+                 Normalization)                 )
+
+                 add_25 (Add)                   (None, 14, 14, 1024  0           ['conv4_3_1x1_increase/bn[0][0]',
+                                                )                                 'activation_76[0][0]']
+
+                 activation_79 (Activation)     (None, 14, 14, 1024  0           ['add_25[0][0]']
+                                                )
+
+                 conv4_4_1x1_reduce (Conv2D)    (None, 14, 14, 256)  262144      ['activation_79[0][0]']
+
+                 conv4_4_1x1_reduce/bn (BatchNo  (None, 14, 14, 256)  1024       ['conv4_4_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_80 (Activation)     (None, 14, 14, 256)  0           ['conv4_4_1x1_reduce/bn[0][0]']
+
+                 conv4_4_3x3 (Conv2D)           (None, 14, 14, 256)  589824      ['activation_80[0][0]']
+
+                 conv4_4_3x3/bn (BatchNormaliza  (None, 14, 14, 256)  1024       ['conv4_4_3x3[0][0]']
+                 tion)
+
+                 activation_81 (Activation)     (None, 14, 14, 256)  0           ['conv4_4_3x3/bn[0][0]']
+
+                 conv4_4_1x1_increase (Conv2D)  (None, 14, 14, 1024  262144      ['activation_81[0][0]']
+                                                )
+
+                 conv4_4_1x1_increase/bn (Batch  (None, 14, 14, 1024  4096       ['conv4_4_1x1_increase[0][0]']
+                 Normalization)                 )
+
+                 add_26 (Add)                   (None, 14, 14, 1024  0           ['conv4_4_1x1_increase/bn[0][0]',
+                                                )                                 'activation_79[0][0]']
+
+                 activation_82 (Activation)     (None, 14, 14, 1024  0           ['add_26[0][0]']
+                                                )
+
+                 conv4_5_1x1_reduce (Conv2D)    (None, 14, 14, 256)  262144      ['activation_82[0][0]']
+
+                 conv4_5_1x1_reduce/bn (BatchNo  (None, 14, 14, 256)  1024       ['conv4_5_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_83 (Activation)     (None, 14, 14, 256)  0           ['conv4_5_1x1_reduce/bn[0][0]']
+
+                 conv4_5_3x3 (Conv2D)           (None, 14, 14, 256)  589824      ['activation_83[0][0]']
+
+                 conv4_5_3x3/bn (BatchNormaliza  (None, 14, 14, 256)  1024       ['conv4_5_3x3[0][0]']
+                 tion)
+
+                 activation_84 (Activation)     (None, 14, 14, 256)  0           ['conv4_5_3x3/bn[0][0]']
+
+                 conv4_5_1x1_increase (Conv2D)  (None, 14, 14, 1024  262144      ['activation_84[0][0]']
+                                                )
+
+                 conv4_5_1x1_increase/bn (Batch  (None, 14, 14, 1024  4096       ['conv4_5_1x1_increase[0][0]']
+                 Normalization)                 )
+
+                 add_27 (Add)                   (None, 14, 14, 1024  0           ['conv4_5_1x1_increase/bn[0][0]',
+                                                )                                 'activation_82[0][0]']
+
+                 activation_85 (Activation)     (None, 14, 14, 1024  0           ['add_27[0][0]']
+                                                )
+
+                 conv4_6_1x1_reduce (Conv2D)    (None, 14, 14, 256)  262144      ['activation_85[0][0]']
+
+                 conv4_6_1x1_reduce/bn (BatchNo  (None, 14, 14, 256)  1024       ['conv4_6_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_86 (Activation)     (None, 14, 14, 256)  0           ['conv4_6_1x1_reduce/bn[0][0]']
+
+                 conv4_6_3x3 (Conv2D)           (None, 14, 14, 256)  589824      ['activation_86[0][0]']
+
+                 conv4_6_3x3/bn (BatchNormaliza  (None, 14, 14, 256)  1024       ['conv4_6_3x3[0][0]']
+                 tion)
+
+                 activation_87 (Activation)     (None, 14, 14, 256)  0           ['conv4_6_3x3/bn[0][0]']
+
+                 conv4_6_1x1_increase (Conv2D)  (None, 14, 14, 1024  262144      ['activation_87[0][0]']
+                                                )
+
+                 conv4_6_1x1_increase/bn (Batch  (None, 14, 14, 1024  4096       ['conv4_6_1x1_increase[0][0]']
+                 Normalization)                 )
+
+                 add_28 (Add)                   (None, 14, 14, 1024  0           ['conv4_6_1x1_increase/bn[0][0]',
+                                                )                                 'activation_85[0][0]']
+
+                 activation_88 (Activation)     (None, 14, 14, 1024  0           ['add_28[0][0]']
+                                                )
+
+                 conv5_1_1x1_reduce (Conv2D)    (None, 7, 7, 512)    524288      ['activation_88[0][0]']
+
+                 conv5_1_1x1_reduce/bn (BatchNo  (None, 7, 7, 512)   2048        ['conv5_1_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_89 (Activation)     (None, 7, 7, 512)    0           ['conv5_1_1x1_reduce/bn[0][0]']
+
+                 conv5_1_3x3 (Conv2D)           (None, 7, 7, 512)    2359296     ['activation_89[0][0]']
+
+                 conv5_1_3x3/bn (BatchNormaliza  (None, 7, 7, 512)   2048        ['conv5_1_3x3[0][0]']
+                 tion)
+
+                 activation_90 (Activation)     (None, 7, 7, 512)    0           ['conv5_1_3x3/bn[0][0]']
+
+                 conv5_1_1x1_increase (Conv2D)  (None, 7, 7, 2048)   1048576     ['activation_90[0][0]']
+
+                 conv5_1_1x1_proj (Conv2D)      (None, 7, 7, 2048)   2097152     ['activation_88[0][0]']
+
+                 conv5_1_1x1_increase/bn (Batch  (None, 7, 7, 2048)  8192        ['conv5_1_1x1_increase[0][0]']
+                 Normalization)
+
+                 conv5_1_1x1_proj/bn (BatchNorm  (None, 7, 7, 2048)  8192        ['conv5_1_1x1_proj[0][0]']
+                 alization)
+
+                 add_29 (Add)                   (None, 7, 7, 2048)   0           ['conv5_1_1x1_increase/bn[0][0]',
+                                                                                  'conv5_1_1x1_proj/bn[0][0]']
+
+                 activation_91 (Activation)     (None, 7, 7, 2048)   0           ['add_29[0][0]']
+
+                 conv5_2_1x1_reduce (Conv2D)    (None, 7, 7, 512)    1048576     ['activation_91[0][0]']
+
+                 conv5_2_1x1_reduce/bn (BatchNo  (None, 7, 7, 512)   2048        ['conv5_2_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_92 (Activation)     (None, 7, 7, 512)    0           ['conv5_2_1x1_reduce/bn[0][0]']
+
+                 conv5_2_3x3 (Conv2D)           (None, 7, 7, 512)    2359296     ['activation_92[0][0]']
+
+                 conv5_2_3x3/bn (BatchNormaliza  (None, 7, 7, 512)   2048        ['conv5_2_3x3[0][0]']
+                 tion)
+
+                 activation_93 (Activation)     (None, 7, 7, 512)    0           ['conv5_2_3x3/bn[0][0]']
+
+                 conv5_2_1x1_increase (Conv2D)  (None, 7, 7, 2048)   1048576     ['activation_93[0][0]']
+
+                 conv5_2_1x1_increase/bn (Batch  (None, 7, 7, 2048)  8192        ['conv5_2_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_30 (Add)                   (None, 7, 7, 2048)   0           ['conv5_2_1x1_increase/bn[0][0]',
+                                                                                  'activation_91[0][0]']
+
+                 activation_94 (Activation)     (None, 7, 7, 2048)   0           ['add_30[0][0]']
+
+                 conv5_3_1x1_reduce (Conv2D)    (None, 7, 7, 512)    1048576     ['activation_94[0][0]']
+
+                 conv5_3_1x1_reduce/bn (BatchNo  (None, 7, 7, 512)   2048        ['conv5_3_1x1_reduce[0][0]']
+                 rmalization)
+
+                 activation_95 (Activation)     (None, 7, 7, 512)    0           ['conv5_3_1x1_reduce/bn[0][0]']
+
+                 conv5_3_3x3 (Conv2D)           (None, 7, 7, 512)    2359296     ['activation_95[0][0]']
+
+                 conv5_3_3x3/bn (BatchNormaliza  (None, 7, 7, 512)   2048        ['conv5_3_3x3[0][0]']
+                 tion)
+
+                 activation_96 (Activation)     (None, 7, 7, 512)    0           ['conv5_3_3x3/bn[0][0]']
+
+                 conv5_3_1x1_increase (Conv2D)  (None, 7, 7, 2048)   1048576     ['activation_96[0][0]']
+
+                 conv5_3_1x1_increase/bn (Batch  (None, 7, 7, 2048)  8192        ['conv5_3_1x1_increase[0][0]']
+                 Normalization)
+
+                 add_31 (Add)                   (None, 7, 7, 2048)   0           ['conv5_3_1x1_increase/bn[0][0]',
+                                                                                  'activation_94[0][0]']
+
+                 activation_97 (Activation)     (None, 7, 7, 2048)   0           ['add_31[0][0]']
+
+                 avg_pool (AveragePooling2D)    (None, 1, 1, 2048)   0           ['activation_97[0][0]']
+
+                 global_average_pooling2d_1 (Gl  (None, 2048)        0           ['avg_pool[0][0]']
+                 obalAveragePooling2D)
+
+                 gaussian_noise_1 (GaussianNois  (None, 2048)        0           ['global_average_pooling2d_1[0][0
+                 e)                                                              ]']
+
+                 dense_x (Dense)                (None, 512)          1049088     ['gaussian_noise_1[0][0]']
+
+                 dropout_1 (Dropout)            (None, 512)          0           ['dense_x[0][0]']
+
+                 dense_1 (Dense)                (None, 7)            3591        ['dropout_1[0][0]']
+
+                ==================================================================================================
+                Total params: 24,613,831
+                Trainable params: 24,560,711
+                Non-trainable params: 53,120
+                __________________________________________________________________________________________________
+                --- Время выполнения: 2.222 сек. ---
+
+                True
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
-
-                pred._Prediction__load_av_model_b5(
-                    show_summary = True, out = []
+                video = Video()
+                video.load_video_model_deep_fe(
+                    show_summary = 1, out = True,
+                    runtime = True, run = True
                 )
 
             .. output-cell::
-                :execution-count: 3
+                :execution-count: 2
                 :linenos:
 
-                [2022-10-17 10:53:03] Неверные типы или значения аргументов в "Prediction.__load_av_model_b5" ...
+                [2022-11-01 12:21:23] Неверные типы или значения аргументов в "Video.load_video_model_deep_fe" ...
+
+                False
         """
 
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
+
         try:
             # Проверка аргументов
-            if type(show_summary) is not bool or type(out) is not bool:
-                raise TypeError
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                    not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__load_av_model_b5.__name__, out=out)
-            return None
+            self._inv_args(__class__.__name__, self.load_video_model_deep_fe.__name__, out = out)
+            return False
         else:
-            input_1 = tf.keras.Input(shape=(64,), name="input_1")
-            x = tf.keras.layers.Dense(units=1, name="dense_1")(input_1)
-            x = tf.keras.layers.Activation("sigmoid", name="activ_1")(x)
+            # Блокировка выполнения
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            model = tf.keras.Model(inputs=input_1, outputs=x)
+            if runtime: self._r_start()
 
-            if show_summary and out:
-                model.summary()
+            # Информационное сообщение
+            self._info(self._formation_video_deep_fe, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
-            return model
+            basis_model = VGGFace(
+                model = 'resnet50', include_top = False, input_shape = (224, 224, 3), pooling = 'avg', weights = None
+            )
 
-    # ------------------------------------------------------------------------------------------------------------------
-    # Внешние методы
-    # ------------------------------------------------------------------------------------------------------------------
+            gauss_noise = tf.keras.layers.GaussianNoise(0.1)(basis_model.output)
+            x = tf.keras.layers.Dense(
+                units = 512, kernel_regularizer = tf.keras.regularizers.l2(1e-4), activation = 'relu', name = 'dense_x'
+            )(gauss_noise)
+            x = tf.keras.layers.Dropout(0.5)(x)
+            x = tf.keras.layers.Dense(7, activation = 'softmax')(x)
+
+            self._video_model_deep_fe = tf.keras.Model(basis_model.input, x)
+
+            if show_summary and out: self._video_model_deep_fe.summary()
+
+            if runtime: self._r_end(out = out)
+
+            return True
 
-    def load_av_models_b5(
+    def load_video_model_nn(
         self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
-        """Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств
+        """Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам
 
         Args:
-            show_summary (bool): Отображение последней сформированной нейросетевой архитектуры моделей
+            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если нейросетевые архитектуры модели сформированы, в обратном случае **False**
+            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 1
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
-
-                pred.load_av_models_b5(
+                video = Video()
+                video.load_video_model_nn(
                     show_summary = True, out = True,
                     runtime = True, run = True
                 )
 
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
-                [2022-12-08 15:19:30] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
+                [2022-10-27 14:46:11] Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам (видео модальность) ...
 
-                Model: "model_4"
+                Model: "model"
                 _________________________________________________________________
                  Layer (type)                Output Shape              Param #
                 =================================================================
-                 input_1 (InputLayer)        [(None, 64)]              0
+                 input_1 (InputLayer)        [(None, 10, 512)]         0
 
-                 dense_1 (Dense)             (None, 1)                 65
+                 lstm (LSTM)                 (None, 1024)              6295552
 
-                 activ_1 (Activation)        (None, 1)                 0
+                 dropout (Dropout)           (None, 1024)              0
+
+                 dense (Dense)               (None, 5)                 5125
+
+                 activation (Activation)     (None, 5)                 0
 
                 =================================================================
-                Total params: 65
-                Trainable params: 65
+                Total params: 6,300,677
+                Trainable params: 6,300,677
                 Non-trainable params: 0
                 _________________________________________________________________
-                --- Время выполнения: 0.141 сек. ---
+                --- Время выполнения: 2.018 сек. ---
 
                 True
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
-
-                pred = Prediction()
+                from oceanai.modules.lab.video import Video
 
-                pred.load_av_models_b5(
+                video = Video()
+                video.load_video_model_nn(
                     show_summary = 1, out = True,
                     runtime = True, run = True
                 )
 
             .. output-cell::
                 :execution-count: 2
                 :linenos:
 
-                [2022-12-08 15:20:36] Неверные типы или значения аргументов в "Prediction.load_av_models_b5" ...
+                [2022-10-27 14:47:22] Неверные типы или значения аргументов в "Video.load_video_model_nn" ...
 
                 False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.load_av_models_b5.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_video_model_nn.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(self._formation_av_models_b5, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            self._info(self._formation_video_model_nn, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
+
+            input_lstm = tf.keras.Input(shape = (10, 512))
 
-            for key, _ in self._av_models_b5.items():
-                self._av_models_b5[key] = self.__load_av_model_b5()
+            x = tf.keras.layers.LSTM(
+                1024, return_sequences = False,
+                kernel_regularizer = tf.keras.regularizers.l2(1e-3)
+            )(input_lstm)
+            x = tf.keras.layers.Dropout(rate = 0.2)(x)
+            x = tf.keras.layers.Dense(units = 5)(x)
+            x = tf.keras.layers.Activation('linear')(x)
 
-            if show_summary and out:
-                self._av_models_b5[key].summary()
+            self._video_model_nn = tf.keras.Model(inputs = input_lstm, outputs = x)
 
-            if runtime:
-                self._r_end(out=out)
+            if show_summary and out: self._video_model_nn.summary()
+
+            if runtime: self._r_end(out = out)
 
             return True
 
-    def load_avt_model_b5(
+    def load_video_models_b5(
         self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
-        """Формирование нейросетевой архитектуры модели для получения оценок персональных качеств
+        """Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств
 
         Args:
             show_summary (bool): Отображение последней сформированной нейросетевой архитектуры моделей
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
+            bool: **True** если нейросетевые архитектуры модели сформированы, в обратном случае **False**
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+                video.load_video_models_b5(
+                    show_summary = True, out = True,
+                    runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-11-04 15:29:26] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (видео модальность) ...
+
+                Model: "model_4"
+                _________________________________________________________________
+                 Layer (type)                Output Shape              Param #
+                =================================================================
+                 input_1 (InputLayer)        [(None, 32)]              0
+
+                 dense_1 (Dense)             (None, 1)                 33
+
+                 activ_1 (Activation)        (None, 1)                 0
+
+                =================================================================
+                Total params: 33
+                Trainable params: 33
+                Non-trainable params: 0
+                _________________________________________________________________
+                --- Время выполнения: 0.116 сек. ---
+
+                True
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+                video.load_video_models_b5(
+                    show_summary = 1, out = True,
+                    runtime = True, run = True
+                )
+
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+
+                [2022-11-04 15:30:15] Неверные типы или значения аргументов в "Video.load_video_models_b5" ...
+
+                False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.load_avt_model_b5.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_video_models_b5.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(self._formation_avt_model_b5, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            self._info(self._formation_video_models_b5, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
-            self._avt_model_b5 = self.__load_avt_model_b5()
+            for key, _ in self._video_models_b5.items():
+                self._video_models_b5[key] = self.__load_video_model_b5()
 
-            if show_summary and out:
-                self._avt_model_b5.summary()
+            if show_summary and out: self._video_models_b5[key].summary()
 
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
             return True
 
-    def load_av_models_weights_b5(
-        self,
-        url_openness: str,
-        url_conscientiousness: str,
-        url_extraversion: str,
-        url_agreeableness: str,
-        url_non_neuroticism: str,
-        force_reload: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+    def load_video_model_weights_hc(
+        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
-        """Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств
+        """Загрузка весов нейросетевой модели для получения оценок по экспертным признакам
 
         Args:
-            url_openness (str): Полный путь к файлу с весами нейросетевой модели (открытость опыту)
-            url_conscientiousness (str): Полный путь к файлу с весами нейросетевой модели (добросовестность)
-            url_extraversion (str): Полный путь к файлу с весами нейросетевой модели (экстраверсия)
-            url_agreeableness (str): Полный путь к файлу с весами нейросетевой модели (доброжелательность)
-            url_non_neuroticism (str): Полный путь к файлу с весами нейросетевой модели ('эмоциональная стабильность')
-            force_reload (bool): Принудительная загрузка файлов с весами нейросетевых моделей из сети
+            url (str): Полный путь к файлу с весами нейросетевой модели
+            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если веса нейросетевых моделей загружены, в обратном случае **False**
+            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
 
         .. dropdown:: Примеры
             :class-body: sd-pr-5
 
             :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 1
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
-                pred.load_av_models_b5(
+                video.load_video_model_hc(
                     show_summary = False, out = True,
                     runtime = True, run = True
                 )
 
             .. output-cell::
                 :execution-count: 1
                 :linenos:
 
-                [2022-12-08 16:56:37] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
+                [2022-10-27 12:55:31] Формирование нейросетевой архитектуры модели для получения оценок по экспертным признакам (видео модальность) ...
 
-                --- Время выполнения: 0.075 сек. ---
+                --- Время выполнения: 0.606 сек. ---
 
                 True
 
             .. code-cell:: python
                 :execution-count: 2
                 :linenos:
                 :tab-width: 8
 
-                pred.path_to_save_ = './models'
-                pred.chunk_size_ = 2000000
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
 
-                url_openness = pred.weights_for_big5_['av']['b5']['openness']['sberdisk']
-                url_conscientiousness = pred.weights_for_big5_['av']['b5']['conscientiousness']['sberdisk']
-                url_extraversion = pred.weights_for_big5_['av']['b5']['extraversion']['sberdisk']
-                url_agreeableness = pred.weights_for_big5_['av']['b5']['agreeableness']['sberdisk']
-                url_non_neuroticism = pred.weights_for_big5_['av']['b5']['non_neuroticism']['sberdisk']
+                url = video.weights_for_big5_['video']['hc']['sberdisk']
 
-                pred.load_av_models_weights_b5(
-                    url_openness = url_openness,
-                    url_conscientiousness = url_conscientiousness,
-                    url_extraversion = url_extraversion,
-                    url_agreeableness = url_agreeableness,
-                    url_non_neuroticism = url_non_neuroticism,
+                video.load_video_model_weights_hc(
+                    url = url,
                     force_reload = True,
                     out = True,
                     runtime = True,
                     run = True
                 )
 
             .. output-cell::
                 :execution-count: 2
                 :linenos:
 
-                [2022-12-08 17:03:18] Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
-
-                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-14-35.h5" (100.0%) ... Открытость опыту
+                [2022-10-27 13:08:04] Загрузка весов нейросетевой модели для получения оценок по экспертным признакам (видео модальность) ...
 
-                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-08-10.h5" (100.0%) ... Добросовестность
+                [2022-10-27 13:08:05] Загрузка файла "weights_2022-08-27_18-53-35.h5" (100.0%) ...
 
-                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-17-57.h5" (100.0%) ... Экстраверсия
-
-                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-25-11.h5" (100.0%) ... Доброжелательность
-
-                [2022-12-08 17:03:21] Загрузка файла "weights_2022-06-14_21-44-09.h5" (100.0%) ... Эмоциональная стабильность
-
-                --- Время выполнения: 3.399 сек. ---
+                --- Время выполнения: 0.493 сек. ---
 
                 True
 
             :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
             .. code-cell:: python
                 :execution-count: 3
                 :linenos:
                 :tab-width: 8
 
-                from oceanai.modules.lab.prediction import Prediction
+                from oceanai.modules.lab.video import Video
 
-                pred = Prediction()
+                video = Video()
 
-                pred.path_to_save_ = './models'
-                pred.chunk_size_ = 2000000
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
 
-                url_openness = pred.weights_for_big5_['av']['b5']['openness']['sberdisk']
-                url_conscientiousness = pred.weights_for_big5_['av']['b5']['conscientiousness']['sberdisk']
-                url_extraversion = pred.weights_for_big5_['av']['b5']['extraversion']['sberdisk']
-                url_agreeableness = pred.weights_for_big5_['av']['b5']['agreeableness']['sberdisk']
-                url_non_neuroticism = pred.weights_for_big5_['av']['b5']['non_neuroticism']['sberdisk']
+                url = video.weights_for_big5_['video']['hc']['sberdisk']
 
-                pred.load_av_models_weights_b5(
-                    url_openness = url_openness,
-                    url_conscientiousness = url_conscientiousness,
-                    url_extraversion = url_extraversion,
-                    url_agreeableness = url_agreeableness,
-                    url_non_neuroticism = url_non_neuroticism,
+                video.load_video_model_weights_hc(
+                    url = url,
                     force_reload = True,
                     out = True,
                     runtime = True,
                     run = True
                 )
 
             .. output-cell::
                 :execution-count: 3
                 :linenos:
 
-                [2022-12-08 17:05:32] Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
+                [2022-10-27 13:09:54] Загрузка весов нейросетевой модели для получения оценок по экспертным признакам (видео модальность) ...
 
-                [2022-12-08 17:05:32] Загрузка файла "weights_2022-08-28_11-14-35.h5" (100.0%) ...
+                [2022-10-27 13:09:54] Загрузка файла "weights_2022-08-27_18-53-35.h5" (100.0%) ...
 
-                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Открытость опыту
+                [2022-10-27 13:09:54] Ой! Что-то пошло не так ... нейросетевая архитектура модели для получения оценок по экспертным признакам не сформирована (видео модальность) ...
 
-                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
-                    Линия: 639
-                    Метод: load_av_models_weights_b5
-                    Тип ошибки: AttributeError
+                --- Время выполнения: 0.424 сек. ---
 
-                [2022-12-08 17:05:33] Загрузка файла "weights_2022-08-28_11-08-10.h5" (100.0%) ...
+                False
+        """
 
-                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Добросовестность
+        if runtime: self._r_start()
 
-                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
-                    Линия: 639
-                    Метод: load_av_models_weights_b5
-                    Тип ошибки: AttributeError
+        if self.__load_model_weights(url, force_reload, self._load_video_model_weights_hc, out, False, run) is True:
+            try: self._video_model_hc.load_weights(self._url_last_filename)
+            except Exception: self._error(self._model_video_hc_not_formation, out = out); return False
+            else: return True
+            finally:
+                if runtime: self._r_end(out = out)
 
-                [2022-12-08 17:05:33] Загрузка файла "weights_2022-08-28_11-17-57.h5" (100.0%) ...
+        return False
 
-                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Экстраверсия
+    def load_video_model_weights_deep_fe(
+        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
+    ) -> bool:
+        """Загрузка весов нейросетевой модели для получения нейросетевых признаков
 
-                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
-                    Линия: 639
-                    Метод: load_av_models_weights_b5
-                    Тип ошибки: AttributeError
+        Args:
+            url (str): Полный путь к файлу с весами нейросетевой модели
+            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
+            out (bool): Отображение
+            runtime (bool): Подсчет времени выполнения
+            run (bool): Блокировка выполнения
 
-                [2022-12-08 17:05:33] Загрузка файла "weights_2022-08-28_11-25-11.h5" (100.0%) ...
+        Returns:
+            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
 
-                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Доброжелательность
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
-                    Линия: 639
-                    Метод: load_av_models_weights_b5
-                    Тип ошибки: AttributeError
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-                [2022-12-08 17:05:33] Загрузка файла "weights_2022-06-14_21-44-09.h5" (100.0%) ...
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Эмоциональная стабильность
+                from oceanai.modules.lab.video import Video
 
-                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
-                    Линия: 639
-                    Метод: load_av_models_weights_b5
-                    Тип ошибки: AttributeError
+                video = Video()
 
-                --- Время выполнения: 1.024 сек. ---
+                video.load_video_model_deep_fe(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
 
-                False
-        """
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+                [2022-11-01 12:41:59] Формирование нейросетевой архитектуры для получения нейросетевых признаков (видео модальность) ...
 
-        try:
-            # Проверка аргументов
-            if (
-                type(url_openness) is not str
-                or not url_openness
-                or type(url_conscientiousness) is not str
-                or not url_conscientiousness
-                or type(url_extraversion) is not str
-                or not url_extraversion
-                or type(url_agreeableness) is not str
-                or not url_agreeableness
-                or type(url_non_neuroticism) is not str
-                or not url_non_neuroticism
-                or type(force_reload) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.load_av_models_weights_b5.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+                --- Время выполнения: 1.306 сек. ---
 
-            if runtime:
-                self._r_start()
+                True
 
-            result_download_models = 0  # Все веса нейросетевых моделей по умолчанию загружены
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
 
-            # Информационное сообщение
-            self._info(self._load_av_models_weights_b5, last=False, out=out)
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
 
-            # Проход по всем URL с весами нейросетевых моделей
-            for cnt, url in enumerate(
-                [
-                    (url_openness, self._b5["ru"][0]),
-                    (url_conscientiousness, self._b5["ru"][1]),
-                    (url_extraversion, self._b5["ru"][2]),
-                    (url_agreeableness, self._b5["ru"][3]),
-                    (url_non_neuroticism, self._b5["ru"][4]),
-                ]
-            ):
-                sections = urlparse(url[0])  # Парсинг URL адреса
+                url = video.weights_for_big5_['video']['fe']['sberdisk']
 
-                try:
-                    # URL файл невалидный
-                    if sections.scheme == "":
-                        raise requests.exceptions.InvalidURL
-                except requests.exceptions.InvalidURL:
-                    url_norm = os.path.normpath(url[0])
+                video.load_video_model_weights_deep_fe(
+                    url = url,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
 
-                    try:
-                        if os.path.isfile(url_norm) is False:
-                            raise FileNotFoundError  # Не файл
-                    except FileNotFoundError:
-                        self._other_error(
-                            self._load_model_weights_error + " " + self._bold_wrapper(url[1].capitalize()), out=out
-                        )
-                        continue
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        continue
-                    else:
-                        self._url_last_filename = url_norm
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
 
-                        # Отображение истории вывода сообщений в ячейке Jupyter
-                        if out:
-                            self.show_notebook_history_output()
-                else:
-                    try:
-                        if force_reload is False:
-                            clear_output(True)
-                        # Загрузка файла из URL
-                        res_download_file_from_url = self._download_file_from_url(
-                            url=url[0], force_reload=force_reload, runtime=False, out=out, run=True
-                        )
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        continue
-                    else:
-                        # Файл загружен
-                        if res_download_file_from_url != 200:
-                            continue
+                [2022-11-01 12:42:51] Загрузка весов нейросетевой модели для получения нейросетевых признаков (видео модальность) ...
 
-                        try:
-                            self._av_models_b5[self._b5["en"][cnt]].load_weights(self._url_last_filename)
-                        except Exception:
-                            self._other_error(
-                                self._load_model_weights_error + " " + self._bold_wrapper(url[1].capitalize()), out=out
-                            )
-                            continue
-                        else:
-                            self._add_last_el_notebook_history_output(self._bold_wrapper(url[1].capitalize()))
+                [2022-11-01 12:43:06] Загрузка файла "weights_2022-11-01_12-27-07.h5" (100.0%) ...
 
-                            result_download_models += 1
+                --- Время выполнения: 14.781 сек. ---
 
-            clear_output(True)
-            # Отображение истории вывода сообщений в ячейке Jupyter
-            if out:
-                self.show_notebook_history_output()
+                True
 
-            if runtime:
-                self._r_end(out=out)
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-            if result_download_models != len(self._b5["ru"]):
-                return False
-            return True
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+                :tab-width: 8
+
+                from oceanai.modules.lab.video import Video
+
+                video = Video()
+
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
+
+                url = video.weights_for_big5_['video']['fe']['sberdisk']
+
+                video.load_video_model_weights_deep_fe(
+                    url = url,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
+
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-11-01 12:44:14] Загрузка весов нейросетевой модели для получения нейросетевых признаков (видео модальность) ...
 
-    def get_av_union_predictions(
-        self,
-        depth: int = 1,
-        recursive: bool = False,
-        sr: int = 44100,
-        window_audio: Union[int, float] = 2.0,
-        step_audio: Union[int, float] = 1.0,
-        reduction_fps: int = 5,
-        window_video: int = 10,
-        step_video: int = 5,
-        lang: str = "ru",
-        accuracy: bool = True,
-        url_accuracy: str = "",
-        logs: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+                [2022-11-01 12:44:28] Загрузка файла "weights_2022-11-01_12-27-07.h5" (100.0%) ...
+
+                [2022-11-01 12:44:28] Ой! Что-то пошло не так ... нейросетевая архитектура модели для получения нейросетевых признаков не сформирована (видео модальность) ...
+
+                --- Время выполнения: 13.926 сек. ---
+
+                False
+        """
+
+        if runtime: self._r_start()
+
+        if self.__load_model_weights(
+            url, force_reload, self._load_video_model_weights_deep_fe, out, False, run
+        ) is True:
+            try:
+                self._video_model_deep_fe.load_weights(self._url_last_filename)
+                self._video_model_deep_fe = tf.keras.Model(
+                    inputs = self._video_model_deep_fe.input,
+                    outputs = [self._video_model_deep_fe.get_layer('dense_x').output]
+                )
+            except Exception: self._error(self._model_video_deep_fe_not_formation, out = out); return False
+            else: return True
+            finally:
+                if runtime: self._r_end(out = out)
+
+        return False
+
+    def load_video_model_weights_nn(
+        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
-        """Получения прогнозов по аудио и видео (мультимодальное объединение)
+        """Загрузка весов нейросетевой модели для получения оценок по нейросетевым признакам
 
         Args:
-            depth (int): Глубина иерархии для получения данных
-            recursive (bool): Рекурсивный поиск данных
-            sr (int): Частота дискретизации
-            window_audio (Union[int, float]): Размер окна сегмента аудио сигнала (в секундах)
-            step_audio (Union[int, float]): Шаг сдвига окна сегмента аудио сигнала (в секундах)
-            reduction_fps (int): Понижение кадровой частоты
-            window_video (int): Размер окна сегмента видео сигнала (в кадрах)
-            step_video (int): Шаг сдвига окна сегмента видео сигнала (в кадрах)
-            lang (str): Язык
-            accuracy (bool): Вычисление точности
-            url_accuracy (str): Полный путь к файлу с верными предсказаниями для подсчета точности
-            logs (bool): При необходимости формировать LOG файл
+            url (str): Полный путь к файлу с весами нейросетевой модели
+            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если прогнозы успешно получены, в обратном случае **False**
+            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
 
-        :bdg-link-light:`Пример <../../user_guide/notebooks/Prediction-get_av_union_predictions.ipynb>`
-        """
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-        # Сброс
-        self._df_files = pd.DataFrame()  # Пустой DataFrame с данными
-        self._df_accuracy = pd.DataFrame()  # Пустой DataFrame с результатами вычисления точности
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-        try:
-            # Проверка аргументов
-            if (
-                type(depth) is not int
-                or depth < 1
-                or type(recursive) is not bool
-                or type(sr) is not int
-                or sr < 1
-                or (
-                    (type(window_audio) is not int or window_audio < 1)
-                    and (type(window_audio) is not float or window_audio <= 0)
-                )
-                or (
-                    (type(step_audio) is not int or step_audio < 1)
-                    and (type(step_audio) is not float or step_audio <= 0)
-                )
-                or type(reduction_fps) is not int
-                or reduction_fps < 1
-                or type(window_video) is not int
-                or window_video < 1
-                or type(step_video) is not int
-                or step_video < 1
-                or not isinstance(lang, str)
-                or lang not in self.lang_traslate
-                or type(accuracy) is not bool
-                or type(url_accuracy) is not str
-                or type(logs) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.get_av_union_predictions.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+                from oceanai.modules.lab.video import Video
 
-            if runtime:
-                self._r_start()
+                video = Video()
 
-            try:
-                # Получение директорий, где хранятся данные
-                path_to_data = self._get_paths(self.path_to_dataset_, depth, out=out)
-                if type(path_to_data) is bool:
-                    return False
+                video.load_video_model_nn(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
 
-                if type(self.keys_dataset_) is not list:
-                    raise TypeError
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
 
-                # Словарь для DataFrame набора данных с данными
-                self._dict_of_files = dict(zip(self.keys_dataset_, [[] for _ in range(0, len(self.keys_dataset_))]))
-                # Словарь для DataFrame набора данных с результатами вычисления точности
-                self._dict_of_accuracy = dict(
-                    zip(self.keys_dataset_[1:], [[] for _ in range(0, len(self.keys_dataset_[1:]))])
+                [2022-10-27 15:17:13] Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам (видео модальность) ...
+
+                --- Время выполнения: 1.991 сек. ---
+
+                True
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
+
+                url = video.weights_for_big5_['video']['nn']['sberdisk']
+
+                video.load_video_model_weights_nn(
+                    url = url,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
                 )
-            except (TypeError, FileNotFoundError):
-                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out=out)
-                return False
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return False
-            else:
-                # Вычисление точности
-                if accuracy is True:
-                    get_av_union_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
-                else:
-                    get_av_union_predictions_info = self._get_union_predictions_info
 
-                get_av_union_predictions_info += self._av_modality
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
 
-                # Вычисление точности
-                if accuracy is True:
-                    # Информационное сообщение
-                    self._info(get_av_union_predictions_info, out=out)
+                [2022-10-27 15:19:08] Загрузка весов нейросетевой модели для получения оценок по нейросетевым признакам (видео модальность) ...
 
-                    if not url_accuracy:
-                        url_accuracy = self._true_traits["sberdisk"]
+                [2022-10-27 15:19:11] Загрузка файла "weights_2022-03-22_16-31-48.h5" (100.0%) ...
 
-                    try:
-                        # Загрузка верных предсказаний
-                        data_true_traits = pd.read_csv(url_accuracy)
-                    except (FileNotFoundError, URLError, UnicodeDecodeError):
-                        self._other_error(self._load_data_true_traits_error, out=out)
-                        return False
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return False
-                    else:
-                        true_traits = []
-                        self._del_last_el_notebook_history_output()
+                --- Время выполнения: 3.423 сек. ---
 
-                paths = []  # Пути до искомых файлов
+                True
 
-                # Проход по всем директориям
-                for curr_path in path_to_data:
-                    empty = True  # По умолчанию директория пустая
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-                    # Рекурсивный поиск данных
-                    if recursive is True:
-                        g = Path(curr_path).rglob("*")
-                    else:
-                        g = Path(curr_path).glob("*")
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+                :tab-width: 8
 
-                    # Формирование словаря для DataFrame
-                    for p in g:
-                        try:
-                            if type(self.ext_) is not list or len(self.ext_) < 1:
-                                raise TypeError
+                from oceanai.modules.lab.video import Video
 
-                            self.ext_ = [x.lower() for x in self.ext_]
-                        except TypeError:
-                            self._other_error(self._wrong_ext, out=out)
-                            return False
-                        except Exception:
-                            self._other_error(self._unknown_err, out=out)
-                            return False
-                        else:
-                            # Расширение файла соответствует расширению искомых файлов
-                            if p.suffix.lower() in self.ext_:
-                                if empty is True:
-                                    empty = False  # Каталог не пустой
+                video = Video()
 
-                                paths.append(p.resolve())
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
 
-                try:
-                    self.__len_paths = len(paths)  # Количество искомых файлов
+                url = video.weights_for_big5_['video']['nn']['sberdisk']
 
-                    if self.__len_paths == 0:
-                        raise TypeError
-                except TypeError:
-                    self._other_error(self._files_not_found, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    # Локальный путь
-                    self.__local_path = lambda path: os.path.join(
-                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))) :]
-                    )
+                video.load_video_model_weights_nn(
+                    url = url,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
 
-                    last = False  # Замена последнего сообщения
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
 
-                    # Проход по всем искомым файлов
-                    for i, curr_path in enumerate(paths):
-                        if i != 0:
-                            last = True
+                [2022-10-27 15:19:40] Загрузка весов нейросетевой модели для получения оценок по нейросетевым признакам (видео модальность) ...
 
-                        # Индикатор выполнения
-                        self._progressbar_union_predictions(
-                            get_av_union_predictions_info,
-                            i,
-                            self.__local_path(curr_path),
-                            self.__len_paths,
-                            True,
-                            last,
-                            out,
-                        )
+                [2022-10-27 15:19:43] Загрузка файла "weights_2022-03-22_16-31-48.h5" (100.0%) ...
 
-                        # Извлечение признаков из акустического сигнала
-                        hc_audio_features, melspectrogram_audio_features = self._get_acoustic_features(
-                            path=str(curr_path.resolve()),
-                            sr=sr,
-                            window=window_audio,
-                            step=step_audio,
-                            last=True,
-                            out=False,
-                            runtime=False,
-                            run=run,
-                        )
+                [2022-10-27 15:19:43] Ой! Что-то пошло не так ... нейросетевая архитектура модели для получения оценок по нейросетевым признакам не сформирована (видео модальность) ...
 
-                        # Извлечение признаков из визуального сигнала
-                        hc_video_features, nn_video_features = self._get_visual_features(
-                            path=str(curr_path.resolve()),
-                            reduction_fps=reduction_fps,
-                            window=window_video,
-                            step=step_video,
-                            lang=lang,
-                            last=True,
-                            out=False,
-                            runtime=False,
-                            run=run,
-                        )
+                --- Время выполнения: 3.469 сек. ---
 
-                        # Признаки из акустического сигнала извлечены
-                        if (
-                            type(hc_audio_features) is list
-                            and type(melspectrogram_audio_features) is list
-                            and type(hc_video_features) is np.ndarray
-                            and type(nn_video_features) is np.ndarray
-                            and len(hc_audio_features) > 0
-                            and len(melspectrogram_audio_features) > 0
-                            and len(hc_video_features) > 0
-                            and len(nn_video_features) > 0
-                        ):
-                            # Коды ошибок нейросетевых моделей (аудио модальность)
-                            code_error_pred_hc_audio = -1
-                            code_error_pred_melspectrogram_audio = -1
+                False
+        """
 
-                            try:
-                                # Оправка экспертных признаков в нейросетевую модель
-                                pred_hc_audio, _ = self.audio_model_hc_(np.array(hc_audio_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_hc_audio = 1
-                            except Exception:
-                                code_error_pred_melspectrogram_audio = 2
+        if runtime: self._r_start()
 
-                            try:
-                                # Отправка нейросетевых признаков в нейросетевую модель
-                                pred_melspectrogram_audio, _ = self.audio_model_nn_(
-                                    np.array(melspectrogram_audio_features, dtype=np.float16)
-                                )
-                            except TypeError:
-                                code_error_pred_melspectrogram_audio = 1
-                            except Exception:
-                                code_error_pred_melspectrogram_audio = 2
+        if self.__load_model_weights(url, force_reload, self._load_video_model_weights_nn, out, False, run) is True:
+            try: self._video_model_nn.load_weights(self._url_last_filename)
+            except Exception: self._error(self._model_video_nn_not_formation, out = out); return False
+            else: return True
+            finally:
+                if runtime: self._r_end(out = out)
 
-                            if code_error_pred_hc_audio != -1 and code_error_pred_melspectrogram_audio != -1:
-                                self._error(self._models_audio_not_formation, out=out)
-                                return False
+        return False
 
-                            if code_error_pred_hc_audio != -1:
-                                self._error(self._model_audio_hc_not_formation, out=out)
-                                return False
+    def load_video_models_weights_b5(
+        self, url_openness: str, url_conscientiousness: str, url_extraversion: str, url_agreeableness: str,
+        url_neuroticism: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
+    ) -> bool:
+        """Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств
 
-                            if code_error_pred_melspectrogram_audio != -1:
-                                self._error(self._model_audio_nn_not_formation, out=out)
-                                return False
+        Args:
+            url_openness (str): Полный путь к файлу с весами нейросетевой модели (открытость опыту)
+            url_conscientiousness (str): Полный путь к файлу с весами нейросетевой модели (добросовестность)
+            url_extraversion (str): Полный путь к файлу с весами нейросетевой модели (экстраверсия)
+            url_agreeableness (str): Полный путь к файлу с весами нейросетевой модели (доброжелательность)
+            url_neuroticism (str): Полный путь к файлу с весами нейросетевой модели (нейротизм)
+            force_reload (bool): Принудительная загрузка файлов с весами нейросетевых моделей из сети
+            out (bool): Отображение
+            runtime (bool): Подсчет времени выполнения
+            run (bool): Блокировка выполнения
 
-                            # Коды ошибок нейросетевых моделей (видео модальность)
-                            code_error_pred_hc_video = -1
-                            code_error_pred_nn_video = -1
+        Returns:
+            bool: **True** если веса нейросетевых моделей загружены, в обратном случае **False**
 
-                            try:
-                                # Оправка экспертных признаков в нейросетевую модель
-                                pred_hc_video, _ = self.video_model_hc_(np.array(hc_video_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_hc_video = 1
-                            except Exception:
-                                code_error_pred_hc_video = 2
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-                            try:
-                                # Отправка нейросетевых признаков в нейросетевую модель
-                                pred_nn_video, _ = self.video_model_nn_(np.array(nn_video_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_nn_video = 1
-                            except Exception:
-                                code_error_pred_nn_video = 2
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-                            if code_error_pred_hc_video != -1 and code_error_pred_nn_video != -1:
-                                self._error(self._models_video_not_formation, out=out)
-                                return False
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-                            if code_error_pred_hc_video != -1:
-                                self._error(self._model_video_hc_not_formation, out=out)
-                                return False
+                from oceanai.modules.lab.video import Video
 
-                            if code_error_pred_nn_video != -1:
-                                self._error(self._model_video_nn_not_formation, out=out)
-                                return False
+                video = Video()
 
-                            # Конкатенация оценок по экспертным и нейросетевым признакам
-                            union_pred = self.__concat_pred_av(
-                                pred_hc_audio.numpy(),
-                                pred_melspectrogram_audio.numpy(),
-                                pred_hc_video.numpy(),
-                                pred_nn_video.numpy(),
-                                out=out,
-                            )
+                video.load_video_models_b5(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
 
-                            if len(union_pred) == 0:
-                                return False
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
 
-                            final_pred = []
+                [2022-11-04 18:56:41] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (видео модальность) ...
 
-                            for cnt, (name_b5, model) in enumerate(self.av_models_b5_.items()):
-                                result = model(np.expand_dims(union_pred[cnt], axis=0)).numpy()[0][0]
+                --- Время выполнения: 0.117 сек. ---
 
-                                final_pred.append(result)
+                True
 
-                            # Добавление данных в словарь для DataFrame
-                            if self._append_to_list_of_files(str(curr_path.resolve()), final_pred, out) is False:
-                                return False
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
 
-                            # Вычисление точности
-                            if accuracy is True:
-                                try:
-                                    true_trait = (
-                                        data_true_traits[data_true_traits.NAME_VIDEO == curr_path.name][
-                                            list(self._b5["en"])
-                                        ]
-                                        .values[0]
-                                        .tolist()
-                                    )
-                                except IndexError:
-                                    self._other_error(self._expert_values_not_found, out=out)
-                                    return False
-                                except Exception:
-                                    self._other_error(self._unknown_err, out=out)
-                                    return False
-                                else:
-                                    true_traits.append(true_trait)
-                        else:
-                            # Добавление данных в словарь для DataFrame
-                            if (
-                                self._append_to_list_of_files(
-                                    str(curr_path.resolve()), [None] * len(self._b5["en"]), out
-                                )
-                                is False
-                            ):
-                                return False
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
 
-                            self._del_last_el_notebook_history_output()
+                url_openness = video.weights_for_big5_['video']['b5']['openness']['sberdisk']
+                url_conscientiousness = video.weights_for_big5_['video']['b5']['conscientiousness']['sberdisk']
+                url_extraversion = video.weights_for_big5_['video']['b5']['extraversion']['sberdisk']
+                url_agreeableness = video.weights_for_big5_['video']['b5']['agreeableness']['sberdisk']
+                url_neuroticism = video.weights_for_big5_['video']['b5']['neuroticism']['sberdisk']
 
-                    # Индикатор выполнения
-                    self._progressbar_union_predictions(
-                        get_av_union_predictions_info,
-                        self.__len_paths,
-                        self.__local_path(paths[-1]),
-                        self.__len_paths,
-                        True,
-                        last,
-                        out,
-                    )
+                video.load_video_models_weights_b5(
+                    url_openness = url_openness,
+                    url_conscientiousness = url_conscientiousness,
+                    url_extraversion = url_extraversion,
+                    url_agreeableness = url_agreeableness,
+                    url_neuroticism = url_neuroticism,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
 
-                    # Отображение в DataFrame с данными
-                    self._df_files = pd.DataFrame.from_dict(data=self._dict_of_files, orient="index").transpose()
-                    self._df_files.index.name = self._keys_id
-                    self._df_files.index += 1
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
 
-                    self._df_files.index = self._df_files.index.map(str)
+                [2022-11-04 18:58:59] Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств (видео модальность) ...
 
-                    self._df_files.Path = [os.path.basename(i) for i in self._df_files.Path]
+                [2022-11-04 18:59:00] Загрузка файла "weights_2022-06-15_16-46-30.h5" (100.0%) ... Открытость опыту
 
-                    # Отображение
-                    if out is True:
-                        self._add_notebook_history_output(self._df_files.iloc[0 : self.num_to_df_display_, :])
+                [2022-11-04 18:59:00] Загрузка файла "weights_2022-06-15_16-48-50.h5" (100.0%) ... Добросовестность
 
-                    # Подсчет точности
-                    if accuracy is True:
-                        mae_curr = []
+                [2022-11-04 18:59:00] Загрузка файла "weights_2022-06-15_16-54-06.h5" (100.0%) ... Экстраверсия
 
-                        for cnt, name_b5 in enumerate(self._df_files.keys().tolist()[1:]):
-                            try:
-                                mae_curr.append(
-                                    mean_absolute_error(
-                                        np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list()
-                                    )
-                                )
-                            except IndexError:
-                                continue
-                            except Exception:
-                                continue
+                [2022-11-04 18:59:01] Загрузка файла "weights_2022-06-15_17-02-03.h5" (100.0%) ... Доброжелательность
 
-                        mae_curr = [round(float(i), 4) for i in mae_curr]
-                        mae_mean = round(float(np.mean(mae_curr)), 4)
-                        accuracy_curr = [round(float(i), 4) for i in 1 - np.asarray(mae_curr)]
-                        accuracy_mean = round(float(np.mean(accuracy_curr)), 4)
+                [2022-11-04 18:59:01] Загрузка файла "weights_2022-06-15_17-06-15.h5" (100.0%) ... Нейротизм
 
-                        for curr_acc in [mae_curr, accuracy_curr]:
-                            # Добавление данных в словарь для DataFrame с результатами вычисления точности
-                            if self._append_to_list_of_accuracy(curr_acc, out) is False:
-                                return False
+                --- Время выполнения: 1.827 сек. ---
 
-                        self._dict_of_accuracy.update({self.__df_accuracy_mean: [mae_mean, accuracy_mean]})
-                        # Отображение в DataFrame с данными
-                        self._df_accuracy = pd.DataFrame.from_dict(
-                            data=self._dict_of_accuracy, orient="index"
-                        ).transpose()
-                        self._df_accuracy.index = self.__df_accuracy_index
-                        self._df_accuracy.index.name = self.__df_accuracy_index_name
+                True
 
-                        # Информационное сообщение
-                        self._info(self._get_union_predictions_result, out=False)
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-                        # Отображение
-                        if out is True:
-                            self._add_notebook_history_output(self._df_accuracy.iloc[0 : self.num_to_df_display_, :])
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+                :tab-width: 8
 
-                        self._info(
-                            self._get_union_predictions_results_mean.format(
-                                self._info_wrapper(str(mae_mean)), self._info_wrapper(str(accuracy_mean))
-                            ),
-                            out=False,
-                        )
+                from oceanai.modules.lab.video import Video
 
-                    clear_output(True)
-                    # Отображение истории вывода сообщений в ячейке Jupyter
-                    if out is True:
-                        self.show_notebook_history_output()
+                video = Video()
 
-                    if logs is True:
-                        # Текущее время для лог-файла
-                        # см. datetime.fromtimestamp()
-                        curr_ts = str(datetime.now().timestamp()).replace(".", "_")
+                video.path_to_save_ = './models'
+                video.chunk_size_ = 2000000
 
-                        name_logs_file = self.get_av_union_predictions.__name__
+                url_openness = video.weights_for_big5_['video']['b5']['openness']['sberdisk']
+                url_conscientiousness = video.weights_for_big5_['video']['b5']['conscientiousness']['sberdisk']
+                url_extraversion = video.weights_for_big5_['video']['b5']['extraversion']['sberdisk']
+                url_agreeableness = video.weights_for_big5_['video']['b5']['agreeableness']['sberdisk']
+                url_neuroticism = video.weights_for_big5_['video']['b5']['neuroticism']['sberdisk']
 
-                        # Сохранение LOG
-                        res_save_logs_df_files = self._save_logs(
-                            self._df_files, name_logs_file + "_df_files_" + curr_ts
+                video.load_video_models_weights_b5(
+                    url_openness = url_openness,
+                    url_conscientiousness = url_conscientiousness,
+                    url_extraversion = url_extraversion,
+                    url_agreeableness = url_agreeableness,
+                    url_neuroticism = url_neuroticism,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
+
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-11-04 19:02:32] Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств (видео модальность) ...
+
+                [2022-11-04 19:02:32] Загрузка файла "weights_2022-06-15_16-46-30.h5" (100.0%) ...
+
+                [2022-11-04 19:02:32] Ой! Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Открытость опыту
+
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/video.py
+                    Линия: 2833
+                    Метод: load_video_models_weights_b5
+                    Тип ошибки: AttributeError
+
+                [2022-11-04 19:02:32] Загрузка файла "weights_2022-06-15_16-48-50.h5" (100.0%) ...
+
+                [2022-11-04 19:02:32] Ой! Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Добросовестность
+
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/video.py
+                    Линия: 2833
+                    Метод: load_video_models_weights_b5
+                    Тип ошибки: AttributeError
+
+                [2022-11-04 19:02:33] Загрузка файла "weights_2022-06-15_16-54-06.h5" (100.0%) ...
+
+                [2022-11-04 19:02:33] Ой! Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Экстраверсия
+
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/video.py
+                    Линия: 2833
+                    Метод: load_video_models_weights_b5
+                    Тип ошибки: AttributeError
+
+                [2022-11-04 19:02:33] Загрузка файла "weights_2022-06-15_17-02-03.h5" (100.0%) ...
+
+                [2022-11-04 19:02:33] Ой! Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Доброжелательность
+
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/video.py
+                    Линия: 2833
+                    Метод: load_video_models_weights_b5
+                    Тип ошибки: AttributeError
+
+                [2022-11-04 19:02:34] Загрузка файла "weights_2022-06-15_17-06-15.h5" (100.0%) ...
+
+                [2022-11-04 19:02:34] Ой! Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Нейротизм
+
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/video.py
+                    Линия: 2833
+                    Метод: load_video_models_weights_b5
+                    Тип ошибки: AttributeError
+
+                --- Время выполнения: 1.831 сек. ---
+
+                False
+        """
+
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
+
+        try:
+            # Проверка аргументов
+            if (type(url_openness) is not str or not url_openness
+                or type(url_conscientiousness) is not str or not url_conscientiousness
+                or type(url_extraversion) is not str or not url_extraversion
+                or type(url_agreeableness) is not str or not url_agreeableness
+                or type(url_neuroticism) is not str or not url_neuroticism
+                or type(force_reload) is not bool
+                or type(out) is not bool
+                or type(runtime) is not bool or type(run) is not bool): raise TypeError
+        except TypeError:
+            self._inv_args(__class__.__name__, self.load_video_models_weights_b5.__name__, out = out); return False
+        else:
+            # Блокировка выполнения
+            if run is False: self._error(self._lock_user, out = out); return False
+
+            if runtime: self._r_start()
+
+            result_download_models = 0 # Все веса нейросетевых моделей по умолчанию загружены
+
+            # Информационное сообщение
+            self._info(self._load_video_models_weights_b5, last = False, out = out)
+
+            # Проход по всем URL с весами нейросетевых моделей
+            for cnt, url in enumerate([
+                (url_openness, self._b5['ru'][0]),
+                (url_conscientiousness, self._b5['ru'][1]),
+                (url_extraversion, self._b5['ru'][2]),
+                (url_agreeableness, self._b5['ru'][3]),
+                (url_neuroticism, self._b5['ru'][4]),
+            ]):
+                sections = urlparse(url[0]) # Парсинг URL адреса
+
+                try:
+                    # URL файл невалидный
+                    if sections.scheme == '': raise requests.exceptions.InvalidURL
+                except requests.exceptions.InvalidURL:
+                    url_norm = os.path.normpath(url[0])
+
+                    try:
+                        if os.path.isfile(url_norm) is False: raise FileNotFoundError # Не файл
+                    except FileNotFoundError: self._other_error(
+                            self._load_model_weights_error + ' ' + self._bold_wrapper(url[1].capitalize()), out = out
+                        ); continue
+                    except Exception: self._other_error(self._unknown_err, out = out); continue
+                    else:
+                        self._url_last_filename = url_norm
+
+                        # Отображение истории вывода сообщений в ячейке Jupyter
+                        if out: self.show_notebook_history_output()
+                else:
+                    try:
+                        if force_reload is False: clear_output(True)
+                        # Загрузка файла из URL
+                        res_download_file_from_url = self._download_file_from_url(
+                            url = url[0], force_reload = force_reload, runtime = False, out = out, run = True
                         )
+                    except Exception: self._other_error(self._unknown_err, out = out); continue
+                    else:
+                        # Файл загружен
+                        if res_download_file_from_url != 200: continue
 
-                        # Подсчет точности
-                        if accuracy is True:
-                            # Сохранение LOG
-                            res_save_logs_df_accuracy = self._save_logs(
-                                self._df_accuracy, name_logs_file + "_df_accuracy_" + curr_ts
-                            )
+                        try:
+                            self._video_models_b5[self._b5['en'][cnt]].load_weights(self._url_last_filename)
+                        except Exception: self._other_error(
+                                self._load_model_weights_error + ' ' + self._bold_wrapper(url[1].capitalize()),
+                                out = out
+                            ); continue
+                        else:
+                            self._add_last_el_notebook_history_output(self._bold_wrapper(url[1].capitalize()))
 
-                        if res_save_logs_df_files is True:
-                            # Сохранение LOG файла/файлов
-                            if accuracy is True and res_save_logs_df_accuracy is True:
-                                logs_s = self._logs_saves_true
-                            else:
-                                logs_s = self._logs_save_true
+                            result_download_models += 1
 
-                            self._info_true(logs_s, out=out)
+            clear_output(True)
+            # Отображение истории вывода сообщений в ячейке Jupyter
+            if out: self.show_notebook_history_output()
 
-                    return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
-    def load_avt_model_weights_b5(
-        self,
-        url: str,
-        force_reload: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Загрузка весов нейросетевой модели для получения оценок персональных качеств
+            if result_download_models != len(self._b5['ru']): return False
+            return True
+
+    def get_visual_features(
+        self, path: str, reduction_fps: int = 5, window: int = 10, step: int = 5,
+        out: bool = True, runtime: bool = True, run: bool = True
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Извлечение признаков из визуального сигнала
 
         Args:
-            url (str): Полный путь к файлу с весами нейросетевой модели
-            force_reload (bool): Принудительная загрузка файлов с весами нейросетевых моделей из сети
+            path (str): Путь к видеофайлу
+            reduction_fps (int): Понижение кадровой частоты
+            window (int): Размер окна сегмента сигнала (в кадрах)
+            step (int): Шаг сдвига окна сегмента сигнала (в кадрах)
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
-        """
+            Tuple[np.ndarray, np.ndarray]: Кортеж с двумя np.ndarray:
 
-        if runtime:
-            self._r_start()
+                1. np.ndarray с экспертными признаками
+                2. np.ndarray с нейросетевыми признаками
 
-        if self.__load_model_weights(url, force_reload, self._load_avt_model_weights_b5, out, False, run) is True:
-            try:
-                self._avt_model_b5.load_weights(self._url_last_filename)
-            except Exception:
-                self._error(self._model_avt_not_formation, out=out)
-                return False
-            else:
-                return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+        :bdg-link-light:`Пример <../../user_guide/notebooks/Video-get_visual_features.ipynb>`
+        """
 
-        return False
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
-    def get_avt_predictions(
-        self,
-        depth: int = 1,
-        recursive: bool = False,
-        sr: int = 44100,
-        window_audio: Union[int, float] = 2.0,
-        step_audio: Union[int, float] = 1.0,
-        reduction_fps: int = 5,
-        window_video: int = 10,
-        step_video: int = 5,
-        asr: bool = False,
-        lang: str = "ru",
-        accuracy=True,
-        url_accuracy: str = "",
-        logs: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+        return self._get_visual_features(
+            path = path, reduction_fps = reduction_fps, window = window, step = step,
+            last = False, out = out, runtime = runtime, run = run
+        )
+
+    def get_video_union_predictions(
+        self, depth: int = 1, recursive: bool = False, reduction_fps: int = 5, window: int = 10, step: int = 5,
+        accuracy = True, url_accuracy: str = '', logs: bool = True, out: bool = True, runtime: bool = True,
+        run: bool = True
     ) -> bool:
-        """Получения прогнозов по аудио, видео и тексту (мультимодальное объединение)
+        """Получения прогнозов по видео
 
         Args:
             depth (int): Глубина иерархии для получения данных
             recursive (bool): Рекурсивный поиск данных
-            sr (int): Частота дискретизации
-            window_audio (Union[int, float]): Размер окна сегмента аудио сигнала (в секундах)
-            step_audio (Union[int, float]): Шаг сдвига окна сегмента аудио сигнала (в секундах)
             reduction_fps (int): Понижение кадровой частоты
-            window_video (int): Размер окна сегмента видео сигнала (в кадрах)
-            step_video (int): Шаг сдвига окна сегмента видео сигнала (в кадрах)
-            asr (bool): Автоматическое распознавание речи
-            lang (str): Язык
+            window (int): Размер окна сегмента сигнала (в кадрах)
+            step (int): Шаг сдвига окна сегмента сигнала (в кадрах)
             accuracy (bool): Вычисление точности
             url_accuracy (str): Полный путь к файлу с верными предсказаниями для подсчета точности
             logs (bool): При необходимости формировать LOG файл
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если прогнозы успешно получены, в обратном случае **False**
+            bool: **True** если веса прогнозы успешно получены, в обратном случае **False**
+
+        :bdg-link-light:`Пример <../../user_guide/notebooks/Video-get_video_union_predictions.ipynb>`
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         # Сброс
-        self._df_files = pd.DataFrame()  # Пустой DataFrame с данными
-        self._df_accuracy = pd.DataFrame()  # Пустой DataFrame с результатами вычисления точности
+        self._df_files = pd.DataFrame() # Пустой DataFrame с данными
+        self._df_accuracy = pd.DataFrame() # Пустой DataFrame с результатами вычисления точности
 
         try:
             # Проверка аргументов
-            if (
-                type(depth) is not int
-                or depth < 1
-                or type(recursive) is not bool
-                or type(sr) is not int
-                or sr < 1
-                or (
-                    (type(window_audio) is not int or window_audio < 1)
-                    and (type(window_audio) is not float or window_audio <= 0)
-                )
-                or (
-                    (type(step_audio) is not int or step_audio < 1)
-                    and (type(step_audio) is not float or step_audio <= 0)
-                )
-                or type(reduction_fps) is not int
-                or reduction_fps < 1
-                or type(window_video) is not int
-                or window_video < 1
-                or type(step_video) is not int
-                or step_video < 1
-                or type(asr) is not bool
-                or not isinstance(lang, str)
-                or lang not in self.lang_traslate
-                or type(accuracy) is not bool
-                or type(url_accuracy) is not str
-                or type(logs) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
+            if (type(depth) is not int or depth < 1 or type(out) is not bool or type(recursive) is not bool
+                    or type(reduction_fps) is not int or reduction_fps < 1
+                    or type(window) is not int or window < 1 or type(step) is not int or step < 1
+                    or type(accuracy) is not bool or type(url_accuracy) is not str
+                    or type(logs) is not bool or type(runtime) is not bool or type(run) is not bool):
                 raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.get_avt_predictions.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.get_video_union_predictions.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             try:
                 # Получение директорий, где хранятся данные
-                path_to_data = self._get_paths(self.path_to_dataset_, depth, out=out)
-                if type(path_to_data) is bool:
-                    return False
+                path_to_data = self._get_paths(self.path_to_dataset_, depth, out = out)
+                if type(path_to_data) is bool: return False
 
-                if type(self.keys_dataset_) is not list:
-                    raise TypeError
+                if type(self.keys_dataset_) is not list: raise TypeError
 
                 # Словарь для DataFrame набора данных с данными
                 self._dict_of_files = dict(zip(self.keys_dataset_, [[] for _ in range(0, len(self.keys_dataset_))]))
                 # Словарь для DataFrame набора данных с результатами вычисления точности
                 self._dict_of_accuracy = dict(
                     zip(self.keys_dataset_[1:], [[] for _ in range(0, len(self.keys_dataset_[1:]))])
                 )
             except (TypeError, FileNotFoundError):
-                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out=out)
-                return False
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
+                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out = out)
                 return False
+            except Exception: self._other_error(self._unknown_err, out = out); return False
             else:
                 # Вычисление точности
                 if accuracy is True:
-                    get_avt_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
-                else:
-                    get_avt_predictions_info = self._get_union_predictions_info
+                    get_video_union_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
+                else: get_video_union_predictions_info = self._get_union_predictions_info
 
-                get_avt_predictions_info += self._av_modality
+                get_video_union_predictions_info += self._video_modality
 
                 # Вычисление точности
                 if accuracy is True:
                     # Информационное сообщение
-                    self._info(get_avt_predictions_info, out=out)
+                    self._info(get_video_union_predictions_info, out = out)
 
-                    if not url_accuracy:
-                        url_accuracy = self._true_traits["sberdisk"]
+                    if not url_accuracy: url_accuracy = self._true_traits['sberdisk']
 
                     try:
                         # Загрузка верных предсказаний
                         data_true_traits = pd.read_csv(url_accuracy)
                     except (FileNotFoundError, URLError, UnicodeDecodeError):
-                        self._other_error(self._load_data_true_traits_error, out=out)
-                        return False
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return False
+                        self._other_error(self._load_data_true_traits_error, out = out); return False
+                    except Exception: self._other_error(self._unknown_err, out = out); return False
                     else:
                         true_traits = []
                         self._del_last_el_notebook_history_output()
 
-                paths = []  # Пути до искомых файлов
+                paths = [] # Пути до искомых файлов
 
                 # Проход по всем директориям
                 for curr_path in path_to_data:
-                    empty = True  # По умолчанию директория пустая
+                    empty = True # По умолчанию директория пустая
 
                     # Рекурсивный поиск данных
-                    if recursive is True:
-                        g = Path(curr_path).rglob("*")
-                    else:
-                        g = Path(curr_path).glob("*")
+                    if recursive is True: g = Path(curr_path).rglob('*')
+                    else: g = Path(curr_path).glob('*')
 
                     # Формирование словаря для DataFrame
                     for p in g:
                         try:
-                            if type(self.ext_) is not list or len(self.ext_) < 1:
-                                raise TypeError
+                            if type(self.ext_) is not list or len(self.ext_) < 1: raise TypeError
 
                             self.ext_ = [x.lower() for x in self.ext_]
-                        except TypeError:
-                            self._other_error(self._wrong_ext, out=out)
-                            return False
-                        except Exception:
-                            self._other_error(self._unknown_err, out=out)
-                            return False
+                        except TypeError: self._other_error(self._wrong_ext, out = out); return False
+                        except Exception: self._other_error(self._unknown_err, out = out); return False
                         else:
                             # Расширение файла соответствует расширению искомых файлов
                             if p.suffix.lower() in self.ext_:
-                                if empty is True:
-                                    empty = False  # Каталог не пустой
+                                if empty is True: empty = False # Каталог не пустой
 
                                 paths.append(p.resolve())
 
                 try:
-                    self.__len_paths = len(paths)  # Количество искомых файлов
+                    self.__len_paths = len(paths) # Количество искомых файлов
 
-                    if self.__len_paths == 0:
-                        raise TypeError
-                except TypeError:
-                    self._other_error(self._files_not_found, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
+                    if self.__len_paths == 0: raise TypeError
+                except TypeError: self._other_error(self._files_not_found, out = out); return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
                 else:
                     # Локальный путь
                     self.__local_path = lambda path: os.path.join(
-                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))) :]
+                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))):]
                     )
 
-                    last = False  # Замена последнего сообщения
+                    last = False # Замена последнего сообщения
 
                     # Проход по всем искомым файлов
                     for i, curr_path in enumerate(paths):
-                        if i != 0:
-                            last = True
+                        if i != 0: last = True
 
                         # Индикатор выполнения
                         self._progressbar_union_predictions(
-                            get_avt_predictions_info,
-                            i,
-                            self.__local_path(curr_path),
-                            self.__len_paths,
-                            True,
-                            last,
-                            out,
-                        )
-
-                        # Извлечение признаков из акустического сигнала
-                        hc_audio_features, melspectrogram_audio_features = self._get_acoustic_features(
-                            path=str(curr_path.resolve()),
-                            sr=sr,
-                            window=window_audio,
-                            step=step_audio,
-                            last=True,
-                            out=False,
-                            runtime=False,
-                            run=run,
+                            get_video_union_predictions_info, i, self.__local_path(curr_path), self.__len_paths,
+                            True, last, out
                         )
 
                         # Извлечение признаков из визуального сигнала
-                        hc_video_features, nn_video_features = self._get_visual_features(
-                            path=str(curr_path.resolve()),
-                            reduction_fps=reduction_fps,
-                            window=window_video,
-                            step=step_video,
-                            lang=lang,
-                            last=True,
-                            out=False,
-                            runtime=False,
-                            run=run,
+                        hc_features, nn_features = self._get_visual_features(
+                            path = str(curr_path.resolve()),
+                            reduction_fps = reduction_fps,
+                            window = window,
+                            step = step,
+                            last = True, out = False, runtime = False, run = run
                         )
 
-                        # Извлечение признаков из текста
-                        hc_text_features, nn_text_features = self.get_text_features(
-                            path=str(curr_path.resolve()),
-                            asr=asr,
-                            lang=lang,
-                            show_text=False,
-                            out=False,
-                            runtime=False,
-                            run=run,
-                        )
-
-                        hc_text_features = np.expand_dims(hc_text_features, axis=0)
-                        nn_text_features = np.expand_dims(nn_text_features, axis=0)
-
-                        if (
-                            type(hc_audio_features) is list
-                            and type(melspectrogram_audio_features) is list
-                            and type(hc_video_features) is np.ndarray
-                            and type(nn_video_features) is np.ndarray
-                            and type(hc_text_features) is np.ndarray
-                            and type(nn_text_features) is np.ndarray
-                            and len(hc_audio_features) > 0
-                            and len(melspectrogram_audio_features) > 0
-                            and len(hc_video_features) > 0
-                            and len(nn_video_features) > 0
-                            and len(hc_text_features) > 0
-                            and len(nn_text_features) > 0
-                        ):
-                            feature_lambda = lambda feature: np.concatenate(
-                                (np.mean(feature, axis=0), np.std(feature, axis=0))
-                            )
-
-                            # Коды ошибок нейросетевых моделей (аудио модальность)
-                            code_error_pred_hc_audio = -1
-                            code_error_pred_melspectrogram_audio = -1
-
-                            try:
-                                # Оправка экспертных признаков в нейросетевую модель
-                                _, features_hc_audio = self.audio_model_hc_(
-                                    np.array(hc_audio_features, dtype=np.float16)
-                                )
-                            except TypeError:
-                                code_error_pred_hc_audio = 1
-                            except Exception:
-                                code_error_pred_melspectrogram_audio = 2
-
-                            try:
-                                # Отправка нейросетевых признаков в нейросетевую модель
-                                _, features_nn_audio = self.audio_model_nn_(
-                                    np.array(melspectrogram_audio_features, dtype=np.float16)
-                                )
-                            except TypeError:
-                                code_error_pred_melspectrogram_audio = 1
-                            except Exception:
-                                code_error_pred_melspectrogram_audio = 2
-
-                            if code_error_pred_hc_audio != -1 and code_error_pred_melspectrogram_audio != -1:
-                                self._error(self._models_audio_not_formation, out=out)
-                                return False
-
-                            if code_error_pred_hc_audio != -1:
-                                self._error(self._model_audio_hc_not_formation, out=out)
-                                return False
-
-                            if code_error_pred_melspectrogram_audio != -1:
-                                self._error(self._model_audio_nn_not_formation, out=out)
-                                return False
-
-                            features_hc_audio = np.expand_dims(feature_lambda(features_hc_audio.numpy()), axis=0)
-                            features_nn_audio = np.expand_dims(feature_lambda(features_nn_audio.numpy()), axis=0)
-
-                            # Коды ошибок нейросетевых моделей (видео модальность)
-                            code_error_pred_hc_video = -1
-                            code_error_pred_nn_video = -1
+                        # Признаки из акустического сигнала извлечены
+                        if (type(hc_features) is np.ndarray and type(nn_features) is np.ndarray
+                            and len(hc_features) > 0 and len(nn_features) > 0):
+                            # Коды ошибок нейросетевых моделей
+                            code_error_pred_hc = -1
+                            code_error_pred_nn = -1
 
                             try:
                                 # Оправка экспертных признаков в нейросетевую модель
-                                _, features_hc_video = self.video_model_hc_(
-                                    np.array(hc_video_features, dtype=np.float16)
-                                )
-                            except TypeError:
-                                code_error_pred_hc_video = 1
-                            except Exception:
-                                code_error_pred_hc_video = 2
+                                pred_hc = self.video_model_hc_(np.array(hc_features, dtype = np.float16)).numpy()
+                            except TypeError: code_error_pred_hc = 1
+                            except Exception: code_error_pred_hc = 2
 
                             try:
                                 # Отправка нейросетевых признаков в нейросетевую модель
-                                _, features_nn_video = self.video_model_nn_(
-                                    np.array(nn_video_features, dtype=np.float16)
-                                )
-                            except TypeError:
-                                code_error_pred_nn_video = 1
-                            except Exception:
-                                code_error_pred_nn_video = 2
-
-                            if code_error_pred_hc_video != -1 and code_error_pred_nn_video != -1:
-                                self._error(self._models_video_not_formation, out=out)
-                                return False
-
-                            if code_error_pred_hc_video != -1:
-                                self._error(self._model_video_hc_not_formation, out=out)
-                                return False
+                                pred_nn = self.video_model_nn_(np.array(nn_features, dtype = np.float16)).numpy()
+                            except TypeError: code_error_pred_nn = 1
+                            except Exception: code_error_pred_nn = 2
 
-                            if code_error_pred_nn_video != -1:
-                                self._error(self._model_video_nn_not_formation, out=out)
-                                return False
-
-                            features_hc_video = np.expand_dims(feature_lambda(features_hc_video.numpy()), axis=0)
-                            features_nn_video = np.expand_dims(feature_lambda(features_nn_video.numpy()), axis=0)
+                            if code_error_pred_hc != -1 and code_error_pred_nn != -1:
+                                self._error(self._models_video_not_formation, out = out); return False
 
-                            # Коды ошибок нейросетевых моделей (текст)
-                            code_error_pred_hc_text = -1
-                            code_error_pred_nn_text = -1
+                            if code_error_pred_hc != -1:
+                                self._error(self._model_video_hc_not_formation, out = out); return False
 
-                            try:
-                                # Оправка экспертных признаков в нейросетевую модель
-                                _, features_hc_text = self.text_model_hc_(np.array(hc_text_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_hc_text = 1
-                            except Exception:
-                                code_error_pred_hc_text = 2
+                            if code_error_pred_nn != -1:
+                                self._error(self._model_video_nn_not_formation, out = out); return False
 
-                            try:
-                                # Отправка нейросетевых признаков в нейросетевую модель
-                                _, features_nn_text = self.text_model_nn_(np.array(nn_text_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_nn_text = 1
-                            except Exception:
-                                code_error_pred_nn_text = 2
+                            # Конкатенация оценок по экспертным и нейросетевым признакам
+                            union_pred = self.__concat_pred(pred_hc, pred_nn, out = out)
 
-                            if code_error_pred_hc_text != -1 and code_error_pred_nn_text != -1:
-                                self._error(self._model_text_not_formation, out=out)
-                                return False
+                            if len(union_pred) == 0: return False
 
-                            if code_error_pred_hc_text != -1:
-                                self._error(self._model_text_hc_not_formation, out=out)
-                                return False
+                            final_pred = []
 
-                            if code_error_pred_nn_text != -1:
-                                self._error(self._model_text_nn_not_formation, out=out)
-                                return False
+                            for cnt, (name_b5, model) in enumerate(self.video_models_b5_.items()):
+                                result = model(np.expand_dims(union_pred[cnt], axis = 0)).numpy()[0][0]
 
-                            try:
-                                final_pred = (
-                                    self.avt_model_b5_(
-                                        [
-                                            features_hc_text.numpy(),
-                                            features_nn_text.numpy(),
-                                            features_hc_audio,
-                                            features_nn_audio,
-                                            features_hc_video,
-                                            features_nn_video,
-                                        ]
-                                    )
-                                    .numpy()[0]
-                                    .tolist()
-                                )
-                            except Exception:
-                                self._other_error(self._unknown_err, out=out)
-                                return False
+                                final_pred.append(result)
 
                             # Добавление данных в словарь для DataFrame
                             if self._append_to_list_of_files(str(curr_path.resolve()), final_pred, out) is False:
                                 return False
+
                             # Вычисление точности
                             if accuracy is True:
                                 try:
-                                    true_trait = (
-                                        data_true_traits[data_true_traits.NAME_VIDEO == curr_path.name][
-                                            list(self._b5["en"])
-                                        ]
-                                        .values[0]
-                                        .tolist()
-                                    )
+                                    true_trait = data_true_traits[
+                                        data_true_traits.NAME_VIDEO == curr_path.name
+                                    ][list(self._b5['en'])].values[0].tolist()
                                 except IndexError:
-                                    self._other_error(self._expert_values_not_found, out=out)
-                                    return False
-                                except Exception:
-                                    self._other_error(self._unknown_err, out=out)
-                                    return False
-                                else:
-                                    true_traits.append(true_trait)
+                                    self._other_error(self._expert_values_not_found, out = out); return False
+                                except Exception: self._other_error(self._unknown_err, out = out); return False
+                                else: true_traits.append(true_trait)
                         else:
                             # Добавление данных в словарь для DataFrame
-                            if (
-                                self._append_to_list_of_files(
-                                    str(curr_path.resolve()), [None] * len(self._b5["en"]), out
-                                )
-                                is False
-                            ):
-                                return False
+                            if self._append_to_list_of_files(
+                                str(curr_path.resolve()), [None] * len(self._b5['en']), out
+                            ) is False: return False
 
                             self._del_last_el_notebook_history_output()
 
                     # Индикатор выполнения
                     self._progressbar_union_predictions(
-                        get_avt_predictions_info,
-                        self.__len_paths,
-                        self.__local_path(paths[-1]),
-                        self.__len_paths,
-                        True,
-                        last,
-                        out,
+                        get_video_union_predictions_info, self.__len_paths, self.__local_path(paths[-1]),
+                        self.__len_paths, True, last, out
                     )
 
                     # Отображение в DataFrame с данными
-                    self._df_files = pd.DataFrame.from_dict(data=self._dict_of_files, orient="index").transpose()
+                    self._df_files = pd.DataFrame.from_dict(data = self._dict_of_files, orient = 'index').transpose()
                     self._df_files.index.name = self._keys_id
                     self._df_files.index += 1
 
                     self._df_files.index = self._df_files.index.map(str)
 
-                    self._df_files.Path = [os.path.basename(i) for i in self._df_files.Path]
                     # Отображение
                     if out is True:
-                        self._add_notebook_history_output(self._df_files.iloc[0 : self.num_to_df_display_, :])
+                        self._add_notebook_history_output(self._df_files.iloc[0:self.num_to_df_display_, :])
 
                     # Подсчет точности
                     if accuracy is True:
                         mae_curr = []
 
                         for cnt, name_b5 in enumerate(self._df_files.keys().tolist()[1:]):
                             try:
                                 mae_curr.append(
                                     mean_absolute_error(
                                         np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list()
                                     )
                                 )
-                            except IndexError:
-                                continue
-                            except Exception:
-                                continue
+                            except IndexError: continue
+                            except Exception: continue
 
                         mae_curr = [round(float(i), 4) for i in mae_curr]
                         mae_mean = round(float(np.mean(mae_curr)), 4)
                         accuracy_curr = [round(float(i), 4) for i in 1 - np.asarray(mae_curr)]
                         accuracy_mean = round(float(np.mean(accuracy_curr)), 4)
 
                         for curr_acc in [mae_curr, accuracy_curr]:
                             # Добавление данных в словарь для DataFrame с результатами вычисления точности
-                            if self._append_to_list_of_accuracy(curr_acc, out) is False:
-                                return False
+                            if self._append_to_list_of_accuracy(curr_acc, out) is False: return False
 
-                        self._dict_of_accuracy.update({self.__df_accuracy_mean: [mae_mean, accuracy_mean]})
+                        self._dict_of_accuracy.update({
+                            self.__df_accuracy_mean: [mae_mean, accuracy_mean]
+                        })
                         # Отображение в DataFrame с данными
-                        self._df_accuracy = pd.DataFrame.from_dict(
-                            data=self._dict_of_accuracy, orient="index"
-                        ).transpose()
+                        self._df_accuracy = pd.DataFrame.from_dict(data = self._dict_of_accuracy,
+                                                                   orient = 'index').transpose()
                         self._df_accuracy.index = self.__df_accuracy_index
                         self._df_accuracy.index.name = self.__df_accuracy_index_name
 
                         # Информационное сообщение
-                        self._info(self._get_union_predictions_result, out=False)
+                        self._info(self._get_union_predictions_result, out = False)
 
                         # Отображение
                         if out is True:
-                            self._add_notebook_history_output(self._df_accuracy.iloc[0 : self.num_to_df_display_, :])
+                            self._add_notebook_history_output(self._df_accuracy.iloc[0:self.num_to_df_display_, :])
 
                         self._info(
                             self._get_union_predictions_results_mean.format(
-                                self._info_wrapper(str(mae_mean)), self._info_wrapper(str(accuracy_mean))
+                                self._info_wrapper(str(mae_mean)),
+                                self._info_wrapper(str(accuracy_mean))
                             ),
-                            out=False,
+                            out = False
                         )
 
                     clear_output(True)
                     # Отображение истории вывода сообщений в ячейке Jupyter
-                    if out is True:
-                        self.show_notebook_history_output()
+                    if out is True: self.show_notebook_history_output()
 
                     if logs is True:
                         # Текущее время для лог-файла
                         # см. datetime.fromtimestamp()
-                        curr_ts = str(datetime.now().timestamp()).replace(".", "_")
+                        curr_ts = str(datetime.now().timestamp()).replace('.', '_')
 
-                        name_logs_file = self.get_avt_predictions.__name__
+                        name_logs_file = self.get_video_union_predictions.__name__
 
                         # Сохранение LOG
                         res_save_logs_df_files = self._save_logs(
-                            self._df_files, name_logs_file + "_df_files_" + curr_ts
+                            self._df_files, name_logs_file + '_df_files_' + curr_ts
                         )
 
                         # Подсчет точности
                         if accuracy is True:
                             # Сохранение LOG
                             res_save_logs_df_accuracy = self._save_logs(
-                                self._df_accuracy, name_logs_file + "_df_accuracy_" + curr_ts
+                                self._df_accuracy, name_logs_file + '_df_accuracy_' + curr_ts
                             )
 
                         if res_save_logs_df_files is True:
                             # Сохранение LOG файла/файлов
-                            if accuracy is True and res_save_logs_df_accuracy is True:
-                                logs_s = self._logs_saves_true
-                            else:
-                                logs_s = self._logs_save_true
+                            if accuracy is True and res_save_logs_df_accuracy is True: logs_s = self._logs_saves_true
+                            else: logs_s = self._logs_save_true
 
-                            self._info_true(logs_s, out=out)
+                            self._info_true(logs_s, out = out)
 
                     return True
             finally:
-                if runtime:
-                    self._r_end(out=out)
-
-
-    def get_avt_predictions_gradio(
-        self,
-        paths: list[str] = [],
-        depth: int = 1,
-        recursive: bool = False,
-        sr: int = 44100,
-        window_audio: Union[int, float] = 2.0,
-        step_audio: Union[int, float] = 1.0,
-        reduction_fps: int = 5,
-        window_video: int = 10,
-        step_video: int = 5,
-        asr: bool = False,
-        lang: str = "ru",
-        accuracy=True,
-        url_accuracy: str = "",
-        logs: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Получения прогнозов по аудио, видео и тексту (мультимодальное объединение)
-
-        Args:
-            depth (int): Глубина иерархии для получения данных
-            recursive (bool): Рекурсивный поиск данных
-            sr (int): Частота дискретизации
-            window_audio (Union[int, float]): Размер окна сегмента аудио сигнала (в секундах)
-            step_audio (Union[int, float]): Шаг сдвига окна сегмента аудио сигнала (в секундах)
-            reduction_fps (int): Понижение кадровой частоты
-            window_video (int): Размер окна сегмента видео сигнала (в кадрах)
-            step_video (int): Шаг сдвига окна сегмента видео сигнала (в кадрах)
-            asr (bool): Автоматическое распознавание речи
-            lang (str): Язык
-            accuracy (bool): Вычисление точности
-            url_accuracy (str): Полный путь к файлу с верными предсказаниями для подсчета точности
-            logs (bool): При необходимости формировать LOG файл
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
-
-        Returns:
-            bool: **True** если прогнозы успешно получены, в обратном случае **False**
-        """
-
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
-
-        # Сброс
-        self._df_files = pd.DataFrame()  # Пустой DataFrame с данными
-        self._df_accuracy = pd.DataFrame()  # Пустой DataFrame с результатами вычисления точности
-
-        try:
-            # Проверка аргументов
-            if (
-                type(depth) is not int
-                or depth < 1
-                or type(recursive) is not bool
-                or type(sr) is not int
-                or sr < 1
-                or (
-                    (type(window_audio) is not int or window_audio < 1)
-                    and (type(window_audio) is not float or window_audio <= 0)
-                )
-                or (
-                    (type(step_audio) is not int or step_audio < 1)
-                    and (type(step_audio) is not float or step_audio <= 0)
-                )
-                or type(reduction_fps) is not int
-                or reduction_fps < 1
-                or type(window_video) is not int
-                or window_video < 1
-                or type(step_video) is not int
-                or step_video < 1
-                or type(asr) is not bool
-                or not isinstance(lang, str)
-                or lang not in self.lang_traslate
-                or type(accuracy) is not bool
-                or type(url_accuracy) is not str
-                or type(logs) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.get_avt_predictions.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
-
-            if runtime:
-                self._r_start()
-
-            try:
-                # Получение директорий, где хранятся данные
-                path_to_data = self._get_paths(self.path_to_dataset_, depth, out=out)
-                if type(path_to_data) is bool:
-                    return False
-
-                if type(self.keys_dataset_) is not list:
-                    raise TypeError
-
-                # Словарь для DataFrame набора данных с данными
-                self._dict_of_files = dict(zip(self.keys_dataset_, [[] for _ in range(0, len(self.keys_dataset_))]))
-                # Словарь для DataFrame набора данных с результатами вычисления точности
-                self._dict_of_accuracy = dict(
-                    zip(self.keys_dataset_[1:], [[] for _ in range(0, len(self.keys_dataset_[1:]))])
-                )
-            except (TypeError, FileNotFoundError):
-                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out=out)
-                return False
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return False
-            else:
-                # Вычисление точности
-                if accuracy is True:
-                    get_avt_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
-                else:
-                    get_avt_predictions_info = self._get_union_predictions_info
-
-                get_avt_predictions_info += self._av_modality
-
-                # Вычисление точности
-                if accuracy is True:
-                    # Информационное сообщение
-                    self._info(get_avt_predictions_info, out=out)
-
-                    if not url_accuracy:
-                        url_accuracy = self._true_traits["sberdisk"]
-
-                    try:
-                        # Загрузка верных предсказаний
-                        data_true_traits = pd.read_csv(url_accuracy)
-                    except (FileNotFoundError, URLError, UnicodeDecodeError):
-                        self._other_error(self._load_data_true_traits_error, out=out)
-                        return False
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return False
-                    else:
-                        true_traits = []
-                        self._del_last_el_notebook_history_output()
-
-                last = False  # Замена последнего сообщения
-
-                # print(paths)
-
-                paths = [i for i in paths if i.endswith(('.mp4', '.avi'))]
-                self.__len_paths = len(paths)
-
-                # Проход по всем искомым файлов
-                for i, curr_path in enumerate(paths):
-                    # print(curr_path)
-                    if i != 0:
-                        last = True
-
-                    # Извлечение признаков из акустического сигнала
-                    hc_audio_features, melspectrogram_audio_features = self._get_acoustic_features(
-                        path=curr_path,
-                        sr=sr,
-                        window=window_audio,
-                        step=step_audio,
-                        last=True,
-                        out=True,
-                        runtime=False,
-                        run=run,
-                    )
-
-                    # print(hc_audio_features, melspectrogram_audio_features)
-
-                    # Извлечение признаков из визуального сигнала
-                    hc_video_features, nn_video_features = self._get_visual_features(
-                        path=curr_path,
-                        reduction_fps=reduction_fps,
-                        window=window_video,
-                        step=step_video,
-                        lang=lang,
-                        last=True,
-                        out=False,
-                        runtime=False,
-                        run=run,
-                    )
-
-                    # Извлечение признаков из текста
-                    hc_text_features, nn_text_features = self.get_text_features(
-                        path=curr_path,
-                        asr=asr,
-                        lang=lang,
-                        show_text=False,
-                        out=False,
-                        runtime=False,
-                        run=run,
-                    )
-
-                    hc_text_features = np.expand_dims(hc_text_features, axis=0)
-                    nn_text_features = np.expand_dims(nn_text_features, axis=0)
-
-                    if (
-                        type(hc_audio_features) is list
-                        and type(melspectrogram_audio_features) is list
-                        and type(hc_video_features) is np.ndarray
-                        and type(nn_video_features) is np.ndarray
-                        and type(hc_text_features) is np.ndarray
-                        and type(nn_text_features) is np.ndarray
-                        and len(hc_audio_features) > 0
-                        and len(melspectrogram_audio_features) > 0
-                        and len(hc_video_features) > 0
-                        and len(nn_video_features) > 0
-                        and len(hc_text_features) > 0
-                        and len(nn_text_features) > 0
-                    ):
-                        feature_lambda = lambda feature: np.concatenate(
-                            (np.mean(feature, axis=0), np.std(feature, axis=0))
-                        )
-
-                        # Коды ошибок нейросетевых моделей (аудио модальность)
-                        code_error_pred_hc_audio = -1
-                        code_error_pred_melspectrogram_audio = -1
-
-                        try:
-                            # Оправка экспертных признаков в нейросетевую модель
-                            _, features_hc_audio = self.audio_model_hc_(
-                                np.array(hc_audio_features, dtype=np.float16)
-                            )
-                        except TypeError:
-                            code_error_pred_hc_audio = 1
-                        except Exception:
-                            code_error_pred_melspectrogram_audio = 2
-
-                        try:
-                            # Отправка нейросетевых признаков в нейросетевую модель
-                            _, features_nn_audio = self.audio_model_nn_(
-                                np.array(melspectrogram_audio_features, dtype=np.float16)
-                            )
-                        except TypeError:
-                            code_error_pred_melspectrogram_audio = 1
-                        except Exception:
-                            code_error_pred_melspectrogram_audio = 2
-
-                        if code_error_pred_hc_audio != -1 and code_error_pred_melspectrogram_audio != -1:
-                            self._error(self._models_audio_not_formation, out=out)
-                            return False
-
-                        if code_error_pred_hc_audio != -1:
-                            self._error(self._model_audio_hc_not_formation, out=out)
-                            return False
-
-                        if code_error_pred_melspectrogram_audio != -1:
-                            self._error(self._model_audio_nn_not_formation, out=out)
-                            return False
-
-                        features_hc_audio = np.expand_dims(feature_lambda(features_hc_audio.numpy()), axis=0)
-                        features_nn_audio = np.expand_dims(feature_lambda(features_nn_audio.numpy()), axis=0)
-
-                        # Коды ошибок нейросетевых моделей (видео модальность)
-                        code_error_pred_hc_video = -1
-                        code_error_pred_nn_video = -1
-
-                        try:
-                            # Оправка экспертных признаков в нейросетевую модель
-                            _, features_hc_video = self.video_model_hc_(
-                                np.array(hc_video_features, dtype=np.float16)
-                            )
-                        except TypeError:
-                            code_error_pred_hc_video = 1
-                        except Exception:
-                            code_error_pred_hc_video = 2
-
-                        try:
-                            # Отправка нейросетевых признаков в нейросетевую модель
-                            _, features_nn_video = self.video_model_nn_(
-                                np.array(nn_video_features, dtype=np.float16)
-                            )
-                        except TypeError:
-                            code_error_pred_nn_video = 1
-                        except Exception:
-                            code_error_pred_nn_video = 2
-
-                        if code_error_pred_hc_video != -1 and code_error_pred_nn_video != -1:
-                            self._error(self._models_video_not_formation, out=out)
-                            return False
-
-                        if code_error_pred_hc_video != -1:
-                            self._error(self._model_video_hc_not_formation, out=out)
-                            return False
-
-                        if code_error_pred_nn_video != -1:
-                            self._error(self._model_video_nn_not_formation, out=out)
-                            return False
-
-                        features_hc_video = np.expand_dims(feature_lambda(features_hc_video.numpy()), axis=0)
-                        features_nn_video = np.expand_dims(feature_lambda(features_nn_video.numpy()), axis=0)
-
-                        # Коды ошибок нейросетевых моделей (текст)
-                        code_error_pred_hc_text = -1
-                        code_error_pred_nn_text = -1
-
-                        try:
-                            # Оправка экспертных признаков в нейросетевую модель
-                            _, features_hc_text = self.text_model_hc_(np.array(hc_text_features, dtype=np.float16))
-                        except TypeError:
-                            code_error_pred_hc_text = 1
-                        except Exception:
-                            code_error_pred_hc_text = 2
-
-                        try:
-                            # Отправка нейросетевых признаков в нейросетевую модель
-                            _, features_nn_text = self.text_model_nn_(np.array(nn_text_features, dtype=np.float16))
-                        except TypeError:
-                            code_error_pred_nn_text = 1
-                        except Exception:
-                            code_error_pred_nn_text = 2
-
-                        if code_error_pred_hc_text != -1 and code_error_pred_nn_text != -1:
-                            self._error(self._model_text_not_formation, out=out)
-                            return False
-
-                        if code_error_pred_hc_text != -1:
-                            self._error(self._model_text_hc_not_formation, out=out)
-                            return False
-
-                        if code_error_pred_nn_text != -1:
-                            self._error(self._model_text_nn_not_formation, out=out)
-                            return False
-
-                        try:
-                            final_pred = (
-                                self.avt_model_b5_(
-                                    [
-                                        features_hc_text.numpy(),
-                                        features_nn_text.numpy(),
-                                        features_hc_audio,
-                                        features_nn_audio,
-                                        features_hc_video,
-                                        features_nn_video,
-                                    ]
-                                )
-                                .numpy()[0]
-                                .tolist()
-                            )
-                        except Exception:
-                            self._other_error(self._unknown_err, out=out)
-                            return False
-
-                        # Добавление данных в словарь для DataFrame
-                        if self._append_to_list_of_files(curr_path, final_pred, out) is False:
-                            return False
-                        # Вычисление точности
-                        if accuracy is True:
-                            try:
-                                true_trait = (
-                                    data_true_traits[data_true_traits.NAME_VIDEO == curr_path.name][
-                                        list(self._b5["en"])
-                                    ]
-                                    .values[0]
-                                    .tolist()
-                                )
-                            except IndexError:
-                                self._other_error(self._expert_values_not_found, out=out)
-                                return False
-                            except Exception:
-                                self._other_error(self._unknown_err, out=out)
-                                return False
-                            else:
-                                true_traits.append(true_trait)
-                    else:
-                        # Добавление данных в словарь для DataFrame
-                        if (
-                            self._append_to_list_of_files(
-                                curr_path, [None] * len(self._b5["en"]), out
-                            )
-                            is False
-                        ):
-                            return False
-
-                        self._del_last_el_notebook_history_output()
-
-                # Отображение в DataFrame с данными
-                self._df_files = pd.DataFrame.from_dict(data=self._dict_of_files, orient="index").transpose()
-                self._df_files.index.name = self._keys_id
-                self._df_files.index += 1
-
-                self._df_files.index = self._df_files.index.map(str)
-
-                self._df_files.Path = [os.path.basename(i) for i in self._df_files.Path]
-                # Отображение
-                if out is True:
-                    self._add_notebook_history_output(self._df_files.iloc[0 : self.num_to_df_display_, :])
-
-                # Подсчет точности
-                if accuracy is True:
-                    mae_curr = []
-
-                    for cnt, name_b5 in enumerate(self._df_files.keys().tolist()[1:]):
-                        try:
-                            mae_curr.append(
-                                mean_absolute_error(
-                                    np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list()
-                                )
-                            )
-                        except IndexError:
-                            continue
-                        except Exception:
-                            continue
-
-                    mae_curr = [round(float(i), 4) for i in mae_curr]
-                    mae_mean = round(float(np.mean(mae_curr)), 4)
-                    accuracy_curr = [round(float(i), 4) for i in 1 - np.asarray(mae_curr)]
-                    accuracy_mean = round(float(np.mean(accuracy_curr)), 4)
-
-                    for curr_acc in [mae_curr, accuracy_curr]:
-                        # Добавление данных в словарь для DataFrame с результатами вычисления точности
-                        if self._append_to_list_of_accuracy(curr_acc, out) is False:
-                            return False
-
-                    self._dict_of_accuracy.update({self.__df_accuracy_mean: [mae_mean, accuracy_mean]})
-                    # Отображение в DataFrame с данными
-                    self._df_accuracy = pd.DataFrame.from_dict(
-                        data=self._dict_of_accuracy, orient="index"
-                    ).transpose()
-                    self._df_accuracy.index = self.__df_accuracy_index
-                    self._df_accuracy.index.name = self.__df_accuracy_index_name
-
-                    # Информационное сообщение
-                    self._info(self._get_union_predictions_result, out=False)
-
-                    # Отображение
-                    if out is True:
-                        self._add_notebook_history_output(self._df_accuracy.iloc[0 : self.num_to_df_display_, :])
-
-                    self._info(
-                        self._get_union_predictions_results_mean.format(
-                            self._info_wrapper(str(mae_mean)), self._info_wrapper(str(accuracy_mean))
-                        ),
-                        out=False,
-                    )
-
-                clear_output(True)
-                # Отображение истории вывода сообщений в ячейке Jupyter
-                if out is True:
-                    self.show_notebook_history_output()
-
-                if logs is True:
-                    # Текущее время для лог-файла
-                    # см. datetime.fromtimestamp()
-                    curr_ts = str(datetime.now().timestamp()).replace(".", "_")
-
-                    name_logs_file = self.get_avt_predictions.__name__
-
-                    # Сохранение LOG
-                    res_save_logs_df_files = self._save_logs(
-                        self._df_files, name_logs_file + "_df_files_" + curr_ts
-                    )
-
-                    # Подсчет точности
-                    if accuracy is True:
-                        # Сохранение LOG
-                        res_save_logs_df_accuracy = self._save_logs(
-                            self._df_accuracy, name_logs_file + "_df_accuracy_" + curr_ts
-                        )
-
-                    if res_save_logs_df_files is True:
-                        # Сохранение LOG файла/файлов
-                        if accuracy is True and res_save_logs_df_accuracy is True:
-                            logs_s = self._logs_saves_true
-                        else:
-                            logs_s = self._logs_save_true
-
-                        self._info_true(logs_s, out=out)
-
-                return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/lab/text.py` & `oceanai-1.0.0a5/oceanai/modules/lab/prediction.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,56 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
-Текст
+Объединение аудио и видео
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-
-import warnings
-
 # Подавление Warning
-for warn in [UserWarning, FutureWarning]:
-    warnings.filterwarnings("ignore", category=warn)
+import warnings
+for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
 
-from dataclasses import dataclass  # Класс данных
+from dataclasses import dataclass # Класс данных
 
-import os  # Взаимодействие с файловой системой
+import os           # Взаимодействие с файловой системой
 import logging
-import requests  # Отправка HTTP запросов
-import liwc  # Анализатор лингвистических запросов и подсчета слов
+import requests     # Отправка HTTP запросов
 import numpy as np  # Научные вычисления
-import pandas as pd  # Обработка и анализ данных
-import subprocess
-import torchaudio  # Работа с аудио от Facebook
-import re
-import gradio
+import pandas as pd # Обработка и анализ данных
 
+from urllib.parse import urlparse
 from urllib.error import URLError
+from pathlib import Path # Работа с путями в файловой системе
 from sklearn.metrics import mean_absolute_error
-from datetime import datetime  # Работа со временем
-
-from transformers import (
-    MarianTokenizer,
-    MarianMTModel,
-    AutoModelForSeq2SeqLM,
-    AutoProcessor,
-    WhisperForConditionalGeneration,
-    BertTokenizer,
-    TFBertModel,
-)
-
-from keras import backend as K
-
-from urllib.parse import urlparse
-from pathlib import Path  # Работа с путями в файловой системе
+from datetime import datetime # Работа со временем
 
 # Типы данных
-from typing import List, Tuple, Optional, Union, Optional, Callable  # Типы данных
-from types import FunctionType
+from typing import List, Dict, Union, Optional, Callable
 
 from IPython.display import clear_output
 
 # Персональные
-from oceanai.modules.lab.download import Download  # Загрузка файлов
+from oceanai.modules.lab.audio import Audio # Аудио
+from oceanai.modules.lab.video import Video # Видео
 
 # Порог регистрации сообщений TensorFlow
 logging.disable(logging.WARNING)
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
-
-# Игнорировать конкретное предупреждение TensorFlow
-warnings.filterwarnings("ignore", category=FutureWarning, module="tensorflow")
-
-import tensorflow as tf  # Машинное обучение от Google
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
+import tensorflow as tf # Машинное обучение от Google
 import keras
 
-from oceanai.modules.lab.utils.attention import Attention  # Модуль внимания
-
-# Слой статистических функционалов (средние значения и стандартные отклонения)
-from oceanai.modules.lab.utils.addition import Addition
-
-
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
-class TextMessages(Download):
+class  PredictionMessages(Audio, Video):
     """Класс для сообщений
 
     Args:
         lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
         color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
         color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
         color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
@@ -92,69 +61,31 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._text_modality: str = self._(" (текстовая модальность) ...")
-        self._formation_text_model_hc: str = self._formation_model_hc + self._text_modality
-        self._formation_text_model_nn: str = self._formation_model_nn + self._text_modality
-        self._formation_text_model_b5: str = (
-            self._("Формирование нейросетевой архитектуры модели для получения " " оценок персональных качеств")
-            + self._text_modality
-        )
-
-        self._load_text_model_weights_hc: str = self._load_model_weights_hc + self._text_modality
-        self._load_text_model_weights_nn: str = self._load_model_weights_nn + self._text_modality
-        self._load_text_model_weights_b5: str = (
-            self._("Загрузка весов нейросетевой модели для получения " "оценок персональных качеств")
-            + self._text_modality
-        )
-
-        self._model_text_hc_not_formation: str = self._model_hc_not_formation + self._text_modality
-        self._model_text_nn_not_formation: str = self._model_nn_not_formation + self._text_modality
-        self._model_text_not_formation: str = (
-            self._oh
-            + self._(
-                "нейросетевая архитектура модели для получения "
-                "оценок по экспертным и нейросетевым признакам не "
-                "сформирована"
-            )
-            + self._text_modality
-        )
-
-        self._load_text_features: str = self._("Загрузка словаря с экспертными признаками ...")
-        self._load_text_features_error: str = self._oh + self._(
-            "не удалось загрузить словарь с экспертными признаками ..."
-        )
-
-        self._load_token_parser_error: str = self._oh + self._("не удалось считать лексикон LIWC ...")
-
-        self._load_translation_model: str = self._(
-            "Формирование токенизатора и нейросетевой модели машинного перевода ..."
-        )
-        self._load_bert_model: str = self._("Формирование токенизатора и нейросетевой модели BERT ...")
-        self._load_bert_model_error: str = self._oh + self._(
-            "не удалось загрузить токенизатор и нейросетевую модель BERT ..."
-        )
+        self._av_modality: str = self._(' (мультимодальное объединение) ...')
 
-        self._get_text_feature_info: str = self._("Извлечение признаков (экспертных и нейросетевых) из текста ...")
+        self._formation_av_models_b5: str = self._formation_models_b5 + self._av_modality
 
-        self._text_is_empty: str = self._oh + self._('текстовый файл "{}" пуст ...')
+        self._load_av_models_weights_b5: str = self._load_models_weights_b5 + self._av_modality
 
+        self._concat_av_pred_error: str = self._concat_pred_error + self._av_modality
+        self._norm_av_pred_error: str = self._norm_pred_error + self._av_modality
 
 # ######################################################################################################################
-# Текст
+# Аудио
 # ######################################################################################################################
 @dataclass
-class Text(TextMessages):
-    """Класс для обработки текста
+class Prediction(PredictionMessages):
+    """Класс для объединения аудио и видео
 
     Args:
         lang (str): Смотреть :attr:`~oceanai.modules.core.language.Language.lang`
         color_simple (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_simple`
         color_info (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_info`
         color_err (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_err`
         color_true (str): Смотреть :attr:`~oceanai.modules.core.settings.Settings.color_true`
@@ -164,1796 +95,1142 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__()  # Выполнение конструктора из суперкласса
-
-        # Нейросетевая модель **tf.keras.Model** для получения оценок по экспертным признакам
-        self._text_model_hc: Optional[tf.keras.Model] = None
-        # Нейросетевая модель **tf.keras.Model** для получения оценок по нейросетевым признакам
-        self._text_model_nn: Optional[tf.keras.Model] = None
-        self._text_model_b5: Optional[tf.keras.Model] = None
-
-        # Словарь для формирования экспертных признаков
-        self._text_features: str = (
-            "https://download.sberdisk.ru/download/file/473268573?token=X3NB5VYGyPn8mjw&filename=LIWC2007.txt",
-        )
-        # BERT модель
-        self._bert_multi_model: str = "https://download.sberdisk.ru/download/file/473319508?token=p8hYNIjxacEARxl&filename=bert-base-multilingual-cased.zip"
-
-        # Нейросетевая модель машинного перевода (RU -> EN)
-        self._translation_model: str = "Helsinki-NLP/opus-mt-ru-en"
-
-        self._tokenizer: Optional[MarianTokenizer] = None  # Токенизатор для машинного перевода
-        self._traslate_model: Optional[MarianMTModel] = None  # Нейросетевая модель для машинного перевода
+        super().__post_init__() # Выполнение конструктора из суперкласса
 
-        self._bert_tokenizer: Optional[BertTokenizer] = None
-        self._bert_model: Optional[TFBertModel] = None
-
-        self._path_to_transriber = "openai/whisper-base"
-
-        self._processor: Optional[AutoProcessor] = None
-        self._model_transcriptions: Optional[WhisperForConditionalGeneration] = None
+        # Нейросетевые модели **tf.keras.Model** для получения результатов оценки персональных качеств
+        self._av_models_b5: Dict[str, Optional[keras.engine.functional.Functional]] = dict(zip(
+            self._b5['en'], [None] * len(self._b5['en'])
+        ))
 
         # ----------------------- Только для внутреннего использования внутри класса
 
-        # Названия мультимодальных корпусов
-        self.__multi_corpora: List[str] = ["fi", "mupta"]
-
-        self.__lang_traslate: List[str] = ["ru", "en"]
-        self.lang_traslate: List[str] = self.__lang_traslate
-
-        self.__parse_text_features: Optional[FunctionType] = None  # Парсинг экспертных признаков
-        self.__category_text_features: List[str] = []  # Словарь с экспертными признаками
-
-        # Поддерживаемые текстовые форматы
-        self.__supported_text_formats: List[str] = ["txt"]
-
-        self.__contractions_dict = {
-            "ain't": "are not",
-            "'s": " is",
-            "aren't": "are not",
-            "can't": "cannot",
-            "can't've": "cannot have",
-            "'cause": "because",
-            "‘cause": "because",
-            "could've": "could have",
-            "couldn't": "could not",
-            "couldn't've": "could not have",
-            "didn't": "did not",
-            "doesn't": "does not",
-            "don't": "do not",
-            "hadn't": "had not",
-            "hadn't've": "had not have",
-            "hasn't": "has not",
-            "haven't": "have not",
-            "he'd": "he would",
-            "he'd've": "he would have",
-            "he'll": "he will",
-            "he'll've": "he will have",
-            "how'd": "how did",
-            "how'd'y": "how do you",
-            "how'll": "how will",
-            "how're": "how are",
-            "i'd": "i would",
-            "i'd've": "i would have",
-            "i'll": "i will",
-            "i 'll": "i will",
-            "i'll've": "i will have",
-            "i'm": "i am",
-            "i've": "i have",
-            "isn't": "is not",
-            "it'd": "it would",
-            "it'd've": "it would have",
-            "it'll": "it will",
-            "it'll've": "it will have",
-            "let's": "let us",
-            "ma'am": "madam",
-            "mayn't": "may not",
-            "might've": "might have",
-            "mightn't": "might not",
-            "mightn't've": "might not have",
-            "must've": "must have",
-            "mustn't": "must not",
-            "mustn't've": "must not have",
-            "needn't": "need not",
-            "needn't've": "need not have",
-            "o'clock": "of the clock",
-            "oughtn't": "ought not",
-            "oughtn't've": "ought not have",
-            "shan't": "shall not",
-            "sha'n't": "shall not",
-            "shan't've": "shall not have",
-            "she'd": "she would",
-            "she'd've": "she would have",
-            "she'll": "she will",
-            "she'll've": "she will have",
-            "should've": "should have",
-            "shouldn't": "should not",
-            "shouldn't've": "should not have",
-            "so've": "so have",
-            "that'd": "that would",
-            "that'll": "that will",
-            "that'd've": "that would have",
-            "there'd": "there would",
-            "there'd've": "there would have",
-            "there'll": "there will",
-            "there're": "there are",
-            "they'd": "they would",
-            "they'd've": "they would have",
-            "they'll": "they will",
-            "they'll've": "they will have",
-            "they're": "they are",
-            "they've": "they have",
-            "to've": "to have",
-            "wasn't": "was not",
-            "we'd": "we would",
-            "we'd've": "we would have",
-            "we'll": "we will",
-            "we'll've": "we will have",
-            "we're": "we are",
-            "we've": "we have",
-            "weren't": "were not",
-            "what'll": "what will",
-            "what'll've": "what will have",
-            "what're": "what are",
-            "what've": "what have",
-            "what'd": "what would",
-            "when've": "when have",
-            "where'd": "where did",
-            "where've": "where have",
-            "who'll": "who will",
-            "who'll've": "who will have",
-            "who've": "who have",
-            "who'd": "who would",
-            "why've": "why have",
-            "will've": "will have",
-            "won't": "will not",
-            "won't've": "will not have",
-            "why'd": "why would",
-            "would've": "would have",
-            "wouldn't": "would not",
-            "wouldn't've": "would not have",
-            "ya'll": "you all",
-            "y'all": "you all",
-            "y'all'd": "you all would",
-            "y'all'd've": "you all would have",
-            "y'all're": "you all are",
-            "y'all've": "you all have",
-            "you'd": "you would",
-            "you'd've": "you would have",
-            "you'll": "you will",
-            "you'll've": "you will have",
-            "you're": "you are",
-            "you've": "you have",
-        }
-
-        self.__forced_decoder_ids: Optional[List[Tuple[int, int]]] = None
-
-        self.__text_pred: str = ""
-
         self.__len_paths: int = 0  # Количество искомых файлов
         self.__local_path: Union[Callable[[str], str], None] = None  # Локальный путь
 
         # Ключи для точности
-        self.__df_accuracy_index: List[str] = ["MAE", "Accuracy"]
-        self.__df_accuracy_index_name: str = "Metrics"
-        self.__df_accuracy_mean: str = "Mean"
+        self.__df_accuracy_index: List[str] = ['MAE', 'Accuracy']
+        self.__df_accuracy_index_name: str = 'Metrics'
+        self.__df_accuracy_mean: str = 'Mean'
+
+        clear_output(False) # Удаление сообщения: INFO: Created TensorFlow Lite XNNPACK delegate for CPU)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     @property
-    def text_model_hc_(self) -> Optional[tf.keras.Model]:
-        """Получение нейросетевой модели **tf.keras.Model** для получения оценок по экспертным признакам
+    def av_models_b5_(self) -> Dict[str, Optional[keras.engine.functional.Functional]]:
+        """Получение нейросетевых моделей **tf.keras.Model** для получения результатов оценки персональных качеств
 
         Returns:
-            Optional[tf.keras.Model]: Нейросетевая модель **tf.keras.Model** или None
-        """
+            Dict: Словарь с нейросетевыми моделями **tf.keras.Model**
 
-        return self._text_model_hc
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-    @property
-    def text_model_nn_(self) -> Optional[tf.keras.Model]:
-        """Получение нейросетевой модели **tf.keras.Model** для получения оценок по нейросетевым признакам
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-        Returns:
-            Optional[tf.keras.Model]: Нейросетевая модель **tf.keras.Model** или None
-        """
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-        return self._text_model_nn
+                from oceanai.modules.lab.prediction import Prediction
 
-    @property
-    def text_model_b5_(self) -> Optional[tf.keras.Model]:
-        """Получение нейросетевой модели **tf.keras.Model** для получения оценок персональных качеств
+                pred = Prediction()
 
-        Returns:
-            Optional[tf.keras.Model]: Нейросетевая модель **tf.keras.Model** или None
-        """
+                pred.load_av_models_b5(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
 
-        return self._text_model_b5
+                pred.av_models_b5_
 
-    # ------------------------------------------------------------------------------------------------------------------
-    # Внутренние методы (приватные)
-    # ------------------------------------------------------------------------------------------------------------------
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
 
-    def __load_model_weights(
-        self,
-        url: str,
-        force_reload: bool = True,
-        info_text: str = "",
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Загрузка весов нейросетевой модели
+                [2022-12-08 15:21:22] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
 
-        .. note::
-            private (приватный метод)
+                --- Время выполнения: 0.305 сек. ---
 
-        Args:
-            url (str): Полный путь к файлу с весами нейросетевой модели
-            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
-            info_text (str): Текст для информационного сообщения
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                {
+                    'openness': <keras.engine.functional.Functional at 0x14eee5790>,
+                    'conscientiousness': <keras.engine.functional.Functional at 0x14f2d9d00>,
+                    'extraversion': <keras.engine.functional.Functional at 0x14f2fb190>,
+                    'agreeableness': <keras.engine.functional.Functional at 0x14f2c7fd0>,
+                    'neuroticism': <keras.engine.functional.Functional at 0x14f2ef940>
+                }
 
-        Returns:
-            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
-        """
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
 
-        try:
-            # Проверка аргументов
-            if (
-                type(url) is not str
-                or not url
-                or type(force_reload) is not bool
-                or type(info_text) is not str
-                or not info_text
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.__load_model_weights.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+                from oceanai.modules.lab.prediction import Prediction
 
-            if runtime:
-                self._r_start()
+                pred = Prediction()
 
-            # Информационное сообщение
-            self._info(info_text, last=False, out=out)
+                pred.av_models_b5_
 
-            sections = urlparse(url)  # Парсинг URL адреса
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
 
-            try:
-                # URL файл невалидный
-                if sections.scheme == "":
-                    raise requests.exceptions.InvalidURL
-            except requests.exceptions.InvalidURL:
-                url = os.path.normpath(url)
+                {
+                    'openness': None,
+                    'conscientiousness': None,
+                    'extraversion': None,
+                    'agreeableness': None,
+                    'neuroticism': None
+                }
+        """
 
-                try:
-                    if os.path.isfile(url) is False:
-                        raise FileNotFoundError  # Не файл
-                except FileNotFoundError:
-                    self._other_error(self._load_model_weights_error, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    self._url_last_filename = url
-                    return True
-            else:
-                try:
-                    if force_reload is False:
-                        clear_output(True)
-                    # Загрузка файла из URL
-                    res_download_file_from_url = self._download_file_from_url(
-                        url=url, force_reload=force_reload, runtime=False, out=out, run=True
-                    )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    # Файл загружен
-                    if res_download_file_from_url != 200:
-                        return False
+        return self._av_models_b5
 
-                    return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+    # ------------------------------------------------------------------------------------------------------------------
+    # Внутренние методы (приватные)
+    # ------------------------------------------------------------------------------------------------------------------
 
-    def __load_text_features(
-        self,
-        url: str,
-        force_reload: bool = True,
-        info_text: str = "",
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Загрузка словаря с экспертными признаками
+    def __norm_pred(self, pred_data: np.ndarray, len_nn: int = 16, out: bool = True) -> np.ndarray:
+        """Нормализация оценок по экспертным и нейросетевым признакам (мультимодальная)
 
         .. note::
             private (приватный метод)
 
         Args:
-            url (str): Полный путь к файлу с экспертными признаками
-            force_reload (bool): Принудительная загрузка файла с экспертными признаками из сети
-            info_text (str): Текст для информационного сообщения
+            pred_data (np.ndarray): Оценки
+            len_nn (int): Максимальный размер вектора оценок
             out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если словарь с экспертными признаками загружен, в обратном случае **False**
-        """
+            np.ndarray: Нормализованные оценки по экспертным и нейросетевым признакам (мультимодальная)
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-        try:
-            # Проверка аргументов
-            if (
-                type(url) is not str
-                or not url
-                or type(force_reload) is not bool
-                or type(info_text) is not str
-                or not info_text
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.__load_text_features.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-            if runtime:
-                self._r_start()
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-            # Информационное сообщение
-            self._info(info_text, last=False, out=out)
+                import numpy as np
+                from oceanai.modules.lab.prediction import Prediction
 
-            sections = urlparse(url)  # Парсинг URL адреса
+                pred = Prediction()
 
-            try:
-                # URL файл невалидный
-                if sections.scheme == "":
-                    raise requests.exceptions.InvalidURL
-            except requests.exceptions.InvalidURL:
-                url = os.path.normpath(url)
+                arr = np.array([
+                    [0.64113516, 0.6217892, 0.54451424, 0.6144415, 0.59334993],
+                    [0.6652424, 0.63606125, 0.572305, 0.63169795, 0.612515]
+                ])
 
-                try:
-                    if os.path.isfile(url) is False:
-                        raise FileNotFoundError  # Не файл
-                except FileNotFoundError:
-                    self._other_error(self._load_text_features_error, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    self._url_last_filename = url
-                    return True
-            else:
-                try:
-                    if force_reload is False:
-                        clear_output(True)
-                    # Загрузка файла из URL
-                    res_download_file_from_url = self._download_file_from_url(
-                        url=url, force_reload=force_reload, runtime=False, out=out, run=True
-                    )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    # Файл загружен
-                    if res_download_file_from_url != 200:
-                        return False
+                pred._Prediction__norm_pred(
+                    pred_data = arr,
+                    len_nn = 4,
+                    out = True
+                )
 
-                    return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                array([
+                    [0.64113516, 0.6217892 , 0.54451424, 0.6144415 , 0.59334993],
+                    [0.6652424 , 0.63606125, 0.572305  , 0.63169795, 0.612515],
+                    [0.65318878, 0.62892523, 0.55840962, 0.62306972, 0.60293247],
+                    [0.65318878, 0.62892523, 0.55840962, 0.62306972, 0.60293247]
+                ])
+
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                import numpy as np
+                from oceanai.modules.lab.prediction import Prediction
+
+                pred = Prediction()
+
+                arr = np.array([])
+
+                pred._Prediction__norm_pred(
+                    pred_data = arr,
+                    len_nn = 4,
+                    out = True
+                )
 
-    def __load_bert_model(
-        self,
-        url: str,
-        force_reload: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Загрузка нейросетевой модели BERT
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-10-20 22:03:17] Неверные типы или значения аргументов в "Prediction.__norm_pred" ...
+
+                array([], dtype=float64)
+        """
+
+        try:
+            # Проверка аргументов
+            if (type(pred_data) is not np.ndarray or len(pred_data) < 1 or type(len_nn) is not int or len_nn < 1
+                or type(out) is not bool): raise TypeError
+        except TypeError: self._inv_args(__class__.__name__, self.__norm_pred.__name__, out = out); return np.array([])
+        else:
+            try:
+                if pred_data.shape[0] < len_nn:
+                    return np.pad(pred_data, ((0, len_nn - pred_data.shape[0]), (0, 0)), 'mean')
+                return pred_data[:len_nn]
+            except ValueError: self._other_error(self._norm_av_pred_error, last = False, out = out); return np.array([])
+            except Exception: self._other_error(self._unknown_err, out = out); return np.array([])
+
+    def __concat_pred_av(
+        self, pred_hc_audio: np.ndarray, pred_nn_audio: np.ndarray,
+        pred_hc_video: np.ndarray, pred_nn_video: np.ndarray, out: bool = True
+    ) -> List[Optional[np.ndarray]]:
+        """Конкатенация оценок по экспертным и нейросетевым признакам (мультимодальная)
 
         .. note::
             private (приватный метод)
 
         Args:
-            url (str): Полный путь к файлу с нейросетевой модели BERT
-            force_reload (bool): Принудительная загрузка файла с нейросетевой модели BERT из сети
+            pred_hc_audio (np.ndarray): Оценки по экспертным признакам (аудио модальность)
+            pred_nn_audio (np.ndarray): Оценки по нейросетевым признакам (аудио модальность)
+            pred_hc_video (np.ndarray): Оценки по экспертным признакам (видео модальность)
+            pred_nn_video (np.ndarray): Оценки по нейросетевым признакам (видео модальность)
             out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если нейросетевая модель BERT загружена, в обратном случае **False**
+            List[Optional[np.ndarray]]: Конкатенированные оценки по экспертным и нейросетевым признакам
+
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
+
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
+
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
+
+                import numpy as np
+                from oceanai.modules.lab.prediction import Prediction
+
+                pred = Prediction()
+
+                arr_hc_audio = np.array([
+                    [0.64113516, 0.6217892, 0.54451424, 0.6144415, 0.59334993],
+                    [0.6652424, 0.63606125, 0.572305, 0.63169795, 0.612515]
+                ])
+
+                arr_nn_audio = np.array([
+                    [0.56030345, 0.7488746, 0.44648764, 0.59893465, 0.5701077],
+                    [0.5900006, 0.7652722, 0.4795154, 0.6409055, 0.6088242]
+                ])
+                arr_hc_video = np.array([
+                    [0.67113516, 0.6517892, 0.59451424, 0.6344415, 0.53334993],
+                    [0.6852424, 0.62606125, 0.562305, 0.67169795, 0.672515]
+                ])
+
+                arr_nn_video = np.array([
+                    [0.58030345, 0.7788746, 0.47648764, 0.53893465, 0.5901077],
+                    [0.5100006, 0.7452722, 0.4495154, 0.6909055, 0.6488242]
+                ])
+
+                pred._Prediction__concat_pred_av(
+                    pred_hc_audio = arr_hc_audio,
+                    pred_nn_audio = arr_nn_audio,
+                    pred_hc_video = arr_hc_video,
+                    pred_nn_video = arr_nn_video,
+                    out = True
+                )
         """
 
         try:
             # Проверка аргументов
-            if (
-                type(url) is not str
-                or not url
-                or type(force_reload) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(pred_hc_audio) is not np.ndarray or len(pred_hc_audio) < 1
+                or type(pred_nn_audio) is not np.ndarray or len(pred_nn_audio) < 1
+                or type(pred_hc_video) is not np.ndarray or len(pred_hc_video) < 1
+                or type(pred_nn_video) is not np.ndarray or len(pred_nn_video) < 1
+                or type(out) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__load_bert_model.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.__concat_pred_av.__name__, out = out); return []
         else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
-
-            if runtime:
-                self._r_start()
+            # Нормализация оценок по экспертным и нейросетевым признакам (аудио модальность)
+            pred_hc_audio_norm = self.__norm_pred(pred_hc_audio, out = False)
+            pred_nn_audio_norm = self.__norm_pred(pred_nn_audio, out = False)
+
+            # Нормализация оценок по экспертным и нейросетевым признакам (видео модальность)
+            pred_hc_video_norm = self.__norm_pred(pred_hc_video, out = False)
+            pred_nn_video_norm = self.__norm_pred(pred_nn_video, out = False)
+
+            if (len(pred_hc_audio_norm) == 0 or len(pred_nn_audio_norm) == 0
+                    or len(pred_hc_video_norm) == 0 or len(pred_nn_video_norm) == 0):
+                self._error(self._concat_av_pred_error, out = out); return []
 
-            sections = urlparse(url)  # Парсинг URL адреса
+            concat = []
 
             try:
-                # URL файл невалидный
-                if sections.scheme == "":
-                    raise requests.exceptions.InvalidURL
-            except requests.exceptions.InvalidURL:
-                url = os.path.normpath(url)
-
-                try:
-                    if os.path.isfile(url) is False:
-                        raise FileNotFoundError  # Не файл
-                except FileNotFoundError:
-                    self._other_error(self._load_bert_model_error, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    self._url_last_filename = url
-                    return True
-            else:
-                try:
-                    if force_reload is False:
-                        clear_output(True)
-                    # Загрузка файла из URL
-                    res_download_file_from_url = self._download_file_from_url(
-                        url=url, force_reload=force_reload, runtime=False, out=out, run=True
+                # Проход по всем персональным качествам личности человека
+                for i in range(len(self._b5['en'])):
+                    concat.append(
+                        np.hstack((
+                            np.asarray(pred_hc_audio_norm)[:, i], np.asarray(pred_nn_audio_norm)[:, i],
+                            np.asarray(pred_hc_video_norm)[:, i], np.asarray(pred_nn_video_norm)[:, i]
+                        ))
                     )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
-                else:
-                    # Файл загружен
-                    if res_download_file_from_url != 200:
-                        return False
+            except IndexError: self._other_error(self._concat_av_pred_error, last = False, out = out); return []
+            except Exception: self._other_error(self._unknown_err, out = out); return []
 
-                    return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+            return concat
 
-    def __translate_and_extract_features(
-        self,
-        text: str,
-        lang: str,
-        show_text: bool = False,
-        last: bool = False,
-        out: bool = True,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """Извлечение признаков из текста
+    def __load_av_model_b5(
+        self, show_summary: bool = False, out: bool = True
+    ) -> Optional[keras.engine.functional.Functional]:
+        """Формирование нейросетевой архитектуры модели для получения результата оценки персонального качества
 
         .. note::
             private (приватный метод)
 
         Args:
-            text (str): Текст
-            lang (str): Язык
-            show_text (bool): Отображение текста
-            last (bool): Замена последнего сообщения
+            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
             out (bool): Отображение
 
         Returns:
-            Tuple[np.ndarray, np.ndarray]: Кортеж с двумя np.ndarray:
+            Optional[keras.engine.functional.Functional]:
+                **None** если неверные типы или значения аргументов, в обратном случае нейросетевая модель
+                **tf.keras.Model** для получения результата оценки персонального качества
 
-                1. np.ndarray с экспертными признаками
-                2. np.ndarray с нейросетевыми признаками
-        """
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-        contractions_re = re.compile("(%s)" % "|".join(self.__contractions_dict.keys()))
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-        expand_contractions = lambda s: contractions_re.sub(lambda match: self.__contractions_dict[match.group(0)], s)
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-        get_norm_text = lambda text: re.sub(
-            r"(?<=[.,])(?=[^\s])",
-            " ",
-            re.sub(
-                r"\[[^\[\]]+\]",
-                "",
-                expand_contractions(
-                    re.sub(
-                        r'[.,"\'?:!/;]',
-                        "",
-                        re.sub(r"((?<=^)(\s*?(\-)??))|(((\-)??\s*?)(?=$))", "", text.lower().strip()),
-                    )
-                ),
-            ),
-        )
-
-        norm_features = lambda feature, length: np.pad(
-            feature[:length, :], ((0, max(0, length - feature.shape[0])), (0, 0)), "constant"
-        )
-
-        if lang == self.__lang_traslate[0]:
-            if len(text) > 700:
-                translation = ""
-                for sentence in text.split(".")[:-1]:
-                    input_ids = self._tokenizer.encode(sentence + ".", return_tensors="pt")
-                    outputs = self._traslate_model.generate(input_ids.to(self._device), max_new_tokens=4000)
-                    translation += self._tokenizer.decode(outputs[0], skip_special_tokens=True) + " "
-            else:
-                input_ids = self._tokenizer.encode(text, return_tensors="pt")
-                outputs = self._traslate_model.generate(input_ids.to(self._device), max_new_tokens=4000)
-                translation = self._tokenizer.decode(outputs[0], skip_special_tokens=True)
-            translation = re.sub(r"(?<=[.,])(?=[^\s])", r" ", translation)
-        else:
-            translation = text
+                from oceanai.modules.lab.prediction import Prediction
 
-        text = get_norm_text(text)
-        translation = get_norm_text(translation)
+                pred = Prediction()
 
-        encoded_input = self._bert_tokenizer(text, return_tensors="tf")
-        dict_new = {}
-        if encoded_input["input_ids"].shape[1] > 512:
-            dict_new["input_ids"] = encoded_input["input_ids"][:, :512]
-            dict_new["token_type_ids"] = encoded_input["token_type_ids"][:, :512]
-            dict_new["attention_mask"] = encoded_input["attention_mask"][:, :512]
-            encoded_input = dict_new
-        features_bert = self._bert_model(encoded_input)[0][0]
-
-        features_liwc = []
-        for i in translation.split(" "):
-            curr_f = np.zeros((1, 64))
-            for j in self.__parse_text_features(i):
-                curr_f[:, self.__category_text_features.index(j)] += 1
-            features_liwc.extend(curr_f)
-
-        features_liwc = np.array(features_liwc)
-
-        if lang == self.__lang_traslate[0]:
-            features_bert = norm_features(features_bert, 414)
-            features_liwc = norm_features(features_liwc, 365)
-        elif lang == self.__lang_traslate[1]:
-            features_bert = norm_features(features_bert, 104)
-            features_liwc = norm_features(features_liwc, 89)
-
-        if not show_text:
-            text = None
-
-        if last is False:
-            # Статистика извлеченных признаков из текста
-            self._stat_text_features(
-                last=last,
-                out=out,
-                shape_hc_features=np.array(features_liwc).shape,
-                shape_nn_features=np.array(features_bert).shape,
-                text=text,
-            )
-
-        return features_liwc, features_bert
-
-    def __process_audio_and_extract_features(
-        self, path: str, win: int, lang: str, show_text: bool, last: bool, out: bool
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        if not self._processor:
-            self._processor = AutoProcessor.from_pretrained(self._path_to_transriber)
-            self._model_transcriptions = WhisperForConditionalGeneration.from_pretrained(self._path_to_transriber).to(
-                self._device
-            )
-
-        if lang == self.__lang_traslate[0]:
-            self.__forced_decoder_ids = self._processor.get_decoder_prompt_ids(language=lang, task="transcribe")
-
-        path_to_wav = os.path.join(str(Path(path).parent), Path(path).stem + "." + "wav")
-
-        if not Path(path_to_wav).is_file():
-            if Path(path).suffix not in ["mp3", "wav"]:
-                ff_audio = "ffmpeg -loglevel quiet -i {} -vn -acodec pcm_s16le -ar 44100 -ac 2 {}".format(
-                    path, path_to_wav
+                pred._Prediction__load_av_model_b5(
+                    show_summary = True, out = True
                 )
-                call_audio = subprocess.call(ff_audio, shell=True)
 
-                try:
-                    if call_audio == 1:
-                        raise OSError
-                except OSError:
-                    self._other_error(self._unknown_err, last=last, out=out)
-                    return np.empty([]), np.empty([])
-                except Exception:
-                    self._other_error(self._unknown_err, last=last, out=out)
-                    return np.empty([]), np.empty([])
-                else:
-                    wav, sr = torchaudio.load(path_to_wav)
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
 
-                    if wav.size(0) > 1:
-                        wav = wav.mean(dim=0, keepdim=True)
+                Model: "model"
+                _________________________________________________________________
+                 Layer (type)                Output Shape              Param #
+                =================================================================
+                 input_1 (InputLayer)        [(None, 64)]              0
 
-                    if sr != 16000:
-                        transform = torchaudio.transforms.Resample(orig_freq=sr, new_freq=16000)
-                        wav = transform(wav)
-                        sr = 16000
-
-                    wav = wav.squeeze(0)
-
-                    for start in range(0, len(wav), win):
-                        inputs = self._processor(wav[start : start + win], sampling_rate=16000, return_tensors="pt")
-                        input_features = inputs.input_features.to(self._device)
-                        if lang == self.__lang_traslate[0]:
-                            generated_ids = self._model_transcriptions.generate(
-                                input_features=input_features,
-                                forced_decoder_ids=self.__forced_decoder_ids,
-                                max_new_tokens=448,
-                            )
-                        elif lang == self.__lang_traslate[1]:
-                            generated_ids = self._model_transcriptions.generate(
-                                input_features=input_features, max_new_tokens=448
-                            )
-                        transcription = self._processor.batch_decode(generated_ids, skip_special_tokens=True)[0]
-                        self.__text_pred += transcription
+                 dense_1 (Dense)             (None, 1)                 65
 
-                    return self.__translate_and_extract_features(self.__text_pred, lang, show_text, last, out)
-        else:
-            wav, sr = torchaudio.load(path_to_wav)
+                 activ_1 (Activation)        (None, 1)                 0
 
-            if wav.size(0) > 1:
-                wav = wav.mean(dim=0, keepdim=True)
+                =================================================================
+                Total params: 65
+                Trainable params: 65
+                Non-trainable params: 0
+                _________________________________________________________________
+                <keras.engine.functional.Functional at 0x147892ee0>
 
-            if sr != 16000:
-                transform = torchaudio.transforms.Resample(orig_freq=sr, new_freq=16000)
-                wav = transform(wav)
-                sr = 16000
-
-            wav = wav.squeeze(0)
-
-            for start in range(0, len(wav), win):
-                inputs = self._processor(wav[start : start + win], sampling_rate=16000, return_tensors="pt")
-                input_features = inputs.input_features.to(self._device)
-                if lang == self.__lang_traslate[0]:
-                    generated_ids = self._model_transcriptions.generate(
-                        input_features=input_features, forced_decoder_ids=self.__forced_decoder_ids
-                    )
-                elif lang == self.__lang_traslate[1]:
-                    generated_ids = self._model_transcriptions.generate(input_features=input_features)
-                transcription = self._processor.batch_decode(generated_ids, skip_special_tokens=True)[0]
-                self.__text_pred += transcription
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-            return self.__translate_and_extract_features(self.__text_pred, lang, show_text, last, out)
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
 
-    def __load_text_model_b5(self, show_summary: bool = False, out: bool = True) -> Optional[tf.keras.Model]:
-        """Формирование нейросетевой архитектуры модели для получения оценок персональных качеств
+                from oceanai.modules.lab.prediction import Prediction
 
-        .. note::
-            private (приватный метод)
+                pred = Prediction()
 
-        Args:
-            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
-            out (bool): Отображение
+                pred._Prediction__load_av_model_b5(
+                    show_summary = True, out = []
+                )
 
-        Returns:
-            Optional[tf.keras.Model]:
-                **None** если неверные типы или значения аргументов, в обратном случае нейросетевая модель
-                **tf.keras.Model** для получения оценок персональных качеств
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
+
+                [2022-10-17 10:53:03] Неверные типы или значения аргументов в "Prediction.__load_av_model_b5" ...
         """
 
         try:
             # Проверка аргументов
-            if type(show_summary) is not bool or type(out) is not bool:
-                raise TypeError
+            if type(show_summary) is not bool or type(out) is not bool: raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.__load_text_model_b5.__name__, out=out)
-            return None
+            self._inv_args(__class__.__name__, self.__load_av_model_b5.__name__, out = out); return None
         else:
-            input_1 = tf.keras.Input(shape=(5,))
-            input_2 = tf.keras.Input(shape=(5,))
-            X = tf.keras.backend.concatenate((input_1, input_2), axis=1)
-            X = tf.keras.layers.Dense(5, activation="sigmoid")(X)
+            input_1 = tf.keras.Input(shape = (64,), name = 'input_1')
+            x = tf.keras.layers.Dense(units = 1, name = 'dense_1')(input_1)
+            x = tf.keras.layers.Activation('sigmoid', name = 'activ_1')(x)
 
-            model = tf.keras.models.Model(inputs=[input_1, input_2], outputs=X)
+            model = tf.keras.Model(inputs = input_1, outputs = x)
 
-            if show_summary and out:
-                model.summary()
+            if show_summary and out: model.summary()
 
             return model
 
     # ------------------------------------------------------------------------------------------------------------------
-    # Внутренние методы (защищенные)
+    # Внешние методы
     # ------------------------------------------------------------------------------------------------------------------
 
-    def _get_text_features(
-        self,
-        path: str,
-        asr: bool = False,
-        lang: str = "ru",
-        show_text: bool = False,
-        last: bool = False,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """Извлечение признаков из текста (без очистки истории вывода сообщений в ячейке Jupyter)
-
-        .. note::
-            protected (защищенный метод)
+    def load_av_models_b5(
+        self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
+    ) -> bool:
+        """Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств
 
         Args:
-            path (str): Путь к видеофайлу или текст
-            asr (bool): Автоматическое распознавание речи
-            lang (str): Язык
-            show_text (bool): Отображение текста
-            last (bool): Замена последнего сообщения
+            show_summary (bool): Отображение последней сформированной нейросетевой архитектуры моделей
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            Tuple[np.ndarray, np.ndarray]: Кортеж с двумя np.ndarray:
-
-                1. np.ndarray с экспертными признаками
-                2. np.ndarray с нейросетевыми признаками
-        """
-
-        try:
-            # Проверка аргументов
-            if (
-                (type(path) is not str or not path) and (type(path) is not gradio.utils.NamedString)
-                or type(asr) is not bool
-                or not isinstance(lang, str)
-                or lang not in self.__lang_traslate
-                or type(last) is not bool
-                or type(show_text) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self._get_text_features.__name__, last=last, out=out)
-            return np.empty([]), np.empty([])
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, last=last, out=out)
-                return np.empty([]), np.empty([])
-
-            if runtime:
-                self._r_start()
-
-            if last is False:
-                # Информационное сообщение
-                self._info(self._get_text_feature_info, out=False)
-                if out:
-                    self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            bool: **True** если нейросетевые архитектуры модели сформированы, в обратном случае **False**
 
-            win = 400000
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-            try:
-                self.__text_pred = ""
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-                if os.path.isfile(path) is False:
-                    raise FileNotFoundError  # Не файл
-            except FileNotFoundError:
-                try:
-                    path_to_text = os.path.join(
-                        str(Path(path).parent), Path(path).stem + "." + self.__supported_text_formats[0]
-                    )
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-                    if os.path.isfile(path_to_text) is False:
-                        raise FileNotFoundError  # Не текстовый файл
-                except FileNotFoundError:
-                    self.__text_pred = path.strip()
-
-                    return self.__translate_and_extract_features(self.__text_pred, lang, show_text, last, out)
-
-                except Exception:
-                    self._other_error(self._unknown_err, last=last, out=out)
-                    return np.empty([]), np.empty([])
-                else:
-                    try:
-                        with open(path_to_text, "r", encoding="utf-8") as file:
-                            lines = file.readlines()
-                            self.__text_pred = " ".join(line.strip() for line in lines)
-                    except Exception:
-                        self._other_error(self._unknown_err, last=last, out=out)
-                        return np.empty([]), np.empty([])
-                    else:
-                        try:
-                            if not self.__text_pred:
-                                raise ValueError
-                        except ValueError:
-                            self._other_error(
-                                self._text_is_empty.format(self._info_wrapper(path_to_text)), last=last, out=out
-                            )
+                from oceanai.modules.lab.prediction import Prediction
 
-                            return np.empty([]), np.empty([])
-                        else:
-                            return np.empty([]), np.empty([])
-            except Exception:
-                self._other_error(self._unknown_err, last=last, out=out)
-                return np.empty([]), np.empty([])
-            else:
-                try:
-                    path_to_text = os.path.join(
-                        str(Path(path).parent), Path(path).stem + "." + self.__supported_text_formats[0]
-                    )
+                pred = Prediction()
 
-                    if os.path.isfile(path_to_text) is False:
-                        raise FileNotFoundError  # Не текстовый файл
-                except FileNotFoundError:
-                    return self.__process_audio_and_extract_features(path, win, lang, show_text, last, out)
-                except Exception:
-                    self._other_error(self._unknown_err, last=last, out=out)
-                    return np.empty([]), np.empty([])
-                else:
-                    try:
-                        with open(path_to_text, "r", encoding="utf-8") as file:
-                            lines = file.readlines()
-                            self.__text_pred = " ".join(line.strip() for line in lines)
-                    except Exception:
-                        self._other_error(self._unknown_err, last=last, out=out)
-                        return np.empty([]), np.empty([])
-                    else:
-                        try:
-                            if not self.__text_pred:
-                                raise ValueError
-                        except ValueError:
-                            self._other_error(
-                                self._text_is_empty.format(self._info_wrapper(path_to_text)), last=last, out=out
-                            )
-                            return np.empty([]), np.empty([])
-                        else:
-                            if asr:
-                                return self.__process_audio_and_extract_features(path, win, lang, show_text, last, out)
-                            else:
-                                return self.__translate_and_extract_features(
-                                    self.__text_pred, lang, show_text, last, out
-                                )
-            finally:
-                if runtime:
-                    self._r_end(out=out)
-
-    # ------------------------------------------------------------------------------------------------------------------
-    # Внешние методы
-    # ------------------------------------------------------------------------------------------------------------------
-
-    def load_text_model_hc(
-        self, corpus: str = "", show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
-    ):
-        """Формирование нейросетевой архитектуры модели для получения оценок по экспертным признакам
-
-        Args:
-            corpus (str): Корпус для тестирования нейросетевой модели
-            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
-
-        Returns:
-            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
-        """
-
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
-
-        try:
-            # Проверка аргументов
-            if (
-                type(corpus) is not str
-                or not corpus
-                or (corpus in self.__multi_corpora) is False
-                or type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.load_text_model_hc.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
-
-            if runtime:
-                self._r_start()
-
-            # Информационное сообщение
-            self._info(self._formation_text_model_hc, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
-
-            # fi
-            if corpus is self.__multi_corpora[0]:
-                input_shape = (89, 64)
-            # mupta
-            elif corpus is self.__multi_corpora[1]:
-                input_shape = (365, 64)
-            else:
-                input_shape = (89, 64)
+                pred.load_av_models_b5(
+                    show_summary = True, out = True,
+                    runtime = True, run = True
+                )
 
-            input_lstm = tf.keras.Input(shape=input_shape, name="model_hc_input")
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
 
-            x_lstm = tf.keras.layers.Bidirectional(
-                tf.keras.layers.LSTM(32, return_sequences=True), name="model_hc_bilstm_1"
-            )(input_lstm)
+                [2022-12-08 15:19:30] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
 
-            x_attention = Attention(use_scale=False, score_mode="dot", name="model_hc_attention")(x_lstm, x_lstm)
+                Model: "model_4"
+                _________________________________________________________________
+                 Layer (type)                Output Shape              Param #
+                =================================================================
+                 input_1 (InputLayer)        [(None, 64)]              0
 
-            x_dence = tf.keras.layers.Dense(32 * 2, name="model_hc_dence_2", activation="relu")(input_lstm)
-            x_dence = tf.keras.layers.Bidirectional(
-                tf.keras.layers.LSTM(32, return_sequences=True), name="model_hc_bilstm_2"
-            )(x_dence)
+                 dense_1 (Dense)             (None, 1)                 65
 
-            x = tf.keras.layers.Add()([x_lstm, x_attention, x_dence])
+                 activ_1 (Activation)        (None, 1)                 0
 
-            # m = tf.reduce_mean(x, axis=1)
-            # s = tf.reduce_std(x, axis=1)
-            # m = tf.keras.backend.mean(x, axis=1)
-            # s = tf.keras.backend.std(x, axis=1)
-        # print('add', K.concatenate((m, s), axis=1).shape)
-            # x = tf.concate((m, s), axis=1)
+                =================================================================
+                Total params: 65
+                Trainable params: 65
+                Non-trainable params: 0
+                _________________________________________________________________
+                --- Время выполнения: 0.141 сек. ---
 
-            # print(x.shape)
+                True
 
-            x = Addition(name="model_hc_add")(x)
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-            x = tf.keras.layers.Dense(5, activation="sigmoid")(x)
-            self._text_model_hc = tf.keras.Model(input_lstm, outputs=x, name="model_hc")
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
 
-            if show_summary and out:
-                self._text_model_hc.summary()
+                from oceanai.modules.lab.prediction import Prediction
 
-            if runtime:
-                self._r_end(out=out)
+                pred = Prediction()
 
-            return True
+                pred.load_av_models_b5(
+                    show_summary = 1, out = True,
+                    runtime = True, run = True
+                )
 
-    def load_text_model_nn(
-        self, corpus: str = "", show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> bool:
-        """Формирование нейросетевой архитектуры для получения оценок по нейросетевым признакам
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
 
-        Args:
-            corpus (str): Корпус для тестирования нейросетевой модели
-            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                [2022-12-08 15:20:36] Неверные типы или значения аргументов в "Prediction.load_av_models_b5" ...
 
-        Returns:
-            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
+                False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(corpus) is not str
-                or not corpus
-                or (corpus in self.__multi_corpora) is False
-                or type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+            if (type(show_summary) is not bool or type(out) is not bool or type(runtime) is not bool or type(run) is
+                not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.load_text_model_nn.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_av_models_b5.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             # Информационное сообщение
-            self._info(self._formation_text_model_nn, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
-
-            # fi
-            if corpus is self.__multi_corpora[0]:
-                input_shape = (104, 768)
-            # mupta
-            elif corpus is self.__multi_corpora[1]:
-                input_shape = (414, 768)
-            else:
-                input_shape = (104, 768)
-
-            input_lstm = tf.keras.Input(shape=input_shape, name="model_nn_input")
-
-            x = tf.keras.layers.Bidirectional(
-                tf.keras.layers.LSTM(32, return_sequences=True), name="model_nn_bilstm_1"
-            )(input_lstm)
+            self._info(self._formation_av_models_b5, last = False, out = False)
+            if out: self.show_notebook_history_output() # Отображение истории вывода сообщений в ячейке Jupyter
 
-            x = Attention(use_scale=False, score_mode="dot", name="model_nn_attention")(x, x)
+            for key, _ in self._av_models_b5.items():
+                self._av_models_b5[key] = self.__load_av_model_b5()
 
-            x = tf.keras.layers.Dense(128, name="model_nn_dence_2")(x)
-            x = Addition(name="model_nn_add")(x)
-            x = tf.keras.layers.Dense(128, name="model_nn_dence_3")(x)
+            if show_summary and out: self._av_models_b5[key].summary()
 
-            x = tf.keras.layers.Dense(5, activation="sigmoid")(x)
-            self._text_model_nn = tf.keras.Model(input_lstm, outputs=x, name="model_nn")
-
-            if show_summary and out:
-                self._text_model_nn.summary()
-
-            if runtime:
-                self._r_end(out=out)
+            if runtime: self._r_end(out = out)
 
             return True
 
-    def load_text_model_b5(
-        self, show_summary: bool = False, out: bool = True, runtime: bool = True, run: bool = True
+    def load_av_models_weights_b5(
+        self, url_openness: str, url_conscientiousness: str, url_extraversion: str, url_agreeableness: str,
+        url_neuroticism: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
     ) -> bool:
-        """Формирование нейросетевой архитектуры модели для получения результатов оценки персональных качеств
+        """Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств
 
         Args:
-            show_summary (bool): Отображение сформированной нейросетевой архитектуры модели
+            url_openness (str): Полный путь к файлу с весами нейросетевой модели (открытость опыту)
+            url_conscientiousness (str): Полный путь к файлу с весами нейросетевой модели (добросовестность)
+            url_extraversion (str): Полный путь к файлу с весами нейросетевой модели (экстраверсия)
+            url_agreeableness (str): Полный путь к файлу с весами нейросетевой модели (доброжелательность)
+            url_neuroticism (str): Полный путь к файлу с весами нейросетевой модели (нейротизм)
+            force_reload (bool): Принудительная загрузка файлов с весами нейросетевых моделей из сети
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если нейросетевая архитектура модели сформирована, в обратном случае **False**
-        """
-
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+            bool: **True** если веса нейросетевых моделей загружены, в обратном случае **False**
 
-        try:
-            # Проверка аргументов
-            if (
-                type(show_summary) is not bool
-                or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.load_text_model_b5.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+        .. dropdown:: Примеры
+            :class-body: sd-pr-5
 
-            if runtime:
-                self._r_start()
+            :bdg-success:`Верно` :bdg-light:`-- 1 --`
 
-            # Информационное сообщение
-            self._info(self._formation_text_model_b5, last=False, out=False)
-            if out:
-                self.show_notebook_history_output()  # Отображение истории вывода сообщений в ячейке Jupyter
+            .. code-cell:: python
+                :execution-count: 1
+                :linenos:
+                :tab-width: 8
 
-            self._text_model_b5 = self.__load_text_model_b5()
+                from oceanai.modules.lab.prediction import Prediction
 
-            if show_summary and out:
-                self._text_model_b5.summary()
+                pred = Prediction()
 
-            if runtime:
-                self._r_end(out=out)
+                pred.load_av_models_b5(
+                    show_summary = False, out = True,
+                    runtime = True, run = True
+                )
 
-            return True
+            .. output-cell::
+                :execution-count: 1
+                :linenos:
+
+                [2022-12-08 16:56:37] Формирование нейросетевых архитектур моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
+
+                --- Время выполнения: 0.075 сек. ---
+
+                True
+
+            .. code-cell:: python
+                :execution-count: 2
+                :linenos:
+                :tab-width: 8
+
+                pred.path_to_save_ = './models'
+                pred.chunk_size_ = 2000000
+
+                url_openness = pred.weights_for_big5_['av']['b5']['openness']['sberdisk']
+                url_conscientiousness = pred.weights_for_big5_['av']['b5']['conscientiousness']['sberdisk']
+                url_extraversion = pred.weights_for_big5_['av']['b5']['extraversion']['sberdisk']
+                url_agreeableness = pred.weights_for_big5_['av']['b5']['agreeableness']['sberdisk']
+                url_neuroticism = pred.weights_for_big5_['av']['b5']['neuroticism']['sberdisk']
+
+                pred.load_av_models_weights_b5(
+                    url_openness = url_openness,
+                    url_conscientiousness = url_conscientiousness,
+                    url_extraversion = url_extraversion,
+                    url_agreeableness = url_agreeableness,
+                    url_neuroticism = url_neuroticism,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
 
-    def load_text_model_weights_hc(
-        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> bool:
-        """Загрузка весов нейросетевой модели для получения оценок по экспертным признакам
+            .. output-cell::
+                :execution-count: 2
+                :linenos:
 
-        Args:
-            url (str): Полный путь к файлу с весами нейросетевой модели
-            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                [2022-12-08 17:03:18] Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
 
-        Returns:
-            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
-        """
+                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-14-35.h5" (100.0%) ... Открытость опыту
 
-        if runtime:
-            self._r_start()
+                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-08-10.h5" (100.0%) ... Добросовестность
 
-        if self.__load_model_weights(url, force_reload, self._load_text_model_weights_hc, out, False, run) is True:
-            try:
-                self._text_model_hc.load_weights(self._url_last_filename)
-                self._text_model_hc = tf.keras.models.Model(
-                    inputs=self._text_model_hc.input,
-                    outputs=[self._text_model_hc.output, self._text_model_hc.get_layer("model_hc_add").output],
-                )
+                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-17-57.h5" (100.0%) ... Экстраверсия
 
-            except Exception:
-                self._error(self._model_text_hc_not_formation, out=out)
-                return False
-            else:
-                return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+                [2022-12-08 17:03:21] Загрузка файла "weights_2022-08-28_11-25-11.h5" (100.0%) ... Доброжелательность
 
-        return False
+                [2022-12-08 17:03:21] Загрузка файла "weights_2022-06-14_21-44-09.h5" (100.0%) ... Нейротизм
 
-    def load_text_model_weights_nn(
-        self, url: str, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> bool:
-        """Загрузка весов нейросетевой модели для получения оценок по нейросетевым признакам
+                --- Время выполнения: 3.399 сек. ---
 
-        Args:
-            url (str): Полный путь к файлу с весами нейросетевой модели
-            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                True
 
-        Returns:
-            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
-        """
+            :bdg-danger:`Ошибка` :bdg-light:`-- 1 --`
 
-        if runtime:
-            self._r_start()
+            .. code-cell:: python
+                :execution-count: 3
+                :linenos:
+                :tab-width: 8
 
-        if self.__load_model_weights(url, force_reload, self._load_text_model_weights_nn, out, False, run) is True:
-            try:
-                self._text_model_nn.load_weights(self._url_last_filename)
-                self._text_model_nn = tf.keras.models.Model(
-                    inputs=self._text_model_nn.input,
-                    outputs=[self._text_model_nn.output, self._text_model_nn.get_layer("model_nn_dence_3").output],
-                )
-            except Exception:
-                self._error(self._model_text_nn_not_formation, out=out)
-                return False
-            else:
-                return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+                from oceanai.modules.lab.prediction import Prediction
 
-        return False
+                pred = Prediction()
 
-    def load_text_model_weights_b5(
-        self,
-        url: str,
-        force_reload: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ) -> bool:
-        """Загрузка весов нейросетевой модели для получения оценок персональных качеств
+                pred.path_to_save_ = './models'
+                pred.chunk_size_ = 2000000
 
-        Args:
-            url (str): Полный путь к файлу с весами нейросетевой модели
-            force_reload (bool): Принудительная загрузка файлов с весами нейросетевых моделей из сети
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                url_openness = pred.weights_for_big5_['av']['b5']['openness']['sberdisk']
+                url_conscientiousness = pred.weights_for_big5_['av']['b5']['conscientiousness']['sberdisk']
+                url_extraversion = pred.weights_for_big5_['av']['b5']['extraversion']['sberdisk']
+                url_agreeableness = pred.weights_for_big5_['av']['b5']['agreeableness']['sberdisk']
+                url_neuroticism = pred.weights_for_big5_['av']['b5']['neuroticism']['sberdisk']
 
-        Returns:
-            bool: **True** если веса нейросетевой модели загружены, в обратном случае **False**
-        """
+                pred.load_av_models_weights_b5(
+                    url_openness = url_openness,
+                    url_conscientiousness = url_conscientiousness,
+                    url_extraversion = url_extraversion,
+                    url_agreeableness = url_agreeableness,
+                    url_neuroticism = url_neuroticism,
+                    force_reload = True,
+                    out = True,
+                    runtime = True,
+                    run = True
+                )
 
-        if runtime:
-            self._r_start()
+            .. output-cell::
+                :execution-count: 3
+                :linenos:
 
-        if self.__load_model_weights(url, force_reload, self._load_text_model_weights_b5, out, False, run) is True:
-            try:
-                self._text_model_b5.load_weights(self._url_last_filename)
-            except Exception:
-                self._error(self._model_text_not_formation, out=out)
-                return False
-            else:
-                return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+                [2022-12-08 17:05:32] Загрузка весов нейросетевых моделей для получения результатов оценки персональных качеств (мультимодальное объединение) ...
 
-        return False
+                [2022-12-08 17:05:32] Загрузка файла "weights_2022-08-28_11-14-35.h5" (100.0%) ...
 
-    def load_text_features(
-        self, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> bool:
-        """Загрузка словаря с экспертными признаками
+                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Открытость опыту
 
-        Args:
-            force_reload (bool): Принудительная загрузка файла с весами нейросетевой модели из сети
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
+                    Линия: 639
+                    Метод: load_av_models_weights_b5
+                    Тип ошибки: AttributeError
 
-        Returns:
-            bool: **True** если словарь с экспертными признаками загружен, в обратном случае **False**
-        """
+                [2022-12-08 17:05:33] Загрузка файла "weights_2022-08-28_11-08-10.h5" (100.0%) ...
 
-        if runtime:
-            self._r_start()
+                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Добросовестность
 
-        if (
-            self.__load_text_features(self._text_features[0], force_reload, self._load_text_features, out, False, run)
-            is True
-        ):
-            try:
-                self.__parse_text_features, self.__category_text_features = liwc.load_token_parser(
-                    self._url_last_filename
-                )
-                self.__category_text_features = sorted(self.__category_text_features)
-            except Exception:
-                self._error(self._load_token_parser_error, out=out)
-                return False
-            else:
-                return True
-            finally:
-                if runtime:
-                    self._r_end(out=out)
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
+                    Линия: 639
+                    Метод: load_av_models_weights_b5
+                    Тип ошибки: AttributeError
 
-    def setup_translation_model(self, out: bool = True, runtime: bool = True, run: bool = True) -> bool:
-        """Формирование токенизатора и нейросетевой модели машинного перевода
+                [2022-12-08 17:05:33] Загрузка файла "weights_2022-08-28_11-17-57.h5" (100.0%) ...
 
-        Args:
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Экстраверсия
 
-        Returns:
-            bool: **True** если токенизатор и нейросетевая модель сформированы, в обратном случае **False**
-        """
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
+                    Линия: 639
+                    Метод: load_av_models_weights_b5
+                    Тип ошибки: AttributeError
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+                [2022-12-08 17:05:33] Загрузка файла "weights_2022-08-28_11-25-11.h5" (100.0%) ...
 
-        try:
-            # Проверка аргументов
-            if type(out) is not bool or type(runtime) is not bool or type(run) is not bool:
-                raise TypeError
-        except TypeError:
-            self._inv_args(__class__.__name__, self.setup_translation_model.__name__, out=out)
-            return False
-        else:
-            # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Доброжелательность
 
-            if runtime:
-                self._r_start()
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
+                    Линия: 639
+                    Метод: load_av_models_weights_b5
+                    Тип ошибки: AttributeError
 
-            # Информационное сообщение
-            self._info(self._load_translation_model, last=False, out=out)
+                [2022-12-08 17:05:33] Загрузка файла "weights_2022-06-14_21-44-09.h5" (100.0%) ...
 
-            try:
-                self._tokenizer = MarianTokenizer.from_pretrained(self._translation_model)
-                self._traslate_model = AutoModelForSeq2SeqLM.from_pretrained(self._translation_model).to(self._device)
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
-                return False
-            else:
-                return True
-        finally:
-            if runtime:
-                self._r_end(out=out)
+                [2022-12-08 17:05:33] Что-то пошло не так ... не удалось загрузить веса нейросетевой модели ... Нейротизм
 
-    def setup_bert_encoder(
-        self, force_reload: bool = True, out: bool = True, runtime: bool = True, run: bool = True
-    ) -> bool:
-        """Формирование токенизатора и нейросетевой модели BERT
+                    Файл: /Users/dl/GitHub/oceanai/oceanai/modules/lab/prediction.py
+                    Линия: 639
+                    Метод: load_av_models_weights_b5
+                    Тип ошибки: AttributeError
 
-        Args:
-            force_reload (bool): Принудительная загрузка файла с нейросетевой моделью BERT из сети
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                --- Время выполнения: 1.024 сек. ---
 
-        Returns:
-            bool: **True** если токенизатор и нейросетевая модель BERT сформированы, в обратном случае **False**
+                False
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         try:
             # Проверка аргументов
-            if (
-                type(force_reload) is not bool
+            if (type(url_openness) is not str or not url_openness
+                or type(url_conscientiousness) is not str or not url_conscientiousness
+                or type(url_extraversion) is not str or not url_extraversion
+                or type(url_agreeableness) is not str or not url_agreeableness
+                or type(url_neuroticism) is not str or not url_neuroticism
+                or type(force_reload) is not bool
                 or type(out) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
-                raise TypeError
+                or type(runtime) is not bool or type(run) is not bool): raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.setup_bert_encoder.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.load_av_models_weights_b5.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
+
+            if runtime: self._r_start()
 
-            if runtime:
-                self._r_start()
+            result_download_models = 0 # Все веса нейросетевых моделей по умолчанию загружены
 
             # Информационное сообщение
-            self._info(self._load_bert_model, last=False, out=out)
+            self._info(self._load_av_models_weights_b5, last = False, out = out)
+
+            # Проход по всем URL с весами нейросетевых моделей
+            for cnt, url in enumerate([
+                (url_openness, self._b5['ru'][0]),
+                (url_conscientiousness, self._b5['ru'][1]),
+                (url_extraversion, self._b5['ru'][2]),
+                (url_agreeableness, self._b5['ru'][3]),
+                (url_neuroticism, self._b5['ru'][4]),
+            ]):
+                sections = urlparse(url[0]) # Парсинг URL адреса
 
-            if self.__load_bert_model(self._bert_multi_model, force_reload, out, False, run) is True:
                 try:
-                    # Распаковка архива
-                    res_unzip = self._unzip(
-                        path_to_zipfile=os.path.join(self._url_last_filename),
-                        new_name=None,
-                        force_reload=force_reload,
-                    )
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
+                    # URL файл невалидный
+                    if sections.scheme == '': raise requests.exceptions.InvalidURL
+                except requests.exceptions.InvalidURL:
+                    url_norm = os.path.normpath(url[0])
+
+                    try:
+                        if os.path.isfile(url_norm) is False: raise FileNotFoundError # Не файл
+                    except FileNotFoundError: self._other_error(
+                            self._load_model_weights_error + ' ' + self._bold_wrapper(url[1].capitalize()), out = out
+                        ); continue
+                    except Exception: self._other_error(self._unknown_err, out = out); continue
+                    else:
+                        self._url_last_filename = url_norm
+
+                        # Отображение истории вывода сообщений в ячейке Jupyter
+                        if out: self.show_notebook_history_output()
                 else:
-                    # Файл распакован
-                    if res_unzip is True:
+                    try:
+                        if force_reload is False: clear_output(True)
+                        # Загрузка файла из URL
+                        res_download_file_from_url = self._download_file_from_url(
+                            url = url[0], force_reload = force_reload, runtime = False, out = out, run = True
+                        )
+                    except Exception: self._other_error(self._unknown_err, out = out); continue
+                    else:
+                        # Файл загружен
+                        if res_download_file_from_url != 200: continue
+
                         try:
-                            self._bert_tokenizer = BertTokenizer.from_pretrained(Path(self._url_last_filename).stem)
-                            self._bert_model = TFBertModel.from_pretrained(Path(self._url_last_filename).stem)
-                        except Exception:
-                            self._other_error(self._unknown_err, out=out)
-                            return False
+                            self._av_models_b5[self._b5['en'][cnt]].load_weights(self._url_last_filename)
+                        except Exception: self._other_error(
+                                self._load_model_weights_error + ' ' + self._bold_wrapper(url[1].capitalize()),
+                                out = out
+                            ); continue
                         else:
-                            return True
-            else:
-                return False
-        finally:
-            if runtime:
-                self._r_end(out=out)
-
-    def get_text_features(
-        self,
-        path: str,
-        asr: bool = False,
-        lang: str = "ru",
-        show_text: bool = False,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
-    ):
-        """Извлечение признаков из текста
+                            self._add_last_el_notebook_history_output(self._bold_wrapper(url[1].capitalize()))
 
-        Args:
-            path (str): Путь к видеофайлу или текст
-            asr (bool): Автоматическое распознавание речи
-            lang (str): Язык
-            show_text (bool): Отображение текста
-            out (bool): Отображение
-            runtime (bool): Подсчет времени выполнения
-            run (bool): Блокировка выполнения
+                            result_download_models += 1
 
-        Returns:
-            Tuple[np.ndarray, np.ndarray]: Кортеж с двумя np.ndarray:
+            clear_output(True)
+            # Отображение истории вывода сообщений в ячейке Jupyter
+            if out: self.show_notebook_history_output()
 
-                1. np.ndarray с экспертными признаками
-                2. np.ndarray с нейросетевыми признаками
-        """
+            if runtime: self._r_end(out = out)
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+            if result_download_models != len(self._b5['ru']): return False
+            return True
 
-        return self._get_text_features(
-            path=path,
-            asr=asr,
-            lang=lang,
-            show_text=show_text,
-            last=False,
-            out=out,
-            runtime=runtime,
-            run=run,
-        )
-
-    def get_text_union_predictions(
-        self,
-        depth: int = 1,
-        recursive: bool = False,
-        asr: bool = False,
-        lang: str = "ru",
-        accuracy=True,
-        url_accuracy: str = "",
-        logs: bool = True,
-        out: bool = True,
-        runtime: bool = True,
-        run: bool = True,
+    def get_av_union_predictions(
+        self, depth: int = 1, recursive: bool = False,
+        sr: int = 44100, window_audio: Union[int, float] = 2.0, step_audio: Union[int, float] = 1.0,
+        reduction_fps: int = 5, window_video: int = 10, step_video: int = 5,
+        accuracy = True, url_accuracy: str = '', logs: bool = True, out: bool = True,
+        runtime: bool = True, run: bool = True
     ) -> bool:
-        """Получения прогнозов по тексту
+        """Получения прогнозов по аудио и видео (мультимодальное объединение)
 
         Args:
             depth (int): Глубина иерархии для получения данных
             recursive (bool): Рекурсивный поиск данных
-            asr (bool): Автоматическое распознавание речи
-            lang (str): Язык
+            sr (int): Частота дискретизации
+            window_audio (Union[int, float]): Размер окна сегмента аудио сигнала (в секундах)
+            step_audio (Union[int, float]): Шаг сдвига окна сегмента аудио сигнала (в секундах)
+            reduction_fps (int): Понижение кадровой частоты
+            window_video (int): Размер окна сегмента видео сигнала (в кадрах)
+            step_video (int): Шаг сдвига окна сегмента видео сигнала (в кадрах)
             accuracy (bool): Вычисление точности
             url_accuracy (str): Полный путь к файлу с верными предсказаниями для подсчета точности
             logs (bool): При необходимости формировать LOG файл
             out (bool): Отображение
             runtime (bool): Подсчет времени выполнения
             run (bool): Блокировка выполнения
 
         Returns:
-            bool: **True** если прогнозы успешно получены, в обратном случае **False**
+            bool: **True** если веса прогнозы успешно получены, в обратном случае **False**
+
+        :bdg-link-light:`Пример <../../user_guide/notebooks/Prediction-get_av_union_predictions.ipynb>`
         """
 
-        self._clear_notebook_history_output()  # Очистка истории вывода сообщений в ячейке Jupyter
+        self._clear_notebook_history_output() # Очистка истории вывода сообщений в ячейке Jupyter
 
         # Сброс
-        self._df_files = pd.DataFrame()  # Пустой DataFrame с данными
-        self._df_accuracy = pd.DataFrame()  # Пустой DataFrame с результатами вычисления точности
+        self._df_files = pd.DataFrame() # Пустой DataFrame с данными
+        self._df_accuracy = pd.DataFrame() # Пустой DataFrame с результатами вычисления точности
 
         try:
             # Проверка аргументов
-            if (
-                type(depth) is not int
-                or depth < 1
-                or type(out) is not bool
-                or type(recursive) is not bool
-                or type(asr) is not bool
-                or not isinstance(lang, str)
-                or lang not in self.__lang_traslate
-                or type(accuracy) is not bool
-                or type(url_accuracy) is not str
-                or type(logs) is not bool
-                or type(runtime) is not bool
-                or type(run) is not bool
-            ):
+            if (type(depth) is not int or depth < 1 or type(recursive) is not bool
+                or type(sr) is not int or sr < 1
+                or ((type(window_audio) is not int or window_audio < 1)
+                    and (type(window_audio) is not float or window_audio <= 0))
+                or ((type(step_audio) is not int or step_audio < 1)
+                    and (type(step_audio) is not float or step_audio <= 0))
+                or type(reduction_fps) is not int or reduction_fps < 1
+                or type(window_video) is not int or window_video < 1 or type(step_video) is not int or step_video < 1
+                or type(accuracy) is not bool or type(url_accuracy) is not str or type(logs) is not bool
+                or type(out) is not bool or type(runtime) is not bool or type(run) is not bool):
                 raise TypeError
         except TypeError:
-            self._inv_args(__class__.__name__, self.get_text_union_predictions.__name__, out=out)
-            return False
+            self._inv_args(__class__.__name__, self.get_av_union_predictions.__name__, out = out); return False
         else:
             # Блокировка выполнения
-            if run is False:
-                self._error(self._lock_user, out=out)
-                return False
+            if run is False: self._error(self._lock_user, out = out); return False
 
-            if runtime:
-                self._r_start()
+            if runtime: self._r_start()
 
             try:
                 # Получение директорий, где хранятся данные
-                path_to_data = self._get_paths(self.path_to_dataset_, depth, out=out)
-                if type(path_to_data) is bool:
-                    return False
+                path_to_data = self._get_paths(self.path_to_dataset_, depth, out = out)
+                if type(path_to_data) is bool: return False
 
-                if type(self.keys_dataset_) is not list:
-                    raise TypeError
+                if type(self.keys_dataset_) is not list: raise TypeError
 
                 # Словарь для DataFrame набора данных с данными
                 self._dict_of_files = dict(zip(self.keys_dataset_, [[] for _ in range(0, len(self.keys_dataset_))]))
                 # Словарь для DataFrame набора данных с результатами вычисления точности
                 self._dict_of_accuracy = dict(
                     zip(self.keys_dataset_[1:], [[] for _ in range(0, len(self.keys_dataset_[1:]))])
                 )
             except (TypeError, FileNotFoundError):
-                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out=out)
-                return False
-            except Exception:
-                self._other_error(self._unknown_err, out=out)
+                self._other_error(self._folder_not_found.format(self._info_wrapper(self.path_to_dataset_)), out = out)
                 return False
+            except Exception: self._other_error(self._unknown_err, out = out); return False
             else:
                 # Вычисление точности
                 if accuracy is True:
-                    get_text_union_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
-                else:
-                    get_text_union_predictions_info = self._get_union_predictions_info
+                    get_av_union_predictions_info = self._get_union_predictions_info + self._get_accuracy_info
+                else: get_av_union_predictions_info = self._get_union_predictions_info
 
-                get_text_union_predictions_info += self._text_modality
+                get_av_union_predictions_info += self._av_modality
 
                 # Вычисление точности
                 if accuracy is True:
                     # Информационное сообщение
-                    self._info(get_text_union_predictions_info, out=out)
+                    self._info(get_av_union_predictions_info, out = out)
 
-                    if not url_accuracy:
-                        url_accuracy = self._true_traits["sberdisk"]
+                    if not url_accuracy: url_accuracy = self._true_traits['sberdisk']
 
                     try:
                         # Загрузка верных предсказаний
                         data_true_traits = pd.read_csv(url_accuracy)
                     except (FileNotFoundError, URLError, UnicodeDecodeError):
-                        self._other_error(self._load_data_true_traits_error, out=out)
-                        return False
-                    except Exception:
-                        self._other_error(self._unknown_err, out=out)
-                        return False
+                        self._other_error(self._load_data_true_traits_error, out = out); return False
+                    except Exception: self._other_error(self._unknown_err, out = out); return False
                     else:
                         true_traits = []
                         self._del_last_el_notebook_history_output()
 
-                paths = []  # Пути до искомых файлов
+                paths = [] # Пути до искомых файлов
 
                 # Проход по всем директориям
                 for curr_path in path_to_data:
                     empty = True  # По умолчанию директория пустая
 
                     # Рекурсивный поиск данных
-                    if recursive is True:
-                        g = Path(curr_path).rglob("*")
-                    else:
-                        g = Path(curr_path).glob("*")
+                    if recursive is True: g = Path(curr_path).rglob('*')
+                    else: g = Path(curr_path).glob('*')
 
                     # Формирование словаря для DataFrame
                     for p in g:
                         try:
-                            if type(self.ext_) is not list or len(self.ext_) < 1:
-                                raise TypeError
+                            if type(self.ext_) is not list or len(self.ext_) < 1: raise TypeError
 
                             self.ext_ = [x.lower() for x in self.ext_]
                         except TypeError:
-                            self._other_error(self._wrong_ext, out=out)
-                            return False
+                            self._other_error(self._wrong_ext, out = out); return False
                         except Exception:
-                            self._other_error(self._unknown_err, out=out)
-                            return False
+                            self._other_error(self._unknown_err, out = out); return False
                         else:
                             # Расширение файла соответствует расширению искомых файлов
                             if p.suffix.lower() in self.ext_:
-                                if empty is True:
-                                    empty = False  # Каталог не пустой
+                                if empty is True: empty = False # Каталог не пустой
 
                                 paths.append(p.resolve())
 
                 try:
-                    self.__len_paths = len(paths)  # Количество искомых файлов
+                    self.__len_paths = len(paths) # Количество искомых файлов
 
-                    if self.__len_paths == 0:
-                        raise TypeError
-                except TypeError:
-                    self._other_error(self._files_not_found, out=out)
-                    return False
-                except Exception:
-                    self._other_error(self._unknown_err, out=out)
-                    return False
+                    if self.__len_paths == 0: raise TypeError
+                except TypeError: self._other_error(self._files_not_found, out = out); return False
+                except Exception: self._other_error(self._unknown_err, out = out); return False
                 else:
                     # Локальный путь
                     self.__local_path = lambda path: os.path.join(
-                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))) :]
+                        *Path(path).parts[-abs((len(Path(path).parts) - len(Path(self.path_to_dataset_).parts))):]
                     )
 
-                    last = False  # Замена последнего сообщения
+                    last = False # Замена последнего сообщения
 
                     # Проход по всем искомым файлов
                     for i, curr_path in enumerate(paths):
-                        if i != 0:
-                            last = True
+                        if i != 0: last = True
 
                         # Индикатор выполнения
                         self._progressbar_union_predictions(
-                            get_text_union_predictions_info,
-                            i,
-                            self.__local_path(curr_path),
-                            self.__len_paths,
-                            True,
-                            last,
-                            out,
+                            get_av_union_predictions_info, i, self.__local_path(curr_path), self.__len_paths,
+                            True, last, out
                         )
 
-                        hc_features, nn_features = self.get_text_features(
-                            path=str(curr_path.resolve()),  # Путь к видеофайлу
-                            asr=asr,  # Распознавание речи
-                            lang=lang,  # Выбор языка
-                            show_text=True,  # Отображение текста
-                            out=False,  # Отображение
-                            runtime=False,  # Подсчет времени выполнения
-                            run=run,  # Блокировка выполнения
+                        # Извлечение признаков из акустического сигнала
+                        hc_audio_features, melspectrogram_audio_features = self._get_acoustic_features(
+                            path = str(curr_path.resolve()),
+                            sr = sr,
+                            window = window_audio,
+                            step = step_audio,
+                            last = True, out = False, runtime = False, run = run
                         )
 
-                        hc_features = np.expand_dims(hc_features, axis=0)
-                        nn_features = np.expand_dims(nn_features, axis=0)
+                        # Извлечение признаков из визуального сигнала
+                        hc_video_features, nn_video_features = self._get_visual_features(
+                            path = str(curr_path.resolve()),
+                            reduction_fps = reduction_fps,
+                            window = window_video,
+                            step = step_video,
+                            last = True, out = False, runtime = False, run = run
+                        )
 
-                        # Признаки из текста извлечены
-                        if len(hc_features) > 0 and len(nn_features) > 0:
-                            # Коды ошибок нейросетевых моделей
-                            code_error_pred_hc = -1
-                            code_error_pred_nn = -1
+                        # Признаки из акустического сигнала извлечены
+                        if (type(hc_audio_features) is list and type(melspectrogram_audio_features) is list
+                                and type(hc_video_features) is np.ndarray and type(nn_video_features) is np.ndarray
+                                and len(hc_audio_features) > 0 and len(melspectrogram_audio_features) > 0
+                                and len(hc_video_features) > 0 and len(nn_video_features) > 0):
+                            # Коды ошибок нейросетевых моделей (аудио модальность)
+                            code_error_pred_hc_audio = -1
+                            code_error_pred_melspectrogram_audio = -1
 
                             try:
                                 # Оправка экспертных признаков в нейросетевую модель
-                                pred_hc, _ = self.text_model_hc_(np.array(hc_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_hc = 1
-                            except Exception:
-                                code_error_pred_hc = 2
+                                pred_hc_audio = self.audio_model_hc_(
+                                    np.array(hc_audio_features, dtype = np.float16)
+                                ).numpy()
+                            except TypeError: code_error_pred_hc_audio = 1
+                            except Exception: code_error_pred_melspectrogram_audio = 2
 
                             try:
                                 # Отправка нейросетевых признаков в нейросетевую модель
-                                pred_nn, _ = self.text_model_nn_(np.array(nn_features, dtype=np.float16))
-                            except TypeError:
-                                code_error_pred_nn = 1
-                            except Exception:
-                                code_error_pred_nn = 2
+                                pred_melspectrogram_audio = self.audio_model_nn_(
+                                    np.array(melspectrogram_audio_features, dtype = np.float16)
+                                ).numpy()
+                            except TypeError: code_error_pred_melspectrogram_audio = 1
+                            except Exception: code_error_pred_melspectrogram_audio = 2
+
+                            if code_error_pred_hc_audio != -1 and code_error_pred_melspectrogram_audio != -1:
+                                self._error(self._models_audio_not_formation, out = out); return False
+
+                            if code_error_pred_hc_audio != -1:
+                                self._error(self._model_audio_hc_not_formation, out = out); return False
+
+                            if code_error_pred_melspectrogram_audio != -1:
+                                self._error(self._model_audio_nn_not_formation, out = out); return False
+
+                            # Коды ошибок нейросетевых моделей (видео модальность)
+                            code_error_pred_hc_video = -1
+                            code_error_pred_nn_video = -1
 
-                            if code_error_pred_hc != -1 and code_error_pred_nn != -1:
-                                self._error(self._model_text_not_formation, out=out)
-                                return False
+                            try:
+                                # Оправка экспертных признаков в нейросетевую модель
+                                pred_hc_video = self.video_model_hc_(
+                                    np.array(hc_video_features, dtype = np.float16)
+                                ).numpy()
+                            except TypeError: code_error_pred_hc_video = 1
+                            except Exception: code_error_pred_hc_video = 2
 
-                            if code_error_pred_hc != -1:
-                                self._error(self._model_text_hc_not_formation, out=out)
-                                return False
+                            try:
+                                # Отправка нейросетевых признаков в нейросетевую модель
+                                pred_nn_video = self.video_model_nn_(
+                                    np.array(nn_video_features, dtype = np.float16)
+                                ).numpy()
+                            except TypeError: code_error_pred_nn_video = 1
+                            except Exception: code_error_pred_nn_video = 2
+
+                            if code_error_pred_hc_video != -1 and code_error_pred_nn_video != -1:
+                                self._error(self._models_video_not_formation, out = out); return False
+
+                            if code_error_pred_hc_video != -1:
+                                self._error(self._model_video_hc_not_formation, out = out); return False
+
+                            if code_error_pred_nn_video != -1:
+                                self._error(self._model_video_nn_not_formation, out = out); return False
+
+                            # Конкатенация оценок по экспертным и нейросетевым признакам
+                            union_pred = self.__concat_pred_av(
+                                pred_hc_audio, pred_melspectrogram_audio, pred_hc_video, pred_nn_video,
+                                out = out
+                            )
 
-                            if code_error_pred_nn != -1:
-                                self._error(self._model_text_nn_not_formation, out=out)
-                                return False
+                            if len(union_pred) == 0: return False
+
+                            final_pred = []
 
-                            # pred_hc = pred_hc.numpy()[0]
-                            # pred_nn = pred_nn.numpy()[0]
+                            for cnt, (name_b5, model) in enumerate(self.av_models_b5_.items()):
+                                result = model(np.expand_dims(union_pred[cnt], axis = 0)).numpy()[0][0]
 
-                            final_pred = self._text_model_b5([pred_hc, pred_nn]).numpy()[0].tolist()
+                                final_pred.append(result)
 
                             # Добавление данных в словарь для DataFrame
                             if self._append_to_list_of_files(str(curr_path.resolve()), final_pred, out) is False:
                                 return False
 
                             # Вычисление точности
                             if accuracy is True:
                                 try:
-                                    true_trait = (
-                                        data_true_traits[data_true_traits.NAME_VIDEO == curr_path.name][
-                                            list(self._b5["en"])
-                                        ]
-                                        .values[0]
-                                        .tolist()
-                                    )
+                                    true_trait = data_true_traits[
+                                        data_true_traits.NAME_VIDEO == curr_path.name
+                                    ][list(self._b5['en'])].values[0].tolist()
                                 except IndexError:
-                                    self._other_error(self._expert_values_not_found, out=out)
-                                    return False
-                                except Exception:
-                                    self._other_error(self._unknown_err, out=out)
-                                    return False
-                                else:
-                                    true_traits.append(true_trait)
+                                    self._other_error(self._expert_values_not_found, out = out); return False
+                                except Exception: self._other_error(self._unknown_err, out = out); return False
+                                else: true_traits.append(true_trait)
                         else:
                             # Добавление данных в словарь для DataFrame
-                            if (
-                                self._append_to_list_of_files(
-                                    str(curr_path.resolve()), [None] * len(self._b5["en"]), out
-                                )
-                                is False
-                            ):
-                                return False
+                            if self._append_to_list_of_files(
+                                str(curr_path.resolve()), [None] * len(self._b5['en']), out
+                            ) is False: return False
+
+                            self._del_last_el_notebook_history_output()
 
                     # Индикатор выполнения
                     self._progressbar_union_predictions(
-                        get_text_union_predictions_info,
-                        self.__len_paths,
-                        self.__local_path(paths[-1]),
-                        self.__len_paths,
-                        True,
-                        last,
-                        out,
+                        get_av_union_predictions_info, self.__len_paths, self.__local_path(paths[-1]),
+                        self.__len_paths, True, last, out
                     )
 
                     # Отображение в DataFrame с данными
-                    self._df_files = pd.DataFrame.from_dict(data=self._dict_of_files, orient="index").transpose()
+                    self._df_files = pd.DataFrame.from_dict(data = self._dict_of_files, orient = 'index').transpose()
                     self._df_files.index.name = self._keys_id
                     self._df_files.index += 1
 
                     self._df_files.index = self._df_files.index.map(str)
 
-                    self._df_files.Path = [os.path.basename(i) for i in self._df_files.Path]
-
                     # Отображение
                     if out is True:
-                        self._add_notebook_history_output(self._df_files.iloc[0 : self.num_to_df_display_, :])
+                        self._add_notebook_history_output(self._df_files.iloc[0:self.num_to_df_display_, :])
 
                     # Подсчет точности
                     if accuracy is True:
                         mae_curr = []
 
                         for cnt, name_b5 in enumerate(self._df_files.keys().tolist()[1:]):
-                            mae_curr.append(
-                                mean_absolute_error(np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list())
-                            )
+                            try:
+                                mae_curr.append(
+                                    mean_absolute_error(
+                                        np.asarray(true_traits)[:, cnt], self._df_files[name_b5].to_list()
+                                    )
+                                )
+                            except IndexError: continue
+                            except Exception: continue
 
                         mae_curr = [round(float(i), 4) for i in mae_curr]
                         mae_mean = round(float(np.mean(mae_curr)), 4)
                         accuracy_curr = [round(float(i), 4) for i in 1 - np.asarray(mae_curr)]
                         accuracy_mean = round(float(np.mean(accuracy_curr)), 4)
 
                         for curr_acc in [mae_curr, accuracy_curr]:
                             # Добавление данных в словарь для DataFrame с результатами вычисления точности
-                            if self._append_to_list_of_accuracy(curr_acc, out) is False:
-                                return False
+                            if self._append_to_list_of_accuracy(curr_acc, out) is False: return False
 
-                        self._dict_of_accuracy.update({self.__df_accuracy_mean: [mae_mean, accuracy_mean]})
+                        self._dict_of_accuracy.update({
+                            self.__df_accuracy_mean: [mae_mean, accuracy_mean]
+                        })
                         # Отображение в DataFrame с данными
-                        self._df_accuracy = pd.DataFrame.from_dict(
-                            data=self._dict_of_accuracy, orient="index"
-                        ).transpose()
+                        self._df_accuracy = pd.DataFrame.from_dict(data = self._dict_of_accuracy,
+                                                                   orient = 'index').transpose()
                         self._df_accuracy.index = self.__df_accuracy_index
                         self._df_accuracy.index.name = self.__df_accuracy_index_name
 
                         # Информационное сообщение
-                        self._info(self._get_union_predictions_result, out=False)
+                        self._info(self._get_union_predictions_result, out = False)
 
                         # Отображение
                         if out is True:
-                            self._add_notebook_history_output(self._df_accuracy.iloc[0 : self.num_to_df_display_, :])
+                            self._add_notebook_history_output(self._df_accuracy.iloc[0:self.num_to_df_display_, :])
 
                         self._info(
                             self._get_union_predictions_results_mean.format(
-                                self._info_wrapper(str(mae_mean)), self._info_wrapper(str(accuracy_mean))
+                                self._info_wrapper(str(mae_mean)),
+                                self._info_wrapper(str(accuracy_mean))
                             ),
-                            out=False,
+                            out = False
                         )
 
                     clear_output(True)
                     # Отображение истории вывода сообщений в ячейке Jupyter
-                    if out is True:
-                        self.show_notebook_history_output()
+                    if out is True: self.show_notebook_history_output()
 
                     if logs is True:
                         # Текущее время для лог-файла
                         # см. datetime.fromtimestamp()
-                        curr_ts = str(datetime.now().timestamp()).replace(".", "_")
+                        curr_ts = str(datetime.now().timestamp()).replace('.', '_')
 
-                        name_logs_file = self.get_text_union_predictions.__name__
+                        name_logs_file = self.get_av_union_predictions.__name__
 
                         # Сохранение LOG
                         res_save_logs_df_files = self._save_logs(
-                            self._df_files, name_logs_file + "_df_files_" + curr_ts
+                            self._df_files, name_logs_file + '_df_files_' + curr_ts
                         )
 
                         # Подсчет точности
                         if accuracy is True:
                             # Сохранение LOG
                             res_save_logs_df_accuracy = self._save_logs(
-                                self._df_accuracy, name_logs_file + "_df_accuracy_" + curr_ts
+                                self._df_accuracy, name_logs_file + '_df_accuracy_' + curr_ts
                             )
 
                         if res_save_logs_df_files is True:
                             # Сохранение LOG файла/файлов
-                            if accuracy is True and res_save_logs_df_accuracy is True:
-                                logs_s = self._logs_saves_true
-                            else:
-                                logs_s = self._logs_save_true
+                            if accuracy is True and res_save_logs_df_accuracy is True: logs_s = self._logs_saves_true
+                            else: logs_s = self._logs_save_true
 
-                            self._info_true(logs_s, out=out)
+                            self._info_true(logs_s, out = out)
 
                     return True
             finally:
-                if runtime:
-                    self._r_end(out=out)
+                if runtime: self._r_end(out = out)
```

### Comparing `oceanai-1.0.0a23/oceanai/modules/locales/en/LC_MESSAGES/base.mo` & `oceanai-1.0.0a5/oceanai/modules/locales/en/LC_MESSAGES/base.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: 1.0\n"
-"POT-Creation-Date: 2023-12-16 21:18+0300\n"
-"PO-Revision-Date: 2023-12-16 21:18+0300\n"
+"POT-Creation-Date: 2022-12-11 11:18+0300\n"
+"PO-Revision-Date: 2022-12-11 11:18+0300\n"
 "Last-Translator: Elena Ryumina <ryumina_ev@mail.ru>, Dmitry Ryumin "
 "<dl_03.03.1991@mail.ru>\n"
 "Language-Team: English <ryumina_ev@mail.ru>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
@@ -19,106 +19,84 @@
 
 msgid " (мультимодальное объединение) ..."
 msgstr " (multimodal fusion) ..."
 
 msgid " (ошибка {})"
 msgstr " (error {})"
 
-msgid " (текстовая модальность) ..."
-msgstr " (text modality) ..."
-
 msgid " и вычисление точности"
-msgstr " and accuracy calculation"
-
-msgid "DataFrame с данными пуст ..."
-msgstr "DataFrame with data is empty ..."
+msgstr " and precision calculation"
 
 msgid "OCEANAI - персональные качества личности человека"
-msgstr "OCEANAI - personality traits"
+msgstr "OCEANAI - personal traits"
 
 msgid "URL указан некорректно ..."
 msgstr "The URL is incorrect ..."
 
 msgid "{}Понижение кадровой частоты: с"
 msgstr "{}FPS down: with"
 
-msgid "{}Размерность матрицы с нейросетевыми признаками одного сегмента:"
-msgstr "{}Dimensionality of the matrix with deep features of one segment:"
-
-msgid "{}Размерность матрицы с нейросетевыми признаками:"
-msgstr "{}Dimensionality of the deep feature matrix:"
-
 msgid "{}Размерность тензора с лог мел-спектрограммами одного сегмента:"
 msgstr "{}Dimension of the tensor with log mel-spectrograms of one segment:"
 
-msgid "{}Текст:"
-msgstr "{}Text:"
+msgid "{}Размерность тензора с нейросетевыми признаками одного сегмента:"
+msgstr "{}Dimension of the tensor with neural network features of one segment:"
 
 msgid "Авторы"
 msgstr "Authors"
 
 msgid "Версия"
 msgstr "Version"
 
 msgid "Время выполнения"
 msgstr "Runtime"
 
 msgid "Выполнение заблокировано пользователем ..."
 msgstr "Run blocked by user ..."
 
 msgid "Загрузка весов нейросетевой модели для получения нейросетевых признаков"
-msgstr "Downloading weights of a neural network model to obtain deep features"
-
-msgid ""
-"Загрузка весов нейросетевой модели для получения оценок персональных качеств"
 msgstr ""
-"Downloading the weights of the neural network model to obtain the "
-"personality traits scores"
+"Downloading weights of a neural network model to obtain neural network "
+"features"
 
 msgid ""
 "Загрузка весов нейросетевой модели для получения оценок по нейросетевым "
 "признакам"
 msgstr ""
-"Downloading the weights of the neural network model to obtain scores for "
-"deep features"
+"Downloading the weights of the neural network model to obtain estimates for "
+"neural network features"
 
 msgid ""
 "Загрузка весов нейросетевой модели для получения оценок по экспертным "
 "признакам"
 msgstr ""
-"Downloading the weights of the neural network model to obtain scores by hand-"
-"crafted features"
+"Downloading the weights of the neural network model to obtain estimates by "
+"expert features"
 
 msgid ""
 "Загрузка весов нейросетевых моделей для получения результатов оценки "
 "персональных качеств"
 msgstr ""
-"Downloading the weights of neural network models to obtain the personality "
-"traits scores"
-
-msgid "Загрузка словаря с экспертными признаками ..."
-msgstr "Downloading a dictionary with hand-crafted features ..."
+"Downloading the weights of neural network models to obtain the results of "
+"assessing personal traits"
 
 msgid "Загрузка файла \"{}\""
-msgstr "Downloading a file \"{}\""
+msgstr "File download \"{}\""
 
 msgid ""
 "Извлечение признаков (экспертных и лог мел-спектрограмм) из акустического "
 "сигнала ..."
 msgstr ""
-"Extraction of features (hand-crafted and mel-spectrograms) from an acoustic "
+"Extraction of features (expert and mel-spectrograms) from an acoustic "
 "signal ..."
 
 msgid ""
 "Извлечение признаков (экспертных и нейросетевых) из визуального сигнала ..."
 msgstr ""
-"Extraction of features (hand-crafted and deep) from a visual signal ..."
-
-msgid "Извлечение признаков (экспертных и нейросетевых) из текста ..."
-msgstr "Feature extraction (hand-crafted and deep) from text ..."
+"Extraction of features (expert and neural network) from a visual signal ..."
 
 msgid "Линия"
 msgstr "Line"
 
 msgid "Лицензия"
 msgstr "License"
 
@@ -141,100 +119,78 @@
 msgid "Неверные типы или значения аргументов ..."
 msgstr "Invalid argument types or values ..."
 
 msgid "Неверные типы или значения аргументов в \"{}\" ..."
 msgstr "Invalid argument types or values in \"{}\" ..."
 
 msgid "Получение прогнозов"
-msgstr "Getting scores"
+msgstr "Getting forecasts"
 
 msgid "Прям беда! "
 msgstr "It is just trouble! "
 
-msgid "Разархивирование архива \"{}\" ..."
-msgstr "Unzipping an archive \"{}\" ..."
-
 msgid "Сопровождающие"
 msgstr "Maintainers"
 
 msgid "Средняя средних абсолютных ошибок: {}, средняя точность: {} ..."
 msgstr "Mean absolute errors: {}, average accuracy: {} ..."
 
 msgid ""
 "Статистика извлеченных признаков из акустического сигнала:{}Общее количество "
 "сегментов с:{}1. экспертными признаками: {}{}2. лог мел-спектрограммами: {}{}"
 "Размерность матрицы экспертных признаков одного сегмента: {} "
 msgstr ""
 "Statistics of the features extracted from the acoustic signal:{}Total number "
-"of segments with:{}1. hand-crafted features: {}{}2. mel-spectrogram log: {}{}"
-"Dimension of the matrix of hand-crafted features of one segment: {} "
+"of segments with:{}1. expert features: {}{}2. mel-spectrogram log: {}{}"
+"Dimension of the matrix of expert features of one segment: {} "
 
 msgid ""
 "Статистика извлеченных признаков из визуального сигнала:{}Общее количество "
 "сегментов с:{}1. экспертными признаками: {}{}2. нейросетевыми признаками: {}"
 "{}Размерность матрицы экспертных признаков одного сегмента: {} "
 msgstr ""
 "Statistics of extracted features from visual signal:{}Total number of "
-"segments since:{}1. hand-crafted features: {}{}2. deep features: {}{}"
-"Dimension of the matrix of hand-crafted features of one segment: {} "
-
-msgid ""
-"Статистика извлеченных признаков из текста:{}Размерность матрицы экспертных "
-"признаков: {} "
-msgstr ""
-"Statistics of extracted features from text:{}Dimensionality of hand-crafted "
-"feature matrix: {} "
+"segments since:{}1. expert features: {}{}2. neural network features: {}{}"
+"Dimension of the matrix of expert features of one segment: {} "
 
 msgid "Тип ошибки"
 msgstr "Error type"
 
 msgid "Точность по отдельным персональным качествам личности человека ..."
-msgstr "Trait-wise accuracy ..."
+msgstr "Accuracy on personal traits ..."
 
 msgid "Файл"
 msgstr "File"
 
 msgid ""
 "Формирование нейросетевой архитектуры для получения нейросетевых признаков"
-msgstr "Formation of neural network architecture for obtaining deep features"
-
-msgid ""
-"Формирование нейросетевой архитектуры для получения оценок по нейросетевым "
-"признакам"
 msgstr ""
-"Formation of a neural network architecture for obtaining scores by deep "
+"Formation of neural network architecture for obtaining neural network "
 "features"
 
 msgid ""
-"Формирование нейросетевой архитектуры модели для получения  оценок "
-"персональных качеств"
+"Формирование нейросетевой архитектуры для получения оценок по нейросетевым "
+"признакам"
 msgstr ""
-"Formation of neural network architecture of the model for obtaining the "
-"personality traits scores"
+"Formation of a neural network architecture for obtaining estimates by neural "
+"network features"
 
 msgid ""
 "Формирование нейросетевой архитектуры модели для получения оценок по "
 "экспертным признакам"
 msgstr ""
 "Formation of the neural network architecture of the model for obtaining "
-"scores by hand-crafted features"
+"estimates by expert features"
 
 msgid ""
 "Формирование нейросетевых архитектур моделей для получения результатов "
 "оценки персональных качеств"
 msgstr ""
 "Formation of neural network architectures of models for obtaining the "
-"personality traits scores"
-
-msgid "Формирование токенизатора и нейросетевой модели BERT ..."
-msgstr "Formation of a tokenizer and neural network model of the BERT ..."
-
-msgid "Формирование токенизатора и нейросетевой модели машинного перевода ..."
-msgstr ""
-"Formation of a tokenizer and neural network model of machine translation ..."
+"results of assessing personal traits"
 
 msgid "Что-то пошло не так ... "
 msgstr "Something went wrong ... "
 
 msgid "в указанной директории необходимые файлы не найдены ..."
 msgstr "required files were not found in the specified directory ..."
 
@@ -259,140 +215,105 @@
 
 msgid "из"
 msgstr "from"
 
 msgid ""
 "конкатенация оценок по экспертным и нейросетевым признакам не произведена"
 msgstr ""
-"concatenation of scores by hand-crafted and deep features was not performed"
+"concatenation of estimates by expert and neural network features was not "
+"performed"
 
 msgid "лог мел-спектрограммы из акустического сигнала не извлечены ..."
 msgstr "mel-spectrogram log from the acoustic signal is not extracted ..."
 
 msgid "не на одном кадре видеопотока лицо не найдено ..."
 msgstr "face not found on more than one frame of the video stream ..."
 
 msgid "не удалось загрузить веса нейросетевой модели ..."
 msgstr "failed to load neural network model weights ..."
 
-msgid "не удалось загрузить словарь с экспертными признаками ..."
-msgstr "failed to download dictionary with hand-crafted features ..."
-
-msgid "не удалось загрузить токенизатор и нейросетевую модель BERT ..."
-msgstr "failed to download the tokenizer and the BERT neural network model ..."
-
 msgid ""
 "не удалось загрузить файл с верными предсказаниями для подсчета точности ..."
 msgstr ""
-"failed to load file with ground truth scores for accuracy calculation ..."
+"failed to load file with correct predictions for precision calculation ..."
 
 msgid "не удалось обработать указанный URL ..."
 msgstr "the specified URL could not be processed ..."
 
-msgid "не удалось переименовать директорию из \"{}\" в \"{}\" ..."
-msgstr "failed to rename the directory from \"{}\" to \"{}\" ..."
-
-msgid "не удалось разархивировать архив \"{}\" ..."
-msgstr "failed to unzip the archive \"{}\" ..."
-
 msgid "не удалось скачать файл \"{}\"{} ..."
 msgstr "failed to download file \"{}\"{} ..."
 
 msgid "не удалось сохранить LOG файл{} ..."
 msgstr "failed to save LOG file{} ..."
 
-msgid "не удалось считать лексикон LIWC ..."
-msgstr "failed to consider the LIWC lexicon ..."
-
 msgid "не указано минимум одно расширение искомых файлов ..."
 msgstr "at least one extension of the files you are looking for is missing ..."
 
 msgid ""
 "нейросетевая архитектура модели для получения нейросетевых признаков не "
 "сформирована"
 msgstr ""
-"the neural network architecture of the model for obtaining deep features is "
-"not formed"
-
-msgid ""
-"нейросетевая архитектура модели для получения оценок по мультимодальным "
-"данным не сформирована"
-msgstr ""
-"neural network architecture of the model for obtaining scores by multimodal "
-"data is not formed"
+"the neural network architecture of the model for obtaining neural network "
+"features is not formed"
 
 msgid ""
 "нейросетевая архитектура модели для получения оценок по нейросетевым "
 "признакам не сформирована"
 msgstr ""
-"the neural network architecture of the model for obtaining scores by deep "
-"features has not been formed"
-
-msgid ""
-"нейросетевая архитектура модели для получения оценок по экспертным и "
-"нейросетевым признакам не сформирована"
-msgstr ""
-"neural network architecture of the model for obtaining scores by hand-"
-"crafted and deep features is not formed"
+"the neural network architecture of the model for obtaining estimates by "
+"neural network features has not been formed"
 
 msgid ""
 "нейросетевая архитектура модели для получения оценок по экспертным признакам "
 "не сформирована"
 msgstr ""
-"the neural network architecture of the model for obtaining scores by hand-"
-"crafted features has not been formed"
+"the neural network architecture of the model for obtaining estimates by "
+"expert features has not been formed"
 
 msgid ""
 "нейросетевые архитектуры моделей для получения оценок по экспертным и "
 "нейросетевым признакам не сформированы"
 msgstr ""
-"neural network architectures of models for obtaining scores by hand-crafted "
-"and deep features have not been formed"
+"neural network architectures of models for obtaining estimates on expert and "
+"neural network features have not been formed"
+
+msgid "нейротизм"
+msgstr "neuroticism"
 
 msgid ""
 "нормализация оценок по экспертным и нейросетевым признакам не произведена"
 msgstr ""
-"normalization of scores by hand-crafted and deep features was not performed"
+"normalization of estimates by expert and neural network features was not "
+"performed"
 
 msgid "общее количество кадров в видеопотоке: {} ..."
 msgstr "total number of frames in the video stream: {} ..."
 
 msgid "открытость опыту"
 msgstr "openness"
 
 msgid "отсутствуют экспертные оценки ..."
-msgstr "no ground truth scores ..."
+msgstr "no expert reviews ..."
 
 msgid "расширение видеофайла должно быть одним из: \"{}\""
 msgstr "video file extension must be one of: \"{}\""
 
 msgid "сек."
 msgstr "sec."
 
 msgid "смотрите настройки ядра и цепочку выполнения действий ..."
 msgstr "see kernel settings and chain of action ..."
 
-msgid ""
-"сумма весов для ранжирования персональных качеств должна быть равна 100 ..."
-msgstr ""
-"the sum of weights for ranking personality traits should be equal to 100 ..."
-
-msgid "текстовый файл \"{}\" пуст ..."
-msgstr "the text file \"{}\" is empty ..."
-
 msgid "указан слишком маленький размер ({}) окна сегмента сигнала ..."
 msgstr "the size ({}) of the signal segment window is too small ..."
 
 msgid "файл \"{}\" не найден ..."
 msgstr "file \"{}\" not found ..."
 
 msgid "файл \"{}\" не содержит акустического сигнала ..."
 msgstr "file \"{}\" does not contain an acoustic signal ..."
 
 msgid "экспертные признаки из акустического сигнала не извлечены ..."
-msgstr "hand-crafted features are not extracted from the acoustic signal ..."
+msgstr "expert signs are not extracted from the acoustic signal ..."
 
 msgid "экстраверсия"
 msgstr "extraversion"
-
-msgid "эмоциональная стабильность"
-msgstr "non-neuroticism"
```

### Comparing `oceanai-1.0.0a23/oceanai.egg-info/SOURCES.txt` & `oceanai-1.0.0a5/oceanai.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 oceanai/__init__.py
 oceanai.egg-info/PKG-INFO
 oceanai.egg-info/SOURCES.txt
 oceanai.egg-info/dependency_links.txt
 oceanai.egg-info/requires.txt
@@ -18,23 +17,16 @@
 oceanai/modules/core/messages.py
 oceanai/modules/core/settings.py
 oceanai/modules/lab/__init__.py
 oceanai/modules/lab/audio.py
 oceanai/modules/lab/build.py
 oceanai/modules/lab/download.py
 oceanai/modules/lab/prediction.py
-oceanai/modules/lab/text.py
-oceanai/modules/lab/unzip.py
 oceanai/modules/lab/video.py
 oceanai/modules/lab/keras_vggface/__init__.py
 oceanai/modules/lab/keras_vggface/models.py
 oceanai/modules/lab/keras_vggface/utils.py
 oceanai/modules/lab/keras_vggface/vggface.py
-oceanai/modules/lab/utils/__init__.py
-oceanai/modules/lab/utils/addition.py
-oceanai/modules/lab/utils/attention.py
-oceanai/modules/lab/utils/gfl.py
 oceanai/modules/locales/en/LC_MESSAGES/base.mo
 oceanai/modules/locales/ru/LC_MESSAGES/base.mo
 test/__init__.py
-test/unit_tests_fi_en.py
-test/unit_tests_mupta_ru.py
+test/unit_tests.py
```

### Comparing `oceanai-1.0.0a23/setup.py` & `oceanai-1.0.0a5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 import sys
 
 from setuptools import setup, find_packages
 
 MIN_PYTHON_VERSION = (3, 9)
 
 if sys.version_info[:2] < MIN_PYTHON_VERSION:
-    raise RuntimeError("Python version required = {}.{}".format(MIN_PYTHON_VERSION[0], MIN_PYTHON_VERSION[1]))
+    raise RuntimeError('Python version required = {}.{}'.format(MIN_PYTHON_VERSION[0], MIN_PYTHON_VERSION[1]))
 
 import oceanai
 
 REQUIRED_PACKAGES = [
-    "ipython >= 8.18.1",
-    "jupyterlab == 3.5.0",
-    "tensorflow >= 2.15.0",
-    "keras >= 2.11.0",
-    "Keras-Applications>=1.0.8",
-    "numpy >= 1.23.5",
-    "scipy >= 1.9.3",
-    "pandas >= 1.5.2",
-    "requests >= 2.28.1",
-    "opensmile >= 2.4.1",
-    "librosa >= 0.9.2",
-    "audioread >= 3.0.0",
-    "scikit-learn >= 1.1.3",
-    "opencv-contrib-python >= 4.6.0.66",
-    "mediapipe >= 0.9.0",
-    "liwc >= 0.5.0",
-    "transformers >= 4.36.0",
-    "sentencepiece >= 0.1.99",
-    "torch == 2.0.1",
-    "torchaudio == 2.0.2",
-    "sacremoses >= 0.0.1",
-    "gradio >= 4.24.0",
+    'ipython >= 8.7.0',
+    'jupyterlab >= 3.5.0',
+    'tensorflow >= 2.11.0',
+    'keras >= 2.11.0',
+    'Keras-Applications>=1.0.8',
+    'numpy >= 1.23.5',
+    'scipy >= 1.9.3',
+    'pandas >= 1.5.2',
+    'requests >= 2.28.1',
+    'opensmile >= 2.4.1',
+    'librosa >= 0.9.2',
+    'audioread >= 3.0.0',
+    'scikit-learn >= 1.1.3',
+    'opencv-contrib-python >= 4.6.0.66',
+    'pymediainfo >= 6.0.1',
+    'mediapipe >= 0.9.0',
 ]
 
 CLASSIFIERS = """\
 Development Status :: 3 - Alpha
 Natural Language :: Russian
 Natural Language :: English
 Intended Audience :: Developers
@@ -71,45 +65,39 @@
 Operating System :: Microsoft :: Windows
 Operating System :: POSIX :: Linux
 Framework :: Jupyter
 Framework :: Jupyter :: JupyterLab :: 4
 Framework :: Sphinx
 """
 
-with open("README.md", "r") as fh:
+with open('README.md', 'r') as fh:
     long_description = fh.read()
 
     setup(
-        name=oceanai.__name__,
-        packages=find_packages(),
-        license=oceanai.__license__,
-        version=oceanai.__release__,
-        author=oceanai.__author__en__,
-        author_email=oceanai.__email__,
-        maintainer=oceanai.__maintainer__en__,
-        maintainer_email=oceanai.__maintainer_email__,
-        url=oceanai.__uri__,
-        description=oceanai.__summary__,
-        long_description=long_description,
-        long_description_content_type="text/markdown",
+        name = oceanai.__name__,
+        packages = find_packages(),
+        license = oceanai.__license__,
+        version = oceanai.__release__,
+        author = oceanai.__author__en__,
+        author_email = oceanai.__email__,
+        maintainer = oceanai.__maintainer__en__,
+        maintainer_email = oceanai.__maintainer_email__,
+        url = oceanai.__uri__,
+        description = oceanai.__summary__,
+        long_description = long_description,
+        long_description_content_type = 'text/markdown',
         install_requires=REQUIRED_PACKAGES,
-        keywords=[
-            "OCEAN-AI",
-            "MachineLearning",
-            "Statistics",
-            "ComputerVision",
-            "ArtificialIntelligence",
-            "Preprocessing",
-        ],
-        include_package_data=True,
-        classifiers=[_f for _f in CLASSIFIERS.split("\n") if _f],
-        python_requires=">=3.9, <4",
-        entry_points={
-            "console_scripts": [],
+        keywords = ['OCEAN-AI', 'MachineLearning', 'Statistics', 'ComputerVision', 'ArtificialIntelligence',
+                    'Preprocessing'],
+        include_package_data = True,
+        classifiers = [_f for _f in CLASSIFIERS.split('\n') if _f],
+        python_requires = '>=3.9, <4',
+        entry_points = {
+            'console_scripts': [],
         },
-        project_urls={
-            "Bug Reports": "https://github.com/DmitryRyumin/oceanai/issues",
-            "Documentation": "https://oceanai.readthedocs.io",
-            "Source Code": "https://github.com/DmitryRyumin/oceanai/tree/main/oceanai",
-            "Download": "https://github.com/DmitryRyumin/oceanai/tags",
+        project_urls = {
+            'Bug Reports': 'https://github.com/DmitryRyumin/oceanai/issues',
+            'Documentation': 'https://oceanai.readthedocs.io',
+            'Source Code': 'https://github.com/DmitryRyumin/oceanai/tree/main/oceanai',
+            'Download': 'https://github.com/DmitryRyumin/oceanai/tags',
         },
     )
```

