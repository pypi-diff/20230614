# Comparing `tmp/scw_gateway-0.1.2.tar.gz` & `tmp/scw_gateway-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.1.2.tar", max compression
+gzip compressed data, was "scw_gateway-0.2.0.tar", max compression
```

## Comparing `scw_gateway-0.1.2.tar` & `scw_gateway-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/cli/__init__.py
--rw-r--r--   0        0        0     3782 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/cli/cli.py
--rw-r--r--   0        0        0      119 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/cli/conf.py
--rw-r--r--   0        0        0     3513 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/cli/gateway.py
--rw-r--r--   0        0        0    15924 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/cli/infra.py
--rw-r--r--   0        0        0     1037 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/cli/model.py
--rw-r--r--   0        0        0      934 2023-05-05 15:34:05.590752 scw_gateway-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 scw_gateway-0.1.2/setup.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 scw_gateway-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/__init__.py
+-rw-r--r--   0        0        0     6509 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/cli.py
+-rw-r--r--   0        0        0      352 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/client.py
+-rw-r--r--   0        0        0     2465 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/conf.py
+-rw-r--r--   0        0        0     5032 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/__init__.py
+-rw-r--r--   0        0        0     2210 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6009 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/function.py
+-rw-r--r--   0        0        0      319 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/image.py
+-rw-r--r--   0        0        0    15754 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2514 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1037 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/model.py
+-rw-r--r--   0        0        0      921 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 scw_gateway-0.2.0/setup.py
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 scw_gateway-0.2.0/PKG-INFO
```

### Comparing `scw_gateway-0.1.2/cli/gateway.py` & `scw_gateway-0.2.0/cli/gateway.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,161 @@
+import json
+from typing import List
+
+import click
 import requests
-import yaml
 from loguru import logger
 
-from cli.conf import CONFIG_FILE
+from cli import conf
 from cli.model import Route
 
 
-class GatewayManager(object):
+def response_hook(response: requests.Response, *_args, **_kwargs):
+    """Response hook to log request and call raise_for_status."""
+    req = response.request
+    logger.debug(f"{req.method}: {req.url}")
+    try:
+        response.raise_for_status()
+    except requests.exceptions.HTTPError as err:
+        body_json = err.response.json()
+        logger.error(f"Error: \n{json.dumps(body_json, indent=2)}")
+        raise
+
+
+class GatewayManager:
+    """Configure routes via the Kong admin API."""
+
+    admin_url: str
+    gateway_url: str
+
     def __init__(self):
         # Local local config
-        with open(CONFIG_FILE, "r") as fh:
-            self.config = yaml.safe_load(fh)
+        self.config = conf.InfraConfiguration.load()
 
