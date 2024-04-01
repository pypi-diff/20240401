# Comparing `tmp/celery_yandex_serverless-0.1.3.tar.gz` & `tmp/celery_yandex_serverless-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_yandex_serverless-0.1.3.tar", max compression
+gzip compressed data, was "celery_yandex_serverless-0.1.4.tar", max compression
```

## Comparing `celery_yandex_serverless-0.1.3.tar` & `celery_yandex_serverless-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6145 2023-04-27 17:18:44.906103 celery_yandex_serverless-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-28 16:34:01.621354 celery_yandex_serverless-0.1.3/celery_yandex_serverless/__init__.py
--rw-r--r--   0        0        0     3381 2023-04-10 16:32:52.281683 celery_yandex_serverless-0.1.3/celery_yandex_serverless/django.py
--rw-r--r--   0        0        0      468 2023-11-09 16:43:53.468006 celery_yandex_serverless-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.3/setup.py
--rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6145 2023-04-27 17:18:44.906103 celery_yandex_serverless-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-28 16:34:01.621354 celery_yandex_serverless-0.1.4/celery_yandex_serverless/__init__.py
+-rw-r--r--   0        0        0     3404 2024-04-01 15:14:35.291775 celery_yandex_serverless-0.1.4/celery_yandex_serverless/django.py
+-rw-r--r--   0        0        0      468 2024-04-01 15:15:00.886597 celery_yandex_serverless-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.4/setup.py
+-rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.4/PKG-INFO
```

### Comparing `celery_yandex_serverless-0.1.3/README.md` & `celery_yandex_serverless-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `celery_yandex_serverless-0.1.3/celery_yandex_serverless/django.py` & `celery_yandex_serverless-0.1.4/celery_yandex_serverless/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 
 logger = logging.getLogger(__name__)
 
 _secret_key_slug = "CELERY_YANDEX_SERVERLESS_KEY"
 _secret_key = getattr(settings, _secret_key_slug, os.environ.get(_secret_key_slug))
-if _secret_key is None:
+if _secret_key is None and not settings.DEBUG:
     logger.error("Define CELERY_YANDEX_SERVERLESS_KEY settings with secret key for serverless worker")
 
 
 def worker_view_factory(celery_app):
     @csrf_exempt
     def _worker_view(request, key: str):
         if _secret_key is None:
```

