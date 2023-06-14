# Comparing `tmp/netbox-cisco-maintenance-0.0.98.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.98.tar", last modified: Tue Jun  6 11:25:01 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.99.tar", last modified: Tue Jun  6 11:43:05 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.98.tar` & `netbox-cisco-maintenance-0.0.99.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.202613 netbox-cisco-maintenance-0.0.98/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 11:25:01.202613 netbox-cisco-maintenance-0.0.98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.198613 netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 11:25:01.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 11:25:01.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 11:25:01.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 11:25:01.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 11:25:01.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.198613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.198613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.198613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37567 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.198613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2064 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.194613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.202613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     4370 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3376 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:25:01.202613 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1944 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 11:25:01.202613 netbox-cisco-maintenance-0.0.98/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 11:24:34.000000 netbox-cisco-maintenance-0.0.98/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4689 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5312 2023-06-06 11:43:05.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1099 2023-06-06 11:43:05.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 11:43:05.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 11:43:05.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-06 11:43:05.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1092 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    38233 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2194 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1826 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.934057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3376 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/no_data_available.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2402 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 11:43:05.938057 netbox-cisco-maintenance-0.0.99/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-06-06 11:42:42.000000 netbox-cisco-maintenance-0.0.99/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.98/LICENSE` & `netbox-cisco-maintenance-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.98/PKG-INFO` & `netbox-cisco-maintenance-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.98
+Version: 0.0.99
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.98/README.md` & `netbox-cisco-maintenance-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.98
+Version: 0.0.99
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 class CiscoSupportAdmin(admin.ModelAdmin):
     list_display = (
         "device",
         "api_status",
         "recommended_release",
         "desired_release",
         "current_release",
+        "desired_release_status",
+        "current_release_status",
         "contract_supplier",
         "sr_no_owner",
         "is_covered",
         "service_contract_number",
         "service_line_descr",
         "coverage_end_date",
         "warranty_end_date",
```

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,28 @@
         self.stdout.write(f"{serial_number} - recommended_release: {recommended_release_stdout}")
 
         # Update recommended_release
         ds.recommended_release = recommended_release
         # (Desired release and current release can't be gathered by the Cisco Support API. They should be
         # added over the RestAPI)
 
+        #### Set desired_release_status and current_release_status ###########################################
+        # Compate the releases to set the status for the desired release and the current release
+        # Verify if the desired release match the recommended release
+        if ds.desired_release in ds.recommended_release:
+            ds.desired_release_status = True
+        else:
+            ds.desired_release_status = False
+
+        # Verify if the current release match the desired release
+        if ds.current_release in ds.desired_release:
+            ds.current_release_status = True
+        else:
+            ds.current_release_status = False
+
         #### Save model object for device ####################################################################
         ds.save()
 
         return
 
     # Updates a single device with current SNI coverage status data
     def update_device_sni_status_data(self, device):
```

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/models.py` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,11 @@
     api_status = models.TextField(blank=True, null=True)
 
     recommended_release = models.TextField(blank=True, null=True)
 
     desired_release = models.TextField(blank=True, null=True)
 
     current_release = models.TextField(blank=True, null=True)
+
+    desired_release_status = models.BooleanField(default=False)
+
+    current_release_status = models.BooleanField(default=False)
```

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
                 {% if not cisco_device_support %}
                     {% include "netbox_cisco_support_plugin/no_data_available.html" %}
                 {% else %}
                     <tr>
                         <td style="width: 40%">Recommended Release</td>
                         <td>{{ cisco_device_support.recommended_release|linebreaks }}</td>
                     </tr>
-                    {{ '<tr class="warning">' if 'TEST' not in 'ABCD' else '<tr>' }}
+                    <tr {{ cisco_device_support.desired_release_status|desired_release_status_class }}>
                         <td>Desired Release</td>
                         <td>{{ cisco_device_support.desired_release }}</td>
                     </tr>
-                    {{ '<tr class="danger">' if cisco_device_support.current_release not in cisco_device_support.desired_release else '<tr>' }}
+                    <tr {{ cisco_device_support.current_release_status|current_release_status_class }}>
                         <td>Current Release</td>
                         <td>{{ cisco_device_support.current_release }}</td>
                     </tr>
                 {% endif %}
             </tbody>
         </table>
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
 {% load filters %}
 ** Cisco Device Software Information **
 Recommended Release {{ cisco_device_support.recommended_release|linebreaks }}
-Desired Release     {{ cisco_device_support.desired_release }}
-Current Release     {{ cisco_device_support.current_release }}
 {% if cisco_device_support %}
 Last updated: {{ cisco_device_support.last_updated }}
 {% endif %}
 ** Cisco Device Support Information **
 {% if cisco_device_support %}
 Last updated: {{ cisco_device_support.last_updated }}
 {% endif %}
```

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.98/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.99/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,7 +72,28 @@
     Set CSS class for boolian fields to display a green thick or a red cross
     """
     return (
         mark_safe('class="mdi mdi-close-thick text-danger"')
         if value
         else mark_safe('class="mdi mdi-check-bold text-success"')
     )
+
+
+@register.filter(is_safe=True)
+def desired_release_status_class(value):
+    """
+    Set CSS class for text fields
+    """
+    if value == "None":
+        return mark_safe('class="danger"')
+
+    if not value:
+        return mark_safe('class="warning"')
+
+
+@register.filter(is_safe=True)
+def current_release_status_class(value):
+    """
+    Set CSS class for text fields
+    """
+    if not value or value == "None":
+        return mark_safe('class="danger"')
```

### Comparing `netbox-cisco-maintenance-0.0.98/setup.py` & `netbox-cisco-maintenance-0.0.99/setup.py`

 * *Files identical despite different names*

