# Comparing `tmp/muvinai-0.2.8.dev0.tar.gz` & `tmp/muvinai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muvinai-0.2.8.dev0.tar", last modified: Tue Nov 29 14:26:53 2022, max compression
+gzip compressed data, was "muvinai-0.2.9.tar", last modified: Mon Dec 26 18:56:57 2022, max compression
```

## Comparing `muvinai-0.2.8.dev0.tar` & `muvinai-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:53.462005 muvinai-0.2.8.dev0/
--rw-r--r--   0 runner    (1001) docker     (122)      296 2022-11-29 14:26:53.458005 muvinai-0.2.8.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      582 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:53.454005 muvinai-0.2.8.dev0/muvinai/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:53.454005 muvinai-0.2.8.dev0/muvinai/objects/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3742 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/objects/boletaObject.py
--rw-r--r--   0 runner    (1001) docker     (122)     2483 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/objects/clientObject.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:53.458005 muvinai-0.2.8.dev0/muvinai/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6657 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/afip.py
--rw-r--r--   0 runner    (1001) docker     (122)     7160 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/authorization.py
--rw-r--r--   0 runner    (1001) docker     (122)     5498 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/db_operations.py
--rw-r--r--   0 runner    (1001) docker     (122)    26412 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/facturacion_afip.py
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/format.py
--rw-r--r--   0 runner    (1001) docker     (122)     9688 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/init_creds.py
--rw-r--r--   0 runner    (1001) docker     (122)    15044 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/mail_sender.py
--rw-r--r--   0 runner    (1001) docker     (122)    11052 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/members.py
--rw-r--r--   0 runner    (1001) docker     (122)     8566 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/mercadopago_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/pagination.py
--rw-r--r--   0 runner    (1001) docker     (122)    32978 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/payments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1376 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/projections.py
--rw-r--r--   0 runner    (1001) docker     (122)      374 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/query_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    14945 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/sportaccess.py
--rw-r--r--   0 runner    (1001) docker     (122)     1696 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/muvinai/utilities/webflow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:26:53.454005 muvinai-0.2.8.dev0/muvinai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      296 2022-11-29 14:26:53.000000 muvinai-0.2.8.dev0/muvinai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-29 14:26:53.000000 muvinai-0.2.8.dev0/muvinai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 14:26:53.000000 muvinai-0.2.8.dev0/muvinai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      160 2022-11-29 14:26:53.000000 muvinai-0.2.8.dev0/muvinai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-29 14:26:53.000000 muvinai-0.2.8.dev0/muvinai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 14:26:53.462005 muvinai-0.2.8.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-11-29 14:26:40.000000 muvinai-0.2.8.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:57.988753 muvinai-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-26 18:56:57.988753 muvinai-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-26 18:56:47.000000 muvinai-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:57.984753 muvinai-0.2.9/muvinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:57.984753 muvinai-0.2.9/muvinai/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/objects/boletaObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/objects/clientObject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:57.988753 muvinai-0.2.9/muvinai/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/afip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/db_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26412 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/facturacion_afip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/init_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16663 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/mail_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/mercadopago_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32978 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/query_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/sportaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-26 18:56:47.000000 muvinai-0.2.9/muvinai/utilities/webflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 18:56:57.984753 muvinai-0.2.9/muvinai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-26 18:56:57.000000 muvinai-0.2.9/muvinai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-26 18:56:57.000000 muvinai-0.2.9/muvinai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-26 18:56:57.000000 muvinai-0.2.9/muvinai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-26 18:56:57.000000 muvinai-0.2.9/muvinai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-26 18:56:57.000000 muvinai-0.2.9/muvinai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-26 18:56:57.988753 muvinai-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-26 18:56:47.000000 muvinai-0.2.9/setup.py
```

### Comparing `muvinai-0.2.8.dev0/README.md` & `muvinai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/objects/boletaObject.py` & `muvinai-0.2.9/muvinai/objects/boletaObject.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/objects/clientObject.py` & `muvinai-0.2.9/muvinai/objects/clientObject.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/afip.py` & `muvinai-0.2.9/muvinai/utilities/afip.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/authorization.py` & `muvinai-0.2.9/muvinai/utilities/authorization.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/dates.py` & `muvinai-0.2.9/muvinai/utilities/dates.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/db_operations.py` & `muvinai-0.2.9/muvinai/utilities/db_operations.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/facturacion_afip.py` & `muvinai-0.2.9/muvinai/utilities/facturacion_afip.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/format.py` & `muvinai-0.2.9/muvinai/utilities/format.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/init_creds.py` & `muvinai-0.2.9/muvinai/utilities/init_creds.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/mail_sender.py` & `muvinai-0.2.9/muvinai/utilities/mail_sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 import mailchimp_transactional as MailchimpTransactional
 from .init_creds import mailchimp_key, test
 from mailchimp_transactional.api_client import ApiClientError
 import iso8601
 import typing
