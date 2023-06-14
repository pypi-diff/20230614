# Comparing `tmp/ipywidgets_bokeh-1.4.0.dev3.tar.gz` & `tmp/ipywidgets_bokeh-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_bokeh-1.4.0.dev3.tar", last modified: Sun Apr 30 09:50:22 2023, max compression
+gzip compressed data, was "ipywidgets_bokeh-1.5.0.tar", last modified: Wed Jun 14 18:16:13 2023, max compression
```

## Comparing `ipywidgets_bokeh-1.4.0.dev3.tar` & `ipywidgets_bokeh-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.175346 ipywidgets_bokeh-1.4.0.dev3/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1494 2020-01-09 14:03:17.000000 ipywidgets_bokeh-1.4.0.dev3/LICENSE.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      184 2021-10-05 19:15:23.000000 ipywidgets_bokeh-1.4.0.dev3/MANIFEST.in
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-30 09:50:22.175346 ipywidgets_bokeh-1.4.0.dev3/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      511 2020-07-10 18:26:09.000000 ipywidgets_bokeh-1.4.0.dev3/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.155346 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       58 2023-04-30 09:47:45.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        3 2019-12-19 13:15:23.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/bokeh.ext.json
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.159345 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)   432832 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3529 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)  3042068 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/ipywidgets_bokeh.js
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.175346 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       55 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/index.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      591 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/index.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      103 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/loader.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1668 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/loader.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1290 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     7924 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       48 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/webpack.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      292 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/webpack.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1221 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4034 2023-04-30 09:49:00.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4480 2023-04-30 09:47:48.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/kernel.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1222 2023-04-30 09:47:55.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/package.json
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1243 2023-03-29 21:38:08.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/widget.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-30 09:50:22.159345 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      900 2023-04-30 09:50:22.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       51 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-04-30 09:50:21.000000 ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      106 2023-04-30 09:50:22.179345 ipywidgets_bokeh-1.4.0.dev3/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1880 2023-04-30 09:47:57.000000 ipywidgets_bokeh-1.4.0.dev3/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-06-14 18:16:13.171538 ipywidgets_bokeh-1.5.0/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1494 2020-01-09 14:03:17.000000 ipywidgets_bokeh-1.5.0/LICENSE.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      184 2021-10-05 19:15:23.000000 ipywidgets_bokeh-1.5.0/MANIFEST.in
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1406 2023-06-14 18:16:13.171538 ipywidgets_bokeh-1.5.0/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      511 2020-07-10 18:26:09.000000 ipywidgets_bokeh-1.5.0/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-06-14 18:16:13.155538 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       53 2023-06-14 17:43:17.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        3 2019-12-19 13:15:23.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/bokeh.ext.json
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-06-14 18:16:13.163538 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)   432832 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3529 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)  3042267 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/ipywidgets_bokeh.js
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-06-14 18:16:13.171538 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       55 2023-06-14 18:15:02.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/index.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      591 2023-06-14 18:15:02.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/index.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      103 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/loader.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1668 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/loader.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1290 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/manager.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     8389 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/manager.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       48 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/webpack.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      292 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/webpack.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1221 2023-06-14 18:15:02.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/widget.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4034 2023-06-14 18:15:01.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/widget.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4475 2023-06-14 17:43:22.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/kernel.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1216 2023-06-14 17:43:36.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/package.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1295 2023-06-14 17:35:36.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/widget.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-06-14 18:16:13.163538 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1406 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      924 2023-06-14 18:16:13.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      145 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-06-14 18:16:12.000000 ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      106 2023-06-14 18:16:13.171538 ipywidgets_bokeh-1.5.0/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2066 2023-06-14 17:43:41.000000 ipywidgets_bokeh-1.5.0/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-06-14 18:16:13.171538 ipywidgets_bokeh-1.5.0/tests/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1749 2023-06-14 17:35:36.000000 ipywidgets_bokeh-1.5.0/tests/test_anywidget.py
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/LICENSE.txt` & `ipywidgets_bokeh-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/PKG-INFO` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ipywidgets_bokeh
-Version: 1.4.0.dev3
+Name: ipywidgets-bokeh
+Version: 1.5.0
 Summary: Allows embedding of Jupyter widgets in Bokeh layouts.
 Home-page: https://github.com/bokeh/ipywidgets_bokeh
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,13 +15,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 ipywidgets_bokeh
 ================
 
 Support for using ipywidgets within [Bokeh](https://bokeh.org). Ipywidgets are normally used in Jupyter notebooks, but this project allows them to be embedded into a Bokeh application so that they can be used alongside and with Bokeh-based plots and Bokeh widgets.  See the separate [jupyter_bokeh](https://github.com/bokeh/jupyter_bokeh) library for support for using Bokeh plots and widgets in Jupyter and ipywidgets (the opposite case from what ipywidgets_bokeh supports).
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/ipywidgets_bokeh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -88163,33 +88163,38 @@
                     name: "bokeh_kernel",
                     id: "" + Ip++
                 };
                 this.kernel = this.kernel_manager.connectTo({
                     model: r,
                     handleComms: !0
                 }), this.kernel.registerCommTarget(this.comm_target_name, ((e, t) => {
-                    const n = this._model_objs.get(t.content.comm_id);
-                    if (null != n && !n.comm_live) {
-                        const t = new xt.services.Comm(e);
-                        this._attach_comm(t, n)
-                    }
-                    this._model_objs.delete(t.content.comm_id)
+                    const n = this._model_objs.get(t.content.comm_id),
+                        r = new xt.services.Comm(e);
+                    null == n && this.handle_comm_open(r, t).then((t => {
+                        if (null != t && !t.comm_live) {
+                            const n = new xt.services.Comm(e);
+                            this._attach_comm(n, t)
+                        }
+                    })), null == n || n.comm_live || this._attach_comm(r, n), this._model_objs.delete(t.content.comm_id)
                 }))
             }
             _attach_comm(e, t) {
                 t.comm = e, e.on_close(t._handle_comm_closed.bind(t)), e.on_msg(t._handle_comm_msg.bind(t)), t.comm_live = !0
             }
             async render(e, t) {
                 const {
                     spec: n,
                     state: r
                 } = e, i = r.state;
                 for (const [e, t] of(0, Dp.entries)(i)) this._known_models.set(e, t);
                 try {
                     const e = await this.set_state(r);
+                    await this.set_state(Object.assign(Object.assign({}, r), {
+                        state: r.full_state
+                    }));
                     for (const t of e) {
                         if (this._model_objs.has(t.model_id)) continue;
                         const e = await this._create_comm(this.comm_target_name, t.model_id);
                         this._attach_comm(e, t), this._model_objs.set(t.model_id, t), t.once("comm:close", (() => {
                             this._model_objs.delete(t.model_id)
                         }))
                     }
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/index.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/index.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/loader.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/loader.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.d.ts` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/manager.d.ts`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/manager.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/manager.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -118,16 +118,24 @@
         };
         this.kernel = this.kernel_manager.connectTo({
             model: kernel_model,
             handleComms: true
         });
         this.kernel.registerCommTarget(this.comm_target_name, (comm, msg) => {
             const model = this._model_objs.get(msg.content.comm_id);
+            const comm_wrapper = new shims.services.Comm(comm);
+            if (model == null) {
+                this.handle_comm_open(comm_wrapper, msg).then((model) => {
+                    if (model != null && !model.comm_live) {
+                        const comm_wrapper = new shims.services.Comm(comm);
+                        this._attach_comm(comm_wrapper, model);
+                    }
+                });
+            }
             if (model != null && !model.comm_live) {
-                const comm_wrapper = new shims.services.Comm(comm);
                 this._attach_comm(comm_wrapper, model);
             }
             this._model_objs.delete(msg.content.comm_id);
         });
     }
     _attach_comm(comm, model) {
         model.comm = comm;
@@ -143,14 +151,17 @@
         } = bundle;
         const new_models = state.state;
         for (const [id, new_model] of entries(new_models)) {
             this._known_models.set(id, new_model);
         }
         try {
             const models = await this.set_state(state);
+            await this.set_state(Object.assign(Object.assign({}, state), {
+                state: state.full_state
+            }));
             for (const model of models) {
                 if (this._model_objs.has(model.model_id))
                     continue;
                 const comm = await this._create_comm(this.comm_target_name, model.model_id);
                 this._attach_comm(comm, model);
                 this._model_objs.set(model.model_id, model);
                 model.once("comm:close", () => {
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.d.ts` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/widget.d.ts`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/dist/lib/widget.js` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/dist/lib/widget.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/kernel.py` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     def flush(self, *args):
         pass
 
 
 class BokehKernel(ipykernel.kernelbase.Kernel):
     implementation = 'ipython'
-    implementation_version = '1.4.0.dev3'
+    implementation_version = '1.5.0'
     banner = 'banner'
 
     shell_stream = Any(ShellStream(), allow_none=True)
 
     def __init__(self):
         super(BokehKernel, self).__init__()
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/package.json` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.5.0'"}*

