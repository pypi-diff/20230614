# Comparing `tmp/myl-discovery-0.3.1.tar.gz` & `tmp/myl-discovery-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.3.1.tar", last modified: Wed Jun 14 08:29:11 2023, max compression
+gzip compressed data, was "myl-discovery-0.4.0.tar", last modified: Wed Jun 14 13:32:05 2023, max compression
```

## Comparing `myl-discovery-0.3.1.tar` & `myl-discovery-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:29:11.811570 myl-discovery-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:29:11.807571 myl-discovery-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:29:11.807571 myl-discovery-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-14 08:29:11.811570 myl-discovery-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:29:11.811570 myl-discovery-0.3.1/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-14 08:29:11.000000 myl-discovery-0.3.1/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-14 08:29:11.000000 myl-discovery-0.3.1/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:29:11.000000 myl-discovery-0.3.1/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 08:29:11.000000 myl-discovery-0.3.1/myl_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 08:29:11.000000 myl-discovery-0.3.1/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 08:29:11.000000 myl-discovery-0.3.1/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:29:11.811570 myl-discovery-0.3.1/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/myldiscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/myldiscovery/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/myldiscovery/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 08:29:01.000000 myl-discovery-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:29:11.811570 myl-discovery-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/setup.cfg
```

### Comparing `myl-discovery-0.3.1/.github/workflows/release.yaml` & `myl-discovery-0.4.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.3.1/LICENSE` & `myl-discovery-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.3.1/PKG-INFO` & `myl-discovery-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.3.1
+Version: 0.4.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,7 +700,114 @@
 from myldiscovery import autodiscover
 autodiscover("me@example.com")
 # {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
 #  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
 ```
 
 
+## Development
+
+### Autodiscovery
+
+#### autoconfig
+
+```shell
+curl -L https://mail.example.com/mail/config-v1.1.xml
+```
+
+Response:
+
+```xml
+<?xml version="1.0" encoding="UTF-8"?>
+<clientConfig version="1.1">
+	<emailProvider id="example.com">
+	    <domain>example.com</domain>
+
+	    <displayName>example.com Email</displayName>
+	    <displayShortName>%EMAILLOCALPART%</displayShortName>
+	    <incomingServer type="imap">
+			<hostname>mail.example.com</hostname>
+			<port>143</port>
+			<socketType>STARTTLS</socketType>
+			<authentication>password-cleartext</authentication>
+			<username>%EMAILADDRESS%</username>
+		</incomingServer>
+	    <outgoingServer type="smtp">
+			<hostname>mail.example.com</hostname>
+			<port>587</port>
+			<socketType>STARTTLS</socketType>
+			<authentication>password-cleartext</authentication>
+			<username>%EMAILADDRESS%</username>
+	    </outgoingServer>
+		<documentation url="https://autodiscover.example.com">
+			<descr lang="en">Generic settings page</descr>
+			<descr lang="fr">Paramètres généraux</descr>
+			<descr lang="es">Configuraciones genéricas</descr>
+			<descr lang="de">Allgemeine Beschreibung der Einstellungen</descr>
+			<descr lang="ru">Страница общих настроек</descr>
+		</documentation>
+	</emailProvider>
+</clientConfig>
+```
+
+### autodiscover
+
+```shell
+curl -L mail.example.com/autodiscover/autodiscover.xml
+```
+
+Response:
+
+```xml
+<?xml version="1.0" encoding="utf-8" ?>
+<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
+        <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
+                <User>
+                        <DisplayName>example.com Email</DisplayName>
+                </User>
+                <Account>
+                        <AccountType>email</AccountType>
+                        <Action>settings</Action>
+                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
+
+                        <Protocol>
+                                <Type>IMAP</Type>
+                                <TTL>1</TTL>
+
+                                <Server>mail.example.com</Server>
+                                <Port>143</Port>
+
+                                <LoginName></LoginName>
+
+                                <DomainRequired>on</DomainRequired>
+                                <DomainName>example.com</DomainName>
+
+                                <SPA>off</SPA>
+                                <Encryption>TLS</Encryption>
+                                <AuthRequired>on</AuthRequired>
+                        </Protocol>
+                </Account>
+                <Account>
+                        <AccountType>email</AccountType>
+                        <Action>settings</Action>
+                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
+
+                        <Protocol>
+                                <Type>SMTP</Type>
+                                <TTL>1</TTL>
+
+                                <Server>mail.example.com</Server>
+                                <Port>587</Port>
+
+                                <LoginName></LoginName>
+
+                                <DomainRequired>on</DomainRequired>
+                                <DomainName>example.com</DomainName>
+
+                                <SPA>off</SPA>
+                                <Encryption>TLS</Encryption>
+                                <AuthRequired>on</AuthRequired>
+                        </Protocol>
+                </Account></Response>
+</Autodiscover>
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `myl-discovery-0.3.1/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.4.0/myl_discovery.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.3.1
+Version: 0.4.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,7 +700,114 @@
 from myldiscovery import autodiscover
 autodiscover("me@example.com")
 # {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
 #  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
 ```
 
 
