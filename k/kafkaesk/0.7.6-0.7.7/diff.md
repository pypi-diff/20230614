# Comparing `tmp/kafkaesk-0.7.6.tar.gz` & `tmp/kafkaesk-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaesk-0.7.6.tar", max compression
+gzip compressed data, was "kafkaesk-0.7.7.tar", max compression
```

## Comparing `kafkaesk-0.7.6.tar` & `kafkaesk-0.7.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1314 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/LICENSE
--rw-r--r--   0        0        0     8653 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/README.md
--rw-r--r--   0        0        0      208 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/__init__.py
--rw-r--r--   0        0        0    22572 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/app.py
--rw-r--r--   0        0        0    18351 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/consumer.py
--rw-r--r--   0        0        0     1121 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/ext/__init__.py
--rw-r--r--   0        0        0      210 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/ext/logging/__init__.py
--rw-r--r--   0        0        0     7620 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/ext/logging/handler.py
--rw-r--r--   0        0        0     1719 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/ext/logging/record.py
--rw-r--r--   0        0        0     5081 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/kafka.py
--rw-r--r--   0        0        0     3980 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/metrics.py
--rw-r--r--   0        0        0        0 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/publish.py
--rw-r--r--   0        0        0        0 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/py.typed
--rw-r--r--   0        0        0      904 2023-01-27 17:08:59.293581 kafkaesk-0.7.6/kafkaesk/utils.py
--rw-r--r--   0        0        0     1674 2023-01-27 17:08:59.297581 kafkaesk-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     9928 1970-01-01 00:00:00.000000 kafkaesk-0.7.6/setup.py
--rw-r--r--   0        0        0     9877 1970-01-01 00:00:00.000000 kafkaesk-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1314 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/LICENSE
+-rw-r--r--   0        0        0     8653 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/README.md
+-rw-r--r--   0        0        0      208 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/__init__.py
+-rw-r--r--   0        0        0    22572 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/app.py
+-rw-r--r--   0        0        0    18351 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/consumer.py
+-rw-r--r--   0        0        0     1121 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/ext/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/ext/logging/__init__.py
+-rw-r--r--   0        0        0     7620 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/ext/logging/handler.py
+-rw-r--r--   0        0        0     1719 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/ext/logging/record.py
+-rw-r--r--   0        0        0     5081 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/kafka.py
+-rw-r--r--   0        0        0     3980 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/publish.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/py.typed
+-rw-r--r--   0        0        0      904 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/kafkaesk/utils.py
+-rw-r--r--   0        0        0     1675 2023-05-01 19:11:14.265697 kafkaesk-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     9870 1970-01-01 00:00:00.000000 kafkaesk-0.7.7/PKG-INFO
```

### Comparing `kafkaesk-0.7.6/LICENSE` & `kafkaesk-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/README.md` & `kafkaesk-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/app.py` & `kafkaesk-0.7.7/kafkaesk/app.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/consumer.py` & `kafkaesk-0.7.7/kafkaesk/consumer.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/exceptions.py` & `kafkaesk-0.7.7/kafkaesk/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/ext/logging/handler.py` & `kafkaesk-0.7.7/kafkaesk/ext/logging/handler.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/ext/logging/record.py` & `kafkaesk-0.7.7/kafkaesk/ext/logging/record.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/kafka.py` & `kafkaesk-0.7.7/kafkaesk/kafka.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/metrics.py` & `kafkaesk-0.7.7/kafkaesk/metrics.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/kafkaesk/utils.py` & `kafkaesk-0.7.7/kafkaesk/utils.py`

 * *Files identical despite different names*

### Comparing `kafkaesk-0.7.6/pyproject.toml` & `kafkaesk-0.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafkaesk"
-version = "0.7.6"
+version = "0.7.7"
 description = "Easy publish and subscribe to events with python and Kafka."
 authors = ["vangheem <vangheem@gmail.com>", "pfreixes <pfreixes@gmail.com>"]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Framework :: AsyncIO",
@@ -19,15 +19,15 @@
 aiokafka = "^0.7.0"
 kafka-python = "^2.0.1"
 pydantic = "^1.5.1"
 orjson = "^3.3.1"
 jsonschema = "^3.2.0"
 prometheus_client = ">= 0.8.0"
 opentracing = "^2.3.0"
