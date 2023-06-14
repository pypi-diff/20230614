# Comparing `tmp/checkmk_dev_tools-0.1.8.tar.gz` & `tmp/checkmk_dev_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmk_dev_tools-0.1.8.tar", max compression
+gzip compressed data, was "checkmk_dev_tools-0.1.9.tar", max compression
```

## Comparing `checkmk_dev_tools-0.1.8.tar` & `checkmk_dev_tools-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1475 2023-06-12 09:05:06.347787 checkmk_dev_tools-0.1.8/Readme.md
--rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.8/cmk_dev/__init__.py
--rwxr-xr-x   0        0        0    23922 2023-06-12 09:05:06.347787 checkmk_dev_tools-0.1.8/cmk_dev/ci_artifacts.py
--rwxr-xr-x   0        0        0     2184 2023-06-05 16:21:12.072374 checkmk_dev_tools-0.1.8/cmk_dev/cli.py
--rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.8/cmk_dev/listen_std.py
--rw-r--r--   0        0        0     2179 2023-06-12 09:05:27.943828 checkmk_dev_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-06-12 13:48:13.632427 checkmk_dev_tools-0.1.9/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-10 11:17:07.102380 checkmk_dev_tools-0.1.9/cmk_dev/__init__.py
+-rwxr-xr-x   0        0        0    24056 2023-06-12 13:48:13.624427 checkmk_dev_tools-0.1.9/cmk_dev/ci_artifacts.py
+-rwxr-xr-x   0        0        0     2184 2023-06-05 16:21:12.072374 checkmk_dev_tools-0.1.9/cmk_dev/cli.py
+-rwxr-xr-x   0        0        0     2249 2023-05-10 11:18:34.886818 checkmk_dev_tools-0.1.9/cmk_dev/listen_std.py
+-rw-r--r--   0        0        0     2179 2023-06-12 13:48:35.972512 checkmk_dev_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 checkmk_dev_tools-0.1.9/PKG-INFO
```

### Comparing `checkmk_dev_tools-0.1.8/Readme.md` & `checkmk_dev_tools-0.1.9/Readme.md`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.8/cmk_dev/ci_artifacts.py` & `checkmk_dev_tools-0.1.9/cmk_dev/ci_artifacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,37 +362,37 @@
     # https://bugs.launchpad.net/python-jenkins/+bug/1973243
     # https://bugs.launchpad.net/python-jenkins/+bug/2018576
     fingerprints = client._session.get(
         f"{build_url}api/json?tree=fingerprint[fileName,hash]"
     ).json()["fingerprint"]
 
     if not fingerprints:
-        raise Fatal(f"No (fingerprinted) artifacts found at {build_url}")
+        raise Fatal(f"no (fingerprinted) artifacts found at {build_url}")
 
     for fingerprint in fingerprints:
         fp_filename, fp_hash = fingerprint["fileName"], fingerprint["hash"]
-        logger().debug("Handle artifact: %s (md5: %s)", fp_filename, fp_hash)
+        logger().debug("fandle artifact: %s (md5: %s)", fp_filename, fp_hash)
         artifact_filename = out_dir / fp_filename
         local_hash = md5from(artifact_filename)
 
         if local_hash == fp_hash:
-            logger().debug("File is already available locally: %s (md5: %s)", fp_filename, fp_hash)
+            logger().debug("file is already available locally: %s (md5: %s)", fp_filename, fp_hash)
             skipped += 1
             continue
 
         if local_hash and local_hash != fp_hash:
             logger().warning(
-                "File exists locally but hashes differ: %s %s != %s",
+                "file exists locally but hashes differ: %s %s != %s",
                 fp_filename,
                 local_hash,
                 fp_hash,
             )
 
         with client._session.get(f"{build_url}artifact/{fp_filename}", stream=True) as reply:
-            logger().debug("Download: %s", fp_filename)
+            logger().debug("download: %s", fp_filename)
             reply.raise_for_status()
             with open(artifact_filename, "wb") as out_file:
                 for chunk in reply.iter_content(chunk_size=1 << 16):
                     out_file.write(chunk)
             downloaded += 1
     return downloaded, skipped
 
@@ -446,34 +446,34 @@
 
     assert build.result in {None, "SUCCESS", "FAILURE"}
 
     result = True
 
     # Prune if the build already failed (might still be ongoing)
     if build.result not in {"SUCCESS", None}:
-        logger().debug("build #%d result was: %s", build.number, build.result)
+        logger().debug("build #%s result was: %s", build.number, build.result)
         return False
 
     if mismatching_parameters := find_mismatching_parameters(params or {}, build.parameters):
         logger().debug(
-            "build #%d has mismatching parameters: %s", build.number, mismatching_parameters
+            "build #%s has mismatching parameters: %s", build.number, mismatching_parameters
         )
         result = False
 
     if time_constraints is None or time_constraints == "today":
         if build.timestamp.date() != datetime.now().date():
             logger().debug(
-                "build #%d does not meet time constraints: %s != %s",
+                "build #%s does not meet time constraints: %s != %s",
                 build.number,
                 build.timestamp.date(),
                 now.date(),
             )
             if result:
                 logger().warning(
-                    "build #%d seems to have no relevant changes, but is invalidated by time"
+                    "build #%s seems to have no relevant changes, but is invalidated by time"
                     " constraint only! You might want to check build conditions."
                 )
             result = False
     else:
         raise Fatal(f"Don't understand time constraint specifier {time_constraints!r}")
 
     return result
@@ -484,30 +484,29 @@
     params: None | JobParams,
     time_constraints: None | str,
 ) -> Build | None:
     """Goes through a job's build items and returns the first one to match certain criteria or None
     if none is found"""
     for build_id, build in job.builds.items():
         if meets_constraints(build, params, time_constraints):
-            print(f"Found matching build: {build_id} ({build.url})")
+            logger().info("found matching build: %s (%s)", build_id, build.url)
             for key, value in build.__dict__.items():
                 logger().debug("  %s: %s", key, value)
             return build
     return None
 
 
 def build_id_from_queue_item(client: Jenkins, queue_id: QueueId) -> BuildId:
     """Waits for queue item with given @queue_id to be scheduled and returns Build instance"""
+    logger().info("waiting for queue item %s to be scheduled", queue_id)
     while True:
         queue_item = client.get_queue_item(queue_id)
-        # print(yaml.dump(queue_item))
         if executable := queue_item.get("executable"):
-            # print(yaml.dump(executable))
             return executable["number"]
-        print(f"Waiting for queue item {queue_item['id']} to be scheduled ({queue_item['why']})")
+        logger().debug("still waiting in queue, because %s", queue_item["why"])
         time.sleep(1)
 
 
 def find_matching_queue_item(client: Jenkins, job: Job, params: None | JobParams) -> BuildId | None:
     """Looks for a queued build matching job and parameters and returns the QueueId"""
     for queue_item in client.get_queue_info():
 
@@ -517,15 +516,15 @@
             continue
         mismatching_parameters = find_mismatching_parameters(
             params or {},
             params_from(queue_item, "ParametersAction", "parameters"),
         )
         if mismatching_parameters:
             logger().debug(
-                "queue item %d has mismatching parameters: %s",
+                "queue item %s has mismatching parameters: %s",
                 queue_item.get("id"),
                 mismatching_parameters,
             )
             continue
         return build_id_from_queue_item(client, cast(int, queue_item.get("id")))
     return None
 
@@ -600,22 +599,24 @@
         path_hashes = {
             path: git_commit_id(used_base_dir, path) for path in (dependency_paths or [])
         }
 
         build_candidate = elect_build_candidate()
 
         if build_candidate.in_progress or build_candidate.building:
-            print(f"Waiting for job #{build_candidate.number} to finish..")
+            logger().info(
+                "build #%s still in progress (%s)", build_candidate.number, build_candidate.url
+            )
             while True:
                 build_candidate = Build(
                     client.get_build_info(job_full_path, build_candidate.number)
                 )
                 # TODO: what's the difference between .in_progress and .building?
                 if build_candidate.in_progress or build_candidate.building:
-                    logger().info("build %d in progress", build_candidate.number)
+                    logger().debug("build %s in progress", build_candidate.number)
                     time.sleep(10)
                     continue
                 break
 
             if build_candidate.result != "SUCCESS":
                 raise Fatal(
                     "The build we started has "
@@ -630,23 +631,28 @@
             )
 
         if not build_candidate.artifacts:
             raise Fatal("Job has no artifacts!")
 
         full_out_dir = used_base_dir / (out_dir or "")
         downloaded, skipped = download_artifacts(client, build_candidate.url, full_out_dir)
-        print(f"{downloaded + skipped} artifacts available in {full_out_dir} ({skipped} skipped)")
+        logger().info(
+            "%d artifacts available in %s (%d skipped, because it existed already)",
+            downloaded + skipped,
+            full_out_dir,
+            skipped,
+        )
 
 
 def main() -> None:
     """Entry point for everything else"""
     try:
         args = parse_args()
         logging.basicConfig(
-            format="%(levelname)s %(asctime)s %(name)s: %(message)s",
+            format="%(name)s %(levelname)s: %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
             level=logging.DEBUG if args.log_level == "ALL_DEBUG" else logging.WARNING,
         )
         logger().setLevel(getattr(logging, args.log_level.split("_")[-1]))
         logger().debug("Parsed args: %s", args)
         args.func(args)
     except Fatal as exc:
```

### Comparing `checkmk_dev_tools-0.1.8/cmk_dev/cli.py` & `checkmk_dev_tools-0.1.9/cmk_dev/cli.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.8/cmk_dev/listen_std.py` & `checkmk_dev_tools-0.1.9/cmk_dev/listen_std.py`

 * *Files identical despite different names*

### Comparing `checkmk_dev_tools-0.1.8/pyproject.toml` & `checkmk_dev_tools-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkmk-dev-tools"
-version = "0.1.8"
+version = "0.1.9"
 description = "Checkmk DevOps tools"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/tribe29/checkmk"
 readme = "Readme.md"
 packages = [
   {include = "cmk_dev/**/*.py"}
 ]
```

### Comparing `checkmk_dev_tools-0.1.8/PKG-INFO` & `checkmk_dev_tools-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmk-dev-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Checkmk DevOps tools
 Home-page: https://github.com/tribe29/checkmk
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

