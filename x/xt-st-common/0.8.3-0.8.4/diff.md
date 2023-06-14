# Comparing `tmp/xt_st_common-0.8.3.tar.gz` & `tmp/xt_st_common-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.8.3.tar", max compression
+gzip compressed data, was "xt_st_common-0.8.4.tar", max compression
```

## Comparing `xt_st_common-0.8.3.tar` & `xt_st_common-0.8.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-12 10:12:11.156918 xt_st_common-0.8.3/README.md
--rw-r--r--   0        0        0     2603 2023-06-12 10:12:11.156918 xt_st_common-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-12 10:11:31.069096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-12 10:11:31.073096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-12 10:11:31.073096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-12 10:11:31.097096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-12 10:11:31.097096 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-12 10:12:11.156918 xt_st_common-0.8.3/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2750 2023-06-12 10:11:31.185095 xt_st_common-0.8.3/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3327 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    41597 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6941 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6936 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-12 10:11:31.189095 xt_st_common-0.8.3/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-14 03:58:20.438397 xt_st_common-0.8.4/README.md
+-rw-r--r--   0        0        0     2603 2023-06-14 03:58:20.438397 xt_st_common-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-14 03:57:43.521948 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-14 03:57:43.525948 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-14 03:58:20.434397 xt_st_common-0.8.4/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2750 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3464 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    42607 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6941 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6936 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.4/PKG-INFO
```

### Comparing `xt_st_common-0.8.3/README.md` & `xt_st_common-0.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.8.3
+# XT-STREAMLIT - 0.8.4
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.8.3/pyproject.toml` & `xt_st_common-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.8.3"
+version = "0.8.4"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.8.4/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/xt_st_common/components.py` & `xt_st_common-0.8.4/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/xt_st_common/config.py` & `xt_st_common-0.8.4/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/xt_st_common/database.py` & `xt_st_common-0.8.4/src/xt_st_common/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,24 +34,29 @@
 @st.cache_data(ttl=30)
 def get_project(project_id: str, cache_id=None) -> Optional[Project]:
     project_dict = get_collection().find_one({"_id": ObjectId(project_id)})
     return Project(**project_dict) if project_dict is not None else None
 
 
 @st.cache_data(ttl=30)
-def get_projects(include_public=False, other_apps=False, cache_id=None) -> List[Project]:
+def get_projects(include_public=False, other_apps=True, shared_project=True, cache_id=None) -> List[Project]:
     current_user = get_user_email()
     or_query = {
         "$or": [
-            {"users": {"$elemMatch": {"$regex": current_user, "$options": "i"}}},
             {"owner": {"$regex": current_user, "$options": "i"}},
         ]
     }
     if include_public:
         or_query["$or"].append({"public": True})
+    if shared_project:
+        or_query["$or"].append({"users": {"$elemMatch": {"$regex": current_user, "$options": "i"}}}),
+
+    if len(or_query["$or"]) == 1:
+        or_query = or_query["$or"][0]
+
     query = or_query if other_apps else {"$and": [{"application": f"{settings.APP_NAME}"}, or_query]}
     return [Project(**item) for item in get_collection().find(query)]
 
 
 @st.cache_data(ttl=30)
 def project_exists(project_id: str, cache_id=None) -> bool:
     return get_collection().count_documents({"_id": ObjectId(project_id)}) > 0
```

### Comparing `xt_st_common-0.8.3/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.8.4/src/xt_st_common/fs_upload_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         relative_root = root.replace(path, "")
 
         # Collect empty directories separately otherwise they never appear in the list
         if include_empty:
             for d in directories:
                 full_dir = Path(root) / d
                 if len(os.listdir(full_dir)) == 0:
-                    files.append(str(Path(relative_root)) / d + os.sep)
+                    files.append(str(Path(relative_root) / d) + os.sep)
 
         # Collect files
         for filename in filenames:
             files.append(Path(relative_root) / filename)
     return files
```

### Comparing `xt_st_common-0.8.3/src/xt_st_common/project_components.py` & `xt_st_common-0.8.4/src/xt_st_common/project_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -352,23 +352,26 @@
 
 
 def _state_name(project_id: str, folder: str) -> str:
     return f"{project_id}-{folder}_fs"
 
 
 @st.cache_data(ttl=15)
