# Comparing `tmp/pulumi_rabbitmq-3.4.0a1686637026.tar.gz` & `tmp/pulumi_rabbitmq-3.4.0a1686760354.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rabbitmq-3.4.0a1686637026.tar", last modified: Tue Jun 13 06:25:58 2023, max compression
+gzip compressed data, was "pulumi_rabbitmq-3.4.0a1686760354.tar", last modified: Wed Jun 14 16:38:13 2023, max compression
```

## Comparing `pulumi_rabbitmq-3.4.0a1686637026.tar` & `pulumi_rabbitmq-3.4.0a1686760354.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:25:58.151021 pulumi_rabbitmq-3.4.0a1686637026/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-13 06:25:58.147021 pulumi_rabbitmq-3.4.0a1686637026/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:25:58.147021 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:25:58.147021 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/federation_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/get_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/get_v_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/operator_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/shovel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/topic_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/v_host.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:25:58.147021 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-13 06:25:58.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 06:25:58.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:25:58.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:25:58.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:25:58.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 06:25:58.000000 pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:25:58.151021 pulumi_rabbitmq-3.4.0a1686637026/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-13 06:25:57.000000 pulumi_rabbitmq-3.4.0a1686637026/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:38:13.113179 pulumi_rabbitmq-3.4.0a1686760354/
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-14 16:38:13.113179 pulumi_rabbitmq-3.4.0a1686760354/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:38:13.113179 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:38:13.113179 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/federation_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/get_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/get_v_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/operator_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/shovel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/topic_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/v_host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:38:13.113179 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-14 16:38:13.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 16:38:13.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:38:13.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:38:13.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 16:38:13.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 16:38:13.000000 pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:38:13.113179 pulumi_rabbitmq-3.4.0a1686760354/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 16:38:12.000000 pulumi_rabbitmq-3.4.0a1686760354/setup.py
```

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1686760354/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1686637026
+Version: 3.4.0a1686760354
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi rabbitmq
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-rabbitmq/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-rabbitmq/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Frabbitmq.svg)](https://www.npmjs.com/package/@pulumi/rabbitmq)
 [![Python version](https://badge.fury.io/py/pulumi-rabbitmq.svg)](https://pypi.org/project/pulumi-rabbitmq)
 [![NuGet version](https://badge.fury.io/nu/pulumi.rabbitmq.svg)](https://badge.fury.io/nu/pulumi.rabbitmq)
```

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/README.md` & `pulumi_rabbitmq-3.4.0a1686760354/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/__init__.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/_inputs.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,24 @@
         """
         :param pulumi.Input[str] uri: The AMQP URI(s) for the upstream. Note that the URI may contain sensitive information, such as a password.
         :param pulumi.Input[str] ack_mode: Determines how the link should acknowledge messages. Valid values are `on-confirm`, `on-publish`, and `no-ack`. Default is `on-confirm`.
         :param pulumi.Input[str] exchange: The name of the upstream exchange.
         :param pulumi.Input[int] expires: The expiry time (in milliseconds) after which an upstream queue for a federated exchange may be deleted if a connection to the upstream is lost.
         :param pulumi.Input[int] max_hops: Maximum number of federation links that messages can traverse before being dropped. Default is `1`.
         :param pulumi.Input[int] message_ttl: The expiry time (in milliseconds) for messages in the upstream queue for a federated exchange (see expires).
+               
+               Applicable to Federated Queues Only
         :param pulumi.Input[int] prefetch_count: Maximum number of unacknowledged messages that may be in flight over a federation link at one time. Default is `1000`.
         :param pulumi.Input[str] queue: The name of the upstream queue.
+               
+               Consult the RabbitMQ [Federation Reference](https://www.rabbitmq.com/federation-reference.html) documentation for detailed information and guidance on setting these values.
         :param pulumi.Input[int] reconnect_delay: Time in seconds to wait after a network link goes down before attempting reconnection. Default is `5`.
         :param pulumi.Input[bool] trust_user_id: Determines how federation should interact with the validated user-id feature. Default is `false`.
+               
+               Applicable to Federated Exchanges Only
         """
         pulumi.set(__self__, "uri", uri)
         if ack_mode is not None:
             pulumi.set(__self__, "ack_mode", ack_mode)
         if exchange is not None:
             pulumi.set(__self__, "exchange", exchange)
         if expires is not None:
@@ -200,14 +206,16 @@
         pulumi.set(self, "max_hops", value)
 
     @property
     @pulumi.getter(name="messageTtl")
     def message_ttl(self) -> Optional[pulumi.Input[int]]:
         """
         The expiry time (in milliseconds) for messages in the upstream queue for a federated exchange (see expires).
+
+        Applicable to Federated Queues Only
         """
         return pulumi.get(self, "message_ttl")
 
     @message_ttl.setter
     def message_ttl(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "message_ttl", value)
 
