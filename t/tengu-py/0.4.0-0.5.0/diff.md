# Comparing `tmp/tengu_py-0.4.0.tar.gz` & `tmp/tengu_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tengu_py-0.4.0.tar", max compression
+gzip compressed data, was "tengu_py-0.5.0.tar", max compression
```

## Comparing `tengu_py-0.4.0.tar` & `tengu_py-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3245 2023-06-09 07:55:19.750353 tengu_py-0.4.0/README.md
--rw-r--r--   0        0        0     1555 2023-06-09 08:06:14.377422 tengu_py-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-05-31 05:29:35.614982 tengu_py-0.4.0/tengu/__init__.py
--rw-r--r--   0        0        0    12664 2023-06-09 08:05:24.801963 tengu_py-0.4.0/tengu/api.py
--rw-r--r--   0        0        0     7311 2023-05-31 05:29:35.614982 tengu_py-0.4.0/tengu/calcq.py
--rw-r--r--   0        0        0     4434 2023-05-31 05:29:35.614982 tengu_py-0.4.0/tengu/data.py
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 tengu_py-0.4.0/setup.py
--rw-r--r--   0        0        0     3817 1970-01-01 00:00:00.000000 tengu_py-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3616 2023-06-14 10:01:55.509126 tengu_py-0.5.0/README.md
+-rw-r--r--   0        0        0     1567 2023-06-14 09:41:40.110661 tengu_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-06-14 09:42:26.699305 tengu_py-0.5.0/tengu/__init__.py
+-rw-r--r--   0        0        0    20155 2023-06-14 09:43:37.936264 tengu_py-0.5.0/tengu/api.py
+-rw-r--r--   0        0        0     7311 2023-05-31 05:29:35.614982 tengu_py-0.5.0/tengu/calcq.py
+-rw-r--r--   0        0        0     4434 2023-05-31 05:29:35.614982 tengu_py-0.5.0/tengu/data.py
+-rw-r--r--   0        0        0     7360 2023-06-14 09:59:34.654578 tengu_py-0.5.0/tengu/local.py
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 tengu_py-0.5.0/setup.py
+-rw-r--r--   0        0        0     4200 1970-01-01 00:00:00.000000 tengu_py-0.5.0/PKG-INFO
```

### Comparing `tengu_py-0.4.0/README.md` & `tengu_py-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,30 +25,48 @@
 # path to protein pdb with correct charges and protonation
 protein_pdb = Path("./examples/4w9f_prepared_protein.pdb")
 
 # get base64 encoded data
 
 file_arg = provider.upload_arg(protein_pdb)
 
-res = client.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#convert", [ 
-{ "value": "PDB" }, file_arg
+res = client.run("github:talo/tengu-prelude/77e44748f1d1e20c463ef34cc40178d4f656ef0a#convert", [ 
+Arg(value = PDB), file_arg
 ])
 
 // res contains "id" - the instance id; and "outs" - the ids of the return values 
 
 // we can pass arguments by "id" reference or by value literal
 
 client.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#pick_conformer", [ 
