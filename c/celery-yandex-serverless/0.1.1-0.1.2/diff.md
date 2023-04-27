# Comparing `tmp/celery_yandex_serverless-0.1.1.tar.gz` & `tmp/celery_yandex_serverless-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_yandex_serverless-0.1.1.tar", max compression
+gzip compressed data, was "celery_yandex_serverless-0.1.2.tar", max compression
```

## Comparing `celery_yandex_serverless-0.1.1.tar` & `celery_yandex_serverless-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5768 2023-04-10 11:45:26.941835 celery_yandex_serverless-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-03-28 16:34:01.621354 celery_yandex_serverless-0.1.1/celery_yandex_serverless/__init__.py
--rw-r--r--   0        0        0     3381 2023-04-10 16:32:52.281683 celery_yandex_serverless-0.1.1/celery_yandex_serverless/django.py
--rw-r--r--   0        0        0      471 2023-04-10 16:33:35.418769 celery_yandex_serverless-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.1/setup.py
--rw-r--r--   0        0        0     6438 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6145 2023-04-27 17:18:44.906103 celery_yandex_serverless-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-28 16:34:01.621354 celery_yandex_serverless-0.1.2/celery_yandex_serverless/__init__.py
+-rw-r--r--   0        0        0     3381 2023-04-10 16:32:52.281683 celery_yandex_serverless-0.1.2/celery_yandex_serverless/django.py
+-rw-r--r--   0        0        0      469 2023-04-27 17:19:01.812792 celery_yandex_serverless-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7053 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.2/setup.py
+-rw-r--r--   0        0        0     6811 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.2/PKG-INFO
```

### Comparing `celery_yandex_serverless-0.1.1/README.md` & `celery_yandex_serverless-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. 
 Он предотвратит нежелательные запуски воркеров по прямому обращению к URL.
 
 ### Создание триггера в Яндекс.Облаке
 
 В консольной команде ниже сделайте замены и выполните ее:
-- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди
+- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди (можно увидеть на странице очереди)
 - `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта
 - `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера
 - `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее
 
 ```bash
 yc serverless trigger create message-queue \
   --name celery \
@@ -123,11 +123,19 @@
 - `DEBUG` - печать содержимого аргументов celery-таска
 
 ## Статьи в Яндекс.Облаке
 - [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)
 - [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).
 - [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).
 