-def get_proj_options(include_public: bool, other_apps: bool = True, cache_id=None):
+def get_proj_options(include_public: bool = False, other_apps: bool = True, shared_project: bool = True, cache_id=None):
     selected_project = get_selected_project()
-    projects = get_projects(include_public, other_apps, get_project_cache())
+    projects = get_projects(include_public, other_apps, shared_project, get_project_cache())
     sel_idx = 0
     options = {}
     for idx, proj in enumerate(projects):
         if selected_project and proj.id == selected_project.id:
             sel_idx = idx
-        options[idx] = proj.name
+        option_str = f"{proj.name} ({proj.application}){'- 📢Public' if proj.public else ''}"
+        if not proj.public and proj.owner.lower() != get_user_email().lower():
+            option_str += " - 🤝Shared"
+        options[idx] = option_str
     return options, projects, sel_idx
 
 
 def on_project_select():
     proj_idx = get_state("project_select")
     include_public = bool(get_state("include_public_projects", False))
     include_other_apps = bool(get_state("include_other_apps", False))
@@ -377,14 +380,21 @@
     if proj_idx is not None and proj_idx > -1:
         selected_project = projects[proj_idx] if proj_idx != -1 else None
         set_selected_project(selected_project)
     else:
         set_selected_project(None)
 
 