-        self.admin_url = [
-            self.config["protocol"],
+        admin_url = [
+            self.config.protocol,
             "://",
-            self.config["gw_admin_host"],
-            ":",
-            str(self.config["gw_admin_port"]),
+            self.config.gw_admin_host,
         ]
-        self.admin_url = "".join(self.admin_url)
 
-        self.gateway_url = [
-            self.config["protocol"],
+        admin_port = self.config.gw_admin_port
+        if admin_port:
+            admin_url.extend([":", str(admin_port)])
+
+        self.admin_url = "".join(admin_url)
+
+        gateway_url = [
+            self.config.protocol,
             "://",
-            self.config["gw_host"],
-            ":",
-            str(self.config["gw_port"]),
+            self.config.gw_host,
         ]
-        self.gateway_url = "".join(self.gateway_url)
+
+        gateway_port = self.config.gw_port
+        if gateway_port:
+            gateway_url.extend([":", str(gateway_port)])
+
+        self.gateway_url = "".join(gateway_url)
 
         self.routes_url = self.admin_url + "/routes"
         self.services_url = self.admin_url + "/services"
-        self.token = self.config.get("gw_admin_token")
+        self.token = self.config.gw_admin_token
 
-        self.auth_headers = dict()
+        self.session = requests.Session()
         if self.token:
-            self.auth_headers["X-Auth-Token"] = self.token
+            self.session.headers["X-Auth-Token"] = self.token
+        self.session.headers["Content-Type"] = "application/json"
+        self.session.hooks["response"].append(response_hook)
 
     def add_route(self, route: Route):
         service_url = f"{self.services_url}/{route.name}"
         route_url = f"{self.routes_url}/{route.name}"
 
-        self._do_request("PUT", service_url, data=route.service_json())
-        resp = self._do_request("PUT", route_url, data=route.route_json())
+        resp = self.session.put(url=service_url, json=route.service_json())
+        resp = self.session.put(url=route_url, json=route.route_json())
 
+        plugins_url = f"{route_url}/plugins"
         if route.cors:
-            plugins_url = f"{route_url}/plugins"
-
             try:
-                self._do_request("POST", plugins_url, data=route.cors_json())
+                self.session.post(url=plugins_url, json=route.cors_json())
             except requests.HTTPError:
                 # TODO - avoid ignoring this, any way to create or update?
                 pass
 
         return resp
 
     def delete_route(self, route: Route):
-        self._do_request("DELETE", f"{self.routes_url}/{route.name}")
-        resp = self._do_request("DELETE", f"{self.services_url}/{route.name}")
+        self.session.delete(url=f"{self.routes_url}/{route.name}")
+        resp = self.session.delete(url=f"{self.services_url}/{route.name}")
         return resp
 
-    def get_routes(self):
-        resp = self._do_request("GET", self.routes_url)
+    def print_routes(self):
+        routes: List[Route] = self.get_routes()
+        routes.sort(key=lambda r: r.relative_url)
+
+        click.secho(
+            f"{'RELATIVE URL':<25} {'TARGET':<40} {'HTTP_METHODS':<10}", bold=True
+        )
+        for r in routes:
+            http_methods = r.http_methods if r.http_methods else "All"
+            click.secho(f"{r.relative_url:<25} {r.target:<40} {http_methods:<10}")
+
+    def get_routes(self) -> List[Route]:
+        resp = self.session.get(url=self.routes_url)
         route_data = {r.get("name"): r for r in resp.json().get("data")}
 
-        resp = self._do_request("GET", self.services_url)
+        resp = self.session.get(url=self.services_url)
         service_data = {s.get("name"): s for s in resp.json().get("data")}
 
         routes = list()
         for _, r in route_data.items():
-            name = r["name"]
-            relative_url = r["paths"][0]
+            route_name = r["name"]
+            route_path = r["paths"][0]
             http_methods = r.get("methods")
 
-            s = service_data.get(name)
-            port = s["port"]
-            host = s["host"]
-            protocol = s["protocol"]
-            url = f"{protocol}://{host}:{port}"
-
-            routes.append(Route(relative_url, url, http_methods=http_methods))
+            service = service_data.get(route_name)
+            if not service:
+                continue
+
+            service_port = service["port"]
+            service_host = service["host"]
+            service_protocol = service["protocol"]
+            service_url = f"{service_protocol}://{service_host}:{service_port}"
+
+            routes.append(
+                Route(
+                    relative_url=route_path,
+                    target=service_url,
+                    http_methods=http_methods,
+                )
+            )
 
         return routes
 
-    def _do_request(self, method, url, data=None) -> requests.Response:
-        logger.debug(f"{method}: {url}")
+    def setup_global_kong_statsd_plugin(self) -> str:
+        """Install the kong statsd plugin on the kong admin API.
 
-        logger.debug(f"AUTH: {self.auth_headers}")
-
-        if method == "GET":
-            resp = requests.get(url, headers=self.auth_headers)
-        elif method == "DELETE":
-            resp = requests.delete(url, headers=self.auth_headers)
-        elif method == "PATCH":
-            resp = requests.patch(url, headers=self.auth_headers, json=data)
-        elif method == "POST":
-            resp = requests.post(url, headers=self.auth_headers, json=data)
-        elif method == "PUT":
-            resp = requests.put(url, headers=self.auth_headers, json=data)
-        else:
-            logger.error(f"Invalid method: {method}")
-            raise RuntimeError("Invalid HTTP method")
-
-        resp.raise_for_status()
-
-        return resp
+        This plugin is used to send metrics to Cockpit.
+        It is installed globally for all services.
+        """
+        plugins_url = self.admin_url + "/plugins"
+
+        # Delete existing statsd plugin if it exists
+        resp = self.session.get(plugins_url)
+        plugins = resp.json()["data"]
+        for plugin in plugins:
+            if plugin["name"] == "statsd":
+                self.session.delete(f"{plugins_url}/{plugin['id']}")
+
+        # Install statsd plugin
+        resp = self.session.post(
+            plugins_url,
+            json={
+                "name": "statsd",
+                "config": {
+                    "port": 8125,
+                    "prefix": "kong",
+                },
+            },
+        )
+        body_json = resp.json()
+        plugin_id = body_json["id"]
+        return plugin_id
```

### Comparing `scw_gateway-0.1.2/cli/model.py` & `scw_gateway-0.2.0/cli/model.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.1.2/pyproject.toml` & `scw_gateway-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.1.2"
-description = ""
+version = "0.2.0"
+description = "CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem"
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
 packages = [{include = "cli"}]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
 python = "^3.10"
@@ -38,9 +38,7 @@
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 testpaths = ["tests"]
 
 [tool.mypy]
 exclude = ["venv", "endpoints"]
-# TODO - enable mypy checking properly and fix issue with kong_pdk
-ignore_missing_imports = true
```

### Comparing `scw_gateway-0.1.2/PKG-INFO` & `scw_gateway-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.1.2
-Summary: 
+Version: 0.2.0
+Summary: CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