+## Обновление
+
+1. `poetry version ...` - обновить версию
+2. закомитить изменения
+3. `git tag ...` - добавить тег с версией пакета
+4. `git push --tags` - запушить тег
+5. `poetry publish --build` - опубликовать пакет
+
 ## Автор
 [Атнагулов Артур](https://atnartur.dev)
 
 Лицензия MIT.
```

### Comparing `celery_yandex_serverless-0.1.1/celery_yandex_serverless/django.py` & `celery_yandex_serverless-0.1.2/celery_yandex_serverless/django.py`

 * *Files identical despite different names*

### Comparing `celery_yandex_serverless-0.1.1/setup.py` & `celery_yandex_serverless-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 ['celery_yandex_serverless']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.101,<2.0.0',
- 'celery>=5.2.7,<6.0.0',
- 'django>=4,<5',
+ 'celery>=5.0,<6.0',
+ 'django>=3,<4',
  'pycurl>=7.45.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'celery-yandex-serverless',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Package for starting Celery worker inside Yandex Cloud Serverless Container',
-    'long_description': '# Celery Yandex Serverless\n\nМодуль, позволяющий запустить celery-worker внутри Yandex Cloud Serverless Container.\n\n**Классический подход с отдельно запущенным воркером**\n\n1. Бекенд отправляет задачу в очередь.\n2. Отдельный процесс воркера забирает задачу из очереди и выполняет ее.\n\n**Serverless-подход**\n\nВ Serverless подходе предполагается, что нет никаких запущенных постоянно процессов приложения. Эти процессы запускаются\nлибо по запросу пользователя, либо по различным тригерам облаком. \n\nМодуль `celery-yandex-serverless` помогает запустить воркер следующим образом:\n1. Бекенд отправляет задачу в очередь\n2. После попадания задачи в очередь срабатывает триггер, который делает http-запрос serverless-контейнеру.\n3. Serverless-контейнер запускает код задачи, который ранее выполнялся в воркере.\n\n## Использование\n\n### Подключение Celery к Yandex Message Queue\n\n1. Перейдите на страницу каталога в Яндекс.Облаке\n2. Зайдите в раздел **Сервисные аккаунты**\n3. Посмотрите название сервисного аккаунта в каталоге Яндекс.Облака\n4. Сгенерируйте `ACCESS_KEY` и `SECRET_KEY` с помощью команды \n(замените `SERVICE_ACCOUNT_NAME` на название сервисного аккаунта):\n\n```bash\nyc iam access-key create --service-account-name SERVICE_ACCOUNT_NAME\n```\n\nКоманда вернет следующую информацию. Сохраните ее, она пригодится в будущем.\n\n```yml{5,6}\naccess_key:\n  id: aje...\n  service_account_id: aje...\n  created_at: "2023-03-24T17:49:01.555836400Z"\n  key_id: YCAJ... # <- Это access key\nsecret: YCPM... # <- Это secret key\n```\n\n### Настройка\nУкажите переменные окружения с использованием только что полученных данных:\n\n```\nAWS_ACCESS_KEY_ID="access key, скопированный выше"\nAWS_SECRET_ACCESS_KEY="secret key, скопированный выше"\nAWS_DEFAULT_REGION="ru-central1"\nCELERY_BROKER_URL=sqs://message-queue.api.cloud.yandex.net:443\nCELERY_BROKER_IS_SECURE=True\n```\n\nВ файле `settings.py` укажите:\n\n```python\nCELERY_BROKER_URL = os.environ.get("CELERY_BROKER_URL")\nCELERY_BROKER_TRANSPORT_OPTIONS = {\n    \'is_secure\': os.environ.get("CELERY_BROKER_IS_SECURE", \'false\').lower() == \'true\'\n}\n```\n\nПосле этого отправьте celery-задачу, чтобы в Яндекс.Облаке появилась очередь.\n\n### Подключение модуля\n\n1. `pip install celery-yandex-serverless` - установите модуль\n2. В urls.py (`projectname` замените на название проекта):\n```python\nfrom django.urls import path\nfrom celery_yandex_serverless.django import worker_view_factory\n\nfrom projectname.celery import app\n\nurlpatterns = [\n    # другие адреса...\n    path("worker/<str:key>/", worker_view_factory(app)),\n]\n```\n\n3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. \nОн предотвратит нежелательные запуски воркеров по прямому обращению к URL.\n\n### Создание триггера в Яндекс.Облаке\n\nВ консольной команде ниже сделайте замены и выполните ее:\n- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди\n- `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта\n- `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера\n- `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее\n\n```bash\nyc serverless trigger create message-queue \\\n  --name celery \\\n  --queue YANDEX_MESSAGE_QUEUE_ARN \\\n  --queue-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-name SERVERLESS_CONTAINER_NAME \\\n  --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \\\n  --batch-size 1 \\\n  --batch-cutoff 10s \n```\n\n### Включение логирования\n\nДобавьте в `settings.py`:\n```python\nLOGGING = {\n    "version": 1,\n    "disable_existing_loggers": False,\n    "loggers": {\n        "celery_yandex_serverless.django": {\n            "level": "INFO",\n        },\n    },\n}\n```\n\nУровни:\n- `INFO` - инфорация о начале и окончании обработки задачи\n- `DEBUG` - печать содержимого аргументов celery-таска\n\n## Статьи в Яндекс.Облаке\n- [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)\n- [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).\n- [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).\n\n## Автор\n[Атнагулов Артур](https://atnartur.dev)\n\nЛицензия MIT.\n',
+    'long_description': '# Celery Yandex Serverless\n\nМодуль, позволяющий запустить celery-worker внутри Yandex Cloud Serverless Container.\n\n**Классический подход с отдельно запущенным воркером**\n\n1. Бекенд отправляет задачу в очередь.\n2. Отдельный процесс воркера забирает задачу из очереди и выполняет ее.\n\n**Serverless-подход**\n\nВ Serverless подходе предполагается, что нет никаких запущенных постоянно процессов приложения. Эти процессы запускаются\nлибо по запросу пользователя, либо по различным тригерам облаком. \n\nМодуль `celery-yandex-serverless` помогает запустить воркер следующим образом:\n1. Бекенд отправляет задачу в очередь\n2. После попадания задачи в очередь срабатывает триггер, который делает http-запрос serverless-контейнеру.\n3. Serverless-контейнер запускает код задачи, который ранее выполнялся в воркере.\n\n## Использование\n\n### Подключение Celery к Yandex Message Queue\n\n1. Перейдите на страницу каталога в Яндекс.Облаке\n2. Зайдите в раздел **Сервисные аккаунты**\n3. Посмотрите название сервисного аккаунта в каталоге Яндекс.Облака\n4. Сгенерируйте `ACCESS_KEY` и `SECRET_KEY` с помощью команды \n(замените `SERVICE_ACCOUNT_NAME` на название сервисного аккаунта):\n\n```bash\nyc iam access-key create --service-account-name SERVICE_ACCOUNT_NAME\n```\n\nКоманда вернет следующую информацию. Сохраните ее, она пригодится в будущем.\n\n```yml{5,6}\naccess_key:\n  id: aje...\n  service_account_id: aje...\n  created_at: "2023-03-24T17:49:01.555836400Z"\n  key_id: YCAJ... # <- Это access key\nsecret: YCPM... # <- Это secret key\n```\n\n### Настройка\nУкажите переменные окружения с использованием только что полученных данных:\n\n```\nAWS_ACCESS_KEY_ID="access key, скопированный выше"\nAWS_SECRET_ACCESS_KEY="secret key, скопированный выше"\nAWS_DEFAULT_REGION="ru-central1"\nCELERY_BROKER_URL=sqs://message-queue.api.cloud.yandex.net:443\nCELERY_BROKER_IS_SECURE=True\n```\n\nВ файле `settings.py` укажите:\n\n```python\nCELERY_BROKER_URL = os.environ.get("CELERY_BROKER_URL")\nCELERY_BROKER_TRANSPORT_OPTIONS = {\n    \'is_secure\': os.environ.get("CELERY_BROKER_IS_SECURE", \'false\').lower() == \'true\'\n}\n```\n\nПосле этого отправьте celery-задачу, чтобы в Яндекс.Облаке появилась очередь.\n\n### Подключение модуля\n\n1. `pip install celery-yandex-serverless` - установите модуль\n2. В urls.py (`projectname` замените на название проекта):\n```python\nfrom django.urls import path\nfrom celery_yandex_serverless.django import worker_view_factory\n\nfrom projectname.celery import app\n\nurlpatterns = [\n    # другие адреса...\n    path("worker/<str:key>/", worker_view_factory(app)),\n]\n```\n\n3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. \nОн предотвратит нежелательные запуски воркеров по прямому обращению к URL.\n\n### Создание триггера в Яндекс.Облаке\n\nВ консольной команде ниже сделайте замены и выполните ее:\n- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди (можно увидеть на странице очереди)\n- `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта\n- `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера\n- `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее\n\n```bash\nyc serverless trigger create message-queue \\\n  --name celery \\\n  --queue YANDEX_MESSAGE_QUEUE_ARN \\\n  --queue-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-name SERVERLESS_CONTAINER_NAME \\\n  --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \\\n  --batch-size 1 \\\n  --batch-cutoff 10s \n```\n\n### Включение логирования\n\nДобавьте в `settings.py`:\n```python\nLOGGING = {\n    "version": 1,\n    "disable_existing_loggers": False,\n    "loggers": {\n        "celery_yandex_serverless.django": {\n            "level": "INFO",\n        },\n    },\n}\n```\n\nУровни:\n- `INFO` - инфорация о начале и окончании обработки задачи\n- `DEBUG` - печать содержимого аргументов celery-таска\n\n## Статьи в Яндекс.Облаке\n- [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)\n- [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).\n- [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).\n\n## Обновление\n\n1. `poetry version ...` - обновить версию\n2. закомитить изменения\n3. `git tag ...` - добавить тег с версией пакета\n4. `git push --tags` - запушить тег\n5. `poetry publish --build` - опубликовать пакет\n\n## Автор\n[Атнагулов Артур](https://atnartur.dev)\n\nЛицензия MIT.\n',
     'author': 'atnartur',
     'author_email': 'i@atnartur.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `celery_yandex_serverless-0.1.1/PKG-INFO` & `celery_yandex_serverless-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: celery-yandex-serverless
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for starting Celery worker inside Yandex Cloud Serverless Container
 Author: atnartur
 Author-email: i@atnartur.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.101,<2.0.0)