-async-timeout = "^3.0.1"
+async-timeout = ">=3.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pytest-docker-fixtures = "^1.3.7"
 pytest-asyncio = "^0.12.0"
 mypy = "0.770"
 flake8 = "^3.8.1"
```

### Comparing `kafkaesk-0.7.6/setup.py` & `kafkaesk-0.7.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,309 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kafkaesk
+Version: 0.7.7
+Summary: Easy publish and subscribe to events with python and Kafka.
+Author: vangheem
+Author-email: vangheem@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Framework :: AsyncIO
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: System :: Distributed Computing
+Requires-Dist: aiokafka (>=0.7.0,<0.8.0)
+Requires-Dist: async-timeout (>=3.0.1)
+Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
+Requires-Dist: kafka-python (>=2.0.1,<3.0.0)
+Requires-Dist: opentracing (>=2.3.0,<3.0.0)
+Requires-Dist: orjson (>=3.3.1,<4.0.0)
+Requires-Dist: prometheus_client (>=0.8.0)
+Requires-Dist: pydantic (>=1.5.1,<2.0.0)
+Project-URL: GitHub, https://github.com/onna/kafkaesk
+Description-Content-Type: text/markdown
 
-packages = \
-['kafkaesk', 'kafkaesk.ext', 'kafkaesk.ext.logging']
+<!-- PROJECT LOGO -->
+<h1 align="center">
+  <br>
+  <img src="https://onna.com/wp-content/uploads/2020/03/h-onna-solid.png" alt="Onna Logo"></a>
+</h1>
 
-package_data = \
-{'': ['*']}
+<h2 align="center">kafkaesk</h2>
 