+## Development
+
+### Autodiscovery
+
+#### autoconfig
+
+```shell
+curl -L https://mail.example.com/mail/config-v1.1.xml
+```
+
+Response:
+
+```xml
+<?xml version="1.0" encoding="UTF-8"?>
+<clientConfig version="1.1">
+	<emailProvider id="example.com">
+	    <domain>example.com</domain>
+
+	    <displayName>example.com Email</displayName>
+	    <displayShortName>%EMAILLOCALPART%</displayShortName>
+	    <incomingServer type="imap">
+			<hostname>mail.example.com</hostname>
+			<port>143</port>
+			<socketType>STARTTLS</socketType>
+			<authentication>password-cleartext</authentication>
+			<username>%EMAILADDRESS%</username>
+		</incomingServer>
+	    <outgoingServer type="smtp">
+			<hostname>mail.example.com</hostname>
+			<port>587</port>
+			<socketType>STARTTLS</socketType>
+			<authentication>password-cleartext</authentication>
+			<username>%EMAILADDRESS%</username>
+	    </outgoingServer>
+		<documentation url="https://autodiscover.example.com">
+			<descr lang="en">Generic settings page</descr>
+			<descr lang="fr">Paramètres généraux</descr>
+			<descr lang="es">Configuraciones genéricas</descr>
+			<descr lang="de">Allgemeine Beschreibung der Einstellungen</descr>
+			<descr lang="ru">Страница общих настроек</descr>
+		</documentation>
+	</emailProvider>
+</clientConfig>
+```
+
+### autodiscover
+
+```shell
+curl -L mail.example.com/autodiscover/autodiscover.xml
+```
+
+Response:
+
+```xml
+<?xml version="1.0" encoding="utf-8" ?>
+<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
+        <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
+                <User>
+                        <DisplayName>example.com Email</DisplayName>
+                </User>
+                <Account>
+                        <AccountType>email</AccountType>
+                        <Action>settings</Action>
+                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
+
+                        <Protocol>
+                                <Type>IMAP</Type>
+                                <TTL>1</TTL>
+
+                                <Server>mail.example.com</Server>
+                                <Port>143</Port>
+
+                                <LoginName></LoginName>
+
+                                <DomainRequired>on</DomainRequired>
+                                <DomainName>example.com</DomainName>
+
+                                <SPA>off</SPA>
+                                <Encryption>TLS</Encryption>
+                                <AuthRequired>on</AuthRequired>
+                        </Protocol>
+                </Account>
+                <Account>
+                        <AccountType>email</AccountType>
+                        <Action>settings</Action>
+                        <ServiceHome>https://autodiscover.example.com</ServiceHome>
+
+                        <Protocol>
+                                <Type>SMTP</Type>
+                                <TTL>1</TTL>
+
+                                <Server>mail.example.com</Server>
+                                <Port>587</Port>
+
+                                <LoginName></LoginName>
+
+                                <DomainRequired>on</DomainRequired>
+                                <DomainName>example.com</DomainName>
+
+                                <SPA>off</SPA>
+                                <Encryption>TLS</Encryption>
+                                <AuthRequired>on</AuthRequired>
+                        </Protocol>
+                </Account></Response>
+</Autodiscover>
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `myl-discovery-0.3.1/myldiscovery/discovery.py` & `myl-discovery-0.4.0/myldiscovery/discovery.py`

 * *Files 22% similar despite different names*

```diff
@@ -66,61 +66,31 @@
 def autodiscover_txt(domain):
     res = resolve_txt(domain, criteria="^mailconf=")
     if not res:
         return
     return res.split("=")[1]
 
 
-def autodiscover(email_addr, srv_only=False):
-    domain = email_addr.split("@")[-1]
-    if not domain:
-        raise ValueError(f"Invalid email address {email_addr}")
-
-    autoconfig = autodiscover_txt(domain) if not srv_only else None
-
-    if not autoconfig:
-        imap = resolve_srv(f"_imaps._tcp.{domain}")
-        smtp = resolve_srv(f"_submission._tcp.{domain}")
+def parse_autoconfig(content):
+    data = xmltodict.parse(content)
 