### Comparing `celery_yandex_serverless-0.1.3/setup.py` & `celery_yandex_serverless-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['boto3>=1.26.101,<2.0.0',
  'celery>=5.0,<6.0',
  'django',
  'pycurl>=7.45.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'celery-yandex-serverless',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Package for starting Celery worker inside Yandex Cloud Serverless Container',
     'long_description': '# Celery Yandex Serverless\n\nМодуль, позволяющий запустить celery-worker внутри Yandex Cloud Serverless Container.\n\n**Классический подход с отдельно запущенным воркером**\n\n1. Бекенд отправляет задачу в очередь.\n2. Отдельный процесс воркера забирает задачу из очереди и выполняет ее.\n\n**Serverless-подход**\n\nВ Serverless подходе предполагается, что нет никаких запущенных постоянно процессов приложения. Эти процессы запускаются\nлибо по запросу пользователя, либо по различным тригерам облаком. \n\nМодуль `celery-yandex-serverless` помогает запустить воркер следующим образом:\n1. Бекенд отправляет задачу в очередь\n2. После попадания задачи в очередь срабатывает триггер, который делает http-запрос serverless-контейнеру.\n3. Serverless-контейнер запускает код задачи, который ранее выполнялся в воркере.\n\n## Использование\n\n### Подключение Celery к Yandex Message Queue\n\n1. Перейдите на страницу каталога в Яндекс.Облаке\n2. Зайдите в раздел **Сервисные аккаунты**\n3. Посмотрите название сервисного аккаунта в каталоге Яндекс.Облака\n4. Сгенерируйте `ACCESS_KEY` и `SECRET_KEY` с помощью команды \n(замените `SERVICE_ACCOUNT_NAME` на название сервисного аккаунта):\n\n```bash\nyc iam access-key create --service-account-name SERVICE_ACCOUNT_NAME\n```\n\nКоманда вернет следующую информацию. Сохраните ее, она пригодится в будущем.\n\n```yml{5,6}\naccess_key:\n  id: aje...\n  service_account_id: aje...\n  created_at: "2023-03-24T17:49:01.555836400Z"\n  key_id: YCAJ... # <- Это access key\nsecret: YCPM... # <- Это secret key\n```\n\n### Настройка\nУкажите переменные окружения с использованием только что полученных данных:\n\n```\nAWS_ACCESS_KEY_ID="access key, скопированный выше"\nAWS_SECRET_ACCESS_KEY="secret key, скопированный выше"\nAWS_DEFAULT_REGION="ru-central1"\nCELERY_BROKER_URL=sqs://message-queue.api.cloud.yandex.net:443\nCELERY_BROKER_IS_SECURE=True\n```\n\nВ файле `settings.py` укажите:\n\n```python\nCELERY_BROKER_URL = os.environ.get("CELERY_BROKER_URL")\nCELERY_BROKER_TRANSPORT_OPTIONS = {\n    \'is_secure\': os.environ.get("CELERY_BROKER_IS_SECURE", \'false\').lower() == \'true\'\n}\n```\n\nПосле этого отправьте celery-задачу, чтобы в Яндекс.Облаке появилась очередь.\n\n### Подключение модуля\n\n1. `pip install celery-yandex-serverless` - установите модуль\n2. В urls.py (`projectname` замените на название проекта):\n```python\nfrom django.urls import path\nfrom celery_yandex_serverless.django import worker_view_factory\n\nfrom projectname.celery import app\n\nurlpatterns = [\n    # другие адреса...\n    path("worker/<str:key>/", worker_view_factory(app)),\n]\n```\n\n3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. \nОн предотвратит нежелательные запуски воркеров по прямому обращению к URL.\n\n### Создание триггера в Яндекс.Облаке\n\nВ консольной команде ниже сделайте замены и выполните ее:\n- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди (можно увидеть на странице очереди)\n- `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта\n- `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера\n- `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее\n\n```bash\nyc serverless trigger create message-queue \\\n  --name celery \\\n  --queue YANDEX_MESSAGE_QUEUE_ARN \\\n  --queue-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-name SERVERLESS_CONTAINER_NAME \\\n  --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \\\n  --batch-size 1 \\\n  --batch-cutoff 10s \n```\n\n### Включение логирования\n\nДобавьте в `settings.py`:\n```python\nLOGGING = {\n    "version": 1,\n    "disable_existing_loggers": False,\n    "loggers": {\n        "celery_yandex_serverless.django": {\n            "level": "INFO",\n        },\n    },\n}\n```\n\nУровни:\n- `INFO` - инфорация о начале и окончании обработки задачи\n- `DEBUG` - печать содержимого аргументов celery-таска\n\n## Статьи в Яндекс.Облаке\n- [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)\n- [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).\n- [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).\n\n## Обновление\n\n1. `poetry version ...` - обновить версию\n2. закомитить изменения\n3. `git tag ...` - добавить тег с версией пакета\n4. `git push --tags` - запушить тег\n5. `poetry publish --build` - опубликовать пакет\n\n## Автор\n[Атнагулов Артур](https://atnartur.dev)\n\nЛицензия MIT.\n',
     'author': 'atnartur',
     'author_email': 'i@atnartur.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `celery_yandex_serverless-0.1.3/PKG-INFO` & `celery_yandex_serverless-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-yandex-serverless
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for starting Celery worker inside Yandex Cloud Serverless Container
 Author: atnartur
 Author-email: i@atnartur.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