+def project_filters():
+    with st.expander("Project Filters"):
+        st.checkbox("Public projects", value=False, key="include_public_projects")
+        st.checkbox("Other Apps", value=True, key="include_other_apps")
+        st.checkbox("Shared projects", value=True, key="include_shared_projects")
+
+
 def project_selector(
     header_text: Optional[str] = "Projects",
     select_box_label="Select Project",
     null_option="-- Select Project --",
     st_context=st.sidebar,
     on_select_change=None,
     enable_filters=True,
@@ -393,40 +403,43 @@
     """UI to select and create projects
     Args:
         root_path (Path): The root Path to where the project folders live
     """
     selected_project = None
 
     if render_layout == "horizontal":
-        container1, container2 = st_context.columns(2)
+        layout_container1, layout_container2 = st_context.columns(2)
     else:
-        container1 = st_context.container()
-        container2 = st_context.container()
+        layout_container1 = st_context.container()
+        layout_container2 = st_context.container()
 
     if header_text is not None:
         st_context.subheader(header_text)
     include_public = bool(get_state("include_public_projects", False))
     include_other_apps = bool(get_state("include_other_apps", False))
+    include_shared_projects = bool(get_state("include_shared_projects", False))
+
     if enable_filters:
-        with container2.expander("Project Filters"):
-            include_public = st.checkbox("Public projects", value=False, key="include_public_projects")
-            include_other_apps = st.checkbox("Other Apps", value=False, key="include_other_apps")
-    options, projects, sel_idx = get_proj_options(include_public, include_other_apps, get_project_cache())
+        with layout_container2:
+            project_filters()
+    options, projects, sel_idx = get_proj_options(
+        include_public, include_other_apps, include_shared_projects, cache_id=get_project_cache()
+    )
     proj_options = {}
 
     # accomodate the null option if one is provided
     if null_option is not None:
         proj_options = {-1: null_option}
         sel_idx = sel_idx + 1
 
     if options is not None:
         proj_options = {**proj_options, **options}
 
     if len(proj_options) > 0:
-        proj_idx = container1.selectbox(
+        proj_idx = layout_container1.selectbox(
             select_box_label,
             key="project_select",
             index=sel_idx,
             on_change=on_select_change,
             options=proj_options.keys(),
             format_func=lambda x: proj_options[x],
         )
@@ -566,28 +579,28 @@
 
     if folder_success_message:
         st.success(folder_success_message)
     if folder_warning_message:
         st.warning(folder_warning_message)
 
     if render_layout == "horizontal":
-        container1, container2 = st_context.columns(2)
+        layout_container1, layout_container2 = st_context.columns(2)
     else:
-        container1 = st_context.container()
-        container2 = st_context.container()
+        layout_container1 = st_context.container()
+        layout_container2 = st_context.container()
 
     folders_dict = project.get_folders_map()
-    folder = container1.selectbox(
+    folder = layout_container1.selectbox(
         folder_select_text,
         options=folders_dict.keys(),
         format_func=lambda x: folders_dict[x],
     )
     path = project.get_folder_path(folder) if folder else None
     if path is not None and folder is not None:
-        row = container1.expander("Folder Actions", expanded=expand_folder_actions)
+        row = layout_container1.expander("Folder Actions", expanded=expand_folder_actions)
 
         state = _state_name(str(project.id), folder)
         if state not in st.session_state:
             st.session_state[state] = 0
 
         if allow_upload and has_project_write_access(project):
             if auto_parse_csv:
@@ -676,110 +689,122 @@
                 set_state(
                     ProjectState.FILE_SUCCESS_MESSAGE,
                     "".join([f"> 1. {msg} \n" for msg in upload_messages]),
                 )
                 st.experimental_rerun()
 
         if render_layout == "compact":
-            folder_container1 = row.container()
-            folder_container2 = row.container()
-            folder_container3 = row.container()
+            folder_add_sub_text_container = row.container()
+            folder_add_sub_button_container = row.container()
+            folder_delete_container = row.container()
 
         else:
-            folder_container1, folder_container2, folder_container3 = row.columns([4, 1, 1])
-            folder_container2.markdown("#")
-            folder_container3.markdown("#")
+            (
+                folder_add_sub_text_container,
+                folder_add_sub_button_container,
+                folder_delete_container,
+            ) = row.columns([4, 1, 1])
+            folder_add_sub_button_container.markdown("#")
+            folder_delete_container.markdown("#")
 
         if allow_folder_add:
-            folder_container1.text_input(
+            folder_add_sub_text_container.text_input(
                 "Add sub folders (use ',' to separate multiple folders and '/' to separate levels) ",
                 key="add_project_folder_name",
                 help="All folders are created relative to the project root. "
                 + "Create multiple folders at once by using ',' as a separator, folders can be "
                 + "multiple levels deep using '/' e.g. folder1/subfolder1, folder1/subfolder22",
                 placeholder="folder1/subfolder1, folder1/subfolder2",
             )
-            folder_container2.button(
+            folder_add_sub_button_container.button(
                 label="Add Folders",
                 help="Create new folder(s)",
                 on_click=add_folders,
             )
 
         if allow_delete and folder != "/":
-            folder_container3.button(
+            folder_delete_container.button(
                 "Delete Selected",
                 key=f"{key_prefix}folder_delete_btn",
                 on_click=submit_delete_folder,
                 args=(folder,),
             )
 
-        files = project.get_files_in_folder(folder, include_subfolders=False)
+        files = project.get_files_in_folder(folder, include_subfolders=True)
         if files is not None and len(files) > 0:
-            selected_key = container2.selectbox(
+            selected_key = layout_container2.selectbox(
                 "Select File",
                 options=files.keys(),
                 key=f"{key_prefix}file_manager_file_select",
             )
             selected_file = files[selected_key] if selected_key in files else None
             if selected_file is not None and selected_key is not None:
-                row = container2.expander("File Actions", expanded=expand_file_actions)
+                row = layout_container2.expander("File Actions", expanded=expand_file_actions)
                 if len(selected_key) > 30:
                     row.caption(selected_key)
 
                 if render_layout == "compact":
-                    file_container0 = row.container()
-                    file_container1, file_container2 = row.columns([5, 3])
-                    file_container3 = row.container()
-                    file_container4 = row.container()
-                    file_container5 = row.container()
+                    file_preview_container = row.container()
+                    file_prepare_container, file_download_container = row.columns([5, 3])
+                    file_download_container = row.container()
+                    file_rename_button_container = row.container()
+                    file_delete_container = row.container()
 
                 else:
-                    file_container0, file_container1, file_container2 = row.columns([1, 1, 1])
-                    file_container3, file_container4, file_container5 = row.columns([2, 1, 1])
-                    file_container4.markdown("#")
-                    file_container5.markdown("#")
+                    (
+                        file_preview_container,
+                        file_prepare_container,
+                        file_download_container,
+                    ) = row.columns([1, 1, 1])
+                    (
+                        file_rename_text_container,
+                        file_rename_button_container,
+                        file_delete_container,
+                    ) = row.columns([2, 1, 1])
+                    file_rename_button_container.markdown("#")
+                    file_delete_container.markdown("#")
 
                 # options = []
                 if allow_delete:
-                    file_container5.button(
+                    file_delete_container.button(
                         "Delete Selected",
                         key=f"{key_prefix}file_delete_btn",
                         on_click=submit_delete_file,
                         args=(selected_file,),
                     )
                 if selected_key.lower().endswith((".zip", ".csv", ".geojson", ".gpkg", ".feather", ".xlsx")):
-                    preview_frame = file_container0.button(
+                    preview_frame = file_preview_container.button(
                         "Preview Frame",
                         key=f"{key_prefix}file_manager_preview_frame",
                     )
                     if preview_frame:
                         with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
                             st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
                 if selected_key.lower().endswith((".json", ".yml", ".yaml", ".toml", ".md", ".txt")) and (
-                    preview_frame := file_container0.button(
+                    preview_frame := file_preview_container.button(
                         "Preview File",
                         key=f"{key_prefix}file_manager_preview_file",
                     )
                 ):
                     with st.expander(f"**File Viewer:** {selected_file.name}", expanded=True):
                         code_format = CODE_FORMAT_MAPPING.get(selected_key.lower().split(".")[-1])
                         if code_format is None:
                             st.write(get_string_preview(selected_file))
                         else:
                             st.code(
                                 get_string_preview(selected_file),
                                 language=code_format,
                             )
-                if file_container1.checkbox(
+                if file_prepare_container.checkbox(
                     "Prepare Download",
                     key=f"{key_prefix}file_manager_download_chbx",
                 ):
                     file_data = storage_client().get_file(selected_file.path)
 
-                    file_container2.download_button(
+                    file_download_container.download_button(
                         "Download",
                         file_data,
                         selected_file.name,
                         key=f"{key_prefix}file_manager_download_button",
                     )
                 if allow_replace and (
                     uploaded_replace_file := row.file_uploader(
@@ -796,30 +821,30 @@
                     _update_key(key_prefix, True)
                     set_state(
                         ProjectState.FILE_SUCCESS_MESSAGE,
                         f"Contents of file: **'{selected_file.path}'** was succesfully replaced",
                     )
                     st.experimental_rerun()
                 if allow_file_rename:
-                    file_container3.text_input(
+                    file_rename_text_container.text_input(
                         "Rename file as:",
                         key="rename_project_file_name",
                         help="Selected file will be renamed to this value when 'Rename Selected' is clicked",
                         placeholder="New file name",
                     )
-                    file_container4.button(
+                    file_rename_button_container.button(
                         label="Rename Selected",
                         help="Rename File",
                         on_click=rename_file,
                         args=(selected_file,),
                     )
 
         else:
-            container2.markdown("##")
-            container2.info("No files in selected folder")
+            layout_container2.markdown("##")
+            layout_container2.info("No files in selected folder")
 
         state_reset()
     return path, folder
 
 
 def get_projects_data(projects):
     selected_project = get_selected_project()
@@ -903,17 +928,16 @@
         filter_container = st_context.container()
         grid_container = st_context.container()
         select_container = st_context.container()
 
         add_container = st_context.container()
         save_container, delete_container = st_context.columns([1, 1])
 
-    with filter_container.expander("Project Filters"):
-        st.checkbox("Public projects", value=False, key="include_public_projects")
-        st.checkbox("Other Apps", value=False, key="include_other_apps")
+    with filter_container:
+        project_filters()
 
     with select_container:
         project, projects = project_selector(
             header_text=None,
             null_option=null_option,
             select_box_label="Select Project",
             st_context=select_container,  # type: ignore
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xt_st_common-0.8.3/src/xt_st_common/project_models.py` & `xt_st_common-0.8.4/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/xt_st_common/session.py` & `xt_st_common-0.8.4/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/xt_st_common/storage.py` & `xt_st_common-0.8.4/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/src/xt_st_common/utils.py` & `xt_st_common-0.8.4/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.3/PKG-INFO` & `xt_st_common-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.8.3
+Version: 0.8.4
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.23.1)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.8.3
+# XT-STREAMLIT - 0.8.4
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