-{ "id": res["outs"][0]["id"] }, { "value": 1 }
+Arg( id =  res["outs"][0]["id"] ), Arg( value = 1 ) }
 ])
 
 client.poll_module_instance(id) 
 // status, progress, logs, outs - out values will be null until module_instance is done
 ```
 
+## Local runner
+
+We also provide a local executor, that will run modules locally, without making remote calls
+
+First, you must have nix installed and configured with an access token for qdx projects.
+
+Then you must install the tengu-runtime with `nix run github:talo/tengu#tengu-runtime -- install`
+
+Finally, you can run locally with
+
+``` python
+from tengu import LocalProvider
+
+client = LocalProvider()
+
+## you should be able to use client.run / client.object / client.module_instance / client.poll_module instance as normal
+```
+
 ## Sample QP Run
 
 ``` python
 frag_keywords = {
     "dimer_cutoff": 25,
     "dimer_mp2_cutoff": 25,
     "fragmentation_level": 2,
@@ -85,34 +103,23 @@
         None,
         default_model,
     ),
     Arg(None, {"frag": frag_keywords, "scf": scf_keywords}),
     Arg(
         None,
         [
-            ("GLY", 993),
-            ("ASP", 994),
-            ("VAL", 863),
-            ("LYS", 882),
-            ("TYR", 931),
-            ("GLY", 935),
-            ("VAL", 911),
-            ("GLU", 930),
-            ("ALA", 880),
-            ("LEU", 983),
-            ("PRO", 933),
-            ("LEU", 855),
-            ("MET", 929),
-            ("SER", 936),
-            ("LEU", 932),
+            ("GLY", 100), # map of amino acids of interest
         ],
     ),
     "GADI",
     {"walltime": 420},
     autopoll = (10, 100) # optionally configure polling to wait on the final instance, 
                          # and clean up if any of the prior instances fails
 )
 
 # if you set autpoll, you will get the results of the qp_collate instance,
 # otherwise you will get an array with all the spawned instances, and have to poll manually
-client.poll_module_instance(qp_collate_instance[2]["id"]) 
+completed_instance = client.poll_module_instance(qp_collate_instance[2]["id"]) 
+
+# the result will be an object, so fetch from object store
+client.object(completed_instance["outs"][0]["id"]) # will return the json qp results
 ```
```

### Comparing `tengu_py-0.4.0/pyproject.toml` & `tengu_py-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 [tool.setuptools.packages]
 [tool.setuptools.packages.find]
 exclude = ["test", "tests"]
 where = [""]
 
 [tool.poetry]
 name = "tengu-py"
-version = "0.4.0"
-description = "Python SDK for interacting with the QDX Tengu API"
+version = "0.5.0"
+description = "Python SDK for interacting with the QDX Tengu API and modules"
 authors = ["Ryan Swart <ryan@talosystems.com>"]
 readme = "README.md"
 packages = [{include = "tengu"}]
 
 [tool.poetry.scripts]
 # tengu = "tengu.__main__:main"
```

### Comparing `tengu_py-0.4.0/tengu/api.py` & `tengu_py-0.5.0/tengu/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,18 +6,86 @@
 
 import dataclasses_json
 from gql import Client, gql
 from gql.transport.requests import RequestsHTTPTransport
 
 ModuleInstanceId = str
 
