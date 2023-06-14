# Comparing `tmp/gardener-cicd-whd-1.2078.0.tar.gz` & `tmp/gardener-cicd-whd-1.2079.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-whd-1.2078.0.tar", last modified: Wed Jun 14 08:20:55 2023, max compression
+gzip compressed data, was "gardener-cicd-whd-1.2079.0.tar", last modified: Wed Jun 14 10:23:39 2023, max compression
```

## Comparing `gardener-cicd-whd-1.2078.0.tar` & `gardener-cicd-whd-1.2079.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:20:55.229835 gardener-cicd-whd-1.2078.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-14 08:20:55.229835 gardener-cicd-whd-1.2078.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:20:55.225835 gardener-cicd-whd-1.2078.0/gardener_cicd_whd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-14 08:20:55.000000 gardener-cicd-whd-1.2078.0/gardener_cicd_whd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      405 2023-06-14 08:20:55.000000 gardener-cicd-whd-1.2078.0/gardener_cicd_whd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 08:20:55.000000 gardener-cicd-whd-1.2078.0/gardener_cicd_whd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-14 08:20:55.000000 gardener-cicd-whd-1.2078.0/gardener_cicd_whd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-14 08:20:55.000000 gardener-cicd-whd-1.2078.0/gardener_cicd_whd.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-14 08:20:55.229835 gardener-cicd-whd-1.2078.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/setup.whd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:20:55.229835 gardener-cicd-whd-1.2078.0/whd/
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16972 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/metric.py
--rw-r--r--   0 root         (0) root         (0)     6297 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/model.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/pipelines.py
--rw-r--r--   0 root         (0) root         (0)    18333 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/pull_request.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/server.py
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/util.py
--rw-r--r--   0 root         (0) root         (0)     3704 2023-06-14 08:19:53.000000 gardener-cicd-whd-1.2078.0/whd/webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 10:23:39.941493 gardener-cicd-whd-1.2079.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-14 10:23:39.941493 gardener-cicd-whd-1.2079.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 10:23:39.937493 gardener-cicd-whd-1.2079.0/gardener_cicd_whd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-14 10:23:39.000000 gardener-cicd-whd-1.2079.0/gardener_cicd_whd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2023-06-14 10:23:39.000000 gardener-cicd-whd-1.2079.0/gardener_cicd_whd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 10:23:39.000000 gardener-cicd-whd-1.2079.0/gardener_cicd_whd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-14 10:23:39.000000 gardener-cicd-whd-1.2079.0/gardener_cicd_whd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-14 10:23:39.000000 gardener-cicd-whd-1.2079.0/gardener_cicd_whd.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-14 10:23:39.941493 gardener-cicd-whd-1.2079.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/setup.whd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 10:23:39.941493 gardener-cicd-whd-1.2079.0/whd/
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17283 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/metric.py
+-rw-r--r--   0 root         (0) root         (0)     6297 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/model.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    18333 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/pull_request.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/server.py
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/util.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2023-06-14 10:23:03.000000 gardener-cicd-whd-1.2079.0/whd/webhook.py
```

### Comparing `gardener-cicd-whd-1.2078.0/LICENSE.md` & `gardener-cicd-whd-1.2079.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/README.md` & `gardener-cicd-whd-1.2079.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/setup.py` & `gardener-cicd-whd-1.2079.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/setup.whd.py` & `gardener-cicd-whd-1.2079.0/setup.whd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/__init__.py` & `gardener-cicd-whd-1.2079.0/whd/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/dispatcher.py` & `gardener-cicd-whd-1.2079.0/whd/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,87 +96,102 @@
         dispatch_start_time: datetime.datetime,
     ):
         ref_type = create_event.ref_type()
         if not ref_type == RefType.BRANCH:
             logger.info(f'ignored create event with type {ref_type}')
             return
 