+from datetime import datetime
+
 from .dates import today_argentina
 from .init_creds import init_mongo
 from .format import muvi_print
 
 mailchimp = MailchimpTransactional.Client(mailchimp_key)
 
 def send_mail_with_attachment(files_attachments:list, receiver_mail, test_mail="matias@muvinai.com",global_vars:list=list()):
@@ -123,46 +125,89 @@
             {"name": "logo", "content": brand["images"]["mail_logo"]},
             {"name": "brand_name", "content": brand["name"]},
             {"name": "email_contacto", "content": brand["email_contacto"]}
         ])
     return send_mail(receiver["email"], global_vars, template, brand)
 
 
-def send_mail(receiver_mail, params, template, brand, test_mail="ignacio@muvinai.com"):
+def send_mail(receiver_mail, params, template, brand, test_mail="ignacio@muvinai.com", send_at=None):
     """ Estructura y envía mail
 
     :param receiver_mail: mail del receptor
     :type receiver_mail: str
     :param params: lista de objetos que son parámetros a pasar al template
     :type params: list
     :param template: nombre del template
     :type template: str
+    :param brand: brand
+    :type brand: dict
     :param test_mail: mail del receptor en caso de test
     :type receiver_mail: str
+    :param send_at: fecha en la cual se debe enviar el mail
+    :type send_at: datetime
     :return: informacion del mail
     :rtype: dict
     """
     print("Enviando mail" + template)
 
     msg = {
         "from_email": brand["mail_sender_address"],
         "from_name": brand["name"],
         "to": [{"email": test_mail}] if test else [{"email": receiver_mail}],
-        "global_merge_vars": params}
+        "global_merge_vars": params
+    }
 
     try:
-        response = mailchimp.messages.send_template(
-            {"template_name": template, "template_content": [], "message": msg})
+        body = {"template_name": template, "template_content": [], "message": msg}
+        if send_at:
+            body['send_at'] = send_at.strftime('%Y-%m-%d %H:%M:%S')
+        response = mailchimp.messages.send_template(body)
         print(response)
         return response[0]
     except ApiClientError as error:
         print("An exception occurred: {}".format(error.text))
         return {}
 
 
+def send_mail_carrito_abandonado(receiver_mail, client_name, plan_slug, corpo_slug, price, brand, send_at=None):
+    """ Enviar mail de carrito abandonado
+
+    :param receiver_mail: documento de cliente del destinatario
+    :type receiver_mail: str
+    :param client_name: nombre de cliente del destinatario
+    :type client_name: str
+    :param plan_slug: slug del plan
+    :type plan_slug: str
+    :param corpo_slug: slug del plan corporativo
+    :type corpo_slug: str
+    :param price: precio del plan
+    :type price: int
+    :param brand: brand del socio
+    :type brand: dict
+    :param send_at: fecha en la cual se debe enviar el mail
+    :type send_at: datetime
+    :return: informacion del mail
+    :rtype: dict
+    """
+
+    url_slug = corpo_slug if corpo_slug else plan_slug
+    global_vars = [
+        {"name": "corpo", "content": corpo_slug},
+        {"name": "name", "content": client_name},
+        {"name": "plan", "content": plan_slug},
+        {"name": "price", "content": price},
+        {"name": "the_url", "content": f"https://www.sportclub.pagar.club/paso2/{url_slug}?utm_source=checkout&utm_medium=email&utm_campaign=carrito_abandonado"}
+    ]
+    if brand["name"] != "SportClub":
+        return
+
+    template = "carrito-abandonado"
+    return send_mail(receiver_mail, global_vars, template, brand, send_at=send_at)
+
+
 def send_mail_cambio_tarjeta(receiver, brand):
     """ Enviar mail indicando al cliente que debe cambiar la tarjeta.
 
             :param receiver: documento de cliente del destinatario
             :type receiver: dict
             :return: informacion del mail
             :rtype: dict
```

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/members.py` & `muvinai-0.2.9/muvinai/utilities/members.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/mercadopago_ops.py` & `muvinai-0.2.9/muvinai/utilities/mercadopago_ops.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/pagination.py` & `muvinai-0.2.9/muvinai/utilities/pagination.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/payments.py` & `muvinai-0.2.9/muvinai/utilities/payments.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/projections.py` & `muvinai-0.2.9/muvinai/utilities/projections.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/sportaccess.py` & `muvinai-0.2.9/muvinai/utilities/sportaccess.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai/utilities/webflow.py` & `muvinai-0.2.9/muvinai/utilities/webflow.py`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/muvinai.egg-info/SOURCES.txt` & `muvinai-0.2.9/muvinai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muvinai-0.2.8.dev0/setup.py` & `muvinai-0.2.9/setup.py`

 * *Files identical despite different names*