-        return {
-            "imap": {
-                "server": imap[0].get("hostname"),
-                "port": int(imap[0].get("port")),
-                # FIXME We might want to "smartly" guess if starttls should be
-                # enabled or not, depending on the port:
-                # 143 -> starttls
-                # 993 -> no
-                "starttls": False,
-            },
-            "smtp": {
-                "server": smtp[0].get("hostname"),
-                "port": int(smtp[0].get("port")),
-                # FIXME We might want to "smartly" guess if starttls should be
-                # enabled or not, depending on the port:
-                # 465 -> starttls
-                # 587 -> no
-                "starttls": False,
-            },
-        }
-
-    res = requests.get(autoconfig)
-    res.raise_for_status()
-
-    data = xmltodict.parse(res.text)
     imap = (
         data.get("clientConfig", {})
         .get("emailProvider", {})
         .get("incomingServer")
     )
     smtp = (
         data.get("clientConfig", {})
         .get("emailProvider", {})
         .get("outgoingServer")
     )
 
+    LOGGER.debug(f"imap settings: {imap}")
+    LOGGER.debug(f"smtp settings: {smtp}")
+
     assert imap is not None
     assert smtp is not None
 
     return {
         "imap": {
             "server": imap.get("hostname"),
             "port": int(imap.get("port")),
@@ -128,7 +98,96 @@
         },
         "smtp": {
             "server": smtp.get("hostname"),
             "port": int(smtp.get("port")),
             "starttls": smtp.get("socketType") == "STARTTLS",
         },
     }
+
+
+def parse_autodiscover(content):
+    data = xmltodict.parse(content)
+    acc = data.get("Autodiscover", {}).get("Response", {}).get("Account", [])
+    imap = next(
+        (
+            item.get("Protocol", {})
+            for item in acc
+            if item.get("Protocol", {}).get("Type", "").lower() == "imap"
+        ),
+        None,
+    )
+    smtp = next(
+        (
+            item.get("Protocol", {})
+            for item in acc
+            if item.get("Protocol", {}).get("Type", "").lower() == "smtp"
+        ),
+        None,
+    )
+
+    LOGGER.debug(f"imap settings: {imap}")
+    LOGGER.debug(f"smtp settings: {smtp}")
+
+    assert imap is not None
+    assert smtp is not None
+
+    return {
+        "imap": {
+            "server": imap.get("Server"),
+            "port": int(imap.get("Port")),
+            "starttls": imap.get("Encryption", "").lower() == "tls",
+        },
+        "smtp": {
+            "server": smtp.get("Server"),
+            "port": int(smtp.get("Port")),
+            "starttls": smtp.get("Encryption", "").lower() == "tls",
+        },
+    }
+
+
+def autodiscover_srv(domain):
+    imap = resolve_srv(f"_imaps._tcp.{domain}")
+    smtp = resolve_srv(f"_submission._tcp.{domain}")
+
+    return {
+        "imap": {
+            "server": imap[0].get("hostname"),
+            "port": int(imap[0].get("port")),
+            # FIXME We might want to "smartly" guess if starttls should be
+            # enabled or not, depending on the port:
+            # 143 -> starttls
+            # 993 -> no
+            "starttls": False,
+        },
+        "smtp": {
+            "server": smtp[0].get("hostname"),
+            "port": int(smtp[0].get("port")),
+            # FIXME We might want to "smartly" guess if starttls should be
+            # enabled or not, depending on the port:
+            # 465 -> starttls
+            # 587 -> no
+            "starttls": False,
+        },
+    }
+
+
+def autodiscover(email_addr, srv_only=False):
+    domain = email_addr.split("@")[-1]
+    if not domain:
+        raise ValueError(f"Invalid email address {email_addr}")
+
+    if srv_only:
+        return autodiscover_srv(domain)
+
+    autoconfig = autodiscover_txt(domain)
+
+    if not autoconfig:
+        return autodiscover_srv(domain)
+
+    res = requests.get(autoconfig)
+    res.raise_for_status()
+
+    try:
+        return parse_autoconfig(res.text)
+    except Exception:
+        LOGGER.warning("Failed to parse autoconfig, trying autodiscover")
+        return parse_autodiscover(res.text)
```

### Comparing `myl-discovery-0.3.1/myldiscovery/main.py` & `myl-discovery-0.4.0/myldiscovery/main.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.3.1/pyproject.toml` & `myl-discovery-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 ]
 dependencies = [
   "dnspython",
   "requests",
   "rich",
   "xmltodict"
 ]
-version = "0.3.1"
+version = "0.4.0"
 
 [project.scripts]
 myl-discovery = "myldiscovery:main"
 
 [tool.black]
 line-length = 79
```