-        self._update_pipeline_definition(
-            event=create_event,
-            delivery_id=delivery_id,
-            repository=repository,
-            hostname=hostname,
-            es_client=es_client,
-            dispatch_start_time=dispatch_start_time,
+        thread = threading.Thread(
+            target=self._update_pipeline_definition,
+            kwargs={
+                'event': create_event,
+                'delivery_id': delivery_id,
+                'repository': repository,
+                'hostname': hostname,
+                'es_client': es_client,
+                'dispatch_start_time': dispatch_start_time,
+            }
         )
+        thread.start()
 
     def dispatch_push_event(
         self,
         push_event,
         delivery_id: str,
         repository: str,
         hostname: str,
         es_client: ccc.elasticsearch.ElasticSearchClient,
         dispatch_start_time: datetime.datetime,
     ):
-        if self._pipeline_definition_changed(push_event):
-            try:
-                self._update_pipeline_definition(
-                    event=push_event,
-                    delivery_id=delivery_id,
-                    repository=repository,
-                    hostname=hostname,
-                    es_client=es_client,
-                    dispatch_start_time=dispatch_start_time,
-                )
-            except ValueError as e:
-                logger.warning(
-                    f'Received error updating pipeline-definitions: "{e}". '
-                    'Will still abort running jobs (if configured) and trigger resource checks.'
-                )
+        def process_push_event(
+            delivery_id,
+            hostname,
+            es_client,
+            repository,
+            dispatch_start_time,
+            event,
+            event_type,
+        ):
+            if self._pipeline_definition_changed(event):
+                try:
+                    self._update_pipeline_definition(
+                        event=event,
+                        delivery_id=delivery_id,
+                        repository=repository,
+                        hostname=hostname,
+                        es_client=es_client,
+                        dispatch_start_time=dispatch_start_time,
+                    )
+                except ValueError as e:
+                    logger.warning(
+                        f'Received error updating pipeline-definitions: "{e}". '
+                        'Will still abort running jobs (if configured) and trigger resource checks.'
+                    )
 
-        self.abort_running_jobs_if_configured(push_event)
+            self.abort_running_jobs_if_configured(event)
 
-        def _check_resources(**kwargs):
             for concourse_api in self.concourse_clients():
                 logger.debug(f'using concourse-api: {concourse_api}')
                 resources = self._matching_resources(
                     concourse_api=concourse_api,
-                    event=push_event,
+                    event=event,
                 )
                 logger.debug('triggering resource-check')
                 whd.util.trigger_resource_check(concourse_api=concourse_api, resources=resources)
 
             process_end_time = datetime.datetime.now()
             process_total_seconds = (
-                process_end_time - kwargs.get('dispatch_start_time')
+                process_end_time - dispatch_start_time
             ).total_seconds()
             webhook_delivery_metric = whd.metric.WebhookDelivery.create(
-                delivery_id=kwargs.get('delivery_id'),
-                event_type=kwargs.get('event_type'),
-                repository=kwargs.get('repository'),
-                hostname=kwargs.get('hostname'),
+                delivery_id=delivery_id,
+                event_type=event_type,
+                repository=repository,
+                hostname=hostname,
                 process_total_seconds=process_total_seconds,
             )
-            if (es_client := kwargs.get('es_client')):
-                ccc.elasticsearch.metric_to_es(
-                    es_client=es_client,
-                    metric=webhook_delivery_metric,
-                    index_name=whd.metric.index_name(webhook_delivery_metric),
-                )
+            if not es_client:
+                return
+
+            ccc.elasticsearch.metric_to_es(
+                es_client=es_client,
+                metric=webhook_delivery_metric,
+                index_name=whd.metric.index_name(webhook_delivery_metric),
+            )
 
         thread = threading.Thread(
-            target=_check_resources,
+            target=process_push_event,
             kwargs={
                 'delivery_id': delivery_id,
                 'hostname': hostname,
                 'es_client': es_client,
                 'repository': repository,
                 'event_type': 'push',
                 'dispatch_start_time': dispatch_start_time,
+                'event': push_event,
             }
         )
         thread.start()
 
     def _update_pipeline_definition(
         self,
         event,
```

### Comparing `gardener-cicd-whd-1.2078.0/whd/metric.py` & `gardener-cicd-whd-1.2079.0/whd/metric.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/model.py` & `gardener-cicd-whd-1.2079.0/whd/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/pipelines.py` & `gardener-cicd-whd-1.2079.0/whd/pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/pull_request.py` & `gardener-cicd-whd-1.2079.0/whd/pull_request.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/server.py` & `gardener-cicd-whd-1.2079.0/whd/server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/util.py` & `gardener-cicd-whd-1.2079.0/whd/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-whd-1.2078.0/whd/webhook.py` & `gardener-cicd-whd-1.2079.0/whd/webhook.py`

 * *Files identical despite different names*

