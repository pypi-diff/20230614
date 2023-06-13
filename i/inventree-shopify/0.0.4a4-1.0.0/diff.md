# Comparing `tmp/inventree-shopify-0.0.4a4.tar.gz` & `tmp/inventree-shopify-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/inventree-shopify/inventree-shopify/dist/tmpgw_bqg0l/inventree-shopify-0.0.4a4.tar", last modified: Wed Aug 17 23:15:19 2022, max compression
+gzip compressed data, was "/home/runner/work/inventree-shopify/inventree-shopify/dist/.tmp-bj6y8gui/inventree-shopify-1.0.0.tar", last modified: Tue Jun 13 23:45:11 2023, max compression
```

## Comparing `inventree-shopify-0.0.4a4.tar` & `inventree-shopify-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/
--rw-r--r--   0 runner    (1001) docker     (121)     8901 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/ShopifyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/migrations/0002_shopifywebhook.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/migrations/0003_shopifywebhook_shopify_webhook_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/migrations/0004_auto_20211019_2321.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5899 2022-08-17 23:15:05.000000 inventree-shopify-0.0.4a4/src/inventree_shopify/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-17 23:15:19.000000 inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify/
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/ShopifyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify/templates/shopify/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/templates/shopify/increase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/templates/shopify/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 23:44:56.000000 inventree-shopify-1.0.0/src/inventree_shopify/templates/shopify/webhooks.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 23:45:11.000000 inventree-shopify-1.0.0/src/inventree_shopify.egg-info/top_level.txt
```

### Comparing `inventree-shopify-0.0.4a4/LICENSE` & `inventree-shopify-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-shopify-0.0.4a4/pyproject.toml` & `inventree-shopify-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires = ["setuptools", "wheel", "pyyaml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inventree-shopify"
-version =  "0.0.4a4"
+version =  "1.0.0"
 description="Shopify integration for InvenTree"
 readme = "README.md"
 license = {text = "MIT"}
 keywords = ["inventree", "inventree-plugin", "shopify"]
 authors = [
     {name = "Matthias J Mair", email =  "info@mjmair.com"}
 ]
 classifiers=[
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",  # Remove after final released
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Framework :: Django",
     "Intended Audience :: Developers",
     "Intended Audience :: Manufacturing",
     "Intended Audience :: End Users/Desktop",
     "Topic :: Scientific/Engineering",
 ]
-requires-python=">=3.6"
+requires-python=">=3.9"
 dependencies = ['requests', 'django']
 
 [project.optional-dependencies]
 dev = ['twine', 'setuptools']
 
 [project.urls]
 repository = "https://github.com/matmair/inventree-shopify"
 "Bug Tracker" = "https://github.com/matmair/inventree-shopify/issues"
 
 [project.entry-points."inventree_plugins"]
-inventree-shopify = "inventree_shopify:ShopifyPlugin.ShopifyPlugin"
+inventree-shopify = "inventree_shopify:ShopifyPlugin"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `inventree-shopify-0.0.4a4/src/inventree_shopify/ShopifyPlugin.py` & `inventree-shopify-1.0.0/src/inventree_shopify/ShopifyPlugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,45 +4,47 @@
 
 from django import forms
 from django.conf.urls import url
 from django.http.response import Http404
 from django.shortcuts import redirect, render
 from django.utils.translation import ugettext_lazy as _
 from plugin import InvenTreePlugin
-from plugin.mixins import (APICallMixin, AppMixin, NavigationMixin,
+from plugin.mixins import (APICallMixin, AppMixin, EventMixin, NavigationMixin,
                            SettingsMixin, UrlsMixin)
+from stock.models import StockItem
 
 
-class ShopifyPlugin(APICallMixin, AppMixin, SettingsMixin, UrlsMixin, NavigationMixin, InvenTreePlugin):
+class ShopifyPlugin(EventMixin, APICallMixin, AppMixin, SettingsMixin, UrlsMixin, NavigationMixin, InvenTreePlugin):
     """Main plugin class for Shopify integration."""
 
     NAME = 'ShopifyPlugin'
     SLUG = 'shopify'
     TITLE = "Shopify Integration App"
 
     NAVIGATION_TAB_NAME = "Shopify"
     NAVIGATION_TAB_ICON = 'fab fa-shopify'
 
     API_TOKEN = 'X-Shopify-Access-Token'
     API_TOKEN_SETTING = 'API_PASSWORD'
 
-    SHOPIFY_API_VERSION = '2021-07'
+    SHOPIFY_API_VERSION = '2023-04'
 
     @property
     def api_url(self):
         """Base URL definifion."""
         return f'https://{self.get_setting("SHOP_URL")}/admin/api/{self.SHOPIFY_API_VERSION}'
 
     def _fetch_levels(self):
         from .models import InventoryLevel, Variant
 
-        levels = self.api_call('inventory_levels', arguments={'inventory_item_ids': [a.inventory_item_id for a in Variant.objects.all()]})
+        levels = self.api_call('inventory_levels.json', url_args={'inventory_item_ids': [a.inventory_item_id for a in Variant.objects.all()]})
         if 'errors' in levels:
             raise ValueError('Errors where found', levels['errors'])
         # create levels in db
+        levels = levels['inventory_levels']
         for level in levels:
             lvl, _ = InventoryLevel.objects.get_or_create(
                 variant=Variant.objects.get(inventory_item_id=level.get('inventory_item_id')),
                 location_id=level.get('location_id'),
                 defaults={
                     'available': level.get('available'),
                 }
@@ -50,18 +52,19 @@
             lvl.updated_at = datetime.datetime.fromisoformat(level.get('updated_at'))
             lvl.available = level.get('available')
             lvl.save()
 
     def _fetch_products(self):
         from .models import Product, Variant
 
-        products = self.api_call('products')
+        products = self.api_call('products.json')
         if 'errors' in products:
             raise ValueError('Errors where found', products['errors'])
         # create products in db
+        products = products['products']
         for product in products:
             Product.objects.update_or_create(
                 id=product.get('id'),
                 defaults={
                     'title': product.get('title'),
                     'body_html': product.get('body_html'),
                     'vendor': product.get('vendor'),
@@ -84,14 +87,40 @@
                         barcode=var.get('barcode'),
                         price=var.get('price'),
                         created_at=datetime.datetime.fromisoformat(var.get('created_at')),
                         updated_at=datetime.datetime.fromisoformat(var.get('updated_at')),
                         product_id=p.get('id'),
                     )
 
+    # region events
+    def process_event(self, event, *args, **kwargs):
+        """Process triggered events."""
+        if event == 'stock_stockitem.saved' and kwargs.get('model', '') == 'StockItem':
+            try:
+                stockitems = StockItem.objects.get(pk=kwargs.get('id'))
+                for level in stockitems.ShopifyInventoryLevel.all():
+                    if level.available == stockitems.quantity:
+                        continue
+                    response = self.api_call(
+                        endpoint='inventory_levels/set.json',
+                        json={
+                            "location_id": level.location_id,
+                            "inventory_item_id": level.variant.inventory_item_id,
+                            "available": int(stockitems.quantity),
+                        },
+                        method="POST",
+                    )
+                    if 'inventory_level' in response:
+                        level.available = stockitems.quantity
+                        level.save()
+
+            except StockItem.DoesNotExist:
+                pass
+    # endregion
+
     # region views
     def view_index(self, request):
         """A basic overview view."""
         from .models import InventoryLevel, Product
 
         try:
             self._fetch_products()
@@ -120,20 +149,20 @@
         else:
             form = IncreaseForm(request.POST)
 
             if form.is_valid():
                 # increase stock
                 response = self.api_call(
                     endpoint='inventory_levels/set.json',
-                    data={
+                    json={
                         "location_id": location,
                         "inventory_item_id": pk,
                         "available": form.cleaned_data['amount']
                     },
-                    get=False
+                    method="POST",
                 )
                 if 'inventory_level' in response:
                     return redirect(f'{self.internal_name}index')
                 context['error'] = _('API call was not sucessfull')
 
         context['form'] = form
         return render(request, 'shopify/increase.html', context)
@@ -145,18 +174,19 @@
         }
         return render(request, 'shopify/webhooks.html', context)
 
     def _webhook_check(self, host):
         # collect current hooks
         target_topics = [
             'inventory_levels/update',
-            'orders/updated',
-            'orders/edited',
+            # 'orders/updated',
+            # 'orders/edited',
         ]
-        webhooks = self.api_call('webhooks')
+        webhooks = self.api_call('webhooks.json')
+        webhooks = webhooks.get('webhooks', [])
 
         # process current hooks
         webhooks_topics = []
         webhooks_wrong_hooks = []
         for item in webhooks:
             if host in item.get('address', ''):
                 webhooks_topics.append(item.get('topic', ''))
@@ -174,40 +204,40 @@
         for topic in target_topics:
             if topic not in webhooks_topics:
                 self._webhook_create(host, topic)
                 changed = True
 
         # return all hooks
         if changed:
-            return self.api_call('webhooks')
+            return self.api_call('webhooks.json')
         return webhooks
 
     def _webhook_create(self, hostname, topic):
         from .models import ShopifyWebhook
 
         webhook = ShopifyWebhook.objects.create(name=f'{self.slug}_{topic}')
         response = self.api_call(
             endpoint='webhooks.json',
-            data={"webhook": {
+            json={"webhook": {
                 "topic": topic,
                 "address": f'https://{hostname}/api/webhook/{webhook.endpoint_id}/',
                 "format": "json",
             }},
-            get=False
+            method="POST"
         )
         if not response.get('webhook', False):
             raise KeyError(response)
         webhook.shopify_webhook_id = response['webhook'].get('id', None)
         webhook.save()
         return True
 
     def _webhook_delete(self, id):
         self.api_call(
             endpoint=f'webhooks/{id}.json',
-            delete=True
+            method="DELETE",
         )
         return True
     # endregion
 
     def setup_urls(self):
         """Returns the URLs defined by this plugin."""
         return [
```

### Comparing `inventree-shopify-0.0.4a4/src/inventree_shopify/admin.py` & `inventree-shopify-1.0.0/src/inventree_shopify/admin.py`

 * *Files identical despite different names*

### Comparing `inventree-shopify-0.0.4a4/src/inventree_shopify/models.py` & `inventree-shopify-1.0.0/src/inventree_shopify/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,21 +97,21 @@
         topic = headers['X-Shopify-Topic']
         if self.check_if_handled(headers):
             return False
 
         if topic == 'inventory_levels/update':
             # handle invetorylevel update
             update_inventory_levels(payload)
-        elif topic == 'orders/edited':
-            # handle order edited
-            pass
-
-        elif topic == 'orders/updated':
-            # handle order update
-            pass
+        # elif topic == 'orders/edited':
+        #     # handle order edited
+        #     pass
+
+        # elif topic == 'orders/updated':
+        #     # handle order update
+        #     pass
 
         return True
 
     def check_if_handled(self, headers: dict) -> bool:
         """Checks if the webhook messages was already handled.
 
         Args:
@@ -135,26 +135,30 @@
         """Shopify expects no returns."""
         return None
 
 
 def update_inventory_levels(payload: dict):
     """Handle updates to inventory levels.
 
-    :param payload: pyload of webhook
+    :param payload: payload of webhook
     :type payload: dict
     """
     # fetch item
     item = InventoryLevel.objects.filter(variant__inventory_item_id=payload['inventory_item_id'], location_id=payload['location_id'])
     if item.exists() and item.count() == 1:
         item = item.first()
         avail = payload['available']
 
         # set item qty
         item.available = avail
         if item.stock_item:
+            # check if the quantity changed and skip if not
+            if item.stock_item.quantity == avail:
+                return
+
             # set stock item qty
             item.stock_item.quantity = avail
             item.stock_item.save()
             # add tracking entry
             item.stock_item.add_tracking_entry(
                 StockHistoryCode.STOCK_COUNT,
                 None,
```

### Comparing `inventree-shopify-0.0.4a4/src/inventree_shopify.egg-info/SOURCES.txt` & `inventree-shopify-1.0.0/src/inventree_shopify.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 src/inventree_shopify.egg-info/PKG-INFO
 src/inventree_shopify.egg-info/SOURCES.txt
 src/inventree_shopify.egg-info/dependency_links.txt
 src/inventree_shopify.egg-info/entry_points.txt
 src/inventree_shopify.egg-info/requires.txt
 src/inventree_shopify.egg-info/top_level.txt
 src/inventree_shopify/migrations/0001_initial.py
-src/inventree_shopify/migrations/0002_shopifywebhook.py
-src/inventree_shopify/migrations/0003_shopifywebhook_shopify_webhook_id.py
-src/inventree_shopify/migrations/0004_auto_20211019_2321.py
-src/inventree_shopify/migrations/__init__.py
+src/inventree_shopify/migrations/__init__.py
+src/inventree_shopify/templates/shopify/increase.html
+src/inventree_shopify/templates/shopify/index.html
+src/inventree_shopify/templates/shopify/webhooks.html
```