```diff
@@ -37,9 +37,9 @@
         "build": "tsc && webpack --mode=production",
         "clean": "rimraf dist",
         "dev": "tsc; webpack --mode=development",
         "lint": "eslint -c eslint.json src/**/*.ts",
         "prepack": "npm run clean && npm run build",
         "test": "echo 'TODO'"
     },
-    "version": "1.4.0-dev.3"
+    "version": "1.5.0"
 }
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh/widget.py` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh/widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,10 +31,11 @@
 
     bundle = Any()
     cdn = String(default="https://unpkg.com")
 
     def __init__(self, *, widget: Widget, **kwargs):
         super().__init__(**kwargs)
         spec = widget.get_view_spec()
-        state = Widget.get_manager_state(widgets=[])
-        state["state"] = embed.dependency_state([widget], drop_defaults=True)
+        state = Widget.get_manager_state(widgets=[widget])
+        state["full_state"] = state["state"]
+        state["state"] = embed.dependency_state([widget], drop_defaults=False)
         self.bundle = dict(spec=spec, state=state)
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/PKG-INFO` & `ipywidgets_bokeh-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ipywidgets-bokeh
-Version: 1.4.0.dev3
+Name: ipywidgets_bokeh
+Version: 1.5.0
 Summary: Allows embedding of Jupyter widgets in Bokeh layouts.
 Home-page: https://github.com/bokeh/ipywidgets_bokeh
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,13 +15,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 ipywidgets_bokeh
 ================
 
 Support for using ipywidgets within [Bokeh](https://bokeh.org). Ipywidgets are normally used in Jupyter notebooks, but this project allows them to be embedded into a Bokeh application so that they can be used alongside and with Bokeh-based plots and Bokeh widgets.  See the separate [jupyter_bokeh](https://github.com/bokeh/jupyter_bokeh) library for support for using Bokeh plots and widgets in Jupyter and ipywidgets (the opposite case from what ipywidgets_bokeh supports).
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/ipywidgets_bokeh.egg-info/SOURCES.txt` & `ipywidgets_bokeh-1.5.0/ipywidgets_bokeh.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 ipywidgets_bokeh/dist/lib/loader.d.ts
 ipywidgets_bokeh/dist/lib/loader.js
 ipywidgets_bokeh/dist/lib/manager.d.ts
 ipywidgets_bokeh/dist/lib/manager.js
 ipywidgets_bokeh/dist/lib/webpack.d.ts
 ipywidgets_bokeh/dist/lib/webpack.js
 ipywidgets_bokeh/dist/lib/widget.d.ts
-ipywidgets_bokeh/dist/lib/widget.js
+ipywidgets_bokeh/dist/lib/widget.js
+tests/test_anywidget.py
```

### Comparing `ipywidgets_bokeh-1.4.0.dev3/setup.py` & `ipywidgets_bokeh-1.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,19 +25,27 @@
             os.chdir("..")
 
 install_requires = [
     "bokeh ==3.*", # TODO 3.2.dev1
     "ipywidgets ==8.*",
     "ipykernel ==6.*,!=6.18.0", # until ipywidgets 8.0.6
 ]
+dev_dependencies = [
+    "anywidget>=0.3.0",
+    "panel>=1.0.4",
+    "pytest>=7.3.1",
+    "pytest-cov>=4.1.0",
+    "pytest-playwright>=0.3.3",
+]
 
 setup_args = dict(
     name="ipywidgets_bokeh",
-    version="1.4.0.dev3",
+    version="1.5.0",
     install_requires=install_requires,
+    extras_require={"dev": dev_dependencies},
     python_requires=">=3.9",
     description="Allows embedding of Jupyter widgets in Bokeh layouts.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bokeh Team",
     author_email="info@bokeh.org",
     license="BSD-3-Clause",
```