-Requires-Dist: celery (>=5.2.7,<6.0.0)
-Requires-Dist: django (>=4,<5)
+Requires-Dist: celery (>=5.0,<6.0)
+Requires-Dist: django (>=3,<4)
 Requires-Dist: pycurl (>=7.45.2,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Celery Yandex Serverless
 
 Модуль, позволяющий запустить celery-worker внутри Yandex Cloud Serverless Container.
 
@@ -100,15 +100,15 @@
 
 3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. 
 Он предотвратит нежелательные запуски воркеров по прямому обращению к URL.
 
 ### Создание триггера в Яндекс.Облаке
 
 В консольной команде ниже сделайте замены и выполните ее:
-- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди
+- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди (можно увидеть на странице очереди)
 - `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта
 - `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера
 - `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее
 
 ```bash
 yc serverless trigger create message-queue \
   --name celery \
@@ -141,12 +141,20 @@
 - `DEBUG` - печать содержимого аргументов celery-таска
 
 ## Статьи в Яндекс.Облаке
 - [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)
 - [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).
 - [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).
 
+## Обновление
+
+1. `poetry version ...` - обновить версию
+2. закомитить изменения
+3. `git tag ...` - добавить тег с версией пакета
+4. `git push --tags` - запушить тег
+5. `poetry publish --build` - опубликовать пакет
+
 ## Автор
 [Атнагулов Артур](https://atnartur.dev)
 
 Лицензия MIT.
```