@@ -224,14 +232,16 @@
         pulumi.set(self, "prefetch_count", value)
 
     @property
     @pulumi.getter
     def queue(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the upstream queue.
+
+        Consult the RabbitMQ [Federation Reference](https://www.rabbitmq.com/federation-reference.html) documentation for detailed information and guidance on setting these values.
         """
         return pulumi.get(self, "queue")
 
     @queue.setter
     def queue(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "queue", value)
 
@@ -248,14 +258,16 @@
         pulumi.set(self, "reconnect_delay", value)
 
     @property
     @pulumi.getter(name="trustUserId")
     def trust_user_id(self) -> Optional[pulumi.Input[bool]]:
         """
         Determines how federation should interact with the validated user-id feature. Default is `false`.
+
+        Applicable to Federated Exchanges Only
         """
         return pulumi.get(self, "trust_user_id")
 
     @trust_user_id.setter
     def trust_user_id(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "trust_user_id", value)
 
@@ -570,14 +582,16 @@
         :param pulumi.Input[bool] destination_add_forward_headers: Whether to add `x-shovelled` headers to shovelled messages.
         :param pulumi.Input[str] destination_address: The AMQP 1.0 destination link address.
         :param pulumi.Input[str] destination_application_properties: Application properties to set when shovelling messages.
         :param pulumi.Input[str] destination_exchange: The exchange to which messages should be published.
                Either this or `destination_queue` must be specified but not both.
         :param pulumi.Input[str] destination_exchange_key: The routing key when using `destination_exchange`.
         :param pulumi.Input[str] destination_properties: Properties to overwrite when shovelling messages.
+               
+               For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
         :param pulumi.Input[str] destination_protocol: The protocol (`amqp091` or `amqp10`) to use when connecting to the destination.
                Defaults to `amqp091`.
         :param pulumi.Input[str] destination_publish_properties: A map of properties to overwrite when shovelling messages.
         :param pulumi.Input[str] destination_queue: The queue to which messages should be published.
                Either this or `destination_exchange` must be specified but not both.
         :param pulumi.Input[int] prefetch_count: The maximum number of unacknowledged messages copied over a shovel at any one time.
         :param pulumi.Input[int] reconnect_delay: The duration in seconds to reconnect to a broker after disconnected.
@@ -781,14 +795,16 @@
         pulumi.set(self, "destination_exchange_key", value)
 
     @property
     @pulumi.getter(name="destinationProperties")
     def destination_properties(self) -> Optional[pulumi.Input[str]]:
         """
         Properties to overwrite when shovelling messages.
+
+        For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
         """
         return pulumi.get(self, "destination_properties")
 
     @destination_properties.setter
     def destination_properties(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_properties", value)
```

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/_utilities.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/binding.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/config/vars.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/exchange.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/federation_upstream.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/federation_upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/get_exchange.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/get_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/get_user.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/get_v_host.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/get_v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/operator_policy.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/operator_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/outputs.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,18 +139,24 @@
         """
         :param str uri: The AMQP URI(s) for the upstream. Note that the URI may contain sensitive information, such as a password.
         :param str ack_mode: Determines how the link should acknowledge messages. Valid values are `on-confirm`, `on-publish`, and `no-ack`. Default is `on-confirm`.
         :param str exchange: The name of the upstream exchange.
         :param int expires: The expiry time (in milliseconds) after which an upstream queue for a federated exchange may be deleted if a connection to the upstream is lost.
         :param int max_hops: Maximum number of federation links that messages can traverse before being dropped. Default is `1`.
         :param int message_ttl: The expiry time (in milliseconds) for messages in the upstream queue for a federated exchange (see expires).
+               
+               Applicable to Federated Queues Only
         :param int prefetch_count: Maximum number of unacknowledged messages that may be in flight over a federation link at one time. Default is `1000`.
         :param str queue: The name of the upstream queue.
+               
+               Consult the RabbitMQ [Federation Reference](https://www.rabbitmq.com/federation-reference.html) documentation for detailed information and guidance on setting these values.
         :param int reconnect_delay: Time in seconds to wait after a network link goes down before attempting reconnection. Default is `5`.
         :param bool trust_user_id: Determines how federation should interact with the validated user-id feature. Default is `false`.
+               
+               Applicable to Federated Exchanges Only
         """
         pulumi.set(__self__, "uri", uri)
         if ack_mode is not None:
             pulumi.set(__self__, "ack_mode", ack_mode)
         if exchange is not None:
             pulumi.set(__self__, "exchange", exchange)
         if expires is not None:
@@ -209,14 +215,16 @@
         return pulumi.get(self, "max_hops")
 
     @property
     @pulumi.getter(name="messageTtl")
     def message_ttl(self) -> Optional[int]:
         """
         The expiry time (in milliseconds) for messages in the upstream queue for a federated exchange (see expires).
+
+        Applicable to Federated Queues Only
         """
         return pulumi.get(self, "message_ttl")
 
     @property
     @pulumi.getter(name="prefetchCount")
     def prefetch_count(self) -> Optional[int]:
         """
@@ -225,14 +233,16 @@
         return pulumi.get(self, "prefetch_count")
 
     @property
     @pulumi.getter
     def queue(self) -> Optional[str]:
         """
         The name of the upstream queue.
+
+        Consult the RabbitMQ [Federation Reference](https://www.rabbitmq.com/federation-reference.html) documentation for detailed information and guidance on setting these values.
         """
         return pulumi.get(self, "queue")
 
     @property
     @pulumi.getter(name="reconnectDelay")
     def reconnect_delay(self) -> Optional[int]:
         """
@@ -241,14 +251,16 @@
         return pulumi.get(self, "reconnect_delay")
 
     @property
     @pulumi.getter(name="trustUserId")
     def trust_user_id(self) -> Optional[bool]:
         """
         Determines how federation should interact with the validated user-id feature. Default is `false`.
+
+        Applicable to Federated Exchanges Only
         """
         return pulumi.get(self, "trust_user_id")
 
 
 @pulumi.output_type
 class OperatorPolicyPolicy(dict):
     @staticmethod
@@ -615,14 +627,16 @@
         :param bool destination_add_forward_headers: Whether to add `x-shovelled` headers to shovelled messages.
         :param str destination_address: The AMQP 1.0 destination link address.
         :param str destination_application_properties: Application properties to set when shovelling messages.
         :param str destination_exchange: The exchange to which messages should be published.
                Either this or `destination_queue` must be specified but not both.
         :param str destination_exchange_key: The routing key when using `destination_exchange`.
         :param str destination_properties: Properties to overwrite when shovelling messages.
+               
+               For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
         :param str destination_protocol: The protocol (`amqp091` or `amqp10`) to use when connecting to the destination.
                Defaults to `amqp091`.
         :param str destination_publish_properties: A map of properties to overwrite when shovelling messages.
         :param str destination_queue: The queue to which messages should be published.
                Either this or `destination_exchange` must be specified but not both.
         :param int prefetch_count: The maximum number of unacknowledged messages copied over a shovel at any one time.
         :param int reconnect_delay: The duration in seconds to reconnect to a broker after disconnected.
@@ -773,14 +787,16 @@
         return pulumi.get(self, "destination_exchange_key")
 
     @property
     @pulumi.getter(name="destinationProperties")
     def destination_properties(self) -> Optional[str]:
         """
         Properties to overwrite when shovelling messages.
+
+        For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
         """
         return pulumi.get(self, "destination_properties")
 
     @property
     @pulumi.getter(name="destinationProtocol")
     def destination_protocol(self) -> Optional[str]:
         """
```

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/permissions.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/policy.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/provider.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/queue.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/shovel.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/shovel.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/topic_permissions.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/topic_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/user.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq/v_host.py` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq/v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-rabbitmq
-Version: 3.4.0a1686637026
+Version: 3.4.0a1686760354
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi rabbitmq
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-rabbitmq/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-rabbitmq/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Frabbitmq.svg)](https://www.npmjs.com/package/@pulumi/rabbitmq)
 [![Python version](https://badge.fury.io/py/pulumi-rabbitmq.svg)](https://pypi.org/project/pulumi-rabbitmq)
 [![NuGet version](https://badge.fury.io/nu/pulumi.rabbitmq.svg)](https://badge.fury.io/nu/pulumi.rabbitmq)
```

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/pulumi_rabbitmq.egg-info/SOURCES.txt` & `pulumi_rabbitmq-3.4.0a1686760354/pulumi_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1686637026/setup.py` & `pulumi_rabbitmq-3.4.0a1686760354/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.4.0a1686637026"
-PLUGIN_VERSION = "3.4.0-alpha.1686637026+57cc66b0"
+VERSION = "3.4.0a1686760354"
+PLUGIN_VERSION = "3.4.0-alpha.1686760354+ccde7a6c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rabbitmq', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "rabbitmq Pulumi Package - Development Version"
 
 
 setup(name='pulumi_rabbitmq',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing RabbitMQ resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