+
+tag = gql(
+    """
+mutation tag($moduleInstanceId: ModuleInstanceId, $argumentId: ArgumentId, $moduleId: ModuleId, $tags: [String!]!) {
+    tag(module_instance: $moduleInstanceId, argument: $argumentId, module: $moduleId, tags: $tags)
+}
+"""
+)
+
+untag = gql(
+    """
+mutation untag($moduleInstanceId: ModuleInstanceId, $argumentId: ArgumentId, $moduleId: ModuleId, $tags: [String!]!) {
+    untag(module_instance: $moduleInstanceId, argument: $argumentId, module: $moduleId, tags: $tags)
+}
+"""
+)
+
+argument = gql(
+    """
+query ($id: ArgumentId!) {
+    argument(id: $id) {
+        id
+        typeinfo
+        value
+        created_at
+        tags
+    }
+    }
+    """
+)
+
+arguments_query = gql(
+    """
+query ($first: Int, $after: String, $last: Int, $before: String, $typeinfo: JSON, $tags: [String!]) {
+    me { account {
+        arguments(first: $first, last: $last, after: $after, before: $before, typeinfo: $typeinfo, tags: $tags) {
+            nodes {
+                id
+                typeinfo
+                value
+                created_at
+                tags
+            }
+        }
+    } }
+}
+"""
+)
+
+
 modules = gql(
     """
-query ($first: Int, $after: String, $last: Int, $before: String, $path: String) {
-    modules(first: $first, last: $last, after: $after, before: $before, path: $path) {
+query ($first: Int, $after: String, $last: Int, $before: String, $path: String, $tags: [String!]) {
+    modules(first: $first, last: $last, after: $after, before: $before, path: $path, tags: $tags) {
+        nodes {
+            id
+            path
+            created_at
+            deleted_at
+            ins
+            outs
+            tags
+        }
+    }
+}
+"""
+)
+
+latest_modules = gql(
+    """
+query ($first: Int, $after: String, $last: Int, $before: String) {
+    latest_modules(first: $first, last: $last, after: $after, before: $before) {
         nodes {
             id
             path
             created_at
             deleted_at
             ins
             outs
@@ -45,14 +113,15 @@
     }
     """
 )
 
 # module instance fragment
 module_instance_fragment = """
     id
+    tags
     created_at
     deleted_at
     account_id
     path
     ins {
       id
       typeinfo
@@ -97,17 +166,17 @@
     stderr {
       nodes { content id created_at }
     }
   } }"""
 )
 
 module_instances_query = gql(
-    """query($first: Int, $after: String, $last: Int, $before: String, $path: String, $status: ModuleInstanceStatus) {
+    """query($first: Int, $after: String, $last: Int, $before: String, $path: String, $name: String, $status: ModuleInstanceStatus, $tags: [String!]) {
     me { account {
-    module_instances(first: $first, last: $last, after: $after, before: $before, path: $path, status: $status) {
+    module_instances(first: $first, last: $last, after: $after, before: $before, path: $path, status: $status, name: $name, tags: $tags) {
     nodes {
     """
     + module_instance_fragment
     + """
   } } } } }"""
 )
 
@@ -129,16 +198,16 @@
 
 
 T1 = TypeVar("T1")
 
 
 @dataclass
 class Arg(Generic[T1], DataClassJsonMixin):
-    id: str | None
-    value: T1 | None
+    id: str | None = None
+    value: T1 | None = None
 
 
 frag_keywords = {
     "dimer_cutoff": 25,
     "dimer_mp2_cutoff": 25,
     "fragmentation_level": 2,
     "method": "MBE",
@@ -174,32 +243,102 @@
         :param url: The URL of the Tengu platform.
         :param access_token: The access token for authentication.
         """
         transport = RequestsHTTPTransport(url=url, headers={"authorization": f"bearer {access_token}"})
 
         self.client = Client(transport=transport)
 
+    def argument(self, id: str) -> Any:
+        """
+        Retrieve an argument from the database.
+
+        :param id: The ID of the argument.
+        :return: The argument.
+        """
+        response = self.client.execute(argument, variable_values={"id": id})
+        return response.get("argument")
+
+    def arguments(
+        self,
+        first: int | None = None,
+        after: str | None = None,
+        last: int | None = None,
+        before: str | None = None,
+        tags: list[str] | None = None,
+    ) -> list[Any]:
+        """
+        Retrieve a list of arguments.
+        """
+        response = self.client.execute(
+            arguments_query,
+            variable_values={
+                "first": first,
+                "after": after,
+                "last": last,
+                "before": before,
+                "tags": tags,
+            },
+        )
+
+        arguments = response["me"]["account"]["arguments"]
+
+        if arguments:
+            arguments = arguments.get("nodes")
+            if arguments:
+                return arguments
+        return []
+
     def object(self, id):
         """
         Retrieve an object from the database.
 
         :param id: The ID of the object.
         :return: The object.
         """
         response = self.client.execute(object_query, variable_values={"id": id})
         return response.get("object")
 
+    def latest_modules(
+        self,
+        first: int | None = None,
+        after: str | None = None,
+        last: int | None = None,
+        before: str | None = None,
+    ):
+        """
+        Retrieve a list of modules.
+
+        :param path: The path of the module.
+        :param name: The name of the module.
+        :param first: The maximum number of modules to retrieve.
+        :param after: The cursor to start retrieving modules from.
+        :param last: The maximum number of modules to retrieve.
+        :param before: The cursor to start retrieving modules from.
+        :return: A list of modules.
+        """
+        response = self.client.execute(
+            latest_modules,
+            variable_values={
+                "first": first,
+                "after": after,
+                "last": last,
+                "before": before,
+            },
+        )
+        return response.get("latest_modules")
+
     def modules(
         self,
         path: str | None = None,
         name: str | None = None,
         first: int | None = None,
         after: str | None = None,
         last: int | None = None,
         before: str | None = None,
+        tags: list[str] | None = None,
     ):
         """
         Retrieve a list of modules.
 
         :param path: The path of the module.
         :param name: The name of the module.
         :param first: The maximum number of modules to retrieve.
@@ -213,36 +352,48 @@
             variable_values={
                 "path": path,
                 "name": name,
                 "first": first,
                 "after": after,
                 "last": last,
                 "before": before,
+                "tags": tags,
             },
         )
         return response.get("modules")
 
     def run(
         self,
         path: str,
         args: list[Arg],
         target: Literal["GADI", "NIX"] | None = None,
         resources: dict[str, Any] | None = None,
+        tags: list[str] | None = None,
+        out_tags: list[list[str] | None] | None = None,
     ):
         """
         Run a module with the given inputs and outputs.
+        :param path: The path of the module.
+        :param args: The arguments to the module.
+        :param target: The target to run the module on.
+        :param resources: The resources to run the module with.
+        :param tags: The tags to apply to the module.
+        :param out_tags: The tags to apply to the outputs of the module.
+                         If provided, must be the same length as the number of outputs.
         """
         response = self.client.execute(
             run_mutation,
             variable_values={
                 "instance": {
                     "path": path,
                     "args": [arg.to_dict() for arg in args],
                     "target": target,
                     "resources": resources,
+                    "tags": tags,
+                    "out_tags": out_tags,
                 }
             },
         )
         module_instance = response.get("run")
         if module_instance:
             return module_instance
         else:
@@ -260,45 +411,67 @@
         lig_res_id: Arg[str],
         model: Arg[dict[str, Any]] = Arg(None, default_model),
         keywords: Arg[dict[str, Any]] = Arg(None, {"frag": frag_keywords, "scf": scf_keywords}),
         amino_acids_of_interest: Arg[list[tuple[str, int]]] = Arg(None, None),
         target: Literal["GADI", "NIX"] | None = None,
         resources: dict[str, Any] | None = None,
         autopoll: tuple[int, int] | None = None,
+        tags: list[str] | None = None,
     ):
         """
         Construct the input and output module instance calls for QP run.
+        :param qp_gen_inputs_path: The path of the QP gen inputs module.
+        :param hermes_energy_path: The path of the Hermes energy module.
+        :param qp_collate_path: The path of the QP collate module.
+        :param pdb: The PDB file containing both the protein and ligand.
+        :param gro: The GRO file containing ligand.
+        :param lig: The ligand file.
+        :param lig_type: The type of ligand file.
+        :param lig_res_id: The residue ID of the ligand.
+        :param model: The model to use for the QP Hermes run.
+        :param keywords: The keywords to use for the QP Hermes run.
+        :param amino_acids_of_interest: The amino acids of interest to restrict the run to.
+        :param target: The target to run the module on.
+        :param resources: The resources to run the module with.
+        :param autopoll: The autopoll interval and timeout.
+        :param tag: The tags to apply to all module instances, arguements and outs.
         """
 
         qp_prep_instance = self.run(
             qp_gen_inputs_path,
             [pdb, gro, lig, lig_type, lig_res_id, model, keywords, amino_acids_of_interest],
+            tags=tags,
+            out_tags=([tags, tags, tags, tags] if tags else None),
         )
         try:
             hermes_instance = self.run(
                 hermes_energy_path,
                 [
                     Arg(qp_prep_instance["outs"][0]["id"], None),
                     Arg(qp_prep_instance["outs"][1]["id"], None),
                     Arg(qp_prep_instance["outs"][2]["id"], None),
                 ],
                 target,
                 resources,
+                tags=tags,
+                out_tags=([tags] if tags else None),
             )
         except:
             self.delete_module_instance(qp_prep_instance["id"])
             raise
 
         try:
             qp_collate_instance = self.run(
                 qp_collate_path,
                 [
                     Arg(hermes_instance["outs"][0]["id"], None),
                     Arg(qp_prep_instance["outs"][3]["id"], None),
                 ],
+                tags=tags,
+                out_tags=([tags] if tags else None),
             )
         except:
             self.delete_module_instance(qp_prep_instance["id"])
             self.delete_module_instance(hermes_instance["id"])
             raise
 
         if autopoll:
@@ -379,22 +552,78 @@
 
         :param file: The file to be uploaded.
         :return: The formatted file.
         """
         with open(file, "rb") as f:
             return Arg(None, value=base64.b64encode(f.read()).decode("utf-8"))
 
+    def tag(
+        self,
+        tags: list[str],
+        module_id: str | None = None,
+        module_instance_id: str | None = None,
+        argument_id: str | None = None,
+    ) -> list[str]:
+        """
+        Add a list of tags to a module, module instance, or argument.
+
+        :param tags: The list of tags to be added.
+        :param module_id: The ID of the module to be tagged.
+        :param module_instance_id: The ID of the module instance to be tagged.
+        :param argument_id: The ID of the argument to be tagged.
+        :return: The resulting full list of tags on the entity.
+        """
+        response = self.client.execute(
+            tag,
+            variable_values={
+                "tags": tags,
+                "moduleId": module_id,
+                "moduleInstanceId": module_instance_id,
+                "argumentId": argument_id,
+            },
+        )
+        return response["tag"]
+
+    def untag(
+        self,
+        tags: list[str],
+        module_id: str | None = None,
+        module_instance_id: str | None = None,
+        argument_id: str | None = None,
+    ) -> list[str]:
+        """
+        Remove a list of tags from a module, module instance, or argument.
+
+        :param tags: The list of tags to be removed.
+        :param module_id: The ID of the module to be untagged.
+        :param module_instance_id: The ID of the module instance to be untagged.
+        :param argument_id: The ID of the argument to be untagged.
+        :return: The list of remaining tags.
+        """
+        response = self.client.execute(
+            untag,
+            variable_values={
+                "tags": tags,
+                "moduleId": module_id,
+                "moduleInstanceId": module_instance_id,
+                "argumentId": argument_id,
+            },
+        )
+        return response["untag"]
+
     def module_instances(
         self,
         before: str | None = None,
         after: str | None = None,
         first: int | None = None,
         last: int | None = None,
         path: str | None = None,
+        name: str | None = None,
         status: Literal["CREATED", "ADMITTED", "QUEUED", "DISPATCHED", "COMPLETED", "FAILED"] | None = None,
+        tags: list[str] | None = None,
     ) -> list[Any]:
         """
         Retrieve a list of module instancees filtered by the given parameters.
 
         :param before: Retrieve module instances before a certain cursor.
         :param after: Retrieve module instances after a certain cursor.
         :param first: Retrieve the first N module instances.
@@ -407,15 +636,17 @@
             module_instances_query,
             variable_values={
                 "first": first,
                 "last": last,
                 "before": before,
                 "after": after,
                 "path": path,
+                "name": name,
                 "status": status,
+                "tags": tags,
             },
         )
         module_instances = response["me"]["account"]["module_instances"]
 
         if module_instances:
             module_instances = module_instances.get("nodes")
             if module_instances:
```

### Comparing `tengu_py-0.4.0/tengu/calcq.py` & `tengu_py-0.5.0/tengu/calcq.py`

 * *Files identical despite different names*

### Comparing `tengu_py-0.4.0/tengu/data.py` & `tengu_py-0.5.0/tengu/data.py`

 * *Files identical despite different names*

### Comparing `tengu_py-0.4.0/setup.py` & `tengu_py-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['dataclasses-json>=0.5.7,<0.6.0',
  'datargs>=0.11.0,<0.12.0',
  'gql[requests]>=3.4.0,<4.0.0',
  'rdkit-pypi>=2022.9.5,<2023.0.0']
 
 setup_kwargs = {
     'name': 'tengu-py',
-    'version': '0.4.0',
-    'description': 'Python SDK for interacting with the QDX Tengu API',
-    'long_description': '# Tengu-py: Python SDK for the QDX Tengu API\n\nThis package exposes a simple provider and CLI for the different tools exposed by the QDX Tengu GraphQL API.\n\n## Usage\n\n### As a library\n\n``` python\nimport json\nfrom pathlib import Path\n\nimport tengu\n\nTOKEN = "your qdx access token"\n\n# get our client to talk with the API\nclient = tengu.Provider(access_token=TOKEN)\n\n# get modules that can be run\nclient.modules()\n\n## running convert\n\n# path to protein pdb with correct charges and protonation\nprotein_pdb = Path("./examples/4w9f_prepared_protein.pdb")\n\n# get base64 encoded data\n\nfile_arg = provider.upload_arg(protein_pdb)\n\nres = client.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#convert", [ \n{ "value": "PDB" }, file_arg\n])\n\n// res contains "id" - the instance id; and "outs" - the ids of the return values \n\n// we can pass arguments by "id" reference or by value literal\n\nclient.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#pick_conformer", [ \n{ "id": res["outs"][0]["id"] }, { "value": 1 }\n])\n\nclient.poll_module_instance(id) \n// status, progress, logs, outs - out values will be null until module_instance is done\n```\n\n## Sample QP Run\n\n``` python\nfrag_keywords = {\n    "dimer_cutoff": 25,\n    "dimer_mp2_cutoff": 25,\n    "fragmentation_level": 2,\n    "method": "MBE",\n    "monomer_cutoff": 30,\n    "monomer_mp2_cutoff": 30,\n    "ngpus_per_node": 4,\n    "reference_fragment": 293,\n    "trimer_cutoff": 10,\n    "trimer_mp2_cutoff": 10,\n    "lattice_energy_calc": True,\n}\n\nscf_keywords = {\n    "convergence_metric": "diis",\n    "dynamic_screening_threshold_exp": 10,\n    "ndiis": 8,\n    "niter": 40,\n    "scf_conv": 0.000001,\n}\n\ndefault_model = {"method": "RIMP2", "basis": "cc-pVDZ", "aux_basis": "cc-pVDZ-RIFIT", "frag_enabled": True}\n\nqp_instances = client.qp_run(\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#qp_gen_inputs",\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#hermes_energy",\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#qp_collate",\n    provider.upload_arg(Path("some.pdb")),\n    provider.upload_arg(Path("some.gro")),\n    provider.upload_arg(Path("some.sdf")),\n    Arg(None, "sdf"),\n    Arg(None, "MOL"),\n    Arg(\n        None,\n        default_model,\n    ),\n    Arg(None, {"frag": frag_keywords, "scf": scf_keywords}),\n    Arg(\n        None,\n        [\n            ("GLY", 993),\n            ("ASP", 994),\n            ("VAL", 863),\n            ("LYS", 882),\n            ("TYR", 931),\n            ("GLY", 935),\n            ("VAL", 911),\n            ("GLU", 930),\n            ("ALA", 880),\n            ("LEU", 983),\n            ("PRO", 933),\n            ("LEU", 855),\n            ("MET", 929),\n            ("SER", 936),\n            ("LEU", 932),\n        ],\n    ),\n    "GADI",\n    {"walltime": 420},\n    autopoll = (10, 100) # optionally configure polling to wait on the final instance, \n                         # and clean up if any of the prior instances fails\n)\n\n# if you set autpoll, you will get the results of the qp_collate instance,\n# otherwise you will get an array with all the spawned instances, and have to poll manually\nclient.poll_module_instance(qp_collate_instance[2]["id"]) \n```\n',
+    'version': '0.5.0',
+    'description': 'Python SDK for interacting with the QDX Tengu API and modules',
+    'long_description': '# Tengu-py: Python SDK for the QDX Tengu API\n\nThis package exposes a simple provider and CLI for the different tools exposed by the QDX Tengu GraphQL API.\n\n## Usage\n\n### As a library\n\n``` python\nimport json\nfrom pathlib import Path\n\nimport tengu\n\nTOKEN = "your qdx access token"\n\n# get our client to talk with the API\nclient = tengu.Provider(access_token=TOKEN)\n\n# get modules that can be run\nclient.modules()\n\n## running convert\n\n# path to protein pdb with correct charges and protonation\nprotein_pdb = Path("./examples/4w9f_prepared_protein.pdb")\n\n# get base64 encoded data\n\nfile_arg = provider.upload_arg(protein_pdb)\n\nres = client.run("github:talo/tengu-prelude/77e44748f1d1e20c463ef34cc40178d4f656ef0a#convert", [ \nArg(value = PDB), file_arg\n])\n\n// res contains "id" - the instance id; and "outs" - the ids of the return values \n\n// we can pass arguments by "id" reference or by value literal\n\nclient.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#pick_conformer", [ \nArg( id =  res["outs"][0]["id"] ), Arg( value = 1 ) }\n])\n\nclient.poll_module_instance(id) \n// status, progress, logs, outs - out values will be null until module_instance is done\n```\n\n## Local runner\n\nWe also provide a local executor, that will run modules locally, without making remote calls\n\nFirst, you must have nix installed and configured with an access token for qdx projects.\n\nThen you must install the tengu-runtime with `nix run github:talo/tengu#tengu-runtime -- install`\n\nFinally, you can run locally with\n\n``` python\nfrom tengu import LocalProvider\n\nclient = LocalProvider()\n\n## you should be able to use client.run / client.object / client.module_instance / client.poll_module instance as normal\n```\n\n## Sample QP Run\n\n``` python\nfrag_keywords = {\n    "dimer_cutoff": 25,\n    "dimer_mp2_cutoff": 25,\n    "fragmentation_level": 2,\n    "method": "MBE",\n    "monomer_cutoff": 30,\n    "monomer_mp2_cutoff": 30,\n    "ngpus_per_node": 4,\n    "reference_fragment": 293,\n    "trimer_cutoff": 10,\n    "trimer_mp2_cutoff": 10,\n    "lattice_energy_calc": True,\n}\n\nscf_keywords = {\n    "convergence_metric": "diis",\n    "dynamic_screening_threshold_exp": 10,\n    "ndiis": 8,\n    "niter": 40,\n    "scf_conv": 0.000001,\n}\n\ndefault_model = {"method": "RIMP2", "basis": "cc-pVDZ", "aux_basis": "cc-pVDZ-RIFIT", "frag_enabled": True}\n\nqp_instances = client.qp_run(\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#qp_gen_inputs",\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#hermes_energy",\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#qp_collate",\n    provider.upload_arg(Path("some.pdb")),\n    provider.upload_arg(Path("some.gro")),\n    provider.upload_arg(Path("some.sdf")),\n    Arg(None, "sdf"),\n    Arg(None, "MOL"),\n    Arg(\n        None,\n        default_model,\n    ),\n    Arg(None, {"frag": frag_keywords, "scf": scf_keywords}),\n    Arg(\n        None,\n        [\n            ("GLY", 100), # map of amino acids of interest\n        ],\n    ),\n    "GADI",\n    {"walltime": 420},\n    autopoll = (10, 100) # optionally configure polling to wait on the final instance, \n                         # and clean up if any of the prior instances fails\n)\n\n# if you set autpoll, you will get the results of the qp_collate instance,\n# otherwise you will get an array with all the spawned instances, and have to poll manually\ncompleted_instance = client.poll_module_instance(qp_collate_instance[2]["id"]) \n\n# the result will be an object, so fetch from object store\nclient.object(completed_instance["outs"][0]["id"]) # will return the json qp results\n```\n',
     'author': 'Ryan Swart',
     'author_email': 'ryan@talosystems.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tengu_py-0.4.0/PKG-INFO` & `tengu_py-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tengu-py
-Version: 0.4.0
-Summary: Python SDK for interacting with the QDX Tengu API
+Version: 0.5.0
+Summary: Python SDK for interacting with the QDX Tengu API and modules
 Author: Ryan Swart
 Author-email: ryan@talosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
@@ -41,30 +41,48 @@
 # path to protein pdb with correct charges and protonation
 protein_pdb = Path("./examples/4w9f_prepared_protein.pdb")
 
 # get base64 encoded data
 
 file_arg = provider.upload_arg(protein_pdb)
 
-res = client.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#convert", [ 
-{ "value": "PDB" }, file_arg
+res = client.run("github:talo/tengu-prelude/77e44748f1d1e20c463ef34cc40178d4f656ef0a#convert", [ 
+Arg(value = PDB), file_arg
 ])
 
 // res contains "id" - the instance id; and "outs" - the ids of the return values 
 
 // we can pass arguments by "id" reference or by value literal
 
 client.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#pick_conformer", [ 
-{ "id": res["outs"][0]["id"] }, { "value": 1 }
+Arg( id =  res["outs"][0]["id"] ), Arg( value = 1 ) }
 ])
 
 client.poll_module_instance(id) 
 // status, progress, logs, outs - out values will be null until module_instance is done
 ```
 
+## Local runner
+
+We also provide a local executor, that will run modules locally, without making remote calls
+
+First, you must have nix installed and configured with an access token for qdx projects.
+
+Then you must install the tengu-runtime with `nix run github:talo/tengu#tengu-runtime -- install`
+
+Finally, you can run locally with
+
+``` python
+from tengu import LocalProvider
+
+client = LocalProvider()
+
+## you should be able to use client.run / client.object / client.module_instance / client.poll_module instance as normal
+```
+
 ## Sample QP Run
 
 ``` python
 frag_keywords = {
     "dimer_cutoff": 25,
     "dimer_mp2_cutoff": 25,
     "fragmentation_level": 2,
@@ -101,35 +119,24 @@
         None,
         default_model,
     ),
     Arg(None, {"frag": frag_keywords, "scf": scf_keywords}),
     Arg(
         None,
         [
-            ("GLY", 993),
-            ("ASP", 994),
-            ("VAL", 863),
-            ("LYS", 882),
-            ("TYR", 931),
-            ("GLY", 935),
-            ("VAL", 911),
-            ("GLU", 930),
-            ("ALA", 880),
-            ("LEU", 983),
-            ("PRO", 933),
-            ("LEU", 855),
-            ("MET", 929),
-            ("SER", 936),
-            ("LEU", 932),
+            ("GLY", 100), # map of amino acids of interest
         ],
     ),
     "GADI",
     {"walltime": 420},
     autopoll = (10, 100) # optionally configure polling to wait on the final instance, 
                          # and clean up if any of the prior instances fails
 )
 
 # if you set autpoll, you will get the results of the qp_collate instance,
 # otherwise you will get an array with all the spawned instances, and have to poll manually
-client.poll_module_instance(qp_collate_instance[2]["id"]) 
+completed_instance = client.poll_module_instance(qp_collate_instance[2]["id"]) 
+
+# the result will be an object, so fetch from object store
+client.object(completed_instance["outs"][0]["id"]) # will return the json qp results
 ```
```