-install_requires = \
-['aiokafka>=0.7.0,<0.8.0',
- 'async-timeout>=3.0.1,<4.0.0',
- 'jsonschema>=3.2.0,<4.0.0',
- 'kafka-python>=2.0.1,<3.0.0',
- 'opentracing>=2.3.0,<3.0.0',
- 'orjson>=3.3.1,<4.0.0',
- 'prometheus_client>=0.8.0',
- 'pydantic>=1.5.1,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['kafkaesk = kafkaesk.app:run']}
-
-setup_kwargs = {
-    'name': 'kafkaesk',
-    'version': '0.7.6',
-    'description': 'Easy publish and subscribe to events with python and Kafka.',
-    'long_description': '<!-- PROJECT LOGO -->\n<h1 align="center">\n  <br>\n  <img src="https://onna.com/wp-content/uploads/2020/03/h-onna-solid.png" alt="Onna Logo"></a>\n</h1>\n\n<h2 align="center">kafkaesk</h2>\n\n<!-- TABLE OF CONTENTS -->\n## Table Of Contents\n\n- [About the Project](#about-the-project)\n- [Publish](#publish)\n- [Subscribe](#subscribe)\n- [Avoiding global object](#avoiding-global-object)\n- [Manual commit](#manual-commit)\n- [kafkaesk contract](#kafkaesk-contract)\n- [Worker](#worker)\n- [Development](#development)\n- [Extensions](#extensions)\n- [Naming](#naming)\n\n\n## About The Project\n\nThis project is meant to help facilitate effortless publishing and subscribing to events with Python and Kafka.\n\n### Guiding principal\n\n- HTTP\n- Language agnostic\n- Contracts built on top of [Kafka](https://kafka.apache.org/)\n\n\n### Alternatives\n - [aiokafka](https://aiokafka.readthedocs.io/en/stable/): can be complex to scale correctly\n - [guillotina_kafka](https://github.com/onna/guillotina_kafka): complex, tied to [Guillotina](https://guillotina.readthedocs.io/en/latest/)\n - [faust](https://faust.readthedocs.io/en/latest/): requires additional data layers, not language agnostic\n - confluent kafka + avro: close but ends up being like grpc. compilation for languages. No asyncio.\n\n> Consider this Python project as syntactic sugar around these ideas.\n\n## Publish\n\nUsing [pydantic](https://pydantic-docs.helpmanual.io/) but can be done with pure JSON.\n\n```python\nimport kafkaesk\nfrom pydantic import BaseModel\n\napp = kafkaesk.Application()\n\n@app.schema("Content", version=1, retention=24 * 60 * 60)\nclass ContentMessage(BaseModel):\n    foo: str\n\n\nasync def foobar():\n    # ...\n    # doing something in an async func\n    await app.publish("content.edited.Resource", data=ContentMessage(foo="bar"))\n```\n\nA convenience method is available in the `subscriber` dependency instance, this allow to header\npropagation from the consumed message.\n\n```python\nimport kafkaesk\nfrom pydantic import BaseModel\n\napp = kafkaesk.Application()\n\n@app.schema("Content", version=1, retention=24 * 60 * 60)\nclass ContentMessage(BaseModel):\n    foo: str\n\n\n@app.subscribe("content.*", "group_id")\nasync def get_messages(data: ContentMessage, subscriber):\n    print(f"{data.foo}")\n    # This will propagate `data` record headers\n    await subscriber.publish("content.edited.Resource", data=ContentMessage(foo="bar"))\n\n```\n\n## Subscribe\n\n```python\nimport kafkaesk\nfrom pydantic import BaseModel\n\napp = kafkaesk.Application()\n\n@app.schema("Content", version=1, retention=24 * 60 * 60)\nclass ContentMessage(BaseModel):\n    foo: str\n\n\n@app.subscribe("content.*", "group_id")\nasync def get_messages(data: ContentMessage):\n    print(f"{data.foo}")\n\n```\n\n## Avoiding global object\n\nIf you do not want to have global application configuration, you can lazily configure\nthe application and register schemas/subscribers separately.\n\n```python\nimport kafkaesk\nfrom pydantic import BaseModel\n\nrouter = kafkaesk.Router()\n\n@router.schema("Content", version=1, retention=24 * 60 * 60)\nclass ContentMessage(BaseModel):\n    foo: str\n\n\n@router.subscribe("content.*", "group_id")\nasync def get_messages(data: ContentMessage):\n    print(f"{data.foo}")\n\n\nif __name__ == "__main__":\n    app = kafkaesk.Application()\n    app.mount(router)\n    kafkaesk.run(app)\n\n```\n\nOptional consumer injected parameters:\n\n- schema: str\n- record: aiokafka.structs.ConsumerRecord\n- app: kafkaesk.app.Application\n- subscriber: kafkaesk.app.BatchConsumer\n\nDepending on the type annotation for the first parameter, you will get different data injected:\n\n- `async def get_messages(data: ContentMessage)`: parses pydantic schema\n- `async def get_messages(data: bytes)`: give raw byte data\n- `async def get_messages(record: aiokafka.structs.ConsumerRecord)`: give kafka record object\n- `async def get_messages(data)`: raw json data in message\n\n## Manual commit\n\nTo accomplish a manual commit strategy yourself:\n\n```python\napp = kafkaesk.Application(auto_commit=False)\n\n@app.subscribe("content.*", "group_id")\nasync def get_messages(data: ContentMessage, subscriber):\n    print(f"{data.foo}")\n    await subscriber.consumer.commit()\n```\n\n## SSL\nAdd these values to your `kafak_settings`:\n    `ssl_context` - this should be a placeholder as the SSL Context is generally created within the application\n    `security_protocol` - one of SSL or PLAINTEXT\n    `sasl_mechanism` - one of PLAIN, GSSAPI, SCRAM-SHA-256, SCRAM-SHA-512, OAUTHBEARER\n    `sasl_plain_username`\n    `sasl_plain_password`\n\n## kafkaesk contract\n\nThis is a library around using kafka.\nKafka itself does not enforce these concepts.\n\n- Every message must provide a json schema\n- Messages produced will be validated against json schema\n- Each topic will have only one schema\n- A single schema can be used for multiple topics\n- Consumed message schema validation is up to the consumer\n- Messages will be consumed at least once. Considering this, your handling should be idempotent\n\n### Message format\n\n```json\n{\n    "schema": "schema_name:1",\n    "data": { ... }\n}\n```\n\n## Worker\n\n```bash\nkafkaesk mymodule:app --kafka-servers=localhost:9092\n```\n\nOptions:\n\n - --kafka-servers: comma separated list of kafka servers\n - --kafka-settings: json encoded options to be passed to https://aiokafka.readthedocs.io/en/stable/api.html#aiokafkaconsumer-class\n - --topic-prefix: prefix to use for topics\n - --replication-factor: what replication factor topics should be created with. Defaults to min(number of servers, 3).\n\n### Application.publish\n\n- stream_id: str: name of stream to send data to\n- data: class that inherits from pydantic.BaseModel\n- key: Optional[bytes]: key for message if it needs one\n\n### Application.subscribe\n\n- stream_id: str: fnmatch pattern of streams to subscribe to\n- group: Optional[str]: consumer group id to use. Will use name of function if not provided\n\n### Application.schema\n\n- id: str: id of the schema to store\n- version: Optional[int]: version of schema to store\n- streams: Optional[List[str]]: if streams are known ahead of time, you can pre-create them before you push data\n- retention: Optional[int]: retention policy in seconds\n\n### Application.configure\n\n- kafka_servers: Optional[List[str]]: kafka servers to connect to\n- topic_prefix: Optional[str]: topic name prefix to subscribe to\n- kafka_settings: Optional[Dict[str, Any]]: additional aiokafka settings to pass in\n- replication_factor: Optional[int]: what replication factor topics should be created with. Defaults to min(number of servers, 3).\n- kafka_api_version: str: default `auto`\n- auto_commit: bool: default `True`\n- auto_commit_interval_ms: int: default `5000`\n\n## Development\n\n### Requirements\n\n- [Docker](https://www.docker.com/)\n- [Poetry](https://python-poetry.org/)\n\n```bash\npoetry install\n```\n\nRun tests:\n\n```bash\ndocker-compose up\nKAFKA=localhost:9092 poetry run pytest tests\n```\n\n## Extensions\n\n### Logging\nThis extension includes classes to extend Python\'s logging framework to publish structured log messages to a Kafka topic.\nThis extension is made up of three main components: an extended `logging.LogRecord` and some custom `logging.Handler`s.\n\nSee `logger.py` in examples directory.\n\n#### Log Record\n`kafkaesk.ext.logging.record.factory` is a function that will return `kafkaesk.ext.logging.record.PydanticLogRecord` objects.\nThe `factory()` function scans through any `args` passed to a logger and checks each item to determine if it is a subclass of `pydantid.BaseModel`.\n\nIf it is a base model instance and `model._is_log_model` evaluates to `True` the model will be removed from `args` and added to `record._pydantic_data`.\nAfter that `factory()` will use logging\'s existing logic to finish creating the log record.\n\n### Handler\nThis extensions ships with two handlers capable of handling `kafkaesk.ext.logging.handler.PydanticLogModel` classes: `kafakesk.ext.logging.handler.PydanticStreamHandler` and `kafkaesk.ext.logging.handler.PydanticKafkaeskHandler`.\n\nThe stream handler is a very small wrapper around `logging.StreamHandler`, the signature is the same, the only difference is that the handler will attempt to convert any pydantic models it receives to a human readable log message.\n\nThe kafkaesk handler has a few more bits going on in the background.\n\nThe handler has two required inputs, a `kafkaesk.app.Application` instance and a stream name.\n\nOnce initialized any logs emitted by the handler will be saved into an internal queue.\nThere is a worker task that handles pulling logs from the queue and writing those logs to the specified topic.\n\n# Naming\n\nIt\'s hard and "kafka" is already a fun name.\nHopefully this library isn\'t literally "kafkaesque" for you.\n',
-    'author': 'vangheem',
-    'author_email': 'vangheem@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+<!-- TABLE OF CONTENTS -->
+## Table Of Contents
+
+- [About the Project](#about-the-project)
+- [Publish](#publish)
+- [Subscribe](#subscribe)
+- [Avoiding global object](#avoiding-global-object)
+- [Manual commit](#manual-commit)
+- [kafkaesk contract](#kafkaesk-contract)
+- [Worker](#worker)
+- [Development](#development)
+- [Extensions](#extensions)
+- [Naming](#naming)
+
+
+## About The Project
+
+This project is meant to help facilitate effortless publishing and subscribing to events with Python and Kafka.
+
+### Guiding principal
+
+- HTTP
+- Language agnostic
+- Contracts built on top of [Kafka](https://kafka.apache.org/)
+
+
+### Alternatives
+ - [aiokafka](https://aiokafka.readthedocs.io/en/stable/): can be complex to scale correctly
+ - [guillotina_kafka](https://github.com/onna/guillotina_kafka): complex, tied to [Guillotina](https://guillotina.readthedocs.io/en/latest/)
+ - [faust](https://faust.readthedocs.io/en/latest/): requires additional data layers, not language agnostic
+ - confluent kafka + avro: close but ends up being like grpc. compilation for languages. No asyncio.
+
+> Consider this Python project as syntactic sugar around these ideas.
+
+## Publish
+
+Using [pydantic](https://pydantic-docs.helpmanual.io/) but can be done with pure JSON.
+
+```python
+import kafkaesk
+from pydantic import BaseModel
+
+app = kafkaesk.Application()
+
+@app.schema("Content", version=1, retention=24 * 60 * 60)
+class ContentMessage(BaseModel):
+    foo: str
+
+
+async def foobar():
+    # ...
+    # doing something in an async func
+    await app.publish("content.edited.Resource", data=ContentMessage(foo="bar"))
+```
+
+A convenience method is available in the `subscriber` dependency instance, this allow to header
+propagation from the consumed message.
+
+```python
+import kafkaesk
+from pydantic import BaseModel
+
+app = kafkaesk.Application()
+
+@app.schema("Content", version=1, retention=24 * 60 * 60)
+class ContentMessage(BaseModel):
+    foo: str
+
+
+@app.subscribe("content.*", "group_id")
+async def get_messages(data: ContentMessage, subscriber):
+    print(f"{data.foo}")
+    # This will propagate `data` record headers
+    await subscriber.publish("content.edited.Resource", data=ContentMessage(foo="bar"))
+
+```
+
+## Subscribe
+
+```python
+import kafkaesk
+from pydantic import BaseModel
+
+app = kafkaesk.Application()
+
+@app.schema("Content", version=1, retention=24 * 60 * 60)
+class ContentMessage(BaseModel):
+    foo: str
+
+
+@app.subscribe("content.*", "group_id")
+async def get_messages(data: ContentMessage):
+    print(f"{data.foo}")
+
+```
+
+## Avoiding global object
+
+If you do not want to have global application configuration, you can lazily configure
+the application and register schemas/subscribers separately.
+
+```python
+import kafkaesk
+from pydantic import BaseModel
+
+router = kafkaesk.Router()
+
+@router.schema("Content", version=1, retention=24 * 60 * 60)
+class ContentMessage(BaseModel):
+    foo: str
+
+
+@router.subscribe("content.*", "group_id")
+async def get_messages(data: ContentMessage):
+    print(f"{data.foo}")
+
+
+if __name__ == "__main__":
+    app = kafkaesk.Application()
+    app.mount(router)
+    kafkaesk.run(app)
+
+```
+
+Optional consumer injected parameters:
+
+- schema: str
+- record: aiokafka.structs.ConsumerRecord
+- app: kafkaesk.app.Application
+- subscriber: kafkaesk.app.BatchConsumer
+
+Depending on the type annotation for the first parameter, you will get different data injected:
+
+- `async def get_messages(data: ContentMessage)`: parses pydantic schema
+- `async def get_messages(data: bytes)`: give raw byte data
+- `async def get_messages(record: aiokafka.structs.ConsumerRecord)`: give kafka record object
+- `async def get_messages(data)`: raw json data in message
+
+## Manual commit
+
+To accomplish a manual commit strategy yourself:
+
+```python
+app = kafkaesk.Application(auto_commit=False)
+
+@app.subscribe("content.*", "group_id")
+async def get_messages(data: ContentMessage, subscriber):
+    print(f"{data.foo}")
+    await subscriber.consumer.commit()
+```
+
+## SSL
+Add these values to your `kafak_settings`:
+    `ssl_context` - this should be a placeholder as the SSL Context is generally created within the application
+    `security_protocol` - one of SSL or PLAINTEXT
+    `sasl_mechanism` - one of PLAIN, GSSAPI, SCRAM-SHA-256, SCRAM-SHA-512, OAUTHBEARER
+    `sasl_plain_username`
+    `sasl_plain_password`
+
+## kafkaesk contract
+
+This is a library around using kafka.
+Kafka itself does not enforce these concepts.
+
+- Every message must provide a json schema
+- Messages produced will be validated against json schema
+- Each topic will have only one schema
+- A single schema can be used for multiple topics
+- Consumed message schema validation is up to the consumer
+- Messages will be consumed at least once. Considering this, your handling should be idempotent
+
+### Message format
+
+```json
+{
+    "schema": "schema_name:1",
+    "data": { ... }
 }
+```
+
+## Worker
+
+```bash
+kafkaesk mymodule:app --kafka-servers=localhost:9092
+```
+
+Options:
+
+ - --kafka-servers: comma separated list of kafka servers
+ - --kafka-settings: json encoded options to be passed to https://aiokafka.readthedocs.io/en/stable/api.html#aiokafkaconsumer-class
+ - --topic-prefix: prefix to use for topics
+ - --replication-factor: what replication factor topics should be created with. Defaults to min(number of servers, 3).
+
+### Application.publish
+
+- stream_id: str: name of stream to send data to
+- data: class that inherits from pydantic.BaseModel
+- key: Optional[bytes]: key for message if it needs one
+
+### Application.subscribe
+
+- stream_id: str: fnmatch pattern of streams to subscribe to
+- group: Optional[str]: consumer group id to use. Will use name of function if not provided
+
+### Application.schema
+
+- id: str: id of the schema to store
+- version: Optional[int]: version of schema to store
+- streams: Optional[List[str]]: if streams are known ahead of time, you can pre-create them before you push data
+- retention: Optional[int]: retention policy in seconds
+
+### Application.configure
+
+- kafka_servers: Optional[List[str]]: kafka servers to connect to
+- topic_prefix: Optional[str]: topic name prefix to subscribe to
+- kafka_settings: Optional[Dict[str, Any]]: additional aiokafka settings to pass in
+- replication_factor: Optional[int]: what replication factor topics should be created with. Defaults to min(number of servers, 3).
+- kafka_api_version: str: default `auto`
+- auto_commit: bool: default `True`
+- auto_commit_interval_ms: int: default `5000`
+
+## Development
+
+### Requirements
+
+- [Docker](https://www.docker.com/)
+- [Poetry](https://python-poetry.org/)
+
+```bash
+poetry install
+```
+
+Run tests:
+
+```bash
+docker-compose up
+KAFKA=localhost:9092 poetry run pytest tests
+```
+
+## Extensions
+
+### Logging
+This extension includes classes to extend Python's logging framework to publish structured log messages to a Kafka topic.
+This extension is made up of three main components: an extended `logging.LogRecord` and some custom `logging.Handler`s.
+
+See `logger.py` in examples directory.
+
+#### Log Record
+`kafkaesk.ext.logging.record.factory` is a function that will return `kafkaesk.ext.logging.record.PydanticLogRecord` objects.
+The `factory()` function scans through any `args` passed to a logger and checks each item to determine if it is a subclass of `pydantid.BaseModel`.
+
+If it is a base model instance and `model._is_log_model` evaluates to `True` the model will be removed from `args` and added to `record._pydantic_data`.
+After that `factory()` will use logging's existing logic to finish creating the log record.
+
+### Handler
+This extensions ships with two handlers capable of handling `kafkaesk.ext.logging.handler.PydanticLogModel` classes: `kafakesk.ext.logging.handler.PydanticStreamHandler` and `kafkaesk.ext.logging.handler.PydanticKafkaeskHandler`.
+
+The stream handler is a very small wrapper around `logging.StreamHandler`, the signature is the same, the only difference is that the handler will attempt to convert any pydantic models it receives to a human readable log message.
+
+The kafkaesk handler has a few more bits going on in the background.
+
+The handler has two required inputs, a `kafkaesk.app.Application` instance and a stream name.
+
+Once initialized any logs emitted by the handler will be saved into an internal queue.
+There is a worker task that handles pulling logs from the queue and writing those logs to the specified topic.
+
+# Naming
 
+It's hard and "kafka" is already a fun name.
+Hopefully this library isn't literally "kafkaesque" for you.
 
-setup(**setup_kwargs)
```

