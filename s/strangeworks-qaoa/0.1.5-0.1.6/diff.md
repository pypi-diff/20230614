# Comparing `tmp/strangeworks_qaoa-0.1.5.tar.gz` & `tmp/strangeworks_qaoa-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.5.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.6.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.5.tar` & `strangeworks_qaoa-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-12 14:41:14.374113 strangeworks_qaoa-0.1.5/LICENSE
--rw-r--r--   0        0        0      679 2023-05-12 14:41:14.374113 strangeworks_qaoa-0.1.5/README.md
--rw-r--r--   0        0        0      791 2023-05-12 14:41:26.858220 strangeworks_qaoa-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      128 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    16215 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    12428 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 18:57:09.948296 strangeworks_qaoa-0.1.6/LICENSE
+-rw-r--r--   0        0        0      679 2023-06-13 18:57:09.948296 strangeworks_qaoa-0.1.6/README.md
+-rw-r--r--   0        0        0      791 2023-06-13 18:57:24.860287 strangeworks_qaoa-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-06-13 18:57:09.952296 strangeworks_qaoa-0.1.6/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    17373 2023-06-13 18:57:09.952296 strangeworks_qaoa-0.1.6/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-06-13 18:57:09.952296 strangeworks_qaoa-0.1.6/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    12428 2023-06-13 18:57:09.952296 strangeworks_qaoa-0.1.6/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.6/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.5/LICENSE` & `strangeworks_qaoa-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.5/README.md` & `strangeworks_qaoa-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.5/pyproject.toml` & `strangeworks_qaoa-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.5"
+version = "0.1.6"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_qaoa-0.1.5/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.6/strangeworks_qaoa/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,30 @@
 import strangeworks_qaoa.utils as utils
 
 
 class StrangeworksQAOA:
     """Strangeworks client object."""
 
     def __init__(self, resource_slug: Optional[str] = " ") -> None:
-        if resource_slug != " " and resource_slug != "":
-            self.rsc = strangeworks.resources(slug=resource_slug)[0]
-        else:
-            rsc_list = strangeworks.resources()
-            for rr in range(len(rsc_list)):
-                if rsc_list[rr].product.slug == "qaoa":
-                    self.rsc = rsc_list[rr]
+        try:
+            if resource_slug != " " and resource_slug != "":
+                self.rsc = strangeworks.resources(slug=resource_slug)[0]
+            else:
+                rsc_list = strangeworks.resources()
+                for rr in range(len(rsc_list)):
+                    if rsc_list[rr].product.slug == "qaoa":
+                        self.rsc = rsc_list[rr]
+            if self.rsc is None:
+                raise StrangeworksError(
+                    "Unable to find resource. Please add resource on platform https://portal.strangeworks.com/products"  # noqa: E501
+                )
+        except Exception as e:
+            raise StrangeworksError(
+                f"Unable to find resource. Please add resource on platform https://portal.strangeworks.com/products: {e}"  # noqa: E501
+            )
 
         self.backend_list = " "
 
     def backends(self):
         """
         To-Do: Add cross check as to which backends the current user actually has
           access to.
@@ -238,14 +247,27 @@
             QUBO = problem["BQM"].to_numpy_matrix(
                 variable_order=problem.get("variable_order")
             )
             H = utils.get_Ham_from_QUBO(QUBO)
         else:
             raise StrangeworksError("Problem not in currently supported format")
 
+        for _, y in H:
+            if type(y) is tuple:
+                for n in y:
+                    if n > (problem_params["nqubits"] - 1):
+                        raise StrangeworksError(
+                            "Specified qubit number is smaller than problem"
+                        )
+            else:
+                if y > (problem_params["nqubits"] - 1):
+                    raise StrangeworksError(
+                        "Specified qubit number is smaller than problem"
+                    )
+
         problem_params["H"] = json.dumps(H)
         problem_params["ising"] = (
             json.dumps(problem_params["ising"])
             if problem_params.get("ising")
             else json.dumps(False)
         )
         problem_params["warm_start"] = (
@@ -271,14 +293,16 @@
         sw_job = strangeworks.execute(self.rsc, input_params, "run_hybrid_job")
 
         return sw_job
 
     def update_status(self, sw_job):
         if type(sw_job) is dict:
             job_slug = sw_job.get("slug")
+        elif type(sw_job) is str:
+            job_slug = sw_job
         else:
             job_slug = sw_job.slug
 
         status = strangeworks.execute(
             self.rsc, {"payload": {"job_slug": job_slug}}, "status"
         )
 
@@ -327,17 +351,18 @@
 
             try:
                 En_exact = utils.get_exact_en(
                     utils.get_graph_from_Ham(H, nqubits),
                     nqubits,
                     ising=json.loads(inputs["ising"]) if inputs.get("ising") else False,
                 )
-            except Exception:
-                En_exact = "!!problem too big for exact solution!!"
-            result_file["En_exact"] = En_exact
+                result_file["En_exact"] = En_exact
+            except Exception as e:
+                print(f"Error with calculating exact solution: {e}")
+                result_file["En_exact"] = f"Error with calculating exact solution: {e}"
         else:
             result_file["En_exact"] = None
 
         if display_results:
             sol = result_file["sol"]
             En_exact = result_file["En_exact"]
             En_sol = result_file["en_min"]
```

### Comparing `strangeworks_qaoa-0.1.5/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.6/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.5/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.6/strangeworks_qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.5/PKG-INFO` & `strangeworks_qaoa-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

