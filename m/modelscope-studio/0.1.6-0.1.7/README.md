# Comparing `tmp/modelscope_studio-0.1.6.tar.gz` & `tmp/modelscope_studio-0.1.7.tar.gz`

## Comparing `modelscope_studio-0.1.6.tar` & `modelscope_studio-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/__init__.py
--rw-r--r--   0        0        0    18957 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/__init__.py
--rw-r--r--   0        0        0    43763 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/__init__.pyi
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/llm_thinking_presets.py
--rw-r--r--   0        0        0  1520165 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/component/index-9933f53a.js
--rw-r--r--   0        0        0  3750909 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/component/index.js
--rw-r--r--   0        0        0  1495878 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/component/style.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/example/index.js
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/example/style.css
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/__init__.py
--rw-r--r--   0        0        0    16142 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/__init__.pyi
--rw-r--r--   0        0        0  1520165 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/component/index-9933f53a.js
--rw-r--r--   0        0        0  3656211 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/component/index.js
--rw-r--r--   0        0        0  1488422 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/component/style.css
--rw-r--r--   0        0        0  1520165 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/example/index-9933f53a.js
--rw-r--r--   0        0        0  3598161 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/example/index.js
--rw-r--r--   0        0        0  1475562 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/example/style.css
--rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/__init__.py
--rw-r--r--   0        0        0   123856 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/__init__.pyi
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0  1848466 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/index.js
--rw-r--r--   0        0        0    25070 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/style.css
--rw-r--r--   0        0        0    78109 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/wrapper-6f348d45-f837cf34.js
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/example/index.js
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/example/style.css
--rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/__init__.py
--rw-r--r--   0        0        0    39621 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/__init__.pyi
--rw-r--r--   0        0        0   203123 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/templates/component/index.js
--rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/templates/component/style.css
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/utils/__init__.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/backend/modelscope_studio/utils/process_links.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/LICENSE
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/README.md
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 modelscope_studio-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/__init__.py
+-rw-r--r--   0        0        0    18957 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/__init__.py
+-rw-r--r--   0        0        0    43763 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/__init__.pyi
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/llm_thinking_presets.py
+-rw-r--r--   0        0        0  1520165 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/component/index-9933f53a.js
+-rw-r--r--   0        0        0  3750909 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/component/index.js
+-rw-r--r--   0        0        0  1495878 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/component/style.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/example/index.js
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/example/style.css
+-rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Flow/__init__.pyi
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/__init__.py
+-rw-r--r--   0        0        0    16142 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/__init__.pyi
+-rw-r--r--   0        0        0  1520165 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/component/index-9933f53a.js
+-rw-r--r--   0        0        0  3656211 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/component/index.js
+-rw-r--r--   0        0        0  1488422 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/component/style.css
+-rw-r--r--   0        0        0  1520165 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/example/index-9933f53a.js
+-rw-r--r--   0        0        0  3598161 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/example/index.js
+-rw-r--r--   0        0        0  1475562 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/example/style.css
+-rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/__init__.py
+-rw-r--r--   0        0        0   123856 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/__init__.pyi
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0  1848470 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/index.js
+-rw-r--r--   0        0        0    25070 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/style.css
+-rw-r--r--   0        0        0    78109 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/wrapper-6f348d45-f837cf34.js
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/example/index.js
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/example/style.css
+-rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/__init__.py
+-rw-r--r--   0        0        0    39621 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/__init__.pyi
+-rw-r--r--   0        0        0   203123 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/templates/component/index.js
+-rw-r--r--   0        0        0    21002 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/templates/component/style.css
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/utils/__init__.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/backend/modelscope_studio/utils/process_links.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/README.md
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 modelscope_studio-0.1.7/PKG-INFO
```

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/__init__.py` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/__init__.py`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/__init__.pyi` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/component/index-9933f53a.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/component/index-9933f53a.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/component/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/component/style.css` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Chatbot/templates/example/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Chatbot/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/__init__.py` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/__init__.pyi` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/__init__.pyi`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/component/index-9933f53a.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/component/index-9933f53a.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/component/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/component/style.css` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/example/index-9933f53a.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/example/index-9933f53a.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/example/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/Markdown/templates/example/style.css` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/Markdown/templates/example/style.css`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/__init__.py` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/__init__.py`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/__init__.pyi` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/__init__.pyi`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2023,31 +2023,31 @@
             }
 
             function Qt(un, ln, Xt, Ht = null) {
                 let Dt, Bt;
                 if (typeof un == "number")
                     Dt = un, Bt = en.unnamed_endpoints[Dt];
                 else {
-                    const jn = un.replace(/^\//, "");
-                    Dt = Vt[jn], Bt = en.named_endpoints[un.trim()];
+                    const En = un.replace(/^\//, "");
+                    Dt = Vt[En], Bt = en.named_endpoints[un.trim()];
                 }
                 if (typeof Dt != "number")
                     throw new Error(
                         "There is no endpoint matching that name of fn_index matching that number."
                     );
                 let Wt, Yt, on = jt.protocol ?? "ws";
                 const rn = typeof un == "number" ? "/predict" : un;
                 let mn, _n = null,
-                    Sn = !1;
+                    yn = !1;
                 const Cn = {};
                 let kn = "";
                 typeof window < "u" && (kn = new URLSearchParams(window.location.search).toString()), bt(`${jt.root}`, ln, Bt, wt).then(
-                    (jn) => {
+                    (En) => {
                         if (mn = {
-                                data: jn || [],
+                                data: En || [],
                                 event_data: Xt,
                                 fn_index: Dt,
                                 trigger_id: Ht
                             }, skip_queue(Dt, jt))
                             Pn({
                                 type: "status",
                                 endpoint: rn,
@@ -2057,49 +2057,49 @@
                                 time: /* @__PURE__ */ new Date()
                             }), ft(
                                 `${jt.root}/run${rn.startsWith("/") ? rn : `/${rn}`}${kn ? "?" + kn : ""}`, {
                                     ...mn,
                                     session_hash: At
                                 },
                                 wt
-                            ).then(([bn, xn]) => {
+                            ).then(([gn, xn]) => {
                                 const zn = Rt ? transform_output(
-                                    bn.data,
+                                    gn.data,
                                     Bt,
                                     jt.root,
                                     jt.root_url
-                                ) : bn.data;
+                                ) : gn.data;
                                 xn == 200 ? (Pn({
                                     type: "data",
                                     endpoint: rn,
                                     fn_index: Dt,
                                     data: zn,
                                     time: /* @__PURE__ */ new Date()
                                 }), Pn({
                                     type: "status",
                                     endpoint: rn,
                                     fn_index: Dt,
                                     stage: "complete",
-                                    eta: bn.average_duration,
+                                    eta: gn.average_duration,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 })) : Pn({
                                     type: "status",
                                     stage: "error",
                                     endpoint: rn,
                                     fn_index: Dt,
-                                    message: bn.error,
+                                    message: gn.error,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
-                            }).catch((bn) => {
+                            }).catch((gn) => {
                                 Pn({
                                     type: "status",
                                     stage: "error",
-                                    message: bn.message,
+                                    message: gn.message,
                                     endpoint: rn,
                                     fn_index: Dt,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             });
                         else if (on == "ws") {
@@ -2107,21 +2107,21 @@
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
                                 endpoint: rn,
                                 fn_index: Dt,
                                 time: /* @__PURE__ */ new Date()
                             });
-                            let bn = new URL(`${Mt}://${resolve_root(
+                            let gn = new URL(`${Mt}://${resolve_root(
                 Pt,
                 jt.path,
                 !0
               )}
 							/queue/join${kn ? "?" + kn : ""}`);
-                            Gt && bn.searchParams.set("__sign", Gt), Wt = new WebSocket(bn), Wt.onclose = (xn) => {
+                            Gt && gn.searchParams.set("__sign", Gt), Wt = new WebSocket(gn), Wt.onclose = (xn) => {
                                 xn.wasClean || Pn({
                                     type: "status",
                                     stage: "error",
                                     broken: !0,
                                     message: BROKEN_CONNECTION_MSG,
                                     queue: !0,
                                     endpoint: rn,
@@ -2134,15 +2134,15 @@
                                         type: On,
                                         status: Un,
                                         data: Gn
                                     } = handle_message(
                                         zn,
                                         Tt[Dt]
                                     );
-                                if (On === "update" && Un && !Sn)
+                                if (On === "update" && Un && !yn)
                                     Pn({
                                         type: "status",
                                         endpoint: rn,
                                         fn_index: Dt,
                                         time: /* @__PURE__ */ new Date(),
                                         ...Un
                                     }), Un.stage === "error" && Wt.close();
@@ -2152,15 +2152,15 @@
                                         session_hash: At
                                     }));
                                     return;
                                 } else
                                     On === "data" ? Wt.send(JSON.stringify({
                                         ...mn,
                                         session_hash: At
-                                    })) : On === "complete" ? Sn = Un : On === "log" ? Pn({
+                                    })) : On === "complete" ? yn = Un : On === "log" ? Pn({
                                         type: "log",
                                         log: Gn.log,
                                         level: Gn.level,
                                         endpoint: rn,
                                         fn_index: Dt
                                     }) : On === "generating" && Pn({
                                         type: "status",
@@ -2178,18 +2178,18 @@
                                         Gn.data,
                                         Bt,
                                         jt.root,
                                         jt.root_url
                                     ) : Gn.data,
                                     endpoint: rn,
                                     fn_index: Dt
-                                }), Sn && (Pn({
+                                }), yn && (Pn({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
-                                    ...Sn,
+                                    ...yn,
                                     stage: Un == null ? void 0 : Un.stage,
                                     queue: !0,
                                     endpoint: rn,
                                     fn_index: Dt
                                 }), Wt.close()));
                             }, semiver(jt.version || "2.0.0", "3.6") < 0 && addEventListener(
                                 "open",
@@ -2206,28 +2206,28 @@
                                 fn_index: Dt,
                                 time: /* @__PURE__ */ new Date()
                             });
                             var An = new URLSearchParams({
                                 fn_index: Dt.toString(),
                                 session_hash: At
                             }).toString();
-                            let bn = new URL(
+                            let gn = new URL(
                                 `${jt.root}/queue/join?${kn ? kn + "&" : ""}${An}`
                             );
-                            Yt = it(bn), Yt.onmessage = async function(xn) {
+                            Yt = it(gn), Yt.onmessage = async function(xn) {
                                 const zn = JSON.parse(xn.data),
                                     {
                                         type: On,
                                         status: Un,
                                         data: Gn
                                     } = handle_message(
                                         zn,
                                         Tt[Dt]
                                     );
-                                if (On === "update" && Un && !Sn)
+                                if (On === "update" && Un && !yn)
                                     Pn({
                                         type: "status",
                                         endpoint: rn,
                                         fn_index: Dt,
                                         time: /* @__PURE__ */ new Date(),
                                         ...Un
                                     }), Un.stage === "error" && Yt.close();
@@ -2247,15 +2247,15 @@
                                         message: BROKEN_CONNECTION_MSG,
                                         queue: !0,
                                         endpoint: rn,
                                         fn_index: Dt,
                                         time: /* @__PURE__ */ new Date()
                                     }), Yt.close());
                                 } else
-                                    On === "complete" ? Sn = Un : On === "log" ? Pn({
+                                    On === "complete" ? yn = Un : On === "log" ? Pn({
                                         type: "log",
                                         log: Gn.log,
                                         level: Gn.level,
                                         endpoint: rn,
                                         fn_index: Dt
                                     }) : On === "generating" && Pn({
                                         type: "status",
@@ -2273,18 +2273,18 @@
                                         Gn.data,
                                         Bt,
                                         jt.root,
                                         jt.root_url
                                     ) : Gn.data,
                                     endpoint: rn,
                                     fn_index: Dt
-                                }), Sn && (Pn({
+                                }), yn && (Pn({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
-                                    ...Sn,
+                                    ...yn,
                                     stage: Un == null ? void 0 : Un.stage,
                                     queue: !0,
                                     endpoint: rn,
                                     fn_index: Dt
                                 }), Yt.close()));
                             };
                         } else
@@ -2297,15 +2297,15 @@
                                 time: /* @__PURE__ */ new Date()
                             }), ft(
                                 `${jt.root}/queue/join?${kn}`, {
                                     ...mn,
                                     session_hash: At
                                 },
                                 wt
-                            ).then(([bn, xn]) => {
+                            ).then(([gn, xn]) => {
                                 if (xn === 503)
                                     Pn({
                                         type: "status",
                                         stage: "error",
                                         message: QUEUE_FULL_MSG,
                                         queue: !0,
                                         endpoint: rn,
@@ -2319,37 +2319,37 @@
                                         message: BROKEN_CONNECTION_MSG,
                                         queue: !0,
                                         endpoint: rn,
                                         fn_index: Dt,
                                         time: /* @__PURE__ */ new Date()
                                     });
                                 else {
-                                    _n = bn.event_id;
+                                    _n = gn.event_id;
                                     let zn = async function(On) {
                                         try {
                                             const {
                                                 type: Un,
                                                 status: Gn,
                                                 data: Zn
                                             } = handle_message(
                                                 On,
                                                 Tt[Dt]
                                             );
                                             if (Un == "heartbeat")
                                                 return;
-                                            if (Un === "update" && Gn && !Sn)
+                                            if (Un === "update" && Gn && !yn)
                                                 Pn({
                                                     type: "status",
                                                     endpoint: rn,
                                                     fn_index: Dt,
                                                     time: /* @__PURE__ */ new Date(),
                                                     ...Gn
                                                 });
                                             else if (Un === "complete")
-                                                Sn = Gn;
+                                                yn = Gn;
                                             else if (Un == "unexpected_error")
                                                 console.error("Unexpected error", Gn == null ? void 0 : Gn.message), Pn({
                                                     type: "status",
                                                     stage: "error",
                                                     message: (Gn == null ? void 0 : Gn.message) || "An Unexpected Error Occurred!",
                                                     queue: !0,
                                                     endpoint: rn,
@@ -2382,18 +2382,18 @@
                                                     Zn.data,
                                                     Bt,
                                                     jt.root,
                                                     jt.root_url
                                                 ) : Zn.data,
                                                 endpoint: rn,
                                                 fn_index: Dt
-                                            }), Sn && Pn({
+                                            }), yn && Pn({
                                                 type: "status",
                                                 time: /* @__PURE__ */ new Date(),
-                                                ...Sn,
+                                                ...yn,
                                                 stage: Gn == null ? void 0 : Gn.stage,
                                                 queue: !0,
                                                 endpoint: rn,
                                                 fn_index: Dt
                                             })), ((Gn == null ? void 0 : Gn.stage) === "complete" || (Gn == null ? void 0 : Gn.stage) === "error") && Ft[_n] && delete Ft[_n];
                                         } catch (Un) {
                                             console.error("Unexpected client exception", Un), Pn({
@@ -2411,48 +2411,48 @@
                                         (On) => zn(On)
                                     ), delete It[_n]), Ft[_n] = zn, zt.add(_n), Ot || Zt();
                                 }
                             }));
                     }
                 );
 
-                function Pn(jn) {
-                    const bn = Cn[jn.type] || [];
-                    bn == null || bn.forEach((xn) => xn(jn));
+                function Pn(En) {
+                    const gn = Cn[En.type] || [];
+                    gn == null || gn.forEach((xn) => xn(En));
                 }
 
-                function Mn(jn, An) {
-                    const bn = Cn,
-                        xn = bn[jn] || [];
-                    return bn[jn] = xn, xn == null || xn.push(An), {
+                function Mn(En, An) {
+                    const gn = Cn,
+                        xn = gn[En] || [];
+                    return gn[En] = xn, xn == null || xn.push(An), {
                         on: Mn,
                         off: Wn,
                         cancel: Rn,
-                        destroy: yn
+                        destroy: Fn
                     };
                 }
 
-                function Wn(jn, An) {
-                    const bn = Cn;
-                    let xn = bn[jn] || [];
-                    return xn = xn == null ? void 0 : xn.filter((zn) => zn !== An), bn[jn] = xn, {
+                function Wn(En, An) {
+                    const gn = Cn;
+                    let xn = gn[En] || [];
+                    return xn = xn == null ? void 0 : xn.filter((zn) => zn !== An), gn[En] = xn, {
                         on: Mn,
                         off: Wn,
                         cancel: Rn,
-                        destroy: yn
+                        destroy: Fn
                     };
                 }
                 async function Rn() {
-                    const jn = {
+                    const En = {
                         stage: "complete",
                         queue: !1,
                         time: /* @__PURE__ */ new Date()
                     };
-                    Sn = jn, Pn({
-                        ...jn,
+                    yn = En, Pn({
+                        ...En,
                         type: "status",
                         endpoint: rn,
                         fn_index: Dt
                     });
                     let An = {};
                     on === "ws" ? (Wt && Wt.readyState === 0 ? Wt.addEventListener("open", () => {
                         Wt.close();
@@ -2473,25 +2473,25 @@
                     } catch {
                         console.warn(
                             "The `/reset` endpoint could not be called. Subsequent endpoint results may be unreliable."
                         );
                     }
                 }
 
-                function yn() {
-                    for (const jn in Cn)
-                        Cn[jn].forEach((An) => {
-                            Wn(jn, An);
+                function Fn() {
+                    for (const En in Cn)
+                        Cn[En].forEach((An) => {
+                            Wn(En, An);
                         });
                 }
                 return {
                     on: Mn,
                     off: Wn,
                     cancel: Rn,
-                    destroy: yn
+                    destroy: Fn
                 };
             }
 
             function Zt() {
                 Ot = !0;
                 let un = new URLSearchParams({
                         session_hash: At
@@ -19654,67 +19654,67 @@
     var Ht = reactExports.useRef(!1);
 
     function Dt() {
         Qt(STATUS_NONE, !0), hn(null, !0);
     }
 
     function Bt(Rn) {
-        var yn = Xt();
-        if (!(Rn && !Rn.deadline && Rn.target !== yn)) {
-            var jn = Ht.current,
+        var Fn = Xt();
+        if (!(Rn && !Rn.deadline && Rn.target !== Fn)) {
+            var En = Ht.current,
                 An;
-            an === STATUS_APPEAR && jn ? An = It == null ? void 0 : It(yn, Rn) : an === STATUS_ENTER && jn ? An = Nt == null ? void 0 : Nt(yn, Rn) : an === STATUS_LEAVE && jn && (An = Ft == null ? void 0 : Ft(yn, Rn)), an !== STATUS_NONE && jn && An !== !1 && Dt();
+            an === STATUS_APPEAR && En ? An = It == null ? void 0 : It(Fn, Rn) : an === STATUS_ENTER && En ? An = Nt == null ? void 0 : Nt(Fn, Rn) : an === STATUS_LEAVE && En && (An = Ft == null ? void 0 : Ft(Fn, Rn)), an !== STATUS_NONE && En && An !== !1 && Dt();
         }
     }
     var Wt = useDomMotionEvents(Bt),
         Yt = _slicedToArray(Wt, 1),
         on = Yt[0],
         rn = function(Rn) {
-            var yn, jn, An;
+            var Fn, En, An;
             switch (Rn) {
                 case STATUS_APPEAR:
-                    return yn = {}, _defineProperty(yn, STEP_PREPARE, Ct), _defineProperty(yn, STEP_START, Lt), _defineProperty(yn, STEP_ACTIVE, At), yn;
+                    return Fn = {}, _defineProperty(Fn, STEP_PREPARE, Ct), _defineProperty(Fn, STEP_START, Lt), _defineProperty(Fn, STEP_ACTIVE, At), Fn;
                 case STATUS_ENTER:
-                    return jn = {}, _defineProperty(jn, STEP_PREPARE, Rt), _defineProperty(jn, STEP_START, Pt), _defineProperty(jn, STEP_ACTIVE, Tt), jn;
+                    return En = {}, _defineProperty(En, STEP_PREPARE, Rt), _defineProperty(En, STEP_START, Pt), _defineProperty(En, STEP_ACTIVE, Tt), En;
                 case STATUS_LEAVE:
                     return An = {}, _defineProperty(An, STEP_PREPARE, Mt), _defineProperty(An, STEP_START, kt), _defineProperty(An, STEP_ACTIVE, Ot), An;
                 default:
                     return {};
             }
         },
         mn = reactExports.useMemo(function() {
             return rn(an);
         }, [an]),
         _n = useStepQueue(an, !_e, function(Rn) {
             if (Rn === STEP_PREPARE) {
-                var yn = mn[STEP_PREPARE];
-                return yn ? yn(Xt()) : SkipStep;
+                var Fn = mn[STEP_PREPARE];
+                return Fn ? Fn(Xt()) : SkipStep;
             }
             if (kn in mn) {
-                var jn;
-                hn(((jn = mn[kn]) === null || jn === void 0 ? void 0 : jn.call(mn, Xt(), null)) || null);
+                var En;
+                hn(((En = mn[kn]) === null || En === void 0 ? void 0 : En.call(mn, Xt(), null)) || null);
             }
             return kn === STEP_ACTIVE && (on(Xt()), wt > 0 && (clearTimeout(ln.current), ln.current = setTimeout(function() {
                 Bt({
                     deadline: !0
                 });
             }, wt))), kn === STEP_PREPARED && Dt(), DoStep;
         }),
-        Sn = _slicedToArray(_n, 2),
-        Cn = Sn[0],
-        kn = Sn[1],
+        yn = _slicedToArray(_n, 2),
+        Cn = yn[0],
+        kn = yn[1],
         Pn = isActive(kn);
     Ht.current = Pn, useIsomorphicLayoutEffect(function() {
         cn(it);
         var Rn = un.current;
         un.current = !0;
-        var yn;
-        !Rn && it && yt && (yn = STATUS_APPEAR), Rn && it && bt && (yn = STATUS_ENTER), (Rn && !it && xt || !Rn && $t && !it && xt) && (yn = STATUS_LEAVE);
-        var jn = rn(yn);
-        yn && (_e || jn[STEP_PREPARE]) ? (Qt(yn), Cn()) : Qt(STATUS_NONE);
+        var Fn;
+        !Rn && it && yt && (Fn = STATUS_APPEAR), Rn && it && bt && (Fn = STATUS_ENTER), (Rn && !it && xt || !Rn && $t && !it && xt) && (Fn = STATUS_LEAVE);
+        var En = rn(Fn);
+        Fn && (_e || En[STEP_PREPARE]) ? (Qt(Fn), Cn()) : Qt(STATUS_NONE);
     }, [it]), reactExports.useEffect(function() {
         (an === STATUS_APPEAR && !yt || // Cancel enter
             an === STATUS_ENTER && !bt || // Cancel leave
             an === STATUS_LEAVE && !xt) && Qt(STATUS_NONE);
     }, [yt, bt, xt]), reactExports.useEffect(function() {
         return function() {
             un.current = !1, clearTimeout(ln.current);
@@ -20055,64 +20055,64 @@
             breadcrumb: Bt,
             menu: Wt,
             pagination: Yt,
             input: on,
             textArea: rn,
             empty: mn,
             badge: _n,
-            radio: Sn,
+            radio: yn,
             rate: Cn,
             switch: kn,
             transfer: Pn,
             avatar: Mn,
             message: Wn,
             tag: Rn,
-            table: yn,
-            card: jn,
+            table: Fn,
+            card: En,
             tabs: An,
-            timeline: bn,
+            timeline: gn,
             timePicker: xn,
             upload: zn,
             notification: On,
             tree: Un,
             colorPicker: Gn,
             datePicker: Zn,
             rangePicker: Yn,
             flex: lr,
             wave: ur,
             dropdown: nr,
             warning: sr,
-            tour: Fn,
+            tour: Dn,
             floatButtonGroup: wn
-        } = _e, En = reactExports.useCallback((Kn, Jn) => {
+        } = _e, Sn = reactExports.useCallback((Kn, Jn) => {
             const {
                 prefixCls: gr
             } = _e;
             if (Jn)
                 return Jn;
             const rr = gr || Pt.getPrefixCls("");
             return Kn ? `${rr}-${Kn}` : rr;
-        }, [Pt.getPrefixCls, _e.prefixCls]), Dn = kt || Pt.iconPrefixCls || defaultIconPrefixCls, cr = ft || Pt.csp;
-        useResetIconStyle(Dn, cr);
+        }, [Pt.getPrefixCls, _e.prefixCls]), jn = kt || Pt.iconPrefixCls || defaultIconPrefixCls, cr = ft || Pt.csp;
+        useResetIconStyle(jn, cr);
         const Tn = useTheme(At, Pt.theme, {
-                prefixCls: En("")
+                prefixCls: Sn("")
             }),
             In = {
                 csp: cr,
                 autoInsertSpaceInButton: mt,
                 alert: gt,
                 anchor: bt,
                 locale: yt || Lt,
                 direction: xt,
                 space: wt,
                 virtual: $t,
                 popupMatchSelectWidth: Rt ?? Ct,
                 popupOverflow: Mt,
-                getPrefixCls: En,
-                iconPrefixCls: Dn,
+                getPrefixCls: Sn,
+                iconPrefixCls: jn,
                 theme: Tn,
                 segmented: Ot,
                 statistic: It,
                 spin: Nt,
                 calendar: Ft,
                 carousel: zt,
                 cascader: jt,
@@ -20135,37 +20135,37 @@
                 result: Ht,
                 slider: Dt,
                 breadcrumb: Bt,
                 menu: Wt,
                 pagination: Yt,
                 empty: mn,
                 badge: _n,
-                radio: Sn,
+                radio: yn,
                 rate: Cn,
                 switch: kn,
                 transfer: Pn,
                 avatar: Mn,
                 message: Wn,
                 tag: Rn,
-                table: yn,
-                card: jn,
+                table: Fn,
+                card: En,
                 tabs: An,
-                timeline: bn,
+                timeline: gn,
                 timePicker: xn,
                 upload: zn,
                 notification: On,
                 tree: Un,
                 colorPicker: Gn,
                 datePicker: Zn,
                 rangePicker: Yn,
                 flex: lr,
                 wave: ur,
                 dropdown: nr,
                 warning: sr,
-                tour: Fn,
+                tour: Dn,
                 floatButtonGroup: wn
             },
             Qn = Object.assign({}, Pt);
         Object.keys(In).forEach((Kn) => {
             In[Kn] !== void 0 && (Qn[Kn] = In[Kn]);
         }), PASSED_PROPS.forEach((Kn) => {
             const Jn = _e[Kn];
@@ -20173,58 +20173,58 @@
         });
         const or = useMemo(() => Qn, Qn, (Kn, Jn) => {
                 const gr = Object.keys(Kn),
                     rr = Object.keys(Jn);
                 return gr.length !== rr.length || gr.some((nn) => Kn[nn] !== Jn[nn]);
             }),
             Xn = reactExports.useMemo(() => ({
-                prefixCls: Dn,
+                prefixCls: jn,
                 csp: cr
-            }), [Dn, cr]);
+            }), [jn, cr]);
         let Vn = /* @__PURE__ */ reactExports.createElement(reactExports.Fragment, null, /* @__PURE__ */ reactExports.createElement(PropWarning, {
             dropdownMatchSelectWidth: Ct
         }), it);
         const hr = reactExports.useMemo(() => {
             var Kn, Jn, gr, rr;
             return merge$1(((Kn = localeValues.Form) === null || Kn === void 0 ? void 0 : Kn.defaultValidateMessages) || {}, ((gr = (Jn = or.locale) === null || Jn === void 0 ? void 0 : Jn.Form) === null || gr === void 0 ? void 0 : gr.defaultValidateMessages) || {}, ((rr = or.form) === null || rr === void 0 ? void 0 : rr.validateMessages) || {}, (_t == null ? void 0 : _t.validateMessages) || {});
         }, [or, _t == null ? void 0 : _t.validateMessages]);
         Object.keys(hr).length > 0 && (Vn = /* @__PURE__ */ reactExports.createElement(ValidateMessagesContext.Provider, {
             value: hr
         }, Vn)), yt && (Vn = /* @__PURE__ */ reactExports.createElement(LocaleProvider$1, {
             locale: yt,
             _ANT_MARK__: ANT_MARK
-        }, Vn)), (Dn || cr) && (Vn = /* @__PURE__ */ reactExports.createElement(IconContext.Provider, {
+        }, Vn)), (jn || cr) && (Vn = /* @__PURE__ */ reactExports.createElement(IconContext.Provider, {
             value: Xn
         }, Vn)), Et && (Vn = /* @__PURE__ */ reactExports.createElement(SizeContextProvider, {
             size: Et
         }, Vn)), Vn = /* @__PURE__ */ reactExports.createElement(MotionWrapper, null, Vn);
         const Nn = reactExports.useMemo(() => {
             const Kn = Tn || {},
                 {
                     algorithm: Jn,
                     token: gr,
                     components: rr,
                     cssVar: nn
                 } = Kn,
                 qt = __rest$i(Kn, ["algorithm", "token", "components", "cssVar"]),
                 dn = Jn && (!Array.isArray(Jn) || Jn.length > 0) ? createTheme(Jn) : defaultTheme,
-                gn = {};
+                vn = {};
             Object.entries(rr || {}).forEach(($n) => {
                 let [Ln, Hn] = $n;
                 const Bn = Object.assign({}, Hn);
-                "algorithm" in Bn && (Bn.algorithm === !0 ? Bn.theme = dn : (Array.isArray(Bn.algorithm) || typeof Bn.algorithm == "function") && (Bn.theme = createTheme(Bn.algorithm)), delete Bn.algorithm), gn[Ln] = Bn;
+                "algorithm" in Bn && (Bn.algorithm === !0 ? Bn.theme = dn : (Array.isArray(Bn.algorithm) || typeof Bn.algorithm == "function") && (Bn.theme = createTheme(Bn.algorithm)), delete Bn.algorithm), vn[Ln] = Bn;
             });
-            const vn = Object.assign(Object.assign({}, seedToken), gr);
+            const bn = Object.assign(Object.assign({}, seedToken), gr);
             return Object.assign(Object.assign({}, qt), {
                 theme: dn,
-                token: vn,
-                components: gn,
+                token: bn,
+                components: vn,
                 override: Object.assign({
-                    override: vn
-                }, gn),
+                    override: bn
+                }, vn),
                 cssVar: nn
             });
         }, [Tn]);
         return At && (Vn = /* @__PURE__ */ reactExports.createElement(DesignTokenContext.Provider, {
             value: Nn
         }, Vn)), or.warning && (Vn = /* @__PURE__ */ reactExports.createElement(WarningContext.Provider, {
             value: or.warning
@@ -22553,56 +22553,56 @@
         } = _e, It = __rest$f(_e, ["loading", "prefixCls", "type", "danger", "shape", "size", "styles", "disabled", "className", "rootClassName", "children", "icon", "ghost", "block", "htmlType", "classNames", "style"]), Nt = _t || "default", {
             getPrefixCls: Ft,
             autoInsertSpaceInButton: zt,
             direction: jt,
             button: Vt
         } = reactExports.useContext(ConfigContext), Gt = Ft("btn", bt), [cn, en, Kt] = useStyle$8(Gt), an = reactExports.useContext(DisabledContext$1), Qt = $t ?? an, Zt = reactExports.useContext(GroupSizeContext), Jt = reactExports.useMemo(() => getLoadingConfig(gt), [gt]), [pn, hn] = reactExports.useState(Jt.loading), [un, ln] = reactExports.useState(!1), Xt = composeRef(it, /* @__PURE__ */ reactExports.createRef()), Ht = reactExports.Children.count(Mt) === 1 && !Lt && !isUnBorderedButtonType(Nt);
         reactExports.useEffect(() => {
-            let jn = null;
-            Jt.delay > 0 ? jn = setTimeout(() => {
-                jn = null, hn(!0);
+            let En = null;
+            Jt.delay > 0 ? En = setTimeout(() => {
+                En = null, hn(!0);
             }, Jt.delay) : hn(Jt.loading);
 
             function An() {
-                jn && (clearTimeout(jn), jn = null);
+                En && (clearTimeout(En), En = null);
             }
             return An;
         }, [Jt]), reactExports.useEffect(() => {
             if (!Xt || !Xt.current || zt === !1)
                 return;
-            const jn = Xt.current.textContent;
-            Ht && isTwoCNChar(jn) ? un || ln(!0) : un && ln(!1);
+            const En = Xt.current.textContent;
+            Ht && isTwoCNChar(En) ? un || ln(!0) : un && ln(!1);
         }, [Xt]);
-        const Dt = (jn) => {
+        const Dt = (En) => {
                 const {
                     onClick: An
                 } = _e;
                 if (pn || Qt) {
-                    jn.preventDefault();
+                    En.preventDefault();
                     return;
                 }
-                An == null || An(jn);
+                An == null || An(En);
             },
             Bt = zt !== !1,
             {
                 compactSize: Wt,
                 compactItemClassnames: Yt
             } = useCompactItemContext(Gt, jt),
             on = {
                 large: "lg",
                 small: "sm",
                 middle: void 0
             },
-            rn = useSize((jn) => {
-                var An, bn;
-                return (bn = (An = xt ?? Wt) !== null && An !== void 0 ? An : Zt) !== null && bn !== void 0 ? bn : jn;
+            rn = useSize((En) => {
+                var An, gn;
+                return (gn = (An = xt ?? Wt) !== null && An !== void 0 ? An : Zt) !== null && gn !== void 0 ? gn : En;
             }),
             mn = rn && on[rn] || "",
             _n = pn ? "loading" : Lt,
-            Sn = omit(It, ["navigate"]),
+            yn = omit(It, ["navigate"]),
             Cn = cls(Gt, en, Kt, {
                 [`${Gt}-${Et}`]: Et !== "default" && Et,
                 [`${Gt}-${Nt}`]: Nt,
                 [`${Gt}-${mn}`]: mn,
                 [`${Gt}-icon-only`]: !Mt && Mt !== 0 && !!_n,
                 [`${Gt}-background-ghost`]: Pt && !isUnBorderedButtonType(Nt),
                 [`${Gt}-loading`]: pn,
@@ -22620,40 +22620,40 @@
                 style: Mn
             }, Lt) : /* @__PURE__ */ React.createElement(LoadingIcon$1, {
                 existIcon: !!Lt,
                 prefixCls: Gt,
                 loading: !!pn
             }),
             Rn = Mt || Mt === 0 ? spaceChildren(Mt, Ht && Bt) : null;
-        if (Sn.href !== void 0)
-            return cn( /* @__PURE__ */ React.createElement("a", Object.assign({}, Sn, {
+        if (yn.href !== void 0)
+            return cn( /* @__PURE__ */ React.createElement("a", Object.assign({}, yn, {
                 className: cls(Cn, {
                     [`${Gt}-disabled`]: Qt
                 }),
-                href: Qt ? void 0 : Sn.href,
+                href: Qt ? void 0 : yn.href,
                 style: kn,
                 onClick: Dt,
                 ref: Xt,
                 tabIndex: Qt ? -1 : 0
             }), Wn, Rn));
-        let yn = /* @__PURE__ */ React.createElement("button", Object.assign({}, It, {
+        let Fn = /* @__PURE__ */ React.createElement("button", Object.assign({}, It, {
             type: At,
             className: Cn,
             style: kn,
             onClick: Dt,
             disabled: Qt,
             ref: Xt
         }), Wn, Rn, !!Yt && /* @__PURE__ */ React.createElement(CompactCmp, {
             key: "compact",
             prefixCls: Gt
         }));
-        return isUnBorderedButtonType(Nt) || (yn = /* @__PURE__ */ React.createElement(Wave$1, {
+        return isUnBorderedButtonType(Nt) || (Fn = /* @__PURE__ */ React.createElement(Wave$1, {
             component: "Button",
             disabled: !!pn
-        }, yn)), cn(yn);
+        }, Fn)), cn(Fn);
     },
     Button$1 = /* @__PURE__ */ reactExports.forwardRef(InternalButton);
 Button$1.Group = Group$3;
 Button$1.__ANT_BUTTON = !0;
 const Button$2 = Button$1;
 var OrderContext = /* @__PURE__ */ reactExports.createContext(null),
     EMPTY_LIST$1 = [];
@@ -23114,60 +23114,60 @@
 
     function Xt() {
         contains(Qt.current, document.activeElement) || (an.current = document.activeElement);
     }
 
     function Ht() {
         if (!contains(Qt.current, document.activeElement)) {
-            var Sn;
-            (Sn = Zt.current) === null || Sn === void 0 || Sn.focus();
+            var yn;
+            (yn = Zt.current) === null || yn === void 0 || yn.focus();
         }
     }
 
-    function Dt(Sn) {
-        if (Sn)
+    function Dt(yn) {
+        if (yn)
             Ht();
         else {
             if (un(!1), It && an.current && xt) {
                 try {
                     an.current.focus({
                         preventScroll: !0
                     });
                 } catch {}
                 an.current = null;
             }
             hn && (Lt == null || Lt());
         }
-        Mt == null || Mt(Sn);
+        Mt == null || Mt(yn);
     }
 
-    function Bt(Sn) {
-        Rt == null || Rt(Sn);
+    function Bt(yn) {
+        Rt == null || Rt(yn);
     }
     var Wt = reactExports.useRef(!1),
         Yt = reactExports.useRef(),
         on = function() {
             clearTimeout(Yt.current), Wt.current = !0;
         },
         rn = function() {
             Yt.current = setTimeout(function() {
                 Wt.current = !1;
             });
         },
         mn = null;
-    jt && (mn = function(Sn) {
-        Wt.current ? Wt.current = !1 : Qt.current === Sn.target && Bt(Sn);
+    jt && (mn = function(yn) {
+        Wt.current ? Wt.current = !1 : Qt.current === yn.target && Bt(yn);
     });
 
-    function _n(Sn) {
-        if (yt && Sn.keyCode === KeyCode.ESC) {
-            Sn.stopPropagation(), Bt(Sn);
+    function _n(yn) {
+        if (yt && yn.keyCode === KeyCode.ESC) {
+            yn.stopPropagation(), Bt(yn);
             return;
         }
-        bt && Sn.keyCode === KeyCode.TAB && Zt.current.changeActive(!Sn.shiftKey);
+        bt && yn.keyCode === KeyCode.TAB && Zt.current.changeActive(!yn.shiftKey);
     }
     return reactExports.useEffect(function() {
         bt && (un(!0), Xt());
     }, [bt]), reactExports.useEffect(function() {
         return function() {
             clearTimeout(Yt.current);
         };
@@ -26476,27 +26476,27 @@
         Bt = useEffectState(zt, 0),
         Wt = _slicedToArray(Bt, 2),
         Yt = Wt[0],
         on = Wt[1],
         rn = reactExports.useState(null),
         mn = _slicedToArray(rn, 2),
         _n = mn[0],
-        Sn = mn[1],
+        yn = mn[1],
         Cn = reactExports.useState(null),
         kn = _slicedToArray(Cn, 2),
         Pn = kn[0],
         Mn = kn[1],
         Wn = reactExports.useMemo(function() {
             return Pn === null && Ft ? Number.MAX_SAFE_INTEGER : Pn || 0;
         }, [Pn, Gt]),
         Rn = reactExports.useState(!1),
-        yn = _slicedToArray(Rn, 2),
-        jn = yn[0],
-        An = yn[1],
-        bn = "".concat(mt, "-item"),
+        Fn = _slicedToArray(Rn, 2),
+        En = Fn[0],
+        An = Fn[1],
+        gn = "".concat(mt, "-item"),
         xn = Math.max(hn, Ht),
         zn = Mt === RESPONSIVE,
         On = bt.length && zn,
         Un = Mt === INVALIDATE,
         Gn = On || typeof Mt == "number" && bt.length > Mt,
         Zn = reactExports.useMemo(function() {
             var Nn = bt;
@@ -26510,107 +26510,107 @@
             return typeof Et == "function" ? Et(Nn) : (Jn = Et && (Nn == null ? void 0 : Nn[Et])) !== null && Jn !== void 0 ? Jn : Kn;
         }, [Et]),
         ur = reactExports.useCallback(_t || function(Nn) {
             return Nn;
         }, [_t]);
 
     function nr(Nn, Kn, Jn) {
-        Pn === Nn && (Kn === void 0 || Kn === _n) || (Mn(Nn), Jn || (An(Nn < bt.length - 1), It == null || It(Nn)), Kn !== void 0 && Sn(Kn));
+        Pn === Nn && (Kn === void 0 || Kn === _n) || (Mn(Nn), Jn || (An(Nn < bt.length - 1), It == null || It(Nn)), Kn !== void 0 && yn(Kn));
     }
 
     function sr(Nn, Kn) {
         cn(Kn.clientWidth);
     }
 
-    function Fn(Nn, Kn) {
+    function Dn(Nn, Kn) {
         Zt(function(Jn) {
             var gr = new Map(Jn);
             return Kn === null ? gr.delete(Nn) : gr.set(Nn, Kn), gr;
         });
     }
 
     function wn(Nn, Kn) {
         Dt(Kn), un(Ht);
     }
 
-    function En(Nn, Kn) {
+    function Sn(Nn, Kn) {
         on(Kn);
     }
 
-    function Dn(Nn) {
+    function jn(Nn) {
         return Qt.get(lr(Zn[Nn], Nn));
     }
     useLayoutEffect(function() {
         if (en && typeof xn == "number" && Zn) {
             var Nn = Yt,
                 Kn = Zn.length,
                 Jn = Kn - 1;
             if (!Kn) {
                 nr(0, null);
                 return;
             }
             for (var gr = 0; gr < Kn; gr += 1) {
-                var rr = Dn(gr);
+                var rr = jn(gr);
                 if (Ft && (rr = rr || 0), rr === void 0) {
                     nr(gr - 1, void 0, !0);
                     break;
                 }
                 if (Nn += rr, // Only one means `totalWidth` is the final width
                     Jn === 0 && Nn <= en || // Last two width will be the final width
-                    gr === Jn - 1 && Nn + Dn(Jn) <= en) {
+                    gr === Jn - 1 && Nn + jn(Jn) <= en) {
                     nr(Jn, null);
                     break;
                 } else if (Nn + xn > en) {
                     nr(gr - 1, Nn - rr - Yt + Ht);
                     break;
                 }
             }
-            kt && Dn(0) + Yt > en && Sn(null);
+            kt && jn(0) + Yt > en && yn(null);
         }
     }, [en, Qt, Ht, Yt, lr, Zn]);
-    var cr = jn && !!Yn.length,
+    var cr = En && !!Yn.length,
         Tn = {};
     _n !== null && On && (Tn = {
         position: "absolute",
         left: _n,
         top: 0
     });
     var In = {
-            prefixCls: bn,
+            prefixCls: gn,
             responsive: On,
             component: Ot,
             invalidate: Un
         },
         Qn = yt ? function(Nn, Kn) {
             var Jn = lr(Nn, Kn);
             return /* @__PURE__ */ reactExports.createElement(OverflowContext.Provider, {
                 key: Jn,
                 value: _objectSpread2(_objectSpread2({}, In), {}, {
                     order: Kn,
                     item: Nn,
                     itemKey: Jn,
-                    registerSize: Fn,
+                    registerSize: Dn,
                     display: Kn <= Wn
                 })
             }, yt(Nn, Kn));
         } : function(Nn, Kn) {
             var Jn = lr(Nn, Kn);
             return /* @__PURE__ */ reactExports.createElement(Item$2, _extends$1({}, In, {
                 order: Kn,
                 key: Jn,
                 item: Nn,
                 renderItem: ur,
                 itemKey: Jn,
-                registerSize: Fn,
+                registerSize: Dn,
                 display: Kn <= Wn
             }));
         },
         or, Xn = {
             order: cr ? Wn : Number.MAX_SAFE_INTEGER,
-            className: "".concat(bn, "-rest"),
+            className: "".concat(gn, "-rest"),
             registerSize: wn,
             display: cr
         };
     if (Pt)
         Pt && (or = /* @__PURE__ */ reactExports.createElement(OverflowContext.Provider, {
             value: _objectSpread2(_objectSpread2({}, In), Xn)
         }, Pt(Yn)));
@@ -26622,16 +26622,16 @@
         className: cls(!Un && mt, Rt),
         style: Ct,
         ref: it
     }, Nt), Zn.map(Qn), Gn ? or : null, kt && /* @__PURE__ */ reactExports.createElement(Item$2, _extends$1({}, In, {
         responsive: zn,
         responsiveDisabled: !On,
         order: Wn,
-        className: "".concat(bn, "-suffix"),
-        registerSize: En,
+        className: "".concat(gn, "-suffix"),
+        registerSize: Sn,
         display: !0,
         style: Tn
     }), kt));
     return zn && (hr = /* @__PURE__ */ reactExports.createElement(RefResizeObserver, {
         onResize: sr,
         disabled: !On
     }, hr)), hr;
@@ -26755,16 +26755,16 @@
                 right: Wt,
                 bottom: Wt
             };
         if (Vt || !Et) {
             var on, rn = Lt.points,
                 mn = Lt.dynamicInset || ((on = Lt._experimental) === null || on === void 0 ? void 0 : on.dynamicInset),
                 _n = mn && rn[0][1] === "r",
-                Sn = mn && rn[0][0] === "b";
-            _n ? (Yt.right = en, Yt.left = Wt) : (Yt.left = Gt, Yt.right = Wt), Sn ? (Yt.bottom = Kt, Yt.top = Wt) : (Yt.top = cn, Yt.bottom = Wt);
+                yn = mn && rn[0][0] === "b";
+            _n ? (Yt.right = en, Yt.left = Wt) : (Yt.left = Gt, Yt.right = Wt), yn ? (Yt.bottom = Kt, Yt.top = Wt) : (Yt.top = cn, Yt.bottom = Wt);
         }
         var Cn = {};
         return Zt && (Zt.includes("height") && pn ? Cn.height = pn : Zt.includes("minHeight") && pn && (Cn.minHeight = pn), Zt.includes("width") && Jt ? Cn.width = Jt : Zt.includes("minWidth") && Jt && (Cn.minWidth = Jt)), Et || (Cn.pointerEvents = "none"), /* @__PURE__ */ reactExports.createElement(It, {
             open: At || un,
             getContainer: Tt && function() {
                 return Tt(_t);
             },
@@ -26793,18 +26793,18 @@
                 onVisibleChanged: function(Pn) {
                     var Mn;
                     Pt == null || (Mn = Pt.onVisibleChanged) === null || Mn === void 0 || Mn.call(Pt, Pn), yt(Pn);
                 }
             }), function(Pn, Mn) {
                 var Wn = Pn.className,
                     Rn = Pn.style,
-                    yn = cls(gt, Wn, mt);
+                    Fn = cls(gt, Wn, mt);
                 return /* @__PURE__ */ reactExports.createElement("div", {
                     ref: composeRef(kn, it, Mn),
-                    className: yn,
+                    className: Fn,
                     style: _objectSpread2(_objectSpread2(_objectSpread2(_objectSpread2({
                         "--arrow-x": "".concat(Mt.x || 0, "px"),
                         "--arrow-y": "".concat(Mt.y || 0, "px")
                     }, Yt), Cn), Rn), {}, {
                         boxSizing: "border-box",
                         zIndex: Nt
                     }, bt),
@@ -27010,15 +27010,15 @@
         Mt = function() {
             Rt.current = {};
         };
     _e || Mt();
     var Lt = useEvent(function() {
             if (it && ft && _e) {
                 let Or = function(Nr, po) {
-                        var eo = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : yn,
+                        var eo = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : Fn,
                             to = hn.x + Nr,
                             oo = hn.y + po,
                             ao = to + on,
                             co = oo + Yt,
                             vo = Math.max(to, eo.left),
                             bo = Math.max(oo, eo.top),
                             _o = Math.min(ao, eo.right),
@@ -27074,114 +27074,114 @@
                     mn = Jt.width,
                     _n = {
                         left: 0,
                         top: 0,
                         right: ln,
                         bottom: Xt
                     },
-                    Sn = {
+                    yn = {
                         left: -Wt,
                         top: -Bt,
                         right: Ht - Wt,
                         bottom: Dt - Bt
                     },
                     Cn = Qt.htmlRegion,
                     kn = "visible",
                     Pn = "visibleFirst";
                 Cn !== "scroll" && Cn !== Pn && (Cn = kn);
                 var Mn = Cn === Pn,
-                    Wn = getVisibleArea(Sn, Ct),
+                    Wn = getVisibleArea(yn, Ct),
                     Rn = getVisibleArea(_n, Ct),
-                    yn = Cn === kn ? Rn : Wn,
-                    jn = Mn ? Rn : yn;
+                    Fn = Cn === kn ? Rn : Wn,
+                    En = Mn ? Rn : Fn;
                 Ot.style.left = "auto", Ot.style.top = "auto", Ot.style.right = "0", Ot.style.bottom = "0";
                 var An = Ot.getBoundingClientRect();
                 Ot.style.left = Gt, Ot.style.top = cn, Ot.style.right = en, Ot.style.bottom = Kt, Ot.style.overflow = an, (Tt = Ot.parentElement) === null || Tt === void 0 || Tt.removeChild(Zt);
-                var bn = toNum(Math.round(on / parseFloat(zt) * 1e3) / 1e3),
+                var gn = toNum(Math.round(on / parseFloat(zt) * 1e3) / 1e3),
                     xn = toNum(Math.round(Yt / parseFloat(jt) * 1e3) / 1e3);
-                if (bn === 0 || xn === 0 || isDOM(ft) && !isVisible(ft))
+                if (gn === 0 || xn === 0 || isDOM(ft) && !isVisible(ft))
                     return;
                 var zn = Qt.offset,
                     On = Qt.targetOffset,
                     Un = getNumberOffset(hn, zn),
                     Gn = _slicedToArray(Un, 2),
                     Zn = Gn[0],
                     Yn = Gn[1],
                     lr = getNumberOffset(Jt, On),
                     ur = _slicedToArray(lr, 2),
                     nr = ur[0],
                     sr = ur[1];
                 Jt.x -= nr, Jt.y -= sr;
-                var Fn = Qt.points || [],
-                    wn = _slicedToArray(Fn, 2),
-                    En = wn[0],
-                    Dn = wn[1],
-                    cr = splitPoints(Dn),
-                    Tn = splitPoints(En),
+                var Dn = Qt.points || [],
+                    wn = _slicedToArray(Dn, 2),
+                    Sn = wn[0],
+                    jn = wn[1],
+                    cr = splitPoints(jn),
+                    Tn = splitPoints(Sn),
                     In = getAlignPoint(Jt, cr),
                     Qn = getAlignPoint(hn, Tn),
                     or = _objectSpread2({}, Qt),
                     Xn = In.x - Qn.x + Zn,
                     Vn = In.y - Qn.y + Yn,
                     hr = Or(Xn, Vn),
                     Nn = Or(Xn, Vn, Rn),
                     Kn = getAlignPoint(Jt, ["t", "l"]),
                     Jn = getAlignPoint(hn, ["t", "l"]),
                     gr = getAlignPoint(Jt, ["b", "r"]),
                     rr = getAlignPoint(hn, ["b", "r"]),
                     nn = Qt.overflow || {},
                     qt = nn.adjustX,
                     dn = nn.adjustY,
-                    gn = nn.shiftX,
-                    vn = nn.shiftY,
+                    vn = nn.shiftX,
+                    bn = nn.shiftY,
                     $n = function(Nr) {
                         return typeof Nr == "boolean" ? Nr : Nr >= 0;
                     },
                     Ln, Hn, Bn, qn;
                 lo();
                 var ir = $n(dn),
                     er = Tn[0] === cr[0];
-                if (ir && Tn[0] === "t" && (Hn > jn.bottom || Rt.current.bt)) {
+                if (ir && Tn[0] === "t" && (Hn > En.bottom || Rt.current.bt)) {
                     var ar = Vn;
                     er ? ar -= Yt - rn : ar = Kn.y - rr.y - Yn;
                     var dr = Or(Xn, ar),
                         mr = Or(Xn, ar, Rn);
                     dr > hr || dr === hr && (!Mn || // Choose recommend one
                         mr >= Nn) ? (Rt.current.bt = !0, Vn = ar, Yn = -Yn, or.points = [reversePoints(Tn, 0), reversePoints(cr, 0)]) : Rt.current.bt = !1;
                 }
-                if (ir && Tn[0] === "b" && (Ln < jn.top || Rt.current.tb)) {
+                if (ir && Tn[0] === "b" && (Ln < En.top || Rt.current.tb)) {
                     var pr = Vn;
                     er ? pr += Yt - rn : pr = gr.y - Jn.y - Yn;
                     var br = Or(Xn, pr),
                         _r = Or(Xn, pr, Rn);
                     br > hr || br === hr && (!Mn || // Choose recommend one
                         _r >= Nn) ? (Rt.current.tb = !0, Vn = pr, Yn = -Yn, or.points = [reversePoints(Tn, 0), reversePoints(cr, 0)]) : Rt.current.tb = !1;
                 }
                 var yr = $n(qt),
                     Pr = Tn[1] === cr[1];
-                if (yr && Tn[1] === "l" && (qn > jn.right || Rt.current.rl)) {
+                if (yr && Tn[1] === "l" && (qn > En.right || Rt.current.rl)) {
                     var Cr = Xn;
                     Pr ? Cr -= on - mn : Cr = Kn.x - rr.x - Zn;
                     var kr = Or(Cr, Vn),
                         Dr = Or(Cr, Vn, Rn);
                     kr > hr || kr === hr && (!Mn || // Choose recommend one
                         Dr >= Nn) ? (Rt.current.rl = !0, Xn = Cr, Zn = -Zn, or.points = [reversePoints(Tn, 1), reversePoints(cr, 1)]) : Rt.current.rl = !1;
                 }
-                if (yr && Tn[1] === "r" && (Bn < jn.left || Rt.current.lr)) {
+                if (yr && Tn[1] === "r" && (Bn < En.left || Rt.current.lr)) {
                     var Br = Xn;
                     Pr ? Br += on - mn : Br = gr.x - Jn.x - Zn;
                     var Yr = Or(Br, Vn),
                         Wr = Or(Br, Vn, Rn);
                     Yr > hr || Yr === hr && (!Mn || // Choose recommend one
                         Wr >= Nn) ? (Rt.current.lr = !0, Xn = Br, Zn = -Zn, or.points = [reversePoints(Tn, 1), reversePoints(cr, 1)]) : Rt.current.lr = !1;
                 }
                 lo();
-                var Mr = gn === !0 ? 0 : gn;
+                var Mr = vn === !0 ? 0 : vn;
                 typeof Mr == "number" && (Bn < Rn.left && (Xn -= Bn - Rn.left - Zn, Jt.x + mn < Rn.left + Mr && (Xn += Jt.x - Rn.left + mn - Mr)), qn > Rn.right && (Xn -= qn - Rn.right - Zn, Jt.x > Rn.right - Mr && (Xn += Jt.x - Rn.right + Mr)));
-                var Ur = vn === !0 ? 0 : vn;
+                var Ur = bn === !0 ? 0 : bn;
                 typeof Ur == "number" && (Ln < Rn.top && (Vn -= Ln - Rn.top - Yn, Jt.y + rn < Rn.top + Ur && (Vn += Jt.y - Rn.top + rn - Ur)), Hn > Rn.bottom && (Vn -= Hn - Rn.bottom - Yn, Jt.y > Rn.bottom - Ur && (Vn += Jt.y - Rn.bottom + Ur)));
                 var qr = hn.x + Xn,
                     Gr = qr + on,
                     jr = hn.y + Vn,
                     Zr = jr + Yt,
                     vr = Jt.x,
                     Er = vr + mn,
@@ -27196,21 +27196,21 @@
                     Xr = (Jr + Hr) / 2,
                     ro = Xr - jr;
                 _t == null || _t(it, or);
                 var so = An.right - hn.x - (Xn + hn.width),
                     fo = An.bottom - hn.y - (Vn + hn.height);
                 wt({
                     ready: !0,
-                    offsetX: Xn / bn,
+                    offsetX: Xn / gn,
                     offsetY: Vn / xn,
-                    offsetR: so / bn,
+                    offsetR: so / gn,
                     offsetB: fo / xn,
-                    arrowX: Qr / bn,
+                    arrowX: Qr / gn,
                     arrowY: ro / xn,
-                    scaleX: bn,
+                    scaleX: gn,
                     scaleY: xn,
                     align: or
                 });
             }
         }),
         Pt = function() {
             $t.current += 1;
@@ -27323,55 +27323,55 @@
                 Bt = ft.popupMotion,
                 Wt = ft.maskMotion,
                 Yt = ft.popupTransitionName,
                 on = ft.popupAnimation,
                 rn = ft.maskTransitionName,
                 mn = ft.maskAnimation,
                 _n = ft.className,
-                Sn = ft.getTriggerDOMNode,
+                yn = ft.getTriggerDOMNode,
                 Cn = _objectWithoutProperties(ft, _excluded$i),
                 kn = jt || Vt || !1,
                 Pn = reactExports.useState(!1),
                 Mn = _slicedToArray(Pn, 2),
                 Wn = Mn[0],
                 Rn = Mn[1];
             useLayoutEffect(function() {
                 Rn(isMobile$1());
             }, []);
-            var yn = reactExports.useRef({}),
-                jn = reactExports.useContext(TriggerContext),
+            var Fn = reactExports.useRef({}),
+                En = reactExports.useContext(TriggerContext),
                 An = reactExports.useMemo(function() {
                     return {
                         registerSubPopup: function(fr, Sr) {
-                            yn.current[fr] = Sr, jn == null || jn.registerSubPopup(fr, Sr);
+                            Fn.current[fr] = Sr, En == null || En.registerSubPopup(fr, Sr);
                         }
                     };
-                }, [jn]),
-                bn = useId(),
+                }, [En]),
+                gn = useId(),
                 xn = reactExports.useState(null),
                 zn = _slicedToArray(xn, 2),
                 On = zn[0],
                 Un = zn[1],
                 Gn = useEvent(function(fr) {
-                    isDOM(fr) && On !== fr && Un(fr), jn == null || jn.registerSubPopup(bn, fr);
+                    isDOM(fr) && On !== fr && Un(fr), En == null || En.registerSubPopup(gn, fr);
                 }),
                 Zn = reactExports.useState(null),
                 Yn = _slicedToArray(Zn, 2),
                 lr = Yn[0],
                 ur = Yn[1],
                 nr = reactExports.useRef(null),
                 sr = useEvent(function(fr) {
                     isDOM(fr) && lr !== fr && (ur(fr), nr.current = fr);
                 }),
-                Fn = reactExports.Children.only(_t),
-                wn = (Fn == null ? void 0 : Fn.props) || {},
-                En = {},
-                Dn = useEvent(function(fr) {
+                Dn = reactExports.Children.only(_t),
+                wn = (Dn == null ? void 0 : Dn.props) || {},
+                Sn = {},
+                jn = useEvent(function(fr) {
                     var Sr, Ar, $r = lr;
-                    return ($r == null ? void 0 : $r.contains(fr)) || ((Sr = getShadowRoot($r)) === null || Sr === void 0 ? void 0 : Sr.host) === fr || fr === $r || (On == null ? void 0 : On.contains(fr)) || ((Ar = getShadowRoot(On)) === null || Ar === void 0 ? void 0 : Ar.host) === fr || fr === On || Object.values(yn.current).some(function(wr) {
+                    return ($r == null ? void 0 : $r.contains(fr)) || ((Sr = getShadowRoot($r)) === null || Sr === void 0 ? void 0 : Sr.host) === fr || fr === $r || (On == null ? void 0 : On.contains(fr)) || ((Ar = getShadowRoot(On)) === null || Ar === void 0 ? void 0 : Ar.host) === fr || fr === On || Object.values(Fn.current).some(function(wr) {
                         return (wr == null ? void 0 : wr.contains(fr)) || fr === wr;
                     });
                 }),
                 cr = getMotion$1(bt, Bt, on, Yt),
                 Tn = getMotion$1(bt, Wt, mn, rn),
                 In = reactExports.useState(Ct || !1),
                 Qn = _slicedToArray(In, 2),
@@ -27403,18 +27403,18 @@
                     }, Sr * 1e3);
                 };
             reactExports.useEffect(function() {
                 return rr;
             }, []);
             var qt = reactExports.useState(!1),
                 dn = _slicedToArray(qt, 2),
-                gn = dn[0],
-                vn = dn[1];
+                vn = dn[0],
+                bn = dn[1];
             useLayoutEffect(function(fr) {
-                (!fr || Vn) && vn(!0);
+                (!fr || Vn) && bn(!0);
             }, [Vn]);
             var $n = reactExports.useState(null),
                 Ln = _slicedToArray($n, 2),
                 Hn = Ln[0],
                 Bn = Ln[1],
                 qn = reactExports.useState([0, 0]),
                 ir = _slicedToArray(qn, 2),
@@ -27439,15 +27439,15 @@
                 Ur = useAction(Wn, Et, xt, wt),
                 qr = _slicedToArray(Ur, 2),
                 Gr = qr[0],
                 jr = qr[1],
                 Zr = Gr.has("click"),
                 vr = jr.has("click") || jr.has("contextMenu"),
                 Er = useEvent(function() {
-                    gn || Mr();
+                    vn || Mr();
                 }),
                 xr = function() {
                     Nn.current && ln && vr && nn(!1);
                 };
             useWatch(Vn, lr, On, Er, xr), useLayoutEffect(function() {
                 Er();
             }, [er, Kt]), useLayoutEffect(function() {
@@ -27477,86 +27477,86 @@
                         Qr(fr.width), ro(fr.height);
                     }
                 },
                 fo = function() {
                     so(), Er();
                 },
                 Or = function(fr) {
-                    vn(!1), Mr(), Mt == null || Mt(fr);
+                    bn(!1), Mr(), Mt == null || Mt(fr);
                 },
                 lo = function() {
                     return new Promise(function(fr) {
                         so(), Bn(function() {
                             return fr;
                         });
                     });
                 };
             useLayoutEffect(function() {
                 Hn && (Mr(), Hn(), Bn(null));
             }, [Hn]);
 
             function Nr(fr, Sr, Ar, $r) {
-                En[fr] = function(wr) {
+                Sn[fr] = function(wr) {
                     var uo;
                     $r == null || $r(wr), nn(Sr, Ar);
                     for (var So = arguments.length, wo = new Array(So > 1 ? So - 1 : 0), ho = 1; ho < So; ho++)
                         wo[ho - 1] = arguments[ho];
                     (uo = wn[fr]) === null || uo === void 0 || uo.call.apply(uo, [wn, wr].concat(wo));
                 };
             }
-            (Zr || vr) && (En.onClick = function(fr) {
+            (Zr || vr) && (Sn.onClick = function(fr) {
                 var Sr;
                 Nn.current && vr ? nn(!1) : !Nn.current && Zr && (dr(fr), nn(!0));
                 for (var Ar = arguments.length, $r = new Array(Ar > 1 ? Ar - 1 : 0), wr = 1; wr < Ar; wr++)
                     $r[wr - 1] = arguments[wr];
                 (Sr = wn.onClick) === null || Sr === void 0 || Sr.call.apply(Sr, [wn, fr].concat($r));
-            }), useWinClick(Vn, vr, lr, On, Ot, Nt, Dn, nn);
+            }), useWinClick(Vn, vr, lr, On, Ot, Nt, jn, nn);
             var po = Gr.has("hover"),
                 eo = jr.has("hover"),
                 to, oo;
             po && (Nr("onMouseEnter", !0, Lt, function(fr) {
                 dr(fr);
             }), Nr("onPointerEnter", !0, Lt, function(fr) {
                 dr(fr);
             }), to = function(fr) {
-                (Vn || gn) && On !== null && On !== void 0 && On.contains(fr.target) && nn(!0, Lt);
-            }, ln && (En.onMouseMove = function(fr) {
+                (Vn || vn) && On !== null && On !== void 0 && On.contains(fr.target) && nn(!0, Lt);
+            }, ln && (Sn.onMouseMove = function(fr) {
                 var Sr;
                 (Sr = wn.onMouseMove) === null || Sr === void 0 || Sr.call(wn, fr);
             })), eo && (Nr("onMouseLeave", !1, kt), Nr("onPointerLeave", !1, kt), oo = function() {
                 nn(!1, kt);
-            }), Gr.has("focus") && Nr("onFocus", !0, At), jr.has("focus") && Nr("onBlur", !1, Tt), Gr.has("contextMenu") && (En.onContextMenu = function(fr) {
+            }), Gr.has("focus") && Nr("onFocus", !0, At), jr.has("focus") && Nr("onBlur", !1, Tt), Gr.has("contextMenu") && (Sn.onContextMenu = function(fr) {
                 var Sr;
                 Nn.current && jr.has("contextMenu") ? nn(!1) : (dr(fr), nn(!0)), fr.preventDefault();
                 for (var Ar = arguments.length, $r = new Array(Ar > 1 ? Ar - 1 : 0), wr = 1; wr < Ar; wr++)
                     $r[wr - 1] = arguments[wr];
                 (Sr = wn.onContextMenu) === null || Sr === void 0 || Sr.call.apply(Sr, [wn, fr].concat($r));
-            }), _n && (En.className = cls(wn.className, _n));
-            var ao = _objectSpread2(_objectSpread2({}, wn), En),
+            }), _n && (Sn.className = cls(wn.className, _n));
+            var ao = _objectSpread2(_objectSpread2({}, wn), Sn),
                 co = {},
                 vo = ["onContextMenu", "onClick", "onMouseDown", "onTouchStart", "onMouseEnter", "onMouseLeave", "onFocus", "onBlur"];
             vo.forEach(function(fr) {
                 Cn[fr] && (co[fr] = function() {
                     for (var Sr, Ar = arguments.length, $r = new Array(Ar), wr = 0; wr < Ar; wr++)
                         $r[wr] = arguments[wr];
                     (Sr = ao[fr]) === null || Sr === void 0 || Sr.call.apply(Sr, [ao].concat($r)), Cn[fr].apply(Cn, $r);
                 });
             });
-            var bo = /* @__PURE__ */ reactExports.cloneElement(Fn, _objectSpread2(_objectSpread2({}, ao), co)),
+            var bo = /* @__PURE__ */ reactExports.cloneElement(Dn, _objectSpread2(_objectSpread2({}, ao), co)),
                 _o = {
                     x: kr,
                     y: Dr
                 },
                 yo = Dt ? _objectSpread2({}, Dt !== !0 ? Dt : {}) : null;
             return /* @__PURE__ */ reactExports.createElement(reactExports.Fragment, null, /* @__PURE__ */ reactExports.createElement(RefResizeObserver, {
                 disabled: !Vn,
                 ref: sr,
                 onResize: fo
             }, /* @__PURE__ */ reactExports.createElement(TriggerWrapper, {
-                getTriggerDOMNode: Sn
+                getTriggerDOMNode: yn
             }, bo)), /* @__PURE__ */ reactExports.createElement(TriggerContext.Provider, {
                 value: An
             }, /* @__PURE__ */ reactExports.createElement(Popup, {
                 portal: _e,
                 ref: Gn,
                 prefixCls: bt,
                 popup: Gt,
@@ -27564,15 +27564,15 @@
                 style: en,
                 target: lr,
                 onMouseEnter: to,
                 onMouseLeave: oo,
                 onPointerEnter: to,
                 zIndex: Jt,
                 open: Vn,
-                keepDom: gn,
+                keepDom: vn,
                 fresh: un,
                 onClick: Xt,
                 mask: Ot,
                 motion: cr,
                 maskMotion: Tn,
                 onVisibleChanged: Or,
                 onPrepare: lo,
@@ -28619,39 +28619,39 @@
             Bt = reactExports.useRef(),
             Wt = Et ?? en,
             Yt = xt ?? Kt,
             on = zt.includes(gt),
             rn = !Vt && on,
             mn = un(cn, gt),
             _n = useActive(gt, Ht, kt, At),
-            Sn = _n.active,
+            yn = _n.active,
             Cn = _objectWithoutProperties(_n, _excluded2$5),
             kn = reactExports.useState(!1),
             Pn = _slicedToArray(kn, 2),
             Mn = Pn[0],
             Wn = Pn[1],
             Rn = function(nr) {
                 Ht || Wn(nr);
             },
-            yn = function(nr) {
+            Fn = function(nr) {
                 Rn(!0), Mt == null || Mt({
                     key: gt,
                     domEvent: nr
                 });
             },
-            jn = function(nr) {
+            En = function(nr) {
                 Rn(!1), Lt == null || Lt({
                     key: gt,
                     domEvent: nr
                 });
             },
             An = reactExports.useMemo(function() {
-                return Sn || (Ft !== "inline" ? Mn || un([Gt], gt) : !1);
-            }, [Ft, Sn, Gt, Mn, gt, un]),
-            bn = useDirectionStyle(ln.length),
+                return yn || (Ft !== "inline" ? Mn || un([Gt], gt) : !1);
+            }, [Ft, yn, Gt, Mn, gt, un]),
+            gn = useDirectionStyle(ln.length),
             xn = function(nr) {
                 Ht || (Pt == null || Pt({
                     key: gt,
                     domEvent: nr
                 }), Ft === "inline" && Qt(gt, !on));
             },
             zn = useMemoCallback(function(nr) {
@@ -28662,15 +28662,15 @@
             },
             Un = function() {
                 Zt(gt);
             },
             Gn = Ot && "".concat(Ot, "-popup"),
             Zn = /* @__PURE__ */ reactExports.createElement("div", _extends$1({
                 role: "menuitem",
-                style: bn,
+                style: gn,
                 className: "".concat(Xt, "-title"),
                 tabIndex: Ht ? null : -1,
                 ref: Dt,
                 title: typeof mt == "string" ? mt : null,
                 "data-menu-id": Vt && Ot ? null : Ot,
                 "aria-expanded": rn,
                 "aria-haspopup": !0,
@@ -28714,16 +28714,16 @@
         }
         var ur = /* @__PURE__ */ reactExports.createElement(ForwardOverflow.Item, _extends$1({
             role: "none"
         }, Tt, {
             component: "li",
             style: it,
             className: cls(Xt, "".concat(Xt, "-").concat(Ft), ft, _defineProperty(_defineProperty(_defineProperty(_defineProperty({}, "".concat(Xt, "-open"), rn), "".concat(Xt, "-active"), An), "".concat(Xt, "-selected"), mn), "".concat(Xt, "-disabled"), Ht)),
-            onMouseEnter: yn,
-            onMouseLeave: jn
+            onMouseEnter: Fn,
+            onMouseLeave: En
         }), Zn, !Vt && /* @__PURE__ */ reactExports.createElement(InlineSubMenuList, {
             id: Gn,
             open: rn,
             keyPath: ln
         }, yt));
         return pn && (ur = pn(ur, _e, {
             selected: mn,
@@ -28886,28 +28886,28 @@
             Bt = Dt === void 0 ? "hover" : Dt,
             Wt = mt.builtinPlacements,
             Yt = mt.itemIcon,
             on = mt.expandIcon,
             rn = mt.overflowedIndicator,
             mn = rn === void 0 ? "..." : rn,
             _n = mt.overflowedIndicatorPopupClassName,
-            Sn = mt.getPopupContainer,
+            yn = mt.getPopupContainer,
             Cn = mt.onClick,
             kn = mt.onOpenChange,
             Pn = mt.onKeyDown;
         mt.openAnimation, mt.openTransitionName;
         var Mn = mt._internalRenderMenuItem,
             Wn = mt._internalRenderSubMenuItem,
             Rn = _objectWithoutProperties(mt, _excluded$9),
-            yn = reactExports.useMemo(function() {
+            Fn = reactExports.useMemo(function() {
                 return parseItems(Ct, $t, EMPTY_LIST);
             }, [Ct, $t]),
-            jn = reactExports.useState(!1),
-            An = _slicedToArray(jn, 2),
-            bn = An[0],
+            En = reactExports.useState(!1),
+            An = _slicedToArray(En, 2),
+            gn = An[0],
             xn = An[1],
             zn = reactExports.useRef(),
             On = useUUID(Mt),
             Un = Rt === "rtl",
             Gn = useMergedState(jt, {
                 value: Vt,
                 postState: function(vr) {
@@ -28923,73 +28923,73 @@
                 function xr() {
                     lr(vr), kn == null || kn(vr);
                 }
                 Er ? reactDomExports.flushSync(xr) : xr();
             },
             nr = reactExports.useState(Yn),
             sr = _slicedToArray(nr, 2),
-            Fn = sr[0],
+            Dn = sr[0],
             wn = sr[1],
-            En = reactExports.useRef(!1),
-            Dn = reactExports.useMemo(function() {
+            Sn = reactExports.useRef(!1),
+            jn = reactExports.useMemo(function() {
                 return (Pt === "inline" || Pt === "vertical") && kt ? ["vertical", kt] : [Pt, !1];
             }, [Pt, kt]),
-            cr = _slicedToArray(Dn, 2),
+            cr = _slicedToArray(jn, 2),
             Tn = cr[0],
             In = cr[1],
             Qn = Tn === "inline",
             or = reactExports.useState(Tn),
             Xn = _slicedToArray(or, 2),
             Vn = Xn[0],
             hr = Xn[1],
             Nn = reactExports.useState(In),
             Kn = _slicedToArray(Nn, 2),
             Jn = Kn[0],
             gr = Kn[1];
         reactExports.useEffect(function() {
-            hr(Tn), gr(In), En.current && (Qn ? lr(Fn) : ur(EMPTY_LIST));
+            hr(Tn), gr(In), Sn.current && (Qn ? lr(Dn) : ur(EMPTY_LIST));
         }, [Tn, In]);
         var rr = reactExports.useState(0),
             nn = _slicedToArray(rr, 2),
             qt = nn[0],
             dn = nn[1],
-            gn = qt >= yn.length - 1 || Vn !== "horizontal" || Tt;
+            vn = qt >= Fn.length - 1 || Vn !== "horizontal" || Tt;
         reactExports.useEffect(function() {
             Qn && wn(Yn);
         }, [Yn]), reactExports.useEffect(function() {
-            return En.current = !0,
+            return Sn.current = !0,
                 function() {
-                    En.current = !1;
+                    Sn.current = !1;
                 };
         }, []);
-        var vn = useKeyRecords(),
-            $n = vn.registerPath,
-            Ln = vn.unregisterPath,
-            Hn = vn.refreshOverflowKeys,
-            Bn = vn.isSubPathKey,
-            qn = vn.getKeyPath,
-            ir = vn.getKeys,
-            er = vn.getSubPathKeys,
+        var bn = useKeyRecords(),
+            $n = bn.registerPath,
+            Ln = bn.unregisterPath,
+            Hn = bn.refreshOverflowKeys,
+            Bn = bn.isSubPathKey,
+            qn = bn.getKeyPath,
+            ir = bn.getKeys,
+            er = bn.getSubPathKeys,
             ar = reactExports.useMemo(function() {
                 return {
                     registerPath: $n,
                     unregisterPath: Ln
                 };
             }, [$n, Ln]),
             dr = reactExports.useMemo(function() {
                 return {
                     isSubPathKey: Bn
                 };
             }, [Bn]);
         reactExports.useEffect(function() {
-            Hn(gn ? EMPTY_LIST : yn.slice(qt + 1).map(function(vr) {
+            Hn(vn ? EMPTY_LIST : Fn.slice(qt + 1).map(function(vr) {
                 return vr.key;
             }));
-        }, [qt, gn]);
-        var mr = useMergedState(Gt || cn && ((ft = yn[0]) === null || ft === void 0 ? void 0 : ft.key), {
+        }, [qt, vn]);
+        var mr = useMergedState(Gt || cn && ((ft = Fn[0]) === null || ft === void 0 ? void 0 : ft.key), {
                 value: Gt
             }),
             pr = _slicedToArray(mr, 2),
             br = pr[0],
             _r = pr[1],
             yr = useMemoCallback(function(vr) {
                 _r(vr);
@@ -29003,15 +29003,15 @@
                 focus: function(vr) {
                     var Er, xr = ir(),
                         Tr = refreshElements(xr, On),
                         Ir = Tr.elements,
                         Kr = Tr.key2element,
                         no = Tr.element2key,
                         Qr = getFocusableElements(zn.current, Ir),
-                        Jr = br ?? (Qr[0] ? no.get(Qr[0]) : (Er = yn.find(function(ro) {
+                        Jr = br ?? (Qr[0] ? no.get(Qr[0]) : (Er = Fn.find(function(ro) {
                             return !ro.props.disabled;
                         })) === null || Er === void 0 ? void 0 : Er.key),
                         Hr = Kr.get(Jr);
                     if (Jr && Hr) {
                         var Xr;
                         Hr == null || (Xr = Hr.focus) === null || Xr === void 0 || Xr.call(Hr, vr);
                     }
@@ -29069,17 +29069,17 @@
         }, []);
         var Gr = reactExports.useMemo(function() {
                 return {
                     _internalRenderMenuItem: Mn,
                     _internalRenderSubMenuItem: Wn
                 };
             }, [Mn, Wn]),
-            jr = Vn !== "horizontal" || Tt ? yn : (
+            jr = Vn !== "horizontal" || Tt ? Fn : (
                 // Need wrap for overflow dropdown that do not response for open
-                yn.map(function(vr, Er) {
+                Fn.map(function(vr, Er) {
                     return (
                         // Always wrap provider to avoid sub node re-mount
                         /* @__PURE__ */
                         reactExports.createElement(InheritableContextProvider, {
                             key: vr.key,
                             overflowDisabled: Er > qt
                         }, vr)
@@ -29099,19 +29099,19 @@
                 tabIndex: wt,
                 data: jr,
                 renderRawItem: function(vr) {
                     return vr;
                 },
                 renderRawRest: function(vr) {
                     var Er = vr.length,
-                        xr = Er ? yn.slice(-Er) : null;
+                        xr = Er ? Fn.slice(-Er) : null;
                     return /* @__PURE__ */ reactExports.createElement(SubMenu, {
                         eventKey: OVERFLOW_KEY,
                         title: mn,
-                        disabled: gn,
+                        disabled: vn,
                         internalPopupClose: Er === 0,
                         popupClassName: _n
                     }, xr);
                 },
                 maxCount: Vn !== "horizontal" || Tt ? ForwardOverflow.INVALIDATE : ForwardOverflow.RESPONSIVE,
                 ssr: "full",
                 "data-menu-list": !0,
@@ -29127,41 +29127,41 @@
         }, /* @__PURE__ */ reactExports.createElement(InheritableContextProvider, {
             prefixCls: bt,
             rootClassName: _t,
             mode: Vn,
             openKeys: Yn,
             rtl: Un,
             disabled: At,
-            motion: bn ? Xt : null,
-            defaultMotions: bn ? Ht : null,
+            motion: gn ? Xt : null,
+            defaultMotions: gn ? Ht : null,
             activeKey: br,
             onActive: yr,
             onInactive: Pr,
             selectedKeys: Dr,
             inlineIndent: ln,
             subMenuOpenDelay: It,
             subMenuCloseDelay: Ft,
             forceSubMenuRender: zt,
             builtinPlacements: Wt,
             triggerSubMenuAction: Bt,
-            getPopupContainer: Sn,
+            getPopupContainer: yn,
             itemIcon: Yt,
             expandIcon: on,
             onItemClick: Wr,
             onOpenChange: Mr
         }, /* @__PURE__ */ reactExports.createElement(PathUserContext.Provider, {
             value: dr
         }, Zr), /* @__PURE__ */ reactExports.createElement("div", {
             style: {
                 display: "none"
             },
             "aria-hidden": !0
         }, /* @__PURE__ */ reactExports.createElement(PathRegisterContext.Provider, {
             value: ar
-        }, yn)))));
+        }, Fn)))));
     }),
     ExportMenu = Menu;
 ExportMenu.Item = MenuItem$1;
 ExportMenu.SubMenu = SubMenu;
 ExportMenu.ItemGroup = MenuItemGroup;
 ExportMenu.Divider = Divider;
 const RadioGroupContext = /* @__PURE__ */ reactExports.createContext(null),
@@ -31046,84 +31046,84 @@
             Bt = Dt[0],
             Wt = Dt[1],
             Yt = reactExports.useState([0, 0]),
             on = _slicedToArray(Yt, 2),
             rn = on[0],
             mn = on[1],
             _n = reactExports.useState([0, 0]),
-            Sn = _slicedToArray(_n, 2),
-            Cn = Sn[0],
-            kn = Sn[1],
+            yn = _slicedToArray(_n, 2),
+            Cn = yn[0],
+            kn = yn[1],
             Pn = useUpdateState( /* @__PURE__ */ new Map()),
             Mn = _slicedToArray(Pn, 2),
             Wn = Mn[0],
             Rn = Mn[1],
-            yn = useOffsets(Tt, Wn, Bt[0]),
-            jn = getUnitValue(ln, Gt),
+            Fn = useOffsets(Tt, Wn, Bt[0]),
+            En = getUnitValue(ln, Gt),
             An = getUnitValue(Bt, Gt),
-            bn = getUnitValue(rn, Gt),
+            gn = getUnitValue(rn, Gt),
             xn = getUnitValue(Cn, Gt),
-            zn = jn < An + bn,
-            On = zn ? jn - xn : jn - bn,
+            zn = En < An + gn,
+            On = zn ? En - xn : En - gn,
             Un = "".concat(At, "-nav-operations-hidden"),
             Gn = 0,
             Zn = 0;
         Gt && yt ? (Gn = 0, Zn = Math.max(0, An - On)) : (Gn = Math.min(0, On - An), Zn = 0);
 
         function Yn(Hn) {
             return Hn < Gn ? Gn : Hn > Zn ? Zn : Hn;
         }
         var lr = reactExports.useRef(null),
             ur = reactExports.useState(),
             nr = _slicedToArray(ur, 2),
             sr = nr[0],
-            Fn = nr[1];
+            Dn = nr[1];
 
         function wn() {
-            Fn(Date.now());
+            Dn(Date.now());
         }
 
-        function En() {
+        function Sn() {
             lr.current && clearTimeout(lr.current);
         }
         useTouchMove(Ft, function(Hn, Bn) {
             function qn(ir, er) {
                 ir(function(ar) {
                     var dr = Yn(ar + er);
                     return dr;
                 });
             }
-            return zn ? (Gt ? qn(an, Hn) : qn(pn, Bn), En(), wn(), !0) : !1;
+            return zn ? (Gt ? qn(an, Hn) : qn(pn, Bn), Sn(), wn(), !0) : !1;
         }), reactExports.useEffect(function() {
-            return En(), sr && (lr.current = setTimeout(function() {
-                Fn(0);
-            }, 100)), En;
+            return Sn(), sr && (lr.current = setTimeout(function() {
+                Dn(0);
+            }, 100)), Sn;
         }, [sr]);
-        var Dn = useVisibleRange(
-                yn,
+        var jn = useVisibleRange(
+                Fn,
                 // Container
                 On,
                 // Transform
                 Gt ? Kt : Jt,
                 // Tabs
                 An,
                 // Add
-                bn,
+                gn,
                 // Operation
                 xn,
                 _objectSpread2(_objectSpread2({}, _e), {}, {
                     tabs: Tt
                 })
             ),
-            cr = _slicedToArray(Dn, 2),
+            cr = _slicedToArray(jn, 2),
             Tn = cr[0],
             In = cr[1],
             Qn = useEvent(function() {
                 var Hn = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : _t,
-                    Bn = yn.get(Hn) || {
+                    Bn = Fn.get(Hn) || {
                         width: 0,
                         height: 0,
                         left: 0,
                         right: 0,
                         top: 0
                     };
                 if (Gt) {
@@ -31197,31 +31197,31 @@
                 kn(er);
                 var ar = getSize(zt);
                 Wt([ar[0] - ir[0], ar[1] - ir[1]]), Vn();
             }),
             Nn = Tt.slice(0, Tn),
             Kn = Tt.slice(In + 1),
             Jn = [].concat(_toConsumableArray(Nn), _toConsumableArray(Kn)),
-            gr = yn.get(_t),
+            gr = Fn.get(_t),
             rr = useIndicator({
                 activeTabOffset: gr,
                 horizontal: Gt,
                 indicator: Pt,
                 rtl: yt
             }),
             nn = rr.style;
         reactExports.useEffect(function() {
             Qn();
-        }, [_t, Gn, Zn, stringify(gr), stringify(yn), Gt]), reactExports.useEffect(function() {
+        }, [_t, Gn, Zn, stringify(gr), stringify(Fn), Gt]), reactExports.useEffect(function() {
             hr();
         }, [yt]);
         var qt = !!Jn.length,
             dn = "".concat(At, "-nav-wrap"),
-            gn, vn, $n, Ln;
-        return Gt ? yt ? (vn = Kt > 0, gn = Kt !== Zn) : (gn = Kt < 0, vn = Kt !== Gn) : ($n = Jt < 0, Ln = Jt !== Gn), /* @__PURE__ */ reactExports.createElement(RefResizeObserver, {
+            vn, bn, $n, Ln;
+        return Gt ? yt ? (bn = Kt > 0, vn = Kt !== Zn) : (vn = Kt < 0, bn = Kt !== Gn) : ($n = Jt < 0, Ln = Jt !== Gn), /* @__PURE__ */ reactExports.createElement(RefResizeObserver, {
             onResize: hr
         }, /* @__PURE__ */ reactExports.createElement("div", {
             ref: useComposeRef(it, Ot),
             role: "tablist",
             className: cls("".concat(At, "-nav"), ft),
             style: mt,
             onKeyDown: function() {
@@ -31231,15 +31231,15 @@
             ref: It,
             position: "left",
             extra: Et,
             prefixCls: At
         }), /* @__PURE__ */ reactExports.createElement(RefResizeObserver, {
             onResize: hr
         }, /* @__PURE__ */ reactExports.createElement("div", {
-            className: cls(dn, _defineProperty(_defineProperty(_defineProperty(_defineProperty({}, "".concat(dn, "-ping-left"), gn), "".concat(dn, "-ping-right"), vn), "".concat(dn, "-ping-top"), $n), "".concat(dn, "-ping-bottom"), Ln)),
+            className: cls(dn, _defineProperty(_defineProperty(_defineProperty(_defineProperty({}, "".concat(dn, "-ping-left"), vn), "".concat(dn, "-ping-right"), bn), "".concat(dn, "-ping-top"), $n), "".concat(dn, "-ping-bottom"), Ln)),
             ref: Ft
         }, /* @__PURE__ */ reactExports.createElement(RefResizeObserver, {
             onResize: hr
         }, /* @__PURE__ */ reactExports.createElement("div", {
             ref: zt,
             className: "".concat(At, "-nav-list"),
             style: {
@@ -31463,23 +31463,23 @@
         }, []);
 
         function _n(kn, Pn) {
             Ft == null || Ft(kn, Pn);
             var Mn = kn !== ln;
             Xt(kn), Mn && (Nt == null || Nt(kn));
         }
-        var Sn = {
+        var yn = {
                 id: rn,
                 activeKey: ln,
                 animated: an,
                 tabPosition: Rt,
                 rtl: Kt,
                 mobile: Jt
             },
-            Cn = _objectSpread2(_objectSpread2({}, Sn), {}, {
+            Cn = _objectSpread2(_objectSpread2({}, yn), {}, {
                 editable: wt,
                 locale: kt,
                 moreIcon: At,
                 moreTransitionName: Tt,
                 tabBarGutter: Mt,
                 onTabClick: _n,
                 onTabScroll: zt,
@@ -31499,15 +31499,15 @@
             ref: it,
             id: ft,
             className: cls(gt, "".concat(gt, "-").concat(Rt), _defineProperty(_defineProperty(_defineProperty({}, "".concat(gt, "-mobile"), Jt), "".concat(gt, "-editable"), wt), "".concat(gt, "-rtl"), Kt), bt)
         }, cn), /* @__PURE__ */ reactExports.createElement(TabNavListWrapper, _extends$1({}, Cn, {
             renderTabBar: It
         })), /* @__PURE__ */ reactExports.createElement(TabPanelList, _extends$1({
             destroyInactiveTabPane: Ot
-        }, Sn, {
+        }, yn, {
             animated: an
         }))));
     });
 const motion = {
     motionAppear: !1,
     motionEnter: !0,
     motionLeave: !0
@@ -32958,52 +32958,52 @@
                 size: Bt
             }, Xt, {
                 className: `${Zt}-head-tabs`,
                 onChange: en,
                 items: Pt.map((Wn) => {
                     var {
                         tab: Rn
-                    } = Wn, yn = __rest$9(Wn, ["tab"]);
+                    } = Wn, Fn = __rest$9(Wn, ["tab"]);
                     return Object.assign({
                         label: Rn
-                    }, yn);
+                    }, Fn);
                 })
             })) : null;
         if (xt || _t || Wt) {
             const Wn = cls(`${Zt}-head`, Kt("header")),
                 Rn = cls(`${Zt}-head-title`, Kt("title")),
-                yn = cls(`${Zt}-extra`, Kt("extra")),
-                jn = Object.assign(Object.assign({}, yt), an("header"));
+                Fn = cls(`${Zt}-extra`, Kt("extra")),
+                En = Object.assign(Object.assign({}, yt), an("header"));
             Ht = /* @__PURE__ */ reactExports.createElement("div", {
                 className: Wn,
-                style: jn
+                style: En
             }, /* @__PURE__ */ reactExports.createElement("div", {
                 className: `${Zt}-head-wrapper`
             }, xt && /* @__PURE__ */ reactExports.createElement("div", {
                 className: Rn,
                 style: an("title")
             }, xt), _t && /* @__PURE__ */ reactExports.createElement("div", {
-                className: yn,
+                className: Fn,
                 style: an("extra")
             }, _t)), Wt);
         }
         const Yt = cls(`${Zt}-cover`, Kt("cover")),
             on = Mt ? /* @__PURE__ */ reactExports.createElement("div", {
                 className: Yt,
                 style: an("cover")
             }, Mt) : null,
             rn = cls(`${Zt}-body`, Kt("body")),
             mn = Object.assign(Object.assign({}, Et), an("body")),
             _n = /* @__PURE__ */ reactExports.createElement("div", {
                 className: rn,
                 style: mn
             }, wt ? un : kt),
-            Sn = cls(`${Zt}-actions`, Kt("actions")),
+            yn = cls(`${Zt}-actions`, Kt("actions")),
             Cn = Lt && Lt.length ? /* @__PURE__ */ reactExports.createElement(ActionNode, {
-                actionClasses: Sn,
+                actionClasses: yn,
                 actionStyle: an("actions"),
                 actions: Lt
             }) : null,
             kn = omit(jt, ["onTabChange"]),
             Pn = cls(Zt, cn == null ? void 0 : cn.className, {
                 [`${Zt}-loading`]: wt,
                 [`${Zt}-bordered`]: $t,
@@ -34882,45 +34882,45 @@
             Bt = Ht[1],
             Wt = useImageTransform(pn, Nt, zt, Qt),
             Yt = Wt.transform,
             on = Wt.resetTransform,
             rn = Wt.updateTransform,
             mn = Wt.dispatchZoomChange,
             _n = useMouseEvent(pn, _t, Et, Ot, Yt, rn, mn),
-            Sn = _n.isMoving,
+            yn = _n.isMoving,
             Cn = _n.onMouseDown,
             kn = _n.onWheel,
             Pn = useTouchEvent(pn, _t, Et, Nt, Yt, rn, mn),
             Mn = Pn.isTouching,
             Wn = Pn.onTouchStart,
             Rn = Pn.onTouchMove,
-            yn = Pn.onTouchEnd,
-            jn = Yt.rotate,
+            Fn = Pn.onTouchEnd,
+            En = Yt.rotate,
             An = Yt.scale,
-            bn = cls(_defineProperty({}, "".concat(it, "-moving"), Sn));
+            gn = cls(_defineProperty({}, "".concat(it, "-moving"), yn));
         reactExports.useEffect(function() {
             Dt || Bt(!0);
         }, [Dt]);
         var xn = function() {
                 on("close");
             },
             zn = function() {
                 mn(BASE_SCALE_RATIO + Ot, "zoomIn");
             },
             On = function() {
                 mn(BASE_SCALE_RATIO / (BASE_SCALE_RATIO + Ot), "zoomOut");
             },
             Un = function() {
                 rn({
-                    rotate: jn + 90
+                    rotate: En + 90
                 }, "rotateRight");
             },
             Gn = function() {
                 rn({
-                    rotate: jn - 90
+                    rotate: En - 90
                 }, "rotateLeft");
             },
             Zn = function() {
                 rn({
                     flipX: !Yt.flipX
                 }, "flipX");
             },
@@ -34947,56 +34947,56 @@
             };
         reactExports.useEffect(function() {
             var wn = addEventListenerWrap(window, "keydown", nr, !1);
             return function() {
                 wn.remove();
             };
         }, [Et, un, Lt]);
-        var Fn = /* @__PURE__ */ React.createElement(PreviewImage, _extends$1({}, Kt, {
+        var Dn = /* @__PURE__ */ React.createElement(PreviewImage, _extends$1({}, Kt, {
             width: _e.width,
             height: _e.height,
             imgRef: pn,
             className: "".concat(it, "-img"),
             alt: mt,
             style: {
-                transform: "translate3d(".concat(Yt.x, "px, ").concat(Yt.y, "px, 0) scale3d(").concat(Yt.flipX ? "-" : "").concat(An, ", ").concat(Yt.flipY ? "-" : "").concat(An, ", 1) rotate(").concat(jn, "deg)"),
+                transform: "translate3d(".concat(Yt.x, "px, ").concat(Yt.y, "px, 0) scale3d(").concat(Yt.flipX ? "-" : "").concat(An, ", ").concat(Yt.flipY ? "-" : "").concat(An, ", 1) rotate(").concat(En, "deg)"),
                 transitionDuration: (!Dt || Mn) && "0s"
             },
             fallback: gt,
             src: ft,
             onWheel: kn,
             onMouseDown: Cn,
             onDoubleClick: sr,
             onTouchStart: Wn,
             onTouchMove: Rn,
-            onTouchEnd: yn,
-            onTouchCancel: yn
+            onTouchEnd: Fn,
+            onTouchCancel: Fn
         }));
         return /* @__PURE__ */ React.createElement(React.Fragment, null, /* @__PURE__ */ React.createElement(DialogWrap, _extends$1({
             transitionName: Vt,
             maskTransitionName: cn,
             closable: !1,
             keyboard: !0,
             prefixCls: it,
             onClose: yt,
             visible: Et,
             classNames: {
-                wrapper: bn
+                wrapper: gn
             },
             rootClassName: $t,
             getContainer: Rt
         }, Jt, {
             afterClose: xn
         }), /* @__PURE__ */ React.createElement("div", {
             className: "".concat(it, "-img-wrapper")
-        }, en ? en(Fn, _objectSpread2({
+        }, en ? en(Dn, _objectSpread2({
             transform: Yt
         }, hn ? {
             current: Lt
-        } : {})) : Fn)), /* @__PURE__ */ React.createElement(Operations, {
+        } : {})) : Dn)), /* @__PURE__ */ React.createElement(Operations, {
             visible: Et,
             transform: Yt,
             maskTransitionName: cn,
             closeIcon: Ct,
             getContainer: Rt,
             prefixCls: it,
             rootClassName: $t,
@@ -35118,26 +35118,26 @@
             Bt = Dt[0],
             Wt = Dt[1],
             Yt = reactExports.useState(null),
             on = _slicedToArray(Yt, 2),
             rn = on[0],
             mn = on[1],
             _n = reactExports.useCallback(function(Pn, Mn, Wn) {
-                var Rn = Gt.findIndex(function(yn) {
-                    return yn.id === Pn;
+                var Rn = Gt.findIndex(function(Fn) {
+                    return Fn.id === Pn;
                 });
                 Wt(!0), mn({
                     x: Mn,
                     y: Wn
                 }), Qt(Rn < 0 ? 0 : Rn), hn(!0);
             }, [Gt]);
         reactExports.useEffect(function() {
             Bt ? pn || Qt(0) : hn(!1);
         }, [Bt]);
-        var Sn = function(Pn, Mn) {
+        var yn = function(Pn, Mn) {
                 Qt(Pn), Ot == null || Ot(Pn, Mn);
             },
             Cn = function() {
                 Wt(!1), mn(null);
             },
             kn = reactExports.useMemo(function() {
                 return {
@@ -35164,15 +35164,15 @@
             getContainer: Rt,
             current: an,
             count: Gt.length,
             countRender: At,
             onTransform: It,
             toolbarRender: Nt,
             imageRender: Ft,
-            onChange: Sn
+            onChange: yn
         }, zt)));
     },
     _excluded = ["src", "alt", "onPreviewClose", "prefixCls", "previewPrefixCls", "placeholder", "fallback", "width", "height", "style", "preview", "className", "onClick", "onError", "wrapperClassName", "wrapperStyle", "rootClassName"],
     _excluded2 = ["src", "visible", "onVisibleChange", "getContainer", "mask", "maskClassName", "movable", "icons", "scaleStep", "minScale", "maxScale", "imageRender", "toolbarRender"],
     ImageInternal = function(_e) {
         var it = _e.src,
             ft = _e.alt,
@@ -35225,92 +35225,92 @@
             rn = useStatus({
                 src: it,
                 isCustomPlaceholder: Nt,
                 fallback: xt
             }),
             mn = _slicedToArray(rn, 3),
             _n = mn[0],
-            Sn = mn[1],
+            yn = mn[1],
             Cn = mn[2],
             kn = reactExports.useState(null),
             Pn = _slicedToArray(kn, 2),
             Mn = Pn[0],
             Wn = Pn[1],
             Rn = reactExports.useContext(PreviewGroupContext),
-            yn = !!Mt,
-            jn = function() {
+            Fn = !!Mt,
+            En = function() {
                 on(!1), Wn(null);
             },
             An = cls(bt, At, Ot, _defineProperty({}, "".concat(bt, "-error"), Cn === "error")),
-            bn = reactExports.useMemo(function() {
+            gn = reactExports.useMemo(function() {
                 var Un = {};
                 return COMMON_PROPS.forEach(function(Gn) {
                     _e[Gn] !== void 0 && (Un[Gn] = _e[Gn]);
                 }), Un;
             }, COMMON_PROPS.map(function(Un) {
                 return _e[Un];
             })),
             xn = reactExports.useMemo(function() {
-                return _objectSpread2(_objectSpread2({}, bn), {}, {
+                return _objectSpread2(_objectSpread2({}, gn), {}, {
                     src: Dt
                 });
-            }, [Dt, bn]),
-            zn = useRegisterImage(yn, xn),
+            }, [Dt, gn]),
+            zn = useRegisterImage(Fn, xn),
             On = function(Un) {
                 var Gn = getOffset(Un.target),
                     Zn = Gn.left,
                     Yn = Gn.top;
                 Rn ? Rn.onPreview(zn, Zn, Yn) : (Wn({
                     x: Zn,
                     y: Yn
                 }), on(!0)), Pt == null || Pt(Un);
             };
         return /* @__PURE__ */ reactExports.createElement(reactExports.Fragment, null, /* @__PURE__ */ reactExports.createElement("div", _extends$1({}, It, {
             className: An,
-            onClick: yn ? On : Pt,
+            onClick: Fn ? On : Pt,
             style: _objectSpread2({
                 width: wt,
                 height: $t
             }, Tt)
-        }), /* @__PURE__ */ reactExports.createElement("img", _extends$1({}, bn, {
+        }), /* @__PURE__ */ reactExports.createElement("img", _extends$1({}, gn, {
             className: cls("".concat(bt, "-img"), _defineProperty({}, "".concat(bt, "-img-placeholder"), Et === !0), Lt),
             style: _objectSpread2({
                 height: $t
             }, Ct),
             ref: _n
-        }, Sn, {
+        }, yn, {
             width: wt,
             height: $t,
             onError: kt
         })), Cn === "loading" && /* @__PURE__ */ reactExports.createElement("div", {
             "aria-hidden": "true",
             className: "".concat(bt, "-placeholder")
-        }, Et), an && yn && /* @__PURE__ */ reactExports.createElement("div", {
+        }, Et), an && Fn && /* @__PURE__ */ reactExports.createElement("div", {
             className: cls("".concat(bt, "-mask"), Qt),
             style: {
                 display: (Ct == null ? void 0 : Ct.display) === "none" ? "none" : void 0
             }
-        }, an)), !Rn && yn && /* @__PURE__ */ reactExports.createElement(Preview, _extends$1({
+        }, an)), !Rn && Fn && /* @__PURE__ */ reactExports.createElement(Preview, _extends$1({
             "aria-hidden": !Yt,
             visible: Yt,
             prefixCls: yt,
-            onClose: jn,
+            onClose: En,
             mousePosition: Mn,
             src: Dt,
             alt: ft,
             fallback: xt,
             getContainer: Kt,
             icons: Jt,
             movable: Zt,
             scaleStep: pn,
             minScale: hn,
             maxScale: un,
             rootClassName: Ot,
             imageRender: ln,
-            imgCommonProps: bn,
+            imgCommonProps: gn,
             toolbarRender: Xt
         }, Ht)));
     };
 ImageInternal.PreviewGroup = Group;
 ImageInternal.displayName = "Image";
 const genBoxStyle = (_e) => ({
         position: _e || "absolute",
@@ -36110,15 +36110,15 @@
             var __webpack_modules__ = [,
                     /* 1 */
                     /***/
                     (_e, it) => {
                         var ft;
                         Object.defineProperty(it, "__esModule", {
                             value: !0
-                        }), it.VerbosityLevel = it.Util = it.UnknownErrorException = it.UnexpectedResponseException = it.TextRenderingMode = it.RenderingIntentFlag = it.PromiseCapability = it.PermissionFlag = it.PasswordResponses = it.PasswordException = it.PageActionEventType = it.OPS = it.MissingPDFException = it.MAX_IMAGE_SIZE_TO_CACHE = it.LINE_FACTOR = it.LINE_DESCENT_FACTOR = it.InvalidPDFException = it.ImageKind = it.IDENTITY_MATRIX = it.FormatError = it.FeatureTest = it.FONT_IDENTITY_MATRIX = it.DocumentActionEventType = it.CMapCompressionType = it.BaseException = it.BASELINE_FACTOR = it.AnnotationType = it.AnnotationReplyType = it.AnnotationPrefix = it.AnnotationMode = it.AnnotationFlag = it.AnnotationFieldFlag = it.AnnotationEditorType = it.AnnotationEditorPrefix = it.AnnotationEditorParamsType = it.AnnotationBorderStyleType = it.AnnotationActionEventType = it.AbortException = void 0, it.assert = hn, it.bytesToString = _n, it.createValidAbsoluteUrl = ln, it.getModificationDate = Gn, it.getUuid = nr, it.getVerbosityLevel = Qt, it.info = Zt, it.isArrayBuffer = On, it.isArrayEqual = Un, it.isNodeJS = void 0, it.normalizeUnicode = ur, it.objectFromMap = Pn, it.objectSize = kn, it.setVerbosityLevel = an, it.shadow = Xt, it.string32 = Cn, it.stringToBytes = Sn, it.stringToPDFString = bn, it.stringToUTF8String = xn, it.unreachable = pn, it.utf8StringToString = zn, it.warn = Jt;
+                        }), it.VerbosityLevel = it.Util = it.UnknownErrorException = it.UnexpectedResponseException = it.TextRenderingMode = it.RenderingIntentFlag = it.PromiseCapability = it.PermissionFlag = it.PasswordResponses = it.PasswordException = it.PageActionEventType = it.OPS = it.MissingPDFException = it.MAX_IMAGE_SIZE_TO_CACHE = it.LINE_FACTOR = it.LINE_DESCENT_FACTOR = it.InvalidPDFException = it.ImageKind = it.IDENTITY_MATRIX = it.FormatError = it.FeatureTest = it.FONT_IDENTITY_MATRIX = it.DocumentActionEventType = it.CMapCompressionType = it.BaseException = it.BASELINE_FACTOR = it.AnnotationType = it.AnnotationReplyType = it.AnnotationPrefix = it.AnnotationMode = it.AnnotationFlag = it.AnnotationFieldFlag = it.AnnotationEditorType = it.AnnotationEditorPrefix = it.AnnotationEditorParamsType = it.AnnotationBorderStyleType = it.AnnotationActionEventType = it.AbortException = void 0, it.assert = hn, it.bytesToString = _n, it.createValidAbsoluteUrl = ln, it.getModificationDate = Gn, it.getUuid = nr, it.getVerbosityLevel = Qt, it.info = Zt, it.isArrayBuffer = On, it.isArrayEqual = Un, it.isNodeJS = void 0, it.normalizeUnicode = ur, it.objectFromMap = Pn, it.objectSize = kn, it.setVerbosityLevel = an, it.shadow = Xt, it.string32 = Cn, it.stringToBytes = yn, it.stringToPDFString = gn, it.stringToUTF8String = xn, it.unreachable = pn, it.utf8StringToString = zn, it.warn = Jt;
                         const mt = typeof process == "object" && process + "" == "[object process]" && !process.versions.nw && !(process.versions.electron && process.type && process.type !== "browser");
                         it.isNodeJS = mt;
                         const gt = [1, 0, 0, 1, 0, 0];
                         it.IDENTITY_MATRIX = gt;
                         const bt = [1e-3, 0, 0, 1e-3, 0, 0];
                         it.FONT_IDENTITY_MATRIX = bt;
                         const _t = 1e7;
@@ -36410,96 +36410,96 @@
                         const en = {
                             NEED_PASSWORD: 1,
                             INCORRECT_PASSWORD: 2
                         };
                         it.PasswordResponses = en;
                         let Kt = Vt.WARNINGS;
 
-                        function an(Fn) {
-                            Number.isInteger(Fn) && (Kt = Fn);
+                        function an(Dn) {
+                            Number.isInteger(Dn) && (Kt = Dn);
                         }
 
                         function Qt() {
                             return Kt;
                         }
 
-                        function Zt(Fn) {
-                            Kt >= Vt.INFOS && console.log(`Info: ${Fn}`);
+                        function Zt(Dn) {
+                            Kt >= Vt.INFOS && console.log(`Info: ${Dn}`);
                         }
 
-                        function Jt(Fn) {
-                            Kt >= Vt.WARNINGS && console.log(`Warning: ${Fn}`);
+                        function Jt(Dn) {
+                            Kt >= Vt.WARNINGS && console.log(`Warning: ${Dn}`);
                         }
 
-                        function pn(Fn) {
-                            throw new Error(Fn);
+                        function pn(Dn) {
+                            throw new Error(Dn);
                         }
 
-                        function hn(Fn, wn) {
-                            Fn || pn(wn);
+                        function hn(Dn, wn) {
+                            Dn || pn(wn);
                         }
 
-                        function un(Fn) {
-                            switch (Fn == null ? void 0 : Fn.protocol) {
+                        function un(Dn) {
+                            switch (Dn == null ? void 0 : Dn.protocol) {
                                 case "http:":
                                 case "https:":
                                 case "ftp:":
                                 case "mailto:":
                                 case "tel:":
                                     return !0;
                                 default:
                                     return !1;
                             }
                         }
 
-                        function ln(Fn, wn = null, En = null) {
-                            if (!Fn)
+                        function ln(Dn, wn = null, Sn = null) {
+                            if (!Dn)
                                 return null;
                             try {
-                                if (En && typeof Fn == "string") {
-                                    if (En.addDefaultProtocol && Fn.startsWith("www.")) {
-                                        const cr = Fn.match(/\./g);
-                                        (cr == null ? void 0 : cr.length) >= 2 && (Fn = `http://${Fn}`);
+                                if (Sn && typeof Dn == "string") {
+                                    if (Sn.addDefaultProtocol && Dn.startsWith("www.")) {
+                                        const cr = Dn.match(/\./g);
+                                        (cr == null ? void 0 : cr.length) >= 2 && (Dn = `http://${Dn}`);
                                     }
-                                    if (En.tryConvertEncoding)
+                                    if (Sn.tryConvertEncoding)
                                         try {
-                                            Fn = xn(Fn);
+                                            Dn = xn(Dn);
                                         } catch {}
                                 }
-                                const Dn = wn ? new URL(Fn, wn) : new URL(Fn);
-                                if (un(Dn))
-                                    return Dn;
+                                const jn = wn ? new URL(Dn, wn) : new URL(Dn);
+                                if (un(jn))
+                                    return jn;
                             } catch {}
                             return null;
                         }
 
-                        function Xt(Fn, wn, En, Dn = !1) {
-                            return Object.defineProperty(Fn, wn, {
-                                value: En,
-                                enumerable: !Dn,
+                        function Xt(Dn, wn, Sn, jn = !1) {
+                            return Object.defineProperty(Dn, wn, {
+                                value: Sn,
+                                enumerable: !jn,
                                 configurable: !0,
                                 writable: !1
-                            }), En;
+                            }), Sn;
                         }
                         const Ht = function() {
-                            function Fn(wn, En) {
-                                this.constructor === Fn && pn("Cannot initialize BaseException."), this.message = wn, this.name = En;
+                            function Dn(wn, Sn) {
+                                this.constructor === Dn && pn("Cannot initialize BaseException."), this.message = wn, this.name = Sn;
                             }
-                            return Fn.prototype = new Error(), Fn.constructor = Fn, Fn;
+                            return Dn.prototype = new Error(), Dn.constructor = Dn, Dn;
                         }();
                         it.BaseException = Ht;
                         class Dt extends Ht {
-                            constructor(wn, En) {
-                                super(wn, "PasswordException"), this.code = En;
+                            constructor(wn, Sn) {
+                                super(wn, "PasswordException"), this.code = Sn;
                             }
                         }
                         it.PasswordException = Dt;
                         class Bt extends Ht {
-                            constructor(wn, En) {
-                                super(wn, "UnknownErrorException"), this.details = En;
+                            constructor(wn, Sn) {
+                                super(wn, "UnknownErrorException"), this.details = Sn;
                             }
                         }
                         it.UnknownErrorException = Bt;
                         class Wt extends Ht {
                             constructor(wn) {
                                 super(wn, "InvalidPDFException");
                             }
@@ -36508,16 +36508,16 @@
                         class Yt extends Ht {
                             constructor(wn) {
                                 super(wn, "MissingPDFException");
                             }
                         }
                         it.MissingPDFException = Yt;
                         class on extends Ht {
-                            constructor(wn, En) {
-                                super(wn, "UnexpectedResponseException"), this.status = En;
+                            constructor(wn, Sn) {
+                                super(wn, "UnexpectedResponseException"), this.status = Sn;
                             }
                         }
                         it.UnexpectedResponseException = on;
                         class rn extends Ht {
                             constructor(wn) {
                                 super(wn, "FormatError");
                             }
@@ -36526,56 +36526,56 @@
                         class mn extends Ht {
                             constructor(wn) {
                                 super(wn, "AbortException");
                             }
                         }
                         it.AbortException = mn;
 
-                        function _n(Fn) {
-                            (typeof Fn != "object" || (Fn == null ? void 0 : Fn.length) === void 0) && pn("Invalid argument for bytesToString");
-                            const wn = Fn.length,
-                                En = 8192;
-                            if (wn < En)
-                                return String.fromCharCode.apply(null, Fn);
-                            const Dn = [];
-                            for (let cr = 0; cr < wn; cr += En) {
-                                const Tn = Math.min(cr + En, wn),
-                                    In = Fn.subarray(cr, Tn);
-                                Dn.push(String.fromCharCode.apply(null, In));
+                        function _n(Dn) {
+                            (typeof Dn != "object" || (Dn == null ? void 0 : Dn.length) === void 0) && pn("Invalid argument for bytesToString");
+                            const wn = Dn.length,
+                                Sn = 8192;
+                            if (wn < Sn)
+                                return String.fromCharCode.apply(null, Dn);
+                            const jn = [];
+                            for (let cr = 0; cr < wn; cr += Sn) {
+                                const Tn = Math.min(cr + Sn, wn),
+                                    In = Dn.subarray(cr, Tn);
+                                jn.push(String.fromCharCode.apply(null, In));
                             }
-                            return Dn.join("");
+                            return jn.join("");
                         }
 
-                        function Sn(Fn) {
-                            typeof Fn != "string" && pn("Invalid argument for stringToBytes");
-                            const wn = Fn.length,
-                                En = new Uint8Array(wn);
-                            for (let Dn = 0; Dn < wn; ++Dn)
-                                En[Dn] = Fn.charCodeAt(Dn) & 255;
-                            return En;
+                        function yn(Dn) {
+                            typeof Dn != "string" && pn("Invalid argument for stringToBytes");
+                            const wn = Dn.length,
+                                Sn = new Uint8Array(wn);
+                            for (let jn = 0; jn < wn; ++jn)
+                                Sn[jn] = Dn.charCodeAt(jn) & 255;
+                            return Sn;
                         }
 
-                        function Cn(Fn) {
-                            return String.fromCharCode(Fn >> 24 & 255, Fn >> 16 & 255, Fn >> 8 & 255, Fn & 255);
+                        function Cn(Dn) {
+                            return String.fromCharCode(Dn >> 24 & 255, Dn >> 16 & 255, Dn >> 8 & 255, Dn & 255);
                         }
 
-                        function kn(Fn) {
-                            return Object.keys(Fn).length;
+                        function kn(Dn) {
+                            return Object.keys(Dn).length;
                         }
 
-                        function Pn(Fn) {
+                        function Pn(Dn) {
                             const wn = /* @__PURE__ */ Object.create(null);
-                            for (const [En, Dn] of Fn)
-                                wn[En] = Dn;
+                            for (const [Sn, jn] of Dn)
+                                wn[Sn] = jn;
                             return wn;
                         }
 
                         function Mn() {
-                            const Fn = new Uint8Array(4);
-                            return Fn[0] = 1, new Uint32Array(Fn.buffer, 0, 1)[0] === 1;
+                            const Dn = new Uint8Array(4);
+                            return Dn[0] = 1, new Uint32Array(Dn.buffer, 0, 1)[0] === 1;
                         }
 
                         function Wn() {
                             try {
                                 return new Function(""), !0;
                             } catch {
                                 return !1;
@@ -36597,185 +36597,185 @@
                                     isMac: !1
                                 }) : Xt(this, "platform", {
                                     isWin: navigator.platform.includes("Win"),
                                     isMac: navigator.platform.includes("Mac")
                                 });
                             }
                             static get isCSSRoundSupported() {
-                                var wn, En;
-                                return Xt(this, "isCSSRoundSupported", (En = (wn = globalThis.CSS) == null ? void 0 : wn.supports) == null ? void 0 : En.call(wn, "width: round(1.5px, 1px)"));
+                                var wn, Sn;
+                                return Xt(this, "isCSSRoundSupported", (Sn = (wn = globalThis.CSS) == null ? void 0 : wn.supports) == null ? void 0 : Sn.call(wn, "width: round(1.5px, 1px)"));
                             }
                         }
                         it.FeatureTest = Rn;
-                        const yn = [...Array(256).keys()].map((Fn) => Fn.toString(16).padStart(2, "0"));
-                        class jn {
-                            static makeHexColor(wn, En, Dn) {
-                                return `#${yn[wn]}${yn[En]}${yn[Dn]}`;
-                            }
-                            static scaleMinMax(wn, En) {
-                                let Dn;
-                                wn[0] ? (wn[0] < 0 && (Dn = En[0], En[0] = En[1], En[1] = Dn), En[0] *= wn[0], En[1] *= wn[0], wn[3] < 0 && (Dn = En[2], En[2] = En[3], En[3] = Dn), En[2] *= wn[3], En[3] *= wn[3]) : (Dn = En[0], En[0] = En[2], En[2] = Dn, Dn = En[1], En[1] = En[3], En[3] = Dn, wn[1] < 0 && (Dn = En[2], En[2] = En[3], En[3] = Dn), En[2] *= wn[1], En[3] *= wn[1], wn[2] < 0 && (Dn = En[0], En[0] = En[1], En[1] = Dn), En[0] *= wn[2], En[1] *= wn[2]), En[0] += wn[4], En[1] += wn[4], En[2] += wn[5], En[3] += wn[5];
-                            }
-                            static transform(wn, En) {
-                                return [wn[0] * En[0] + wn[2] * En[1], wn[1] * En[0] + wn[3] * En[1], wn[0] * En[2] + wn[2] * En[3], wn[1] * En[2] + wn[3] * En[3], wn[0] * En[4] + wn[2] * En[5] + wn[4], wn[1] * En[4] + wn[3] * En[5] + wn[5]];
-                            }
-                            static applyTransform(wn, En) {
-                                const Dn = wn[0] * En[0] + wn[1] * En[2] + En[4],
-                                    cr = wn[0] * En[1] + wn[1] * En[3] + En[5];
-                                return [Dn, cr];
-                            }
-                            static applyInverseTransform(wn, En) {
-                                const Dn = En[0] * En[3] - En[1] * En[2],
-                                    cr = (wn[0] * En[3] - wn[1] * En[2] + En[2] * En[5] - En[4] * En[3]) / Dn,
-                                    Tn = (-wn[0] * En[1] + wn[1] * En[0] + En[4] * En[1] - En[5] * En[0]) / Dn;
+                        const Fn = [...Array(256).keys()].map((Dn) => Dn.toString(16).padStart(2, "0"));
+                        class En {
+                            static makeHexColor(wn, Sn, jn) {
+                                return `#${Fn[wn]}${Fn[Sn]}${Fn[jn]}`;
+                            }
+                            static scaleMinMax(wn, Sn) {
+                                let jn;
+                                wn[0] ? (wn[0] < 0 && (jn = Sn[0], Sn[0] = Sn[1], Sn[1] = jn), Sn[0] *= wn[0], Sn[1] *= wn[0], wn[3] < 0 && (jn = Sn[2], Sn[2] = Sn[3], Sn[3] = jn), Sn[2] *= wn[3], Sn[3] *= wn[3]) : (jn = Sn[0], Sn[0] = Sn[2], Sn[2] = jn, jn = Sn[1], Sn[1] = Sn[3], Sn[3] = jn, wn[1] < 0 && (jn = Sn[2], Sn[2] = Sn[3], Sn[3] = jn), Sn[2] *= wn[1], Sn[3] *= wn[1], wn[2] < 0 && (jn = Sn[0], Sn[0] = Sn[1], Sn[1] = jn), Sn[0] *= wn[2], Sn[1] *= wn[2]), Sn[0] += wn[4], Sn[1] += wn[4], Sn[2] += wn[5], Sn[3] += wn[5];
+                            }
+                            static transform(wn, Sn) {
+                                return [wn[0] * Sn[0] + wn[2] * Sn[1], wn[1] * Sn[0] + wn[3] * Sn[1], wn[0] * Sn[2] + wn[2] * Sn[3], wn[1] * Sn[2] + wn[3] * Sn[3], wn[0] * Sn[4] + wn[2] * Sn[5] + wn[4], wn[1] * Sn[4] + wn[3] * Sn[5] + wn[5]];
+                            }
+                            static applyTransform(wn, Sn) {
+                                const jn = wn[0] * Sn[0] + wn[1] * Sn[2] + Sn[4],
+                                    cr = wn[0] * Sn[1] + wn[1] * Sn[3] + Sn[5];
+                                return [jn, cr];
+                            }
+                            static applyInverseTransform(wn, Sn) {
+                                const jn = Sn[0] * Sn[3] - Sn[1] * Sn[2],
+                                    cr = (wn[0] * Sn[3] - wn[1] * Sn[2] + Sn[2] * Sn[5] - Sn[4] * Sn[3]) / jn,
+                                    Tn = (-wn[0] * Sn[1] + wn[1] * Sn[0] + Sn[4] * Sn[1] - Sn[5] * Sn[0]) / jn;
                                 return [cr, Tn];
                             }
-                            static getAxialAlignedBoundingBox(wn, En) {
-                                const Dn = this.applyTransform(wn, En),
-                                    cr = this.applyTransform(wn.slice(2, 4), En),
-                                    Tn = this.applyTransform([wn[0], wn[3]], En),
-                                    In = this.applyTransform([wn[2], wn[1]], En);
-                                return [Math.min(Dn[0], cr[0], Tn[0], In[0]), Math.min(Dn[1], cr[1], Tn[1], In[1]), Math.max(Dn[0], cr[0], Tn[0], In[0]), Math.max(Dn[1], cr[1], Tn[1], In[1])];
+                            static getAxialAlignedBoundingBox(wn, Sn) {
+                                const jn = this.applyTransform(wn, Sn),
+                                    cr = this.applyTransform(wn.slice(2, 4), Sn),
+                                    Tn = this.applyTransform([wn[0], wn[3]], Sn),
+                                    In = this.applyTransform([wn[2], wn[1]], Sn);
+                                return [Math.min(jn[0], cr[0], Tn[0], In[0]), Math.min(jn[1], cr[1], Tn[1], In[1]), Math.max(jn[0], cr[0], Tn[0], In[0]), Math.max(jn[1], cr[1], Tn[1], In[1])];
                             }
                             static inverseTransform(wn) {
-                                const En = wn[0] * wn[3] - wn[1] * wn[2];
-                                return [wn[3] / En, -wn[1] / En, -wn[2] / En, wn[0] / En, (wn[2] * wn[5] - wn[4] * wn[3]) / En, (wn[4] * wn[1] - wn[5] * wn[0]) / En];
+                                const Sn = wn[0] * wn[3] - wn[1] * wn[2];
+                                return [wn[3] / Sn, -wn[1] / Sn, -wn[2] / Sn, wn[0] / Sn, (wn[2] * wn[5] - wn[4] * wn[3]) / Sn, (wn[4] * wn[1] - wn[5] * wn[0]) / Sn];
                             }
                             static singularValueDecompose2dScale(wn) {
-                                const En = [wn[0], wn[2], wn[1], wn[3]],
-                                    Dn = wn[0] * En[0] + wn[1] * En[2],
-                                    cr = wn[0] * En[1] + wn[1] * En[3],
-                                    Tn = wn[2] * En[0] + wn[3] * En[2],
-                                    In = wn[2] * En[1] + wn[3] * En[3],
-                                    Qn = (Dn + In) / 2,
-                                    or = Math.sqrt((Dn + In) ** 2 - 4 * (Dn * In - Tn * cr)) / 2,
+                                const Sn = [wn[0], wn[2], wn[1], wn[3]],
+                                    jn = wn[0] * Sn[0] + wn[1] * Sn[2],
+                                    cr = wn[0] * Sn[1] + wn[1] * Sn[3],
+                                    Tn = wn[2] * Sn[0] + wn[3] * Sn[2],
+                                    In = wn[2] * Sn[1] + wn[3] * Sn[3],
+                                    Qn = (jn + In) / 2,
+                                    or = Math.sqrt((jn + In) ** 2 - 4 * (jn * In - Tn * cr)) / 2,
                                     Xn = Qn + or || 1,
                                     Vn = Qn - or || 1;
                                 return [Math.sqrt(Xn), Math.sqrt(Vn)];
                             }
                             static normalizeRect(wn) {
-                                const En = wn.slice(0);
-                                return wn[0] > wn[2] && (En[0] = wn[2], En[2] = wn[0]), wn[1] > wn[3] && (En[1] = wn[3], En[3] = wn[1]), En;
+                                const Sn = wn.slice(0);
+                                return wn[0] > wn[2] && (Sn[0] = wn[2], Sn[2] = wn[0]), wn[1] > wn[3] && (Sn[1] = wn[3], Sn[3] = wn[1]), Sn;
                             }
-                            static intersect(wn, En) {
-                                const Dn = Math.max(Math.min(wn[0], wn[2]), Math.min(En[0], En[2])),
-                                    cr = Math.min(Math.max(wn[0], wn[2]), Math.max(En[0], En[2]));
-                                if (Dn > cr)
+                            static intersect(wn, Sn) {
+                                const jn = Math.max(Math.min(wn[0], wn[2]), Math.min(Sn[0], Sn[2])),
+                                    cr = Math.min(Math.max(wn[0], wn[2]), Math.max(Sn[0], Sn[2]));
+                                if (jn > cr)
                                     return null;
-                                const Tn = Math.max(Math.min(wn[1], wn[3]), Math.min(En[1], En[3])),
-                                    In = Math.min(Math.max(wn[1], wn[3]), Math.max(En[1], En[3]));
-                                return Tn > In ? null : [Dn, Tn, cr, In];
+                                const Tn = Math.max(Math.min(wn[1], wn[3]), Math.min(Sn[1], Sn[3])),
+                                    In = Math.min(Math.max(wn[1], wn[3]), Math.max(Sn[1], Sn[3]));
+                                return Tn > In ? null : [jn, Tn, cr, In];
                             }
-                            static bezierBoundingBox(wn, En, Dn, cr, Tn, In, Qn, or) {
+                            static bezierBoundingBox(wn, Sn, jn, cr, Tn, In, Qn, or) {
                                 const Xn = [],
                                     Vn = [
                                         [],
                                         []
                                     ];
                                 let hr, Nn, Kn, Jn, gr, rr, nn, qt;
                                 for (let $n = 0; $n < 2; ++$n) {
-                                    if ($n === 0 ? (Nn = 6 * wn - 12 * Dn + 6 * Tn, hr = -3 * wn + 9 * Dn - 9 * Tn + 3 * Qn, Kn = 3 * Dn - 3 * wn) : (Nn = 6 * En - 12 * cr + 6 * In, hr = -3 * En + 9 * cr - 9 * In + 3 * or, Kn = 3 * cr - 3 * En), Math.abs(hr) < 1e-12) {
+                                    if ($n === 0 ? (Nn = 6 * wn - 12 * jn + 6 * Tn, hr = -3 * wn + 9 * jn - 9 * Tn + 3 * Qn, Kn = 3 * jn - 3 * wn) : (Nn = 6 * Sn - 12 * cr + 6 * In, hr = -3 * Sn + 9 * cr - 9 * In + 3 * or, Kn = 3 * cr - 3 * Sn), Math.abs(hr) < 1e-12) {
                                         if (Math.abs(Nn) < 1e-12)
                                             continue;
                                         Jn = -Kn / Nn, 0 < Jn && Jn < 1 && Xn.push(Jn);
                                         continue;
                                     }
                                     nn = Nn * Nn - 4 * Kn * hr, qt = Math.sqrt(nn), !(nn < 0) && (gr = (-Nn + qt) / (2 * hr), 0 < gr && gr < 1 && Xn.push(gr), rr = (-Nn - qt) / (2 * hr), 0 < rr && rr < 1 && Xn.push(rr));
                                 }
                                 let dn = Xn.length,
-                                    gn;
-                                const vn = dn;
+                                    vn;
+                                const bn = dn;
                                 for (; dn--;)
-                                    Jn = Xn[dn], gn = 1 - Jn, Vn[0][dn] = gn * gn * gn * wn + 3 * gn * gn * Jn * Dn + 3 * gn * Jn * Jn * Tn + Jn * Jn * Jn * Qn, Vn[1][dn] = gn * gn * gn * En + 3 * gn * gn * Jn * cr + 3 * gn * Jn * Jn * In + Jn * Jn * Jn * or;
-                                return Vn[0][vn] = wn, Vn[1][vn] = En, Vn[0][vn + 1] = Qn, Vn[1][vn + 1] = or, Vn[0].length = Vn[1].length = vn + 2, [Math.min(...Vn[0]), Math.min(...Vn[1]), Math.max(...Vn[0]), Math.max(...Vn[1])];
+                                    Jn = Xn[dn], vn = 1 - Jn, Vn[0][dn] = vn * vn * vn * wn + 3 * vn * vn * Jn * jn + 3 * vn * Jn * Jn * Tn + Jn * Jn * Jn * Qn, Vn[1][dn] = vn * vn * vn * Sn + 3 * vn * vn * Jn * cr + 3 * vn * Jn * Jn * In + Jn * Jn * Jn * or;
+                                return Vn[0][bn] = wn, Vn[1][bn] = Sn, Vn[0][bn + 1] = Qn, Vn[1][bn + 1] = or, Vn[0].length = Vn[1].length = bn + 2, [Math.min(...Vn[0]), Math.min(...Vn[1]), Math.max(...Vn[0]), Math.max(...Vn[1])];
                             }
                         }
-                        it.Util = jn;
+                        it.Util = En;
                         const An = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 728, 711, 710, 729, 733, 731, 730, 732, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 8226, 8224, 8225, 8230, 8212, 8211, 402, 8260, 8249, 8250, 8722, 8240, 8222, 8220, 8221, 8216, 8217, 8218, 8482, 64257, 64258, 321, 338, 352, 376, 381, 305, 322, 339, 353, 382, 0, 8364];
 
-                        function bn(Fn) {
-                            if (Fn[0] >= "ï") {
-                                let En;
-                                if (Fn[0] === "þ" && Fn[1] === "ÿ" ? En = "utf-16be" : Fn[0] === "ÿ" && Fn[1] === "þ" ? En = "utf-16le" : Fn[0] === "ï" && Fn[1] === "»" && Fn[2] === "¿" && (En = "utf-8"), En)
+                        function gn(Dn) {
+                            if (Dn[0] >= "ï") {
+                                let Sn;
+                                if (Dn[0] === "þ" && Dn[1] === "ÿ" ? Sn = "utf-16be" : Dn[0] === "ÿ" && Dn[1] === "þ" ? Sn = "utf-16le" : Dn[0] === "ï" && Dn[1] === "»" && Dn[2] === "¿" && (Sn = "utf-8"), Sn)
                                     try {
-                                        const Dn = new TextDecoder(En, {
+                                        const jn = new TextDecoder(Sn, {
                                                 fatal: !0
                                             }),
-                                            cr = Sn(Fn);
-                                        return Dn.decode(cr);
-                                    } catch (Dn) {
-                                        Jt(`stringToPDFString: "${Dn}".`);
+                                            cr = yn(Dn);
+                                        return jn.decode(cr);
+                                    } catch (jn) {
+                                        Jt(`stringToPDFString: "${jn}".`);
                                     }
                             }
                             const wn = [];
-                            for (let En = 0, Dn = Fn.length; En < Dn; En++) {
-                                const cr = An[Fn.charCodeAt(En)];
-                                wn.push(cr ? String.fromCharCode(cr) : Fn.charAt(En));
+                            for (let Sn = 0, jn = Dn.length; Sn < jn; Sn++) {
+                                const cr = An[Dn.charCodeAt(Sn)];
+                                wn.push(cr ? String.fromCharCode(cr) : Dn.charAt(Sn));
                             }
                             return wn.join("");
                         }
 
-                        function xn(Fn) {
-                            return decodeURIComponent(escape(Fn));
+                        function xn(Dn) {
+                            return decodeURIComponent(escape(Dn));
                         }
 
-                        function zn(Fn) {
-                            return unescape(encodeURIComponent(Fn));
+                        function zn(Dn) {
+                            return unescape(encodeURIComponent(Dn));
                         }
 
-                        function On(Fn) {
-                            return typeof Fn == "object" && (Fn == null ? void 0 : Fn.byteLength) !== void 0;
+                        function On(Dn) {
+                            return typeof Dn == "object" && (Dn == null ? void 0 : Dn.byteLength) !== void 0;
                         }
 
-                        function Un(Fn, wn) {
-                            if (Fn.length !== wn.length)
+                        function Un(Dn, wn) {
+                            if (Dn.length !== wn.length)
                                 return !1;
-                            for (let En = 0, Dn = Fn.length; En < Dn; En++)
-                                if (Fn[En] !== wn[En])
+                            for (let Sn = 0, jn = Dn.length; Sn < jn; Sn++)
+                                if (Dn[Sn] !== wn[Sn])
                                     return !1;
                             return !0;
                         }
 
-                        function Gn(Fn = /* @__PURE__ */ new Date()) {
-                            return [Fn.getUTCFullYear().toString(), (Fn.getUTCMonth() + 1).toString().padStart(2, "0"), Fn.getUTCDate().toString().padStart(2, "0"), Fn.getUTCHours().toString().padStart(2, "0"), Fn.getUTCMinutes().toString().padStart(2, "0"), Fn.getUTCSeconds().toString().padStart(2, "0")].join("");
+                        function Gn(Dn = /* @__PURE__ */ new Date()) {
+                            return [Dn.getUTCFullYear().toString(), (Dn.getUTCMonth() + 1).toString().padStart(2, "0"), Dn.getUTCDate().toString().padStart(2, "0"), Dn.getUTCHours().toString().padStart(2, "0"), Dn.getUTCMinutes().toString().padStart(2, "0"), Dn.getUTCSeconds().toString().padStart(2, "0")].join("");
                         }
                         class Zn {
                             constructor() {
-                                Ut(this, ft, !1), this.promise = new Promise((wn, En) => {
-                                    this.resolve = (Dn) => {
-                                        sn(this, ft, !0), wn(Dn);
-                                    }, this.reject = (Dn) => {
-                                        sn(this, ft, !0), En(Dn);
+                                Ut(this, ft, !1), this.promise = new Promise((wn, Sn) => {
+                                    this.resolve = (jn) => {
+                                        sn(this, ft, !0), wn(jn);
+                                    }, this.reject = (jn) => {
+                                        sn(this, ft, !0), Sn(jn);
                                     };
                                 });
                             }
                             get settled() {
                                 return St(this, ft);
                             }
                         }
                         ft = /* @__PURE__ */ new WeakMap(), it.PromiseCapability = Zn;
                         let Yn = null,
                             lr = null;
 
-                        function ur(Fn) {
+                        function ur(Dn) {
                             return Yn || (Yn = /([\u00a0\u00b5\u037e\u0eb3\u2000-\u200a\u202f\u2126\ufb00-\ufb04\ufb06\ufb20-\ufb36\ufb38-\ufb3c\ufb3e\ufb40-\ufb41\ufb43-\ufb44\ufb46-\ufba1\ufba4-\ufba9\ufbae-\ufbb1\ufbd3-\ufbdc\ufbde-\ufbe7\ufbea-\ufbf8\ufbfc-\ufbfd\ufc00-\ufc5d\ufc64-\ufcf1\ufcf5-\ufd3d\ufd88\ufdf4\ufdfa-\ufdfb\ufe71\ufe77\ufe79\ufe7b\ufe7d]+)|(\ufb05+)/gu, lr = /* @__PURE__ */ new Map([
                                 ["ﬅ", "ſt"]
-                            ])), Fn.replaceAll(Yn, (wn, En, Dn) => En ? En.normalize("NFKC") : lr.get(Dn));
+                            ])), Dn.replaceAll(Yn, (wn, Sn, jn) => Sn ? Sn.normalize("NFKC") : lr.get(jn));
                         }
 
                         function nr() {
                             if (typeof crypto < "u" && typeof(crypto == null ? void 0 : crypto.randomUUID) == "function")
                                 return crypto.randomUUID();
-                            const Fn = new Uint8Array(32);
+                            const Dn = new Uint8Array(32);
                             if (typeof crypto < "u" && typeof(crypto == null ? void 0 : crypto.getRandomValues) == "function")
-                                crypto.getRandomValues(Fn);
+                                crypto.getRandomValues(Dn);
                             else
                                 for (let wn = 0; wn < 32; wn++)
-                                    Fn[wn] = Math.floor(Math.random() * 255);
-                            return _n(Fn);
+                                    Dn[wn] = Math.floor(Math.random() * 255);
+                            return _n(Dn);
                         }
                         const sr = "pdfjs_internal_id_";
                         it.AnnotationPrefix = sr;
                     },
                     /* 2 */
                     /***/
                     (__unused_webpack_module, exports, __w_pdfjs_require__) => {
@@ -38345,16 +38345,16 @@
                                         pageWidth: Yt,
                                         pageHeight: on,
                                         pageX: rn,
                                         pageY: mn
                                     }
                                 } = this.parent.viewport;
                                 this.rotation = Wt, this.pageRotation = (360 + Wt - this._uiManager.viewParameters.rotation) % 360, this.pageDimensions = [Yt, on], this.pageTranslation = [rn, mn];
-                                const [_n, Sn] = this.parentDimensions;
-                                this.x = Bt.x / _n, this.y = Bt.y / Sn, this.isAttachedToDOM = !1, this.deleted = !1;
+                                const [_n, yn] = this.parentDimensions;
+                                this.x = Bt.x / _n, this.y = Bt.y / yn, this.isAttachedToDOM = !1, this.deleted = !1;
                             }
                             get editorType() {
                                 return Object.getPrototypeOf(this).constructor._type;
                             }
                             static get _defaultLineColor() {
                                 return (0, hn.shadow)(this, "_defaultLineColor", this._colorManager.getHexCode("CanvasText"));
                             }
@@ -38468,16 +38468,16 @@
                                     } = this.div.getBoundingClientRect();
                                     this.parent.findNewParent(this, Cn, kn) && (this.x -= Math.floor(this.x), this.y -= Math.floor(this.y));
                                 }
                                 let {
                                     x: rn,
                                     y: mn
                                 } = this;
-                                const [_n, Sn] = tn(this, Tt, Ot).call(this);
-                                rn += _n, mn += Sn, this.div.style.left = `${(100 * rn).toFixed(2)}%`, this.div.style.top = `${(100 * mn).toFixed(2)}%`, this.div.scrollIntoView({
+                                const [_n, yn] = tn(this, Tt, Ot).call(this);
+                                rn += _n, mn += yn, this.div.style.left = `${(100 * rn).toFixed(2)}%`, this.div.style.top = `${(100 * mn).toFixed(2)}%`, this.div.scrollIntoView({
                                     block: "nearest"
                                 });
                             }
                             fixAndSetPosition() {
                                 const [Bt, Wt] = this.pageDimensions;
                                 let {
                                     x: Yt,
@@ -38496,16 +38496,16 @@
                                         Yt = Math.min(Bt, Math.max(rn, Yt)), on = Math.min(Wt, Math.max(mn, on));
                                         break;
                                     case 270:
                                         Yt = Math.min(Bt, Math.max(mn, Yt)), on = Math.max(0, Math.min(Wt - rn, on));
                                         break;
                                 }
                                 this.x = Yt /= Bt, this.y = on /= Wt;
-                                const [_n, Sn] = tn(this, Tt, Ot).call(this);
-                                Yt += _n, on += Sn;
+                                const [_n, yn] = tn(this, Tt, Ot).call(this);
+                                Yt += _n, on += yn;
                                 const {
                                     style: Cn
                                 } = this.div;
                                 Cn.left = `${(100 * Yt).toFixed(2)}%`, Cn.top = `${(100 * on).toFixed(2)}%`, this.moveInDOM();
                             }
                             screenToPageTranslation(Bt, Wt) {
                                 var Yt;
@@ -38601,44 +38601,44 @@
                             _setParentAndPosition(Bt, Wt, Yt) {
                                 Bt.changeParent(this), this.x = Wt, this.y = Yt, this.fixAndSetPosition();
                             }
                             getRect(Bt, Wt) {
                                 const Yt = this.parentScale,
                                     [on, rn] = this.pageDimensions,
                                     [mn, _n] = this.pageTranslation,
-                                    Sn = Bt / Yt,
+                                    yn = Bt / Yt,
                                     Cn = Wt / Yt,
                                     kn = this.x * on,
                                     Pn = this.y * rn,
                                     Mn = this.width * on,
                                     Wn = this.height * rn;
                                 switch (this.rotation) {
                                     case 0:
-                                        return [kn + Sn + mn, rn - Pn - Cn - Wn + _n, kn + Sn + Mn + mn, rn - Pn - Cn + _n];
+                                        return [kn + yn + mn, rn - Pn - Cn - Wn + _n, kn + yn + Mn + mn, rn - Pn - Cn + _n];
                                     case 90:
-                                        return [kn + Cn + mn, rn - Pn + Sn + _n, kn + Cn + Wn + mn, rn - Pn + Sn + Mn + _n];
+                                        return [kn + Cn + mn, rn - Pn + yn + _n, kn + Cn + Wn + mn, rn - Pn + yn + Mn + _n];
                                     case 180:
-                                        return [kn - Sn - Mn + mn, rn - Pn + Cn + _n, kn - Sn + mn, rn - Pn + Cn + Wn + _n];
+                                        return [kn - yn - Mn + mn, rn - Pn + Cn + _n, kn - yn + mn, rn - Pn + Cn + Wn + _n];
                                     case 270:
-                                        return [kn - Cn - Wn + mn, rn - Pn - Sn - Mn + _n, kn - Cn + mn, rn - Pn - Sn + _n];
+                                        return [kn - Cn - Wn + mn, rn - Pn - yn - Mn + _n, kn - Cn + mn, rn - Pn - yn + _n];
                                     default:
                                         throw new Error("Invalid rotation");
                                 }
                             }
                             getRectInCurrentCoords(Bt, Wt) {
-                                const [Yt, on, rn, mn] = Bt, _n = rn - Yt, Sn = mn - on;
+                                const [Yt, on, rn, mn] = Bt, _n = rn - Yt, yn = mn - on;
                                 switch (this.rotation) {
                                     case 0:
-                                        return [Yt, Wt - mn, _n, Sn];
+                                        return [Yt, Wt - mn, _n, yn];
                                     case 90:
-                                        return [Yt, Wt - on, Sn, _n];
+                                        return [Yt, Wt - on, yn, _n];
                                     case 180:
-                                        return [rn, Wt - on, _n, Sn];
+                                        return [rn, Wt - on, _n, yn];
                                     case 270:
-                                        return [rn, Wt - mn, Sn, _n];
+                                        return [rn, Wt - mn, yn, _n];
                                     default:
                                         throw new Error("Invalid rotation");
                                 }
                             }
                             onceAdded() {}
                             isEmpty() {
                                 return !1;
@@ -38668,16 +38668,16 @@
                             static deserialize(Bt, Wt, Yt) {
                                 const on = new this.prototype.constructor({
                                     parent: Wt,
                                     id: Wt.getNextId(),
                                     uiManager: Yt
                                 });
                                 on.rotation = Bt.rotation;
-                                const [rn, mn] = on.pageDimensions, [_n, Sn, Cn, kn] = on.getRectInCurrentCoords(Bt.rect, mn);
-                                return on.x = _n / rn, on.y = Sn / mn, on.width = Cn / rn, on.height = kn / mn, on;
+                                const [rn, mn] = on.pageDimensions, [_n, yn, Cn, kn] = on.getRectInCurrentCoords(Bt.rect, mn);
+                                return on.x = _n / rn, on.y = yn / mn, on.width = Cn / rn, on.height = kn / mn, on;
                             }
                             remove() {
                                 var Bt;
                                 this.div.removeEventListener("focusin", St(this, wt)), this.div.removeEventListener("focusout", St(this, $t)), this.isEmpty() || this.commit(), this.parent ? this.parent.remove(this) : this._uiManager.removeEditor(this), (Bt = St(this, bt)) == null || Bt.remove(), sn(this, bt, null), sn(this, _t, null);
                             }
                             get isResizable() {
                                 return !1;
@@ -38788,89 +38788,89 @@
                             const rn = {
                                 passive: !0,
                                 capture: !0
                             };
                             window.addEventListener("pointermove", Yt, rn);
                             const mn = this.x,
                                 _n = this.y,
-                                Sn = this.width,
+                                yn = this.width,
                                 Cn = this.height,
                                 kn = this.parent.div.style.cursor,
                                 Pn = this.div.style.cursor;
                             this.div.style.cursor = this.parent.div.style.cursor = window.getComputedStyle(Bt.target).cursor;
                             const Mn = () => {
                                 this._isDraggable = on, window.removeEventListener("pointerup", Mn), window.removeEventListener("blur", Mn), window.removeEventListener("pointermove", Yt, rn), this.parent.div.style.cursor = kn, this.div.style.cursor = Pn;
                                 const Wn = this.x,
                                     Rn = this.y,
-                                    yn = this.width,
-                                    jn = this.height;
-                                Wn === mn && Rn === _n && yn === Sn && jn === Cn || this.addCommands({
+                                    Fn = this.width,
+                                    En = this.height;
+                                Wn === mn && Rn === _n && Fn === yn && En === Cn || this.addCommands({
                                     cmd: () => {
-                                        this.width = yn, this.height = jn, this.x = Wn, this.y = Rn;
-                                        const [An, bn] = this.parentDimensions;
-                                        this.setDims(An * yn, bn * jn), this.fixAndSetPosition();
+                                        this.width = Fn, this.height = En, this.x = Wn, this.y = Rn;
+                                        const [An, gn] = this.parentDimensions;
+                                        this.setDims(An * Fn, gn * En), this.fixAndSetPosition();
                                     },
                                     undo: () => {
-                                        this.width = Sn, this.height = Cn, this.x = mn, this.y = _n;
-                                        const [An, bn] = this.parentDimensions;
-                                        this.setDims(An * Sn, bn * Cn), this.fixAndSetPosition();
+                                        this.width = yn, this.height = Cn, this.x = mn, this.y = _n;
+                                        const [An, gn] = this.parentDimensions;
+                                        this.setDims(An * yn, gn * Cn), this.fixAndSetPosition();
                                     },
                                     mustExec: !0
                                 });
                             };
                             window.addEventListener("pointerup", Mn), window.addEventListener("blur", Mn);
                         }, en = /* @__PURE__ */ new WeakSet(), Kt = function(Dt, Bt) {
-                            const [Wt, Yt] = this.parentDimensions, on = this.x, rn = this.y, mn = this.width, _n = this.height, Sn = ln.MIN_SIZE / Wt, Cn = ln.MIN_SIZE / Yt, kn = (En) => Math.round(En * 1e4) / 1e4, Pn = tn(this, Ft, zt).call(this, this.rotation), Mn = (En, Dn) => [Pn[0] * En + Pn[2] * Dn, Pn[1] * En + Pn[3] * Dn], Wn = tn(this, Ft, zt).call(this, 360 - this.rotation), Rn = (En, Dn) => [Wn[0] * En + Wn[2] * Dn, Wn[1] * En + Wn[3] * Dn];
-                            let yn, jn, An = !1,
-                                bn = !1;
+                            const [Wt, Yt] = this.parentDimensions, on = this.x, rn = this.y, mn = this.width, _n = this.height, yn = ln.MIN_SIZE / Wt, Cn = ln.MIN_SIZE / Yt, kn = (Sn) => Math.round(Sn * 1e4) / 1e4, Pn = tn(this, Ft, zt).call(this, this.rotation), Mn = (Sn, jn) => [Pn[0] * Sn + Pn[2] * jn, Pn[1] * Sn + Pn[3] * jn], Wn = tn(this, Ft, zt).call(this, 360 - this.rotation), Rn = (Sn, jn) => [Wn[0] * Sn + Wn[2] * jn, Wn[1] * Sn + Wn[3] * jn];
+                            let Fn, En, An = !1,
+                                gn = !1;
                             switch (Dt) {
                                 case "topLeft":
-                                    An = !0, yn = (En, Dn) => [0, 0], jn = (En, Dn) => [En, Dn];
+                                    An = !0, Fn = (Sn, jn) => [0, 0], En = (Sn, jn) => [Sn, jn];
                                     break;
                                 case "topMiddle":
-                                    yn = (En, Dn) => [En / 2, 0], jn = (En, Dn) => [En / 2, Dn];
+                                    Fn = (Sn, jn) => [Sn / 2, 0], En = (Sn, jn) => [Sn / 2, jn];
                                     break;
                                 case "topRight":
-                                    An = !0, yn = (En, Dn) => [En, 0], jn = (En, Dn) => [0, Dn];
+                                    An = !0, Fn = (Sn, jn) => [Sn, 0], En = (Sn, jn) => [0, jn];
                                     break;
                                 case "middleRight":
-                                    bn = !0, yn = (En, Dn) => [En, Dn / 2], jn = (En, Dn) => [0, Dn / 2];
+                                    gn = !0, Fn = (Sn, jn) => [Sn, jn / 2], En = (Sn, jn) => [0, jn / 2];
                                     break;
                                 case "bottomRight":
-                                    An = !0, yn = (En, Dn) => [En, Dn], jn = (En, Dn) => [0, 0];
+                                    An = !0, Fn = (Sn, jn) => [Sn, jn], En = (Sn, jn) => [0, 0];
                                     break;
                                 case "bottomMiddle":
-                                    yn = (En, Dn) => [En / 2, Dn], jn = (En, Dn) => [En / 2, 0];
+                                    Fn = (Sn, jn) => [Sn / 2, jn], En = (Sn, jn) => [Sn / 2, 0];
                                     break;
                                 case "bottomLeft":
-                                    An = !0, yn = (En, Dn) => [0, Dn], jn = (En, Dn) => [En, 0];
+                                    An = !0, Fn = (Sn, jn) => [0, jn], En = (Sn, jn) => [Sn, 0];
                                     break;
                                 case "middleLeft":
-                                    bn = !0, yn = (En, Dn) => [0, Dn / 2], jn = (En, Dn) => [En, Dn / 2];
+                                    gn = !0, Fn = (Sn, jn) => [0, jn / 2], En = (Sn, jn) => [Sn, jn / 2];
                                     break;
                             }
-                            const xn = yn(mn, _n),
-                                zn = jn(mn, _n);
+                            const xn = Fn(mn, _n),
+                                zn = En(mn, _n);
                             let On = Mn(...zn);
                             const Un = kn(on + On[0]),
                                 Gn = kn(rn + On[1]);
                             let Zn = 1,
                                 Yn = 1,
                                 [lr, ur] = this.screenToPageTranslation(Bt.movementX, Bt.movementY);
                             if ([lr, ur] = Rn(lr / Wt, ur / Yt), An) {
-                                const En = Math.hypot(mn, _n);
-                                Zn = Yn = Math.max(Math.min(Math.hypot(zn[0] - xn[0] - lr, zn[1] - xn[1] - ur) / En, 1 / mn, 1 / _n), Sn / mn, Cn / _n);
+                                const Sn = Math.hypot(mn, _n);
+                                Zn = Yn = Math.max(Math.min(Math.hypot(zn[0] - xn[0] - lr, zn[1] - xn[1] - ur) / Sn, 1 / mn, 1 / _n), yn / mn, Cn / _n);
                             } else
-                                bn ? Zn = Math.max(Sn, Math.min(1, Math.abs(zn[0] - xn[0] - lr))) / mn : Yn = Math.max(Cn, Math.min(1, Math.abs(zn[1] - xn[1] - ur))) / _n;
+                                gn ? Zn = Math.max(yn, Math.min(1, Math.abs(zn[0] - xn[0] - lr))) / mn : Yn = Math.max(Cn, Math.min(1, Math.abs(zn[1] - xn[1] - ur))) / _n;
                             const nr = kn(mn * Zn),
                                 sr = kn(_n * Yn);
-                            On = Mn(...jn(nr, sr));
-                            const Fn = Un - On[0],
+                            On = Mn(...En(nr, sr));
+                            const Dn = Un - On[0],
                                 wn = Gn - On[1];
-                            this.width = nr, this.height = sr, this.x = Fn, this.y = wn, this.setDims(Wt * nr, Yt * sr), this.fixAndSetPosition();
+                            this.width = nr, this.height = sr, this.x = Dn, this.y = wn, this.setDims(Wt * nr, Yt * sr), this.fixAndSetPosition();
                         }, an = /* @__PURE__ */ new WeakSet(), Qt = async function() {
                             var Dt;
                             const Bt = St(this, bt);
                             if (!Bt)
                                 return;
                             if (!St(this, mt) && !St(this, gt)) {
                                 Bt.classList.remove("done"), (Dt = St(this, _t)) == null || Dt.remove();
@@ -38941,24 +38941,24 @@
                                 };
                             }
                         }
                     },
                     /* 5 */
                     /***/
                     (_e, it, ft) => {
-                        var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt, cn, en, Kt, an, Qt, Zt, Jt, pn, hn, un, ln, Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, Sn, Cn, kn, Pn, Mn, Wn, Rn, yn, jn, An, bn, xn, zn, On, Un, Gn, Zn, Yn, lr, ur, nr, sr, Fn, wn, En, Dn;
+                        var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt, cn, en, Kt, an, Qt, Zt, Jt, pn, hn, un, ln, Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, yn, Cn, kn, Pn, Mn, Wn, Rn, Fn, En, An, gn, xn, zn, On, Un, Gn, Zn, Yn, lr, ur, nr, sr, Dn, wn, Sn, jn;
                         Object.defineProperty(it, "__esModule", {
                             value: !0
                         }), it.KeyboardManager = it.CommandManager = it.ColorManager = it.AnnotationEditorUIManager = void 0, it.bindEvents = In, it.opacityToHex = Qn;
                         var cr = ft(1),
                             Tn = ft(6);
 
                         function In(nn, qt, dn) {
-                            for (const gn of dn)
-                                qt.addEventListener(gn, nn[gn].bind(nn));
+                            for (const vn of dn)
+                                qt.addEventListener(vn, nn[vn].bind(nn));
                         }
 
                         function Qn(nn) {
                             return Math.round(Math.min(255, Math.max(1, 255 * nn))).toString(16).padStart(2, "0");
                         }
                         class or {
                             constructor() {
@@ -38972,27 +38972,27 @@
                         const Xn = class {
                             constructor() {
                                 Ut(this, yt), Ut(this, gt, (0, cr.getUuid)()), Ut(this, bt, 0), Ut(this, _t, null);
                             }
                             static get _isSVGFittingCanvas() {
                                 const qt = 'data:image/svg+xml;charset=UTF-8,<svg viewBox="0 0 1 1" width="1" height="1" xmlns="http://www.w3.org/2000/svg"><rect width="1" height="1" style="fill:red;"/></svg>',
                                     dn = new OffscreenCanvas(1, 3).getContext("2d"),
-                                    gn = new Image();
-                                gn.src = qt;
-                                const vn = gn.decode().then(() => (dn.drawImage(gn, 0, 0, 1, 1, 0, 0, 1, 3), new Uint32Array(dn.getImageData(0, 0, 1, 1).data.buffer)[0] === 0));
-                                return (0, cr.shadow)(this, "_isSVGFittingCanvas", vn);
+                                    vn = new Image();
+                                vn.src = qt;
+                                const bn = vn.decode().then(() => (dn.drawImage(vn, 0, 0, 1, 1, 0, 0, 1, 3), new Uint32Array(dn.getImageData(0, 0, 1, 1).data.buffer)[0] === 0));
+                                return (0, cr.shadow)(this, "_isSVGFittingCanvas", bn);
                             }
                             async getFromFile(qt) {
                                 const {
                                     lastModified: dn,
-                                    name: gn,
-                                    size: vn,
+                                    name: vn,
+                                    size: bn,
                                     type: $n
                                 } = qt;
-                                return tn(this, yt, Et).call(this, `${dn}_${gn}_${vn}_${$n}`, qt);
+                                return tn(this, yt, Et).call(this, `${dn}_${vn}_${bn}_${$n}`, qt);
                             }
                             async getFromUrl(qt) {
                                 return tn(this, yt, Et).call(this, qt, qt);
                             }
                             async getFromId(qt) {
                                 St(this, _t) || sn(this, _t, /* @__PURE__ */ new Map());
                                 const dn = St(this, _t).get(qt);
@@ -39021,69 +39021,69 @@
                             try {
                                 dn || (dn = {
                                     bitmap: null,
                                     id: `image_${St(this, gt)}_${Vr(this, bt)._++}`,
                                     refCounter: 0,
                                     isSvg: !1
                                 });
-                                let gn;
+                                let vn;
                                 if (typeof qt == "string") {
                                     dn.url = qt;
-                                    const vn = await fetch(qt);
-                                    if (!vn.ok)
-                                        throw new Error(vn.statusText);
-                                    gn = await vn.blob();
+                                    const bn = await fetch(qt);
+                                    if (!bn.ok)
+                                        throw new Error(bn.statusText);
+                                    vn = await bn.blob();
                                 } else
-                                    gn = dn.file = qt;
-                                if (gn.type === "image/svg+xml") {
-                                    const vn = Xn._isSVGFittingCanvas,
+                                    vn = dn.file = qt;
+                                if (vn.type === "image/svg+xml") {
+                                    const bn = Xn._isSVGFittingCanvas,
                                         $n = new FileReader(),
                                         Ln = new Image(),
                                         Hn = new Promise((Bn, qn) => {
                                             Ln.onload = () => {
                                                 dn.bitmap = Ln, dn.isSvg = !0, Bn();
                                             }, $n.onload = async () => {
                                                 const ir = dn.svgUrl = $n.result;
-                                                Ln.src = await vn ? `${ir}#svgView(preserveAspectRatio(none))` : ir;
+                                                Ln.src = await bn ? `${ir}#svgView(preserveAspectRatio(none))` : ir;
                                             }, Ln.onerror = $n.onerror = qn;
                                         });
-                                    $n.readAsDataURL(gn), await Hn;
+                                    $n.readAsDataURL(vn), await Hn;
                                 } else
-                                    dn.bitmap = await createImageBitmap(gn);
+                                    dn.bitmap = await createImageBitmap(vn);
                                 dn.refCounter = 1;
-                            } catch (gn) {
-                                console.error(gn), dn = null;
+                            } catch (vn) {
+                                console.error(vn), dn = null;
                             }
                             return St(this, _t).set(nn, dn), dn && St(this, _t).set(dn.id, dn), dn;
                         };
                         let Vn = Xn;
                         class hr {
                             constructor(qt = 128) {
                                 Ut(this, xt, []), Ut(this, wt, !1), Ut(this, $t, void 0), Ut(this, Ct, -1), sn(this, $t, qt);
                             }
                             add({
                                 cmd: qt,
                                 undo: dn,
-                                mustExec: gn,
-                                type: vn = NaN,
+                                mustExec: vn,
+                                type: bn = NaN,
                                 overwriteIfSameType: $n = !1,
                                 keepUndo: Ln = !1
                             }) {
-                                if (gn && qt(), St(this, wt))
+                                if (vn && qt(), St(this, wt))
                                     return;
                                 const Hn = {
                                     cmd: qt,
                                     undo: dn,
-                                    type: vn
+                                    type: bn
                                 };
                                 if (St(this, Ct) === -1) {
                                     St(this, xt).length > 0 && (St(this, xt).length = 0), sn(this, Ct, 0), St(this, xt).push(Hn);
                                     return;
                                 }
-                                if ($n && St(this, xt)[St(this, Ct)].type === vn) {
+                                if ($n && St(this, xt)[St(this, Ct)].type === bn) {
                                     Ln && (Hn.undo = St(this, xt)[St(this, Ct)].undo), St(this, xt)[St(this, Ct)] = Hn;
                                     return;
                                 }
                                 const Bn = St(this, Ct) + 1;
                                 Bn === St(this, $t) ? St(this, xt).splice(0, 1) : (sn(this, Ct, Bn), Bn < St(this, xt).length && St(this, xt).splice(Bn)), St(this, xt).push(Hn);
                             }
                             undo() {
@@ -39105,41 +39105,41 @@
                         xt = /* @__PURE__ */ new WeakMap(), wt = /* @__PURE__ */ new WeakMap(), $t = /* @__PURE__ */ new WeakMap(), Ct = /* @__PURE__ */ new WeakMap(), it.CommandManager = hr;
                         class Nn {
                             constructor(qt) {
                                 Ut(this, Rt), this.buffer = [], this.callbacks = /* @__PURE__ */ new Map(), this.allKeys = /* @__PURE__ */ new Set();
                                 const {
                                     isMac: dn
                                 } = cr.FeatureTest.platform;
-                                for (const [gn, vn, $n = {}] of qt)
-                                    for (const Ln of gn) {
+                                for (const [vn, bn, $n = {}] of qt)
+                                    for (const Ln of vn) {
                                         const Hn = Ln.startsWith("mac+");
                                         dn && Hn ? (this.callbacks.set(Ln.slice(4), {
-                                            callback: vn,
+                                            callback: bn,
                                             options: $n
                                         }), this.allKeys.add(Ln.split("+").at(-1))) : !dn && !Hn && (this.callbacks.set(Ln, {
-                                            callback: vn,
+                                            callback: bn,
                                             options: $n
                                         }), this.allKeys.add(Ln.split("+").at(-1)));
                                     }
                             }
                             exec(qt, dn) {
                                 if (!this.allKeys.has(dn.key))
                                     return;
-                                const gn = this.callbacks.get(tn(this, Rt, Mt).call(this, dn));
-                                if (!gn)
+                                const vn = this.callbacks.get(tn(this, Rt, Mt).call(this, dn));
+                                if (!vn)
                                     return;
                                 const {
-                                    callback: vn,
+                                    callback: bn,
                                     options: {
                                         bubbles: $n = !1,
                                         args: Ln = [],
                                         checker: Hn = null
                                     }
-                                } = gn;
-                                Hn && !Hn(qt, dn) || (vn.bind(qt, ...Ln)(), $n || (dn.stopPropagation(), dn.preventDefault()));
+                                } = vn;
+                                Hn && !Hn(qt, dn) || (bn.bind(qt, ...Ln)(), $n || (dn.stopPropagation(), dn.preventDefault()));
                             }
                         }
                         Rt = /* @__PURE__ */ new WeakSet(), Mt = function(nn) {
                             nn.altKey && this.buffer.push("alt"), nn.ctrlKey && this.buffer.push("ctrl"), nn.metaKey && this.buffer.push("meta"), nn.shiftKey && this.buffer.push("shift"), this.buffer.push(nn.key);
                             const qt = this.buffer.join("+");
                             return this.buffer.length = 0, qt;
                         }, it.KeyboardManager = Nn;
@@ -39151,53 +39151,53 @@
                                 ]);
                                 return (0, Tn.getColorValues)(qt), (0, cr.shadow)(this, "_colors", qt);
                             }
                             convert(qt) {
                                 const dn = (0, Tn.getRGB)(qt);
                                 if (!window.matchMedia("(forced-colors: active)").matches)
                                     return dn;
-                                for (const [gn, vn] of this._colors)
-                                    if (vn.every(($n, Ln) => $n === dn[Ln]))
-                                        return Po._colorsMapping.get(gn);
+                                for (const [vn, bn] of this._colors)
+                                    if (bn.every(($n, Ln) => $n === dn[Ln]))
+                                        return Po._colorsMapping.get(vn);
                                 return dn;
                             }
                             getHexCode(qt) {
                                 const dn = this._colors.get(qt);
                                 return dn ? cr.Util.makeHexColor(...dn) : qt;
                             }
                         };
                         tr(Kn, "_colorsMapping", /* @__PURE__ */ new Map([
                             ["CanvasText", [0, 0, 0]],
                             ["Canvas", [255, 255, 255]]
                         ]));
                         let Jn = Kn;
                         it.ColorManager = Jn;
                         const gr = class Eo {
-                            constructor(qt, dn, gn, vn, $n, Ln) {
-                                Ut(this, Sn), Ut(this, kn), Ut(this, Mn), Ut(this, Rn), Ut(this, jn), Ut(this, bn), Ut(this, zn), Ut(this, Un), Ut(this, Zn), Ut(this, lr), Ut(this, nr), Ut(this, Fn), Ut(this, En), Ut(this, Lt, null), Ut(this, Pt, /* @__PURE__ */ new Map()), Ut(this, kt, /* @__PURE__ */ new Map()), Ut(this, At, null), Ut(this, Tt, null), Ut(this, Ot, new hr()), Ut(this, It, 0), Ut(this, Nt, /* @__PURE__ */ new Set()), Ut(this, Ft, null), Ut(this, zt, null), Ut(this, jt, /* @__PURE__ */ new Set()), Ut(this, Vt, null), Ut(this, Gt, new or()), Ut(this, cn, !1), Ut(this, en, !1), Ut(this, Kt, null), Ut(this, an, cr.AnnotationEditorType.NONE), Ut(this, Qt, /* @__PURE__ */ new Set()), Ut(this, Zt, null), Ut(this, Jt, this.blur.bind(this)), Ut(this, pn, this.focus.bind(this)), Ut(this, hn, this.copy.bind(this)), Ut(this, un, this.cut.bind(this)), Ut(this, ln, this.paste.bind(this)), Ut(this, Xt, this.keydown.bind(this)), Ut(this, Ht, this.onEditingAction.bind(this)), Ut(this, Dt, this.onPageChanging.bind(this)), Ut(this, Bt, this.onScaleChanging.bind(this)), Ut(this, Wt, this.onRotationChanging.bind(this)), Ut(this, Yt, {
+                            constructor(qt, dn, vn, bn, $n, Ln) {
+                                Ut(this, yn), Ut(this, kn), Ut(this, Mn), Ut(this, Rn), Ut(this, En), Ut(this, gn), Ut(this, zn), Ut(this, Un), Ut(this, Zn), Ut(this, lr), Ut(this, nr), Ut(this, Dn), Ut(this, Sn), Ut(this, Lt, null), Ut(this, Pt, /* @__PURE__ */ new Map()), Ut(this, kt, /* @__PURE__ */ new Map()), Ut(this, At, null), Ut(this, Tt, null), Ut(this, Ot, new hr()), Ut(this, It, 0), Ut(this, Nt, /* @__PURE__ */ new Set()), Ut(this, Ft, null), Ut(this, zt, null), Ut(this, jt, /* @__PURE__ */ new Set()), Ut(this, Vt, null), Ut(this, Gt, new or()), Ut(this, cn, !1), Ut(this, en, !1), Ut(this, Kt, null), Ut(this, an, cr.AnnotationEditorType.NONE), Ut(this, Qt, /* @__PURE__ */ new Set()), Ut(this, Zt, null), Ut(this, Jt, this.blur.bind(this)), Ut(this, pn, this.focus.bind(this)), Ut(this, hn, this.copy.bind(this)), Ut(this, un, this.cut.bind(this)), Ut(this, ln, this.paste.bind(this)), Ut(this, Xt, this.keydown.bind(this)), Ut(this, Ht, this.onEditingAction.bind(this)), Ut(this, Dt, this.onPageChanging.bind(this)), Ut(this, Bt, this.onScaleChanging.bind(this)), Ut(this, Wt, this.onRotationChanging.bind(this)), Ut(this, Yt, {
                                     isEditing: !1,
                                     isEmpty: !0,
                                     hasSomethingToUndo: !1,
                                     hasSomethingToRedo: !1,
                                     hasSelectedEditor: !1
-                                }), Ut(this, on, [0, 0]), Ut(this, rn, null), Ut(this, mn, null), Ut(this, _n, null), sn(this, mn, qt), sn(this, _n, dn), sn(this, At, gn), this._eventBus = vn, this._eventBus._on("editingaction", St(this, Ht)), this._eventBus._on("pagechanging", St(this, Dt)), this._eventBus._on("scalechanging", St(this, Bt)), this._eventBus._on("rotationchanging", St(this, Wt)), sn(this, Tt, $n.annotationStorage), sn(this, Vt, $n.filterFactory), sn(this, Zt, Ln), this.viewParameters = {
+                                }), Ut(this, on, [0, 0]), Ut(this, rn, null), Ut(this, mn, null), Ut(this, _n, null), sn(this, mn, qt), sn(this, _n, dn), sn(this, At, vn), this._eventBus = bn, this._eventBus._on("editingaction", St(this, Ht)), this._eventBus._on("pagechanging", St(this, Dt)), this._eventBus._on("scalechanging", St(this, Bt)), this._eventBus._on("rotationchanging", St(this, Wt)), sn(this, Tt, $n.annotationStorage), sn(this, Vt, $n.filterFactory), sn(this, Zt, Ln), this.viewParameters = {
                                     realScale: Tn.PixelsPerInch.PDF_TO_CSS_UNITS,
                                     rotation: 0
                                 };
                             }
                             static get _keyboardManager() {
                                 const qt = Eo.prototype,
                                     dn = ($n) => {
                                         const {
                                             activeElement: Ln
                                         } = document;
                                         return Ln && St($n, mn).contains(Ln) && $n.hasSomethingToControl();
                                     },
-                                    gn = this.TRANSLATE_SMALL,
-                                    vn = this.TRANSLATE_BIG;
+                                    vn = this.TRANSLATE_SMALL,
+                                    bn = this.TRANSLATE_BIG;
                                 return (0, cr.shadow)(this, "_keyboardManager", new Nn([
                                     [
                                         ["ctrl+a", "mac+meta+a"], qt.selectAll
                                     ],
                                     [
                                         ["ctrl+z", "mac+meta+z"], qt.undo
                                     ],
@@ -39208,64 +39208,64 @@
                                         ["Backspace", "alt+Backspace", "ctrl+Backspace", "shift+Backspace", "mac+Backspace", "mac+alt+Backspace", "mac+ctrl+Backspace", "Delete", "ctrl+Delete", "shift+Delete", "mac+Delete"], qt.delete
                                     ],
                                     [
                                         ["Escape", "mac+Escape"], qt.unselectAll
                                     ],
                                     [
                                         ["ArrowLeft", "mac+ArrowLeft"], qt.translateSelectedEditors, {
-                                            args: [-gn, 0],
+                                            args: [-vn, 0],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ctrl+ArrowLeft", "mac+shift+ArrowLeft"], qt.translateSelectedEditors, {
-                                            args: [-vn, 0],
+                                            args: [-bn, 0],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ArrowRight", "mac+ArrowRight"], qt.translateSelectedEditors, {
-                                            args: [gn, 0],
+                                            args: [vn, 0],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ctrl+ArrowRight", "mac+shift+ArrowRight"], qt.translateSelectedEditors, {
-                                            args: [vn, 0],
+                                            args: [bn, 0],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ArrowUp", "mac+ArrowUp"], qt.translateSelectedEditors, {
-                                            args: [0, -gn],
+                                            args: [0, -vn],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ctrl+ArrowUp", "mac+shift+ArrowUp"], qt.translateSelectedEditors, {
-                                            args: [0, -vn],
+                                            args: [0, -bn],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ArrowDown", "mac+ArrowDown"], qt.translateSelectedEditors, {
-                                            args: [0, gn],
+                                            args: [0, vn],
                                             checker: dn
                                         }
                                     ],
                                     [
                                         ["ctrl+ArrowDown", "mac+shift+ArrowDown"], qt.translateSelectedEditors, {
-                                            args: [0, vn],
+                                            args: [0, bn],
                                             checker: dn
                                         }
                                     ]
                                 ]));
                             }
                             destroy() {
-                                tn(this, Rn, yn).call(this), tn(this, kn, Pn).call(this), this._eventBus._off("editingaction", St(this, Ht)), this._eventBus._off("pagechanging", St(this, Dt)), this._eventBus._off("scalechanging", St(this, Bt)), this._eventBus._off("rotationchanging", St(this, Wt));
+                                tn(this, Rn, Fn).call(this), tn(this, kn, Pn).call(this), this._eventBus._off("editingaction", St(this, Ht)), this._eventBus._off("pagechanging", St(this, Dt)), this._eventBus._off("scalechanging", St(this, Bt)), this._eventBus._off("rotationchanging", St(this, Wt));
                                 for (const qt of St(this, kt).values())
                                     qt.destroy();
                                 St(this, kt).clear(), St(this, Pt).clear(), St(this, jt).clear(), sn(this, Lt, null), St(this, Qt).clear(), St(this, Ot).destroy(), St(this, At).destroy();
                             }
                             get hcmFilter() {
                                 return (0, cr.shadow)(this, "hcmFilter", St(this, Zt) ? St(this, Vt).addHCMFilter(St(this, Zt).foreground, St(this, Zt).background) : "none");
                             }
@@ -39281,23 +39281,23 @@
                             }) {
                                 sn(this, It, qt - 1);
                             }
                             focusMainContainer() {
                                 St(this, mn).focus();
                             }
                             findParent(qt, dn) {
-                                for (const gn of St(this, kt).values()) {
+                                for (const vn of St(this, kt).values()) {
                                     const {
-                                        x: vn,
+                                        x: bn,
                                         y: $n,
                                         width: Ln,
                                         height: Hn
-                                    } = gn.div.getBoundingClientRect();
-                                    if (qt >= vn && qt <= vn + Ln && dn >= $n && dn <= $n + Hn)
-                                        return gn;
+                                    } = vn.div.getBoundingClientRect();
+                                    if (qt >= bn && qt <= bn + Ln && dn >= $n && dn <= $n + Hn)
+                                        return vn;
                                 }
                                 return null;
                             }
                             disableUserSelect(qt = !1) {
                                 St(this, _n).classList.toggle("noUserSelect", qt);
                             }
                             addShouldRescale(qt) {
@@ -39340,29 +39340,29 @@
                                 sn(this, Kt, null), dn.addEventListener("focusin", () => {
                                     qt._focusEventsAllowed = !0;
                                 }, {
                                     once: !0
                                 }), dn.focus();
                             }
                             addEditListeners() {
-                                tn(this, Mn, Wn).call(this), tn(this, jn, An).call(this);
+                                tn(this, Mn, Wn).call(this), tn(this, En, An).call(this);
                             }
                             removeEditListeners() {
-                                tn(this, Rn, yn).call(this), tn(this, bn, xn).call(this);
+                                tn(this, Rn, Fn).call(this), tn(this, gn, xn).call(this);
                             }
                             copy(qt) {
                                 var dn;
                                 if (qt.preventDefault(), (dn = St(this, Lt)) == null || dn.commitOrRemove(), !this.hasSelection)
                                     return;
-                                const gn = [];
-                                for (const vn of St(this, Qt)) {
-                                    const $n = vn.serialize(!0);
-                                    $n && gn.push($n);
+                                const vn = [];
+                                for (const bn of St(this, Qt)) {
+                                    const $n = bn.serialize(!0);
+                                    $n && vn.push($n);
                                 }
-                                gn.length !== 0 && qt.clipboardData.setData("application/pdfjs", JSON.stringify(gn));
+                                vn.length !== 0 && qt.clipboardData.setData("application/pdfjs", JSON.stringify(vn));
                             }
                             cut(qt) {
                                 this.copy(qt), this.delete();
                             }
                             paste(qt) {
                                 qt.preventDefault();
                                 const {
@@ -39370,39 +39370,39 @@
                                 } = qt;
                                 for (const $n of dn.items)
                                     for (const Ln of St(this, zt))
                                         if (Ln.isHandlingMimeForPasting($n.type)) {
                                             Ln.paste($n, this.currentLayer);
                                             return;
                                         }
-                                let gn = dn.getData("application/pdfjs");
-                                if (!gn)
+                                let vn = dn.getData("application/pdfjs");
+                                if (!vn)
                                     return;
                                 try {
-                                    gn = JSON.parse(gn);
+                                    vn = JSON.parse(vn);
                                 } catch ($n) {
                                     (0, cr.warn)(`paste: "${$n.message}".`);
                                     return;
                                 }
-                                if (!Array.isArray(gn))
+                                if (!Array.isArray(vn))
                                     return;
                                 this.unselectAll();
-                                const vn = this.currentLayer;
+                                const bn = this.currentLayer;
                                 try {
                                     const $n = [];
-                                    for (const Bn of gn) {
-                                        const qn = vn.deserialize(Bn);
+                                    for (const Bn of vn) {
+                                        const qn = bn.deserialize(Bn);
                                         if (!qn)
                                             return;
                                         $n.push(qn);
                                     }
                                     const Ln = () => {
                                             for (const Bn of $n)
                                                 tn(this, nr, sr).call(this, Bn);
-                                            tn(this, En, Dn).call(this, $n);
+                                            tn(this, Sn, jn).call(this, $n);
                                         },
                                         Hn = () => {
                                             for (const Bn of $n)
                                                 Bn.remove();
                                         };
                                     this.addCommands({
                                         cmd: Ln,
@@ -39417,21 +39417,21 @@
                                 var dn;
                                 (dn = this.getActive()) != null && dn.shouldGetKeyboardEvents() || Eo._keyboardManager.exec(this, qt);
                             }
                             onEditingAction(qt) {
                                 ["undo", "redo", "delete", "selectAll"].includes(qt.name) && this[qt.name]();
                             }
                             setEditingState(qt) {
-                                qt ? (tn(this, Sn, Cn).call(this), tn(this, Mn, Wn).call(this), tn(this, jn, An).call(this), tn(this, zn, On).call(this, {
+                                qt ? (tn(this, yn, Cn).call(this), tn(this, Mn, Wn).call(this), tn(this, En, An).call(this), tn(this, zn, On).call(this, {
                                     isEditing: St(this, an) !== cr.AnnotationEditorType.NONE,
-                                    isEmpty: tn(this, Fn, wn).call(this),
+                                    isEmpty: tn(this, Dn, wn).call(this),
                                     hasSomethingToUndo: St(this, Ot).hasSomethingToUndo(),
                                     hasSomethingToRedo: St(this, Ot).hasSomethingToRedo(),
                                     hasSelectedEditor: !1
-                                })) : (tn(this, kn, Pn).call(this), tn(this, Rn, yn).call(this), tn(this, bn, xn).call(this), tn(this, zn, On).call(this, {
+                                })) : (tn(this, kn, Pn).call(this), tn(this, Rn, Fn).call(this), tn(this, gn, xn).call(this), tn(this, zn, On).call(this, {
                                     isEditing: !1
                                 }), this.disableUserSelect(!1));
                             }
                             registerEditorTypes(qt) {
                                 if (!St(this, zt)) {
                                     sn(this, zt, qt);
                                     for (const dn of St(this, zt))
@@ -39459,20 +39459,20 @@
                             updateMode(qt, dn = null) {
                                 if (St(this, an) !== qt) {
                                     if (sn(this, an, qt), qt === cr.AnnotationEditorType.NONE) {
                                         this.setEditingState(!1), tn(this, lr, ur).call(this);
                                         return;
                                     }
                                     this.setEditingState(!0), tn(this, Zn, Yn).call(this), this.unselectAll();
-                                    for (const gn of St(this, kt).values())
-                                        gn.updateMode(qt);
+                                    for (const vn of St(this, kt).values())
+                                        vn.updateMode(qt);
                                     if (dn) {
-                                        for (const gn of St(this, Pt).values())
-                                            if (gn.annotationElementId === dn) {
-                                                this.setSelected(gn), gn.enterInEditMode();
+                                        for (const vn of St(this, Pt).values())
+                                            if (vn.annotationElementId === dn) {
+                                                this.setSelected(vn), vn.enterInEditMode();
                                                 break;
                                             }
                                     }
                                 }
                             }
                             updateToolbar(qt) {
                                 qt !== St(this, an) && this._eventBus.dispatch("switchannotationeditormode", {
@@ -39482,31 +39482,31 @@
                             }
                             updateParams(qt, dn) {
                                 if (St(this, zt)) {
                                     if (qt === cr.AnnotationEditorParamsType.CREATE) {
                                         this.currentLayer.addNewEditor(qt);
                                         return;
                                     }
-                                    for (const gn of St(this, Qt))
-                                        gn.updateParams(qt, dn);
-                                    for (const gn of St(this, zt))
-                                        gn.updateDefaultParams(qt, dn);
+                                    for (const vn of St(this, Qt))
+                                        vn.updateParams(qt, dn);
+                                    for (const vn of St(this, zt))
+                                        vn.updateDefaultParams(qt, dn);
                                 }
                             }
                             enableWaiting(qt = !1) {
                                 if (St(this, en) !== qt) {
                                     sn(this, en, qt);
                                     for (const dn of St(this, kt).values())
                                         qt ? dn.disableClick() : dn.enableClick(), dn.div.classList.toggle("waiting", qt);
                                 }
                             }
                             getEditors(qt) {
                                 const dn = [];
-                                for (const gn of St(this, Pt).values())
-                                    gn.pageIndex === qt && dn.push(gn);
+                                for (const vn of St(this, Pt).values())
+                                    vn.pageIndex === qt && dn.push(vn);
                                 return dn;
                             }
                             getEditor(qt) {
                                 return St(this, Pt).get(qt);
                             }
                             addEditor(qt) {
                                 St(this, Pt).set(qt.id, qt);
@@ -39556,88 +39556,88 @@
                             get hasSelection() {
                                 return St(this, Qt).size !== 0;
                             }
                             undo() {
                                 St(this, Ot).undo(), tn(this, zn, On).call(this, {
                                     hasSomethingToUndo: St(this, Ot).hasSomethingToUndo(),
                                     hasSomethingToRedo: !0,
-                                    isEmpty: tn(this, Fn, wn).call(this)
+                                    isEmpty: tn(this, Dn, wn).call(this)
                                 });
                             }
                             redo() {
                                 St(this, Ot).redo(), tn(this, zn, On).call(this, {
                                     hasSomethingToUndo: !0,
                                     hasSomethingToRedo: St(this, Ot).hasSomethingToRedo(),
-                                    isEmpty: tn(this, Fn, wn).call(this)
+                                    isEmpty: tn(this, Dn, wn).call(this)
                                 });
                             }
                             addCommands(qt) {
                                 St(this, Ot).add(qt), tn(this, zn, On).call(this, {
                                     hasSomethingToUndo: !0,
                                     hasSomethingToRedo: !1,
-                                    isEmpty: tn(this, Fn, wn).call(this)
+                                    isEmpty: tn(this, Dn, wn).call(this)
                                 });
                             }
                             delete() {
                                 if (this.commitOrRemove(), !this.hasSelection)
                                     return;
                                 const qt = [...St(this, Qt)],
                                     dn = () => {
-                                        for (const vn of qt)
-                                            vn.remove();
+                                        for (const bn of qt)
+                                            bn.remove();
                                     },
-                                    gn = () => {
-                                        for (const vn of qt)
-                                            tn(this, nr, sr).call(this, vn);
+                                    vn = () => {
+                                        for (const bn of qt)
+                                            tn(this, nr, sr).call(this, bn);
                                     };
                                 this.addCommands({
                                     cmd: dn,
-                                    undo: gn,
+                                    undo: vn,
                                     mustExec: !0
                                 });
                             }
                             commitOrRemove() {
                                 var qt;
                                 (qt = St(this, Lt)) == null || qt.commitOrRemove();
                             }
                             hasSomethingToControl() {
                                 return St(this, Lt) || this.hasSelection;
                             }
                             selectAll() {
                                 for (const qt of St(this, Qt))
                                     qt.commit();
-                                tn(this, En, Dn).call(this, St(this, Pt).values());
+                                tn(this, Sn, jn).call(this, St(this, Pt).values());
                             }
                             unselectAll() {
                                 if (St(this, Lt)) {
                                     St(this, Lt).commitOrRemove();
                                     return;
                                 }
                                 if (this.hasSelection) {
                                     for (const qt of St(this, Qt))
                                         qt.unselect();
                                     St(this, Qt).clear(), tn(this, zn, On).call(this, {
                                         hasSelectedEditor: !1
                                     });
                                 }
                             }
-                            translateSelectedEditors(qt, dn, gn = !1) {
-                                if (gn || this.commitOrRemove(), !this.hasSelection)
+                            translateSelectedEditors(qt, dn, vn = !1) {
+                                if (vn || this.commitOrRemove(), !this.hasSelection)
                                     return;
                                 St(this, on)[0] += qt, St(this, on)[1] += dn;
-                                const [vn, $n] = St(this, on), Ln = [...St(this, Qt)], Hn = 1e3;
+                                const [bn, $n] = St(this, on), Ln = [...St(this, Qt)], Hn = 1e3;
                                 St(this, rn) && clearTimeout(St(this, rn)), sn(this, rn, setTimeout(() => {
                                     sn(this, rn, null), St(this, on)[0] = St(this, on)[1] = 0, this.addCommands({
                                         cmd: () => {
                                             for (const Bn of Ln)
-                                                St(this, Pt).has(Bn.id) && Bn.translateInPage(vn, $n);
+                                                St(this, Pt).has(Bn.id) && Bn.translateInPage(bn, $n);
                                         },
                                         undo: () => {
                                             for (const Bn of Ln)
-                                                St(this, Pt).has(Bn.id) && Bn.translateInPage(-vn, -$n);
+                                                St(this, Pt).has(Bn.id) && Bn.translateInPage(-bn, -$n);
                                         },
                                         mustExec: !1
                                     });
                                 }, Hn));
                                 for (const Bn of Ln)
                                     Bn.translateInPage(qt, dn);
                             }
@@ -39659,51 +39659,51 @@
                                 if (!St(this, Ft))
                                     return !1;
                                 this.disableUserSelect(!1);
                                 const qt = St(this, Ft);
                                 sn(this, Ft, null);
                                 let dn = !1;
                                 for (const [{
-                                        x: vn,
+                                        x: bn,
                                         y: $n,
                                         pageIndex: Ln
                                     }, Hn] of qt)
-                                    Hn.newX = vn, Hn.newY = $n, Hn.newPageIndex = Ln, dn || (dn = vn !== Hn.savedX || $n !== Hn.savedY || Ln !== Hn.savedPageIndex);
+                                    Hn.newX = bn, Hn.newY = $n, Hn.newPageIndex = Ln, dn || (dn = bn !== Hn.savedX || $n !== Hn.savedY || Ln !== Hn.savedPageIndex);
                                 if (!dn)
                                     return !1;
-                                const gn = (vn, $n, Ln, Hn) => {
-                                    if (St(this, Pt).has(vn.id)) {
+                                const vn = (bn, $n, Ln, Hn) => {
+                                    if (St(this, Pt).has(bn.id)) {
                                         const Bn = St(this, kt).get(Hn);
-                                        Bn ? vn._setParentAndPosition(Bn, $n, Ln) : (vn.pageIndex = Hn, vn.x = $n, vn.y = Ln);
+                                        Bn ? bn._setParentAndPosition(Bn, $n, Ln) : (bn.pageIndex = Hn, bn.x = $n, bn.y = Ln);
                                     }
                                 };
                                 return this.addCommands({
                                     cmd: () => {
-                                        for (const [vn, {
+                                        for (const [bn, {
                                                 newX: $n,
                                                 newY: Ln,
                                                 newPageIndex: Hn
                                             }] of qt)
-                                            gn(vn, $n, Ln, Hn);
+                                            vn(bn, $n, Ln, Hn);
                                     },
                                     undo: () => {
-                                        for (const [vn, {
+                                        for (const [bn, {
                                                 savedX: $n,
                                                 savedY: Ln,
                                                 savedPageIndex: Hn
                                             }] of qt)
-                                            gn(vn, $n, Ln, Hn);
+                                            vn(bn, $n, Ln, Hn);
                                     },
                                     mustExec: !0
                                 }), !0;
                             }
                             dragSelectedEditors(qt, dn) {
                                 if (St(this, Ft))
-                                    for (const gn of St(this, Ft).keys())
-                                        gn.drag(qt, dn);
+                                    for (const vn of St(this, Ft).keys())
+                                        vn.drag(qt, dn);
                             }
                             rebuild(qt) {
                                 if (qt.parent === null) {
                                     const dn = this.getLayer(qt.pageIndex);
                                     dn ? (dn.changeParent(qt), dn.addOrRebuild(qt)) : (this.addEditor(qt), this.addToAnnotationStorage(qt), qt.rebuild());
                                 } else
                                     qt.parent.addOrRebuild(qt);
@@ -39717,29 +39717,29 @@
                             getMode() {
                                 return St(this, an);
                             }
                             get imageManager() {
                                 return (0, cr.shadow)(this, "imageManager", new Vn());
                             }
                         };
-                        Lt = /* @__PURE__ */ new WeakMap(), Pt = /* @__PURE__ */ new WeakMap(), kt = /* @__PURE__ */ new WeakMap(), At = /* @__PURE__ */ new WeakMap(), Tt = /* @__PURE__ */ new WeakMap(), Ot = /* @__PURE__ */ new WeakMap(), It = /* @__PURE__ */ new WeakMap(), Nt = /* @__PURE__ */ new WeakMap(), Ft = /* @__PURE__ */ new WeakMap(), zt = /* @__PURE__ */ new WeakMap(), jt = /* @__PURE__ */ new WeakMap(), Vt = /* @__PURE__ */ new WeakMap(), Gt = /* @__PURE__ */ new WeakMap(), cn = /* @__PURE__ */ new WeakMap(), en = /* @__PURE__ */ new WeakMap(), Kt = /* @__PURE__ */ new WeakMap(), an = /* @__PURE__ */ new WeakMap(), Qt = /* @__PURE__ */ new WeakMap(), Zt = /* @__PURE__ */ new WeakMap(), Jt = /* @__PURE__ */ new WeakMap(), pn = /* @__PURE__ */ new WeakMap(), hn = /* @__PURE__ */ new WeakMap(), un = /* @__PURE__ */ new WeakMap(), ln = /* @__PURE__ */ new WeakMap(), Xt = /* @__PURE__ */ new WeakMap(), Ht = /* @__PURE__ */ new WeakMap(), Dt = /* @__PURE__ */ new WeakMap(), Bt = /* @__PURE__ */ new WeakMap(), Wt = /* @__PURE__ */ new WeakMap(), Yt = /* @__PURE__ */ new WeakMap(), on = /* @__PURE__ */ new WeakMap(), rn = /* @__PURE__ */ new WeakMap(), mn = /* @__PURE__ */ new WeakMap(), _n = /* @__PURE__ */ new WeakMap(), Sn = /* @__PURE__ */ new WeakSet(), Cn = function() {
+                        Lt = /* @__PURE__ */ new WeakMap(), Pt = /* @__PURE__ */ new WeakMap(), kt = /* @__PURE__ */ new WeakMap(), At = /* @__PURE__ */ new WeakMap(), Tt = /* @__PURE__ */ new WeakMap(), Ot = /* @__PURE__ */ new WeakMap(), It = /* @__PURE__ */ new WeakMap(), Nt = /* @__PURE__ */ new WeakMap(), Ft = /* @__PURE__ */ new WeakMap(), zt = /* @__PURE__ */ new WeakMap(), jt = /* @__PURE__ */ new WeakMap(), Vt = /* @__PURE__ */ new WeakMap(), Gt = /* @__PURE__ */ new WeakMap(), cn = /* @__PURE__ */ new WeakMap(), en = /* @__PURE__ */ new WeakMap(), Kt = /* @__PURE__ */ new WeakMap(), an = /* @__PURE__ */ new WeakMap(), Qt = /* @__PURE__ */ new WeakMap(), Zt = /* @__PURE__ */ new WeakMap(), Jt = /* @__PURE__ */ new WeakMap(), pn = /* @__PURE__ */ new WeakMap(), hn = /* @__PURE__ */ new WeakMap(), un = /* @__PURE__ */ new WeakMap(), ln = /* @__PURE__ */ new WeakMap(), Xt = /* @__PURE__ */ new WeakMap(), Ht = /* @__PURE__ */ new WeakMap(), Dt = /* @__PURE__ */ new WeakMap(), Bt = /* @__PURE__ */ new WeakMap(), Wt = /* @__PURE__ */ new WeakMap(), Yt = /* @__PURE__ */ new WeakMap(), on = /* @__PURE__ */ new WeakMap(), rn = /* @__PURE__ */ new WeakMap(), mn = /* @__PURE__ */ new WeakMap(), _n = /* @__PURE__ */ new WeakMap(), yn = /* @__PURE__ */ new WeakSet(), Cn = function() {
                             window.addEventListener("focus", St(this, pn)), window.addEventListener("blur", St(this, Jt));
                         }, kn = /* @__PURE__ */ new WeakSet(), Pn = function() {
                             window.removeEventListener("focus", St(this, pn)), window.removeEventListener("blur", St(this, Jt));
                         }, Mn = /* @__PURE__ */ new WeakSet(), Wn = function() {
                             window.addEventListener("keydown", St(this, Xt), {
                                 capture: !0
                             });
-                        }, Rn = /* @__PURE__ */ new WeakSet(), yn = function() {
+                        }, Rn = /* @__PURE__ */ new WeakSet(), Fn = function() {
                             window.removeEventListener("keydown", St(this, Xt), {
                                 capture: !0
                             });
-                        }, jn = /* @__PURE__ */ new WeakSet(), An = function() {
+                        }, En = /* @__PURE__ */ new WeakSet(), An = function() {
                             document.addEventListener("copy", St(this, hn)), document.addEventListener("cut", St(this, un)), document.addEventListener("paste", St(this, ln));
-                        }, bn = /* @__PURE__ */ new WeakSet(), xn = function() {
+                        }, gn = /* @__PURE__ */ new WeakSet(), xn = function() {
                             document.removeEventListener("copy", St(this, hn)), document.removeEventListener("cut", St(this, un)), document.removeEventListener("paste", St(this, ln));
                         }, zn = /* @__PURE__ */ new WeakSet(), On = function(nn) {
                             Object.entries(nn).some(([qt, dn]) => St(this, Yt)[qt] !== dn) && this._eventBus.dispatch("annotationeditorstateschanged", {
                                 source: this,
                                 details: Object.assign(St(this, Yt), nn)
                             });
                         }, Un = /* @__PURE__ */ new WeakSet(), Gn = function(nn) {
@@ -39758,22 +39758,22 @@
                                 sn(this, cn, !1);
                                 for (const nn of St(this, kt).values())
                                     nn.disable();
                             }
                         }, nr = /* @__PURE__ */ new WeakSet(), sr = function(nn) {
                             const qt = St(this, kt).get(nn.pageIndex);
                             qt ? qt.addOrRebuild(nn) : this.addEditor(nn);
-                        }, Fn = /* @__PURE__ */ new WeakSet(), wn = function() {
+                        }, Dn = /* @__PURE__ */ new WeakSet(), wn = function() {
                             if (St(this, Pt).size === 0)
                                 return !0;
                             if (St(this, Pt).size === 1)
                                 for (const nn of St(this, Pt).values())
                                     return nn.isEmpty();
                             return !1;
-                        }, En = /* @__PURE__ */ new WeakSet(), Dn = function(nn) {
+                        }, Sn = /* @__PURE__ */ new WeakSet(), jn = function(nn) {
                             St(this, Qt).clear();
                             for (const qt of nn)
                                 qt.isEmpty() || (St(this, Qt).add(qt), qt.select());
                             tn(this, zn, On).call(this, {
                                 hasSelectedEditor: !0
                             });
                         }, tr(gr, "TRANSLATE_SMALL", 1), tr(gr, "TRANSLATE_BIG", 10);
@@ -39782,220 +39782,220 @@
                     },
                     /* 6 */
                     /***/
                     (_e, it, ft) => {
                         var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt;
                         Object.defineProperty(it, "__esModule", {
                             value: !0
-                        }), it.StatTimer = it.RenderingCancelledException = it.PixelsPerInch = it.PageViewport = it.PDFDateString = it.DOMStandardFontDataFactory = it.DOMSVGFactory = it.DOMFilterFactory = it.DOMCanvasFactory = it.DOMCMapReaderFactory = void 0, it.deprecated = Sn, it.getColorValues = Wn, it.getCurrentTransform = Rn, it.getCurrentTransformInverse = yn, it.getFilenameFromUrl = Wt, it.getPdfFilenameFromUrl = Yt, it.getRGB = Mn, it.getXfaPageViewport = Pn, it.isDataScheme = Dt, it.isPdfFile = Bt, it.isValidFetchUrl = rn, it.loadScript = _n, it.noContextMenu = mn, it.setLayerDimensions = jn;
+                        }), it.StatTimer = it.RenderingCancelledException = it.PixelsPerInch = it.PageViewport = it.PDFDateString = it.DOMStandardFontDataFactory = it.DOMSVGFactory = it.DOMFilterFactory = it.DOMCanvasFactory = it.DOMCMapReaderFactory = void 0, it.deprecated = yn, it.getColorValues = Wn, it.getCurrentTransform = Rn, it.getCurrentTransformInverse = Fn, it.getFilenameFromUrl = Wt, it.getPdfFilenameFromUrl = Yt, it.getRGB = Mn, it.getXfaPageViewport = Pn, it.isDataScheme = Dt, it.isPdfFile = Bt, it.isValidFetchUrl = rn, it.loadScript = _n, it.noContextMenu = mn, it.setLayerDimensions = En;
                         var cn = ft(7),
                             en = ft(1);
                         const Kt = "http://www.w3.org/2000/svg",
                             an = class {};
                         tr(an, "CSS", 96), tr(an, "PDF", 72), tr(an, "PDF_TO_CSS_UNITS", an.CSS / an.PDF);
                         let Qt = an;
                         it.PixelsPerInch = Qt;
                         class Zt extends cn.BaseFilterFactory {
                             constructor({
-                                docId: bn,
+                                docId: gn,
                                 ownerDocument: xn = globalThis.document
                             } = {}) {
-                                super(), Ut(this, Mt), Ut(this, Pt), Ut(this, At), Ut(this, Ot), Ut(this, Nt), Ut(this, zt), Ut(this, Vt), Ut(this, mt, void 0), Ut(this, gt, void 0), Ut(this, bt, void 0), Ut(this, _t, void 0), Ut(this, yt, void 0), Ut(this, Et, void 0), Ut(this, xt, void 0), Ut(this, wt, void 0), Ut(this, $t, void 0), Ut(this, Ct, void 0), Ut(this, Rt, 0), sn(this, bt, bn), sn(this, _t, xn);
+                                super(), Ut(this, Mt), Ut(this, Pt), Ut(this, At), Ut(this, Ot), Ut(this, Nt), Ut(this, zt), Ut(this, Vt), Ut(this, mt, void 0), Ut(this, gt, void 0), Ut(this, bt, void 0), Ut(this, _t, void 0), Ut(this, yt, void 0), Ut(this, Et, void 0), Ut(this, xt, void 0), Ut(this, wt, void 0), Ut(this, $t, void 0), Ut(this, Ct, void 0), Ut(this, Rt, 0), sn(this, bt, gn), sn(this, _t, xn);
                             }
-                            addFilter(bn) {
-                                if (!bn)
+                            addFilter(gn) {
+                                if (!gn)
                                     return "none";
-                                let xn = St(this, Mt, Lt).get(bn);
+                                let xn = St(this, Mt, Lt).get(gn);
                                 if (xn)
                                     return xn;
                                 let zn, On, Un, Gn;
-                                if (bn.length === 1) {
-                                    const ur = bn[0],
+                                if (gn.length === 1) {
+                                    const ur = gn[0],
                                         nr = new Array(256);
                                     for (let sr = 0; sr < 256; sr++)
                                         nr[sr] = ur[sr] / 255;
                                     Gn = zn = On = Un = nr.join(",");
                                 } else {
-                                    const [ur, nr, sr] = bn, Fn = new Array(256), wn = new Array(256), En = new Array(256);
-                                    for (let Dn = 0; Dn < 256; Dn++)
-                                        Fn[Dn] = ur[Dn] / 255, wn[Dn] = nr[Dn] / 255, En[Dn] = sr[Dn] / 255;
-                                    zn = Fn.join(","), On = wn.join(","), Un = En.join(","), Gn = `${zn}${On}${Un}`;
+                                    const [ur, nr, sr] = gn, Dn = new Array(256), wn = new Array(256), Sn = new Array(256);
+                                    for (let jn = 0; jn < 256; jn++)
+                                        Dn[jn] = ur[jn] / 255, wn[jn] = nr[jn] / 255, Sn[jn] = sr[jn] / 255;
+                                    zn = Dn.join(","), On = wn.join(","), Un = Sn.join(","), Gn = `${zn}${On}${Un}`;
                                 }
                                 if (xn = St(this, Mt, Lt).get(Gn), xn)
-                                    return St(this, Mt, Lt).set(bn, xn), xn;
+                                    return St(this, Mt, Lt).set(gn, xn), xn;
                                 const Zn = `g_${St(this, bt)}_transfer_map_${Vr(this, Rt)._++}`,
                                     Yn = `url(#${Zn})`;
-                                St(this, Mt, Lt).set(bn, Yn), St(this, Mt, Lt).set(Gn, Yn);
+                                St(this, Mt, Lt).set(gn, Yn), St(this, Mt, Lt).set(Gn, Yn);
                                 const lr = tn(this, Ot, It).call(this, Zn);
                                 return tn(this, zt, jt).call(this, zn, On, Un, lr), Yn;
                             }
-                            addHCMFilter(bn, xn) {
+                            addHCMFilter(gn, xn) {
                                 var zn;
-                                const On = `${bn}-${xn}`;
+                                const On = `${gn}-${xn}`;
                                 if (St(this, Et) === On)
                                     return St(this, xt);
-                                if (sn(this, Et, On), sn(this, xt, "none"), (zn = St(this, yt)) == null || zn.remove(), !bn || !xn)
+                                if (sn(this, Et, On), sn(this, xt, "none"), (zn = St(this, yt)) == null || zn.remove(), !gn || !xn)
                                     return St(this, xt);
-                                const Un = tn(this, Vt, Gt).call(this, bn);
-                                bn = en.Util.makeHexColor(...Un);
+                                const Un = tn(this, Vt, Gt).call(this, gn);
+                                gn = en.Util.makeHexColor(...Un);
                                 const Gn = tn(this, Vt, Gt).call(this, xn);
-                                if (xn = en.Util.makeHexColor(...Gn), St(this, Pt, kt).style.color = "", bn === "#000000" && xn === "#ffffff" || bn === xn)
+                                if (xn = en.Util.makeHexColor(...Gn), St(this, Pt, kt).style.color = "", gn === "#000000" && xn === "#ffffff" || gn === xn)
                                     return St(this, xt);
                                 const Zn = new Array(256);
                                 for (let sr = 0; sr <= 255; sr++) {
-                                    const Fn = sr / 255;
-                                    Zn[sr] = Fn <= 0.03928 ? Fn / 12.92 : ((Fn + 0.055) / 1.055) ** 2.4;
+                                    const Dn = sr / 255;
+                                    Zn[sr] = Dn <= 0.03928 ? Dn / 12.92 : ((Dn + 0.055) / 1.055) ** 2.4;
                                 }
                                 const Yn = Zn.join(","),
                                     lr = `g_${St(this, bt)}_hcm_filter`,
                                     ur = sn(this, wt, tn(this, Ot, It).call(this, lr));
                                 tn(this, zt, jt).call(this, Yn, Yn, Yn, ur), tn(this, At, Tt).call(this, ur);
-                                const nr = (sr, Fn) => {
+                                const nr = (sr, Dn) => {
                                     const wn = Un[sr] / 255,
-                                        En = Gn[sr] / 255,
-                                        Dn = new Array(Fn + 1);
-                                    for (let cr = 0; cr <= Fn; cr++)
-                                        Dn[cr] = wn + cr / Fn * (En - wn);
-                                    return Dn.join(",");
+                                        Sn = Gn[sr] / 255,
+                                        jn = new Array(Dn + 1);
+                                    for (let cr = 0; cr <= Dn; cr++)
+                                        jn[cr] = wn + cr / Dn * (Sn - wn);
+                                    return jn.join(",");
                                 };
                                 return tn(this, zt, jt).call(this, nr(0, 5), nr(1, 5), nr(2, 5), ur), sn(this, xt, `url(#${lr})`), St(this, xt);
                             }
-                            addHighlightHCMFilter(bn, xn, zn, On) {
+                            addHighlightHCMFilter(gn, xn, zn, On) {
                                 var Un;
-                                const Gn = `${bn}-${xn}-${zn}-${On}`;
+                                const Gn = `${gn}-${xn}-${zn}-${On}`;
                                 if (St(this, $t) === Gn)
                                     return St(this, Ct);
-                                if (sn(this, $t, Gn), sn(this, Ct, "none"), (Un = St(this, wt)) == null || Un.remove(), !bn || !xn)
+                                if (sn(this, $t, Gn), sn(this, Ct, "none"), (Un = St(this, wt)) == null || Un.remove(), !gn || !xn)
                                     return St(this, Ct);
-                                const [Zn, Yn] = [bn, xn].map(tn(this, Vt, Gt).bind(this));
+                                const [Zn, Yn] = [gn, xn].map(tn(this, Vt, Gt).bind(this));
                                 let lr = Math.round(0.2126 * Zn[0] + 0.7152 * Zn[1] + 0.0722 * Zn[2]),
                                     ur = Math.round(0.2126 * Yn[0] + 0.7152 * Yn[1] + 0.0722 * Yn[2]),
                                     [nr, sr] = [zn, On].map(tn(this, Vt, Gt).bind(this));
                                 ur < lr && ([lr, ur, nr, sr] = [ur, lr, sr, nr]), St(this, Pt, kt).style.color = "";
-                                const Fn = (Dn, cr, Tn) => {
+                                const Dn = (jn, cr, Tn) => {
                                         const In = new Array(256),
                                             Qn = (ur - lr) / Tn,
-                                            or = Dn / 255,
-                                            Xn = (cr - Dn) / (255 * Tn);
+                                            or = jn / 255,
+                                            Xn = (cr - jn) / (255 * Tn);
                                         let Vn = 0;
                                         for (let hr = 0; hr <= Tn; hr++) {
                                             const Nn = Math.round(lr + hr * Qn),
                                                 Kn = or + hr * Xn;
                                             for (let Jn = Vn; Jn <= Nn; Jn++)
                                                 In[Jn] = Kn;
                                             Vn = Nn + 1;
                                         }
                                         for (let hr = Vn; hr < 256; hr++)
                                             In[hr] = In[Vn - 1];
                                         return In.join(",");
                                     },
                                     wn = `g_${St(this, bt)}_hcm_highlight_filter`,
-                                    En = sn(this, wt, tn(this, Ot, It).call(this, wn));
-                                return tn(this, At, Tt).call(this, En), tn(this, zt, jt).call(this, Fn(nr[0], sr[0], 5), Fn(nr[1], sr[1], 5), Fn(nr[2], sr[2], 5), En), sn(this, Ct, `url(#${wn})`), St(this, Ct);
+                                    Sn = sn(this, wt, tn(this, Ot, It).call(this, wn));
+                                return tn(this, At, Tt).call(this, Sn), tn(this, zt, jt).call(this, Dn(nr[0], sr[0], 5), Dn(nr[1], sr[1], 5), Dn(nr[2], sr[2], 5), Sn), sn(this, Ct, `url(#${wn})`), St(this, Ct);
                             }
-                            destroy(bn = !1) {
-                                bn && (St(this, xt) || St(this, Ct)) || (St(this, gt) && (St(this, gt).parentNode.parentNode.remove(), sn(this, gt, null)), St(this, mt) && (St(this, mt).clear(), sn(this, mt, null)), sn(this, Rt, 0));
+                            destroy(gn = !1) {
+                                gn && (St(this, xt) || St(this, Ct)) || (St(this, gt) && (St(this, gt).parentNode.parentNode.remove(), sn(this, gt, null)), St(this, mt) && (St(this, mt).clear(), sn(this, mt, null)), sn(this, Rt, 0));
                             }
                         }
                         mt = /* @__PURE__ */ new WeakMap(), gt = /* @__PURE__ */ new WeakMap(), bt = /* @__PURE__ */ new WeakMap(), _t = /* @__PURE__ */ new WeakMap(), yt = /* @__PURE__ */ new WeakMap(), Et = /* @__PURE__ */ new WeakMap(), xt = /* @__PURE__ */ new WeakMap(), wt = /* @__PURE__ */ new WeakMap(), $t = /* @__PURE__ */ new WeakMap(), Ct = /* @__PURE__ */ new WeakMap(), Rt = /* @__PURE__ */ new WeakMap(), Mt = /* @__PURE__ */ new WeakSet(), Lt = function() {
                             return St(this, mt) || sn(this, mt, /* @__PURE__ */ new Map());
                         }, Pt = /* @__PURE__ */ new WeakSet(), kt = function() {
                             if (!St(this, gt)) {
                                 const An = St(this, _t).createElement("div"),
                                     {
-                                        style: bn
+                                        style: gn
                                     } = An;
-                                bn.visibility = "hidden", bn.contain = "strict", bn.width = bn.height = 0, bn.position = "absolute", bn.top = bn.left = 0, bn.zIndex = -1;
+                                gn.visibility = "hidden", gn.contain = "strict", gn.width = gn.height = 0, gn.position = "absolute", gn.top = gn.left = 0, gn.zIndex = -1;
                                 const xn = St(this, _t).createElementNS(Kt, "svg");
                                 xn.setAttribute("width", 0), xn.setAttribute("height", 0), sn(this, gt, St(this, _t).createElementNS(Kt, "defs")), An.append(xn), xn.append(St(this, gt)), St(this, _t).body.append(An);
                             }
                             return St(this, gt);
                         }, At = /* @__PURE__ */ new WeakSet(), Tt = function(An) {
-                            const bn = St(this, _t).createElementNS(Kt, "feColorMatrix");
-                            bn.setAttribute("type", "matrix"), bn.setAttribute("values", "0.2126 0.7152 0.0722 0 0 0.2126 0.7152 0.0722 0 0 0.2126 0.7152 0.0722 0 0 0 0 0 1 0"), An.append(bn);
+                            const gn = St(this, _t).createElementNS(Kt, "feColorMatrix");
+                            gn.setAttribute("type", "matrix"), gn.setAttribute("values", "0.2126 0.7152 0.0722 0 0 0.2126 0.7152 0.0722 0 0 0.2126 0.7152 0.0722 0 0 0 0 0 1 0"), An.append(gn);
                         }, Ot = /* @__PURE__ */ new WeakSet(), It = function(An) {
-                            const bn = St(this, _t).createElementNS(Kt, "filter");
-                            return bn.setAttribute("color-interpolation-filters", "sRGB"), bn.setAttribute("id", An), St(this, Pt, kt).append(bn), bn;
-                        }, Nt = /* @__PURE__ */ new WeakSet(), Ft = function(An, bn, xn) {
-                            const zn = St(this, _t).createElementNS(Kt, bn);
+                            const gn = St(this, _t).createElementNS(Kt, "filter");
+                            return gn.setAttribute("color-interpolation-filters", "sRGB"), gn.setAttribute("id", An), St(this, Pt, kt).append(gn), gn;
+                        }, Nt = /* @__PURE__ */ new WeakSet(), Ft = function(An, gn, xn) {
+                            const zn = St(this, _t).createElementNS(Kt, gn);
                             zn.setAttribute("type", "discrete"), zn.setAttribute("tableValues", xn), An.append(zn);
-                        }, zt = /* @__PURE__ */ new WeakSet(), jt = function(An, bn, xn, zn) {
+                        }, zt = /* @__PURE__ */ new WeakSet(), jt = function(An, gn, xn, zn) {
                             const On = St(this, _t).createElementNS(Kt, "feComponentTransfer");
-                            zn.append(On), tn(this, Nt, Ft).call(this, On, "feFuncR", An), tn(this, Nt, Ft).call(this, On, "feFuncG", bn), tn(this, Nt, Ft).call(this, On, "feFuncB", xn);
+                            zn.append(On), tn(this, Nt, Ft).call(this, On, "feFuncR", An), tn(this, Nt, Ft).call(this, On, "feFuncG", gn), tn(this, Nt, Ft).call(this, On, "feFuncB", xn);
                         }, Vt = /* @__PURE__ */ new WeakSet(), Gt = function(An) {
                             return St(this, Pt, kt).style.color = An, Mn(getComputedStyle(St(this, Pt, kt)).getPropertyValue("color"));
                         }, it.DOMFilterFactory = Zt;
                         class Jt extends cn.BaseCanvasFactory {
                             constructor({
-                                ownerDocument: bn = globalThis.document
+                                ownerDocument: gn = globalThis.document
                             } = {}) {
-                                super(), this._document = bn;
+                                super(), this._document = gn;
                             }
-                            _createCanvas(bn, xn) {
+                            _createCanvas(gn, xn) {
                                 const zn = this._document.createElement("canvas");
-                                return zn.width = bn, zn.height = xn, zn;
+                                return zn.width = gn, zn.height = xn, zn;
                             }
                         }
                         it.DOMCanvasFactory = Jt;
-                        async function pn(An, bn = !1) {
+                        async function pn(An, gn = !1) {
                             if (rn(An, document.baseURI)) {
                                 const xn = await fetch(An);
                                 if (!xn.ok)
                                     throw new Error(xn.statusText);
-                                return bn ? new Uint8Array(await xn.arrayBuffer()) : (0, en.stringToBytes)(await xn.text());
+                                return gn ? new Uint8Array(await xn.arrayBuffer()) : (0, en.stringToBytes)(await xn.text());
                             }
                             return new Promise((xn, zn) => {
                                 const On = new XMLHttpRequest();
-                                On.open("GET", An, !0), bn && (On.responseType = "arraybuffer"), On.onreadystatechange = () => {
+                                On.open("GET", An, !0), gn && (On.responseType = "arraybuffer"), On.onreadystatechange = () => {
                                     if (On.readyState === XMLHttpRequest.DONE) {
                                         if (On.status === 200 || On.status === 0) {
                                             let Un;
-                                            if (bn && On.response ? Un = new Uint8Array(On.response) : !bn && On.responseText && (Un = (0, en.stringToBytes)(On.responseText)), Un) {
+                                            if (gn && On.response ? Un = new Uint8Array(On.response) : !gn && On.responseText && (Un = (0, en.stringToBytes)(On.responseText)), Un) {
                                                 xn(Un);
                                                 return;
                                             }
                                         }
                                         zn(new Error(On.statusText));
                                     }
                                 }, On.send(null);
                             });
                         }
                         class hn extends cn.BaseCMapReaderFactory {
-                            _fetchData(bn, xn) {
-                                return pn(bn, this.isCompressed).then((zn) => ({
+                            _fetchData(gn, xn) {
+                                return pn(gn, this.isCompressed).then((zn) => ({
                                     cMapData: zn,
                                     compressionType: xn
                                 }));
                             }
                         }
                         it.DOMCMapReaderFactory = hn;
                         class un extends cn.BaseStandardFontDataFactory {
-                            _fetchData(bn) {
-                                return pn(bn, !0);
+                            _fetchData(gn) {
+                                return pn(gn, !0);
                             }
                         }
                         it.DOMStandardFontDataFactory = un;
                         class ln extends cn.BaseSVGFactory {
-                            _createSVG(bn) {
-                                return document.createElementNS(Kt, bn);
+                            _createSVG(gn) {
+                                return document.createElementNS(Kt, gn);
                             }
                         }
                         it.DOMSVGFactory = ln;
                         class Xt {
                             constructor({
-                                viewBox: bn,
+                                viewBox: gn,
                                 scale: xn,
                                 rotation: zn,
                                 offsetX: On = 0,
                                 offsetY: Un = 0,
                                 dontFlip: Gn = !1
                             }) {
-                                this.viewBox = bn, this.scale = xn, this.rotation = zn, this.offsetX = On, this.offsetY = Un;
-                                const Zn = (bn[2] + bn[0]) / 2,
-                                    Yn = (bn[3] + bn[1]) / 2;
+                                this.viewBox = gn, this.scale = xn, this.rotation = zn, this.offsetX = On, this.offsetY = Un;
+                                const Zn = (gn[2] + gn[0]) / 2,
+                                    Yn = (gn[3] + gn[1]) / 2;
                                 let lr, ur, nr, sr;
                                 switch (zn %= 360, zn < 0 && (zn += 360), zn) {
                                     case 180:
                                         lr = -1, ur = 0, nr = 0, sr = 1;
                                         break;
                                     case 90:
                                         lr = 0, ur = 1, nr = 1, sr = 0;
@@ -40006,166 +40006,166 @@
                                     case 0:
                                         lr = 1, ur = 0, nr = 0, sr = -1;
                                         break;
                                     default:
                                         throw new Error("PageViewport: Invalid rotation, must be a multiple of 90 degrees.");
                                 }
                                 Gn && (nr = -nr, sr = -sr);
-                                let Fn, wn, En, Dn;
-                                lr === 0 ? (Fn = Math.abs(Yn - bn[1]) * xn + On, wn = Math.abs(Zn - bn[0]) * xn + Un, En = (bn[3] - bn[1]) * xn, Dn = (bn[2] - bn[0]) * xn) : (Fn = Math.abs(Zn - bn[0]) * xn + On, wn = Math.abs(Yn - bn[1]) * xn + Un, En = (bn[2] - bn[0]) * xn, Dn = (bn[3] - bn[1]) * xn), this.transform = [lr * xn, ur * xn, nr * xn, sr * xn, Fn - lr * xn * Zn - nr * xn * Yn, wn - ur * xn * Zn - sr * xn * Yn], this.width = En, this.height = Dn;
+                                let Dn, wn, Sn, jn;
+                                lr === 0 ? (Dn = Math.abs(Yn - gn[1]) * xn + On, wn = Math.abs(Zn - gn[0]) * xn + Un, Sn = (gn[3] - gn[1]) * xn, jn = (gn[2] - gn[0]) * xn) : (Dn = Math.abs(Zn - gn[0]) * xn + On, wn = Math.abs(Yn - gn[1]) * xn + Un, Sn = (gn[2] - gn[0]) * xn, jn = (gn[3] - gn[1]) * xn), this.transform = [lr * xn, ur * xn, nr * xn, sr * xn, Dn - lr * xn * Zn - nr * xn * Yn, wn - ur * xn * Zn - sr * xn * Yn], this.width = Sn, this.height = jn;
                             }
                             get rawDims() {
                                 const {
-                                    viewBox: bn
+                                    viewBox: gn
                                 } = this;
                                 return (0, en.shadow)(this, "rawDims", {
-                                    pageWidth: bn[2] - bn[0],
-                                    pageHeight: bn[3] - bn[1],
-                                    pageX: bn[0],
-                                    pageY: bn[1]
+                                    pageWidth: gn[2] - gn[0],
+                                    pageHeight: gn[3] - gn[1],
+                                    pageX: gn[0],
+                                    pageY: gn[1]
                                 });
                             }
                             clone({
-                                scale: bn = this.scale,
+                                scale: gn = this.scale,
                                 rotation: xn = this.rotation,
                                 offsetX: zn = this.offsetX,
                                 offsetY: On = this.offsetY,
                                 dontFlip: Un = !1
                             } = {}) {
                                 return new Xt({
                                     viewBox: this.viewBox.slice(),
-                                    scale: bn,
+                                    scale: gn,
                                     rotation: xn,
                                     offsetX: zn,
                                     offsetY: On,
                                     dontFlip: Un
                                 });
                             }
-                            convertToViewportPoint(bn, xn) {
-                                return en.Util.applyTransform([bn, xn], this.transform);
+                            convertToViewportPoint(gn, xn) {
+                                return en.Util.applyTransform([gn, xn], this.transform);
                             }
-                            convertToViewportRectangle(bn) {
-                                const xn = en.Util.applyTransform([bn[0], bn[1]], this.transform),
-                                    zn = en.Util.applyTransform([bn[2], bn[3]], this.transform);
+                            convertToViewportRectangle(gn) {
+                                const xn = en.Util.applyTransform([gn[0], gn[1]], this.transform),
+                                    zn = en.Util.applyTransform([gn[2], gn[3]], this.transform);
                                 return [xn[0], xn[1], zn[0], zn[1]];
                             }
-                            convertToPdfPoint(bn, xn) {
-                                return en.Util.applyInverseTransform([bn, xn], this.transform);
+                            convertToPdfPoint(gn, xn) {
+                                return en.Util.applyInverseTransform([gn, xn], this.transform);
                             }
                         }
                         it.PageViewport = Xt;
                         class Ht extends en.BaseException {
-                            constructor(bn, xn = 0) {
-                                super(bn, "RenderingCancelledException"), this.extraDelay = xn;
+                            constructor(gn, xn = 0) {
+                                super(gn, "RenderingCancelledException"), this.extraDelay = xn;
                             }
                         }
                         it.RenderingCancelledException = Ht;
 
                         function Dt(An) {
-                            const bn = An.length;
+                            const gn = An.length;
                             let xn = 0;
-                            for (; xn < bn && An[xn].trim() === "";)
+                            for (; xn < gn && An[xn].trim() === "";)
                                 xn++;
                             return An.substring(xn, xn + 5).toLowerCase() === "data:";
                         }
 
                         function Bt(An) {
                             return typeof An == "string" && /\.pdf$/i.test(An);
                         }
 
-                        function Wt(An, bn = !1) {
-                            return bn || ([An] = An.split(/[#?]/, 1)), An.substring(An.lastIndexOf("/") + 1);
+                        function Wt(An, gn = !1) {
+                            return gn || ([An] = An.split(/[#?]/, 1)), An.substring(An.lastIndexOf("/") + 1);
                         }
 
-                        function Yt(An, bn = "document.pdf") {
+                        function Yt(An, gn = "document.pdf") {
                             if (typeof An != "string")
-                                return bn;
+                                return gn;
                             if (Dt(An))
-                                return (0, en.warn)('getPdfFilenameFromUrl: ignore "data:"-URL for performance reasons.'), bn;
+                                return (0, en.warn)('getPdfFilenameFromUrl: ignore "data:"-URL for performance reasons.'), gn;
                             const xn = /^(?:(?:[^:]+:)?\/\/[^/]+)?([^?#]*)(\?[^#]*)?(#.*)?$/,
                                 zn = /[^/?#=]+\.pdf\b(?!.*\.pdf\b)/i,
                                 On = xn.exec(An);
                             let Un = zn.exec(On[1]) || zn.exec(On[2]) || zn.exec(On[3]);
                             if (Un && (Un = Un[0], Un.includes("%")))
                                 try {
                                     Un = zn.exec(decodeURIComponent(Un))[0];
                                 } catch {}
-                            return Un || bn;
+                            return Un || gn;
                         }
                         class on {
                             constructor() {
                                 tr(this, "started", /* @__PURE__ */ Object.create(null)), tr(this, "times", []);
                             }
-                            time(bn) {
-                                bn in this.started && (0, en.warn)(`Timer is already running for ${bn}`), this.started[bn] = Date.now();
+                            time(gn) {
+                                gn in this.started && (0, en.warn)(`Timer is already running for ${gn}`), this.started[gn] = Date.now();
                             }
-                            timeEnd(bn) {
-                                bn in this.started || (0, en.warn)(`Timer has not been started for ${bn}`), this.times.push({
-                                    name: bn,
-                                    start: this.started[bn],
+                            timeEnd(gn) {
+                                gn in this.started || (0, en.warn)(`Timer has not been started for ${gn}`), this.times.push({
+                                    name: gn,
+                                    start: this.started[gn],
                                     end: Date.now()
-                                }), delete this.started[bn];
+                                }), delete this.started[gn];
                             }
                             toString() {
-                                const bn = [];
+                                const gn = [];
                                 let xn = 0;
                                 for (const {
                                         name: zn
                                     }
                                     of this.times)
                                     xn = Math.max(zn.length, xn);
                                 for (const {
                                         name: zn,
                                         start: On,
                                         end: Un
                                     }
                                     of this.times)
-                                    bn.push(`${zn.padEnd(xn)} ${Un - On}ms
+                                    gn.push(`${zn.padEnd(xn)} ${Un - On}ms
 `);
-                                return bn.join("");
+                                return gn.join("");
                             }
                         }
                         it.StatTimer = on;
 
-                        function rn(An, bn) {
+                        function rn(An, gn) {
                             try {
                                 const {
                                     protocol: xn
-                                } = bn ? new URL(An, bn) : new URL(An);
+                                } = gn ? new URL(An, gn) : new URL(An);
                                 return xn === "http:" || xn === "https:";
                             } catch {
                                 return !1;
                             }
                         }
 
                         function mn(An) {
                             An.preventDefault();
                         }
 
-                        function _n(An, bn = !1) {
+                        function _n(An, gn = !1) {
                             return new Promise((xn, zn) => {
                                 const On = document.createElement("script");
                                 On.src = An, On.onload = function(Un) {
-                                    bn && On.remove(), xn(Un);
+                                    gn && On.remove(), xn(Un);
                                 }, On.onerror = function() {
                                     zn(new Error(`Cannot load script at: ${On.src}`));
                                 }, (document.head || document.documentElement).append(On);
                             });
                         }
 
-                        function Sn(An) {
+                        function yn(An) {
                             console.log("Deprecated API usage: " + An);
                         }
                         let Cn;
                         class kn {
-                            static toDateObject(bn) {
-                                if (!bn || typeof bn != "string")
+                            static toDateObject(gn) {
+                                if (!gn || typeof gn != "string")
                                     return null;
                                 Cn || (Cn = new RegExp("^D:(\\d{4})(\\d{2})?(\\d{2})?(\\d{2})?(\\d{2})?(\\d{2})?([Z|+|-])?(\\d{2})?'?(\\d{2})?'?"));
-                                const xn = Cn.exec(bn);
+                                const xn = Cn.exec(gn);
                                 if (!xn)
                                     return null;
                                 const zn = parseInt(xn[1], 10);
                                 let On = parseInt(xn[2], 10);
                                 On = On >= 1 && On <= 12 ? On - 1 : 0;
                                 let Un = parseInt(xn[3], 10);
                                 Un = Un >= 1 && Un <= 31 ? Un : 1;
@@ -40181,82 +40181,82 @@
                                 let nr = parseInt(xn[9], 10) || 0;
                                 return nr = nr >= 0 && nr <= 59 ? nr : 0, lr === "-" ? (Gn += ur, Zn += nr) : lr === "+" && (Gn -= ur, Zn -= nr), new Date(Date.UTC(zn, On, Un, Gn, Zn, Yn));
                             }
                         }
                         it.PDFDateString = kn;
 
                         function Pn(An, {
-                            scale: bn = 1,
+                            scale: gn = 1,
                             rotation: xn = 0
                         }) {
                             const {
                                 width: zn,
                                 height: On
                             } = An.attributes.style, Un = [0, 0, parseInt(zn), parseInt(On)];
                             return new Xt({
                                 viewBox: Un,
-                                scale: bn,
+                                scale: gn,
                                 rotation: xn
                             });
                         }
 
                         function Mn(An) {
                             if (An.startsWith("#")) {
-                                const bn = parseInt(An.slice(1), 16);
-                                return [(bn & 16711680) >> 16, (bn & 65280) >> 8, bn & 255];
+                                const gn = parseInt(An.slice(1), 16);
+                                return [(gn & 16711680) >> 16, (gn & 65280) >> 8, gn & 255];
                             }
-                            return An.startsWith("rgb(") ? An.slice(4, -1).split(",").map((bn) => parseInt(bn)) : An.startsWith("rgba(") ? An.slice(5, -1).split(",").map((bn) => parseInt(bn)).slice(0, 3) : ((0, en.warn)(`Not a valid color format: "${An}"`), [0, 0, 0]);
+                            return An.startsWith("rgb(") ? An.slice(4, -1).split(",").map((gn) => parseInt(gn)) : An.startsWith("rgba(") ? An.slice(5, -1).split(",").map((gn) => parseInt(gn)).slice(0, 3) : ((0, en.warn)(`Not a valid color format: "${An}"`), [0, 0, 0]);
                         }
 
                         function Wn(An) {
-                            const bn = document.createElement("span");
-                            bn.style.visibility = "hidden", document.body.append(bn);
+                            const gn = document.createElement("span");
+                            gn.style.visibility = "hidden", document.body.append(gn);
                             for (const xn of An.keys()) {
-                                bn.style.color = xn;
-                                const zn = window.getComputedStyle(bn).color;
+                                gn.style.color = xn;
+                                const zn = window.getComputedStyle(gn).color;
                                 An.set(xn, Mn(zn));
                             }
-                            bn.remove();
+                            gn.remove();
                         }
 
                         function Rn(An) {
                             const {
-                                a: bn,
+                                a: gn,
                                 b: xn,
                                 c: zn,
                                 d: On,
                                 e: Un,
                                 f: Gn
                             } = An.getTransform();
-                            return [bn, xn, zn, On, Un, Gn];
+                            return [gn, xn, zn, On, Un, Gn];
                         }
 
-                        function yn(An) {
+                        function Fn(An) {
                             const {
-                                a: bn,
+                                a: gn,
                                 b: xn,
                                 c: zn,
                                 d: On,
                                 e: Un,
                                 f: Gn
                             } = An.getTransform().invertSelf();
-                            return [bn, xn, zn, On, Un, Gn];
+                            return [gn, xn, zn, On, Un, Gn];
                         }
 
-                        function jn(An, bn, xn = !1, zn = !0) {
-                            if (bn instanceof Xt) {
+                        function En(An, gn, xn = !1, zn = !0) {
+                            if (gn instanceof Xt) {
                                 const {
                                     pageWidth: On,
                                     pageHeight: Un
-                                } = bn.rawDims, {
+                                } = gn.rawDims, {
                                     style: Gn
                                 } = An, Zn = en.FeatureTest.isCSSRoundSupported, Yn = `var(--scale-factor) * ${On}px`, lr = `var(--scale-factor) * ${Un}px`, ur = Zn ? `round(${Yn}, 1px)` : `calc(${Yn})`, nr = Zn ? `round(${lr}, 1px)` : `calc(${lr})`;
-                                !xn || bn.rotation % 180 === 0 ? (Gn.width = ur, Gn.height = nr) : (Gn.width = nr, Gn.height = ur);
+                                !xn || gn.rotation % 180 === 0 ? (Gn.width = ur, Gn.height = nr) : (Gn.width = nr, Gn.height = ur);
                             }
-                            zn && An.setAttribute("data-main-rotation", bn.rotation);
+                            zn && An.setAttribute("data-main-rotation", gn.rotation);
                         }
                     },
                     /* 7 */
                     /***/
                     (_e, it, ft) => {
                         Object.defineProperty(it, "__esModule", {
                             value: !0
@@ -40778,98 +40778,98 @@
                                     const Dt = this.cache[Ht];
                                     this.canvasFactory.destroy(Dt), delete this.cache[Ht];
                                 }
                             }
                         }
 
                         function Ot(Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n) {
-                            const [Sn, Cn, kn, Pn, Mn, Wn] = (0, Et.getCurrentTransform)(Xt);
+                            const [yn, Cn, kn, Pn, Mn, Wn] = (0, Et.getCurrentTransform)(Xt);
                             if (Cn === 0 && kn === 0) {
-                                const jn = on * Sn + Mn,
-                                    An = Math.round(jn),
-                                    bn = rn * Pn + Wn,
-                                    xn = Math.round(bn),
-                                    zn = (on + mn) * Sn + Mn,
+                                const En = on * yn + Mn,
+                                    An = Math.round(En),
+                                    gn = rn * Pn + Wn,
+                                    xn = Math.round(gn),
+                                    zn = (on + mn) * yn + Mn,
                                     On = Math.abs(Math.round(zn) - An) || 1,
                                     Un = (rn + _n) * Pn + Wn,
                                     Gn = Math.abs(Math.round(Un) - xn) || 1;
-                                return Xt.setTransform(Math.sign(Sn), 0, 0, Math.sign(Pn), An, xn), Xt.drawImage(Ht, Dt, Bt, Wt, Yt, 0, 0, On, Gn), Xt.setTransform(Sn, Cn, kn, Pn, Mn, Wn), [On, Gn];
+                                return Xt.setTransform(Math.sign(yn), 0, 0, Math.sign(Pn), An, xn), Xt.drawImage(Ht, Dt, Bt, Wt, Yt, 0, 0, On, Gn), Xt.setTransform(yn, Cn, kn, Pn, Mn, Wn), [On, Gn];
                             }
-                            if (Sn === 0 && Pn === 0) {
-                                const jn = rn * kn + Mn,
-                                    An = Math.round(jn),
-                                    bn = on * Cn + Wn,
-                                    xn = Math.round(bn),
+                            if (yn === 0 && Pn === 0) {
+                                const En = rn * kn + Mn,
+                                    An = Math.round(En),
+                                    gn = on * Cn + Wn,
+                                    xn = Math.round(gn),
                                     zn = (rn + _n) * kn + Mn,
                                     On = Math.abs(Math.round(zn) - An) || 1,
                                     Un = (on + mn) * Cn + Wn,
                                     Gn = Math.abs(Math.round(Un) - xn) || 1;
-                                return Xt.setTransform(0, Math.sign(Cn), Math.sign(kn), 0, An, xn), Xt.drawImage(Ht, Dt, Bt, Wt, Yt, 0, 0, Gn, On), Xt.setTransform(Sn, Cn, kn, Pn, Mn, Wn), [Gn, On];
+                                return Xt.setTransform(0, Math.sign(Cn), Math.sign(kn), 0, An, xn), Xt.drawImage(Ht, Dt, Bt, Wt, Yt, 0, 0, Gn, On), Xt.setTransform(yn, Cn, kn, Pn, Mn, Wn), [Gn, On];
                             }
                             Xt.drawImage(Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n);
-                            const Rn = Math.hypot(Sn, Cn),
-                                yn = Math.hypot(kn, Pn);
-                            return [Rn * mn, yn * _n];
+                            const Rn = Math.hypot(yn, Cn),
+                                Fn = Math.hypot(kn, Pn);
+                            return [Rn * mn, Fn * _n];
                         }
 
                         function It(Xt) {
                             const {
                                 width: Ht,
                                 height: Dt
                             } = Xt;
                             if (Ht > Pt || Dt > Pt)
                                 return null;
                             const Bt = 1e3,
                                 Wt = new Uint8Array([0, 2, 4, 0, 1, 0, 5, 4, 8, 10, 0, 8, 0, 2, 1, 0]),
                                 Yt = Ht + 1;
                             let on = new Uint8Array(Yt * (Dt + 1)),
                                 rn, mn, _n;
-                            const Sn = Ht + 7 & -8;
-                            let Cn = new Uint8Array(Sn * Dt),
+                            const yn = Ht + 7 & -8;
+                            let Cn = new Uint8Array(yn * Dt),
                                 kn = 0;
                             for (const Rn of Xt.data) {
-                                let yn = 128;
-                                for (; yn > 0;)
-                                    Cn[kn++] = Rn & yn ? 0 : 255, yn >>= 1;
+                                let Fn = 128;
+                                for (; Fn > 0;)
+                                    Cn[kn++] = Rn & Fn ? 0 : 255, Fn >>= 1;
                             }
                             let Pn = 0;
                             for (kn = 0, Cn[kn] !== 0 && (on[0] = 1, ++Pn), mn = 1; mn < Ht; mn++)
                                 Cn[kn] !== Cn[kn + 1] && (on[mn] = Cn[kn] ? 2 : 1, ++Pn), kn++;
                             for (Cn[kn] !== 0 && (on[mn] = 2, ++Pn), rn = 1; rn < Dt; rn++) {
-                                kn = rn * Sn, _n = rn * Yt, Cn[kn - Sn] !== Cn[kn] && (on[_n] = Cn[kn] ? 1 : 8, ++Pn);
-                                let Rn = (Cn[kn] ? 4 : 0) + (Cn[kn - Sn] ? 8 : 0);
+                                kn = rn * yn, _n = rn * Yt, Cn[kn - yn] !== Cn[kn] && (on[_n] = Cn[kn] ? 1 : 8, ++Pn);
+                                let Rn = (Cn[kn] ? 4 : 0) + (Cn[kn - yn] ? 8 : 0);
                                 for (mn = 1; mn < Ht; mn++)
-                                    Rn = (Rn >> 2) + (Cn[kn + 1] ? 4 : 0) + (Cn[kn - Sn + 1] ? 8 : 0), Wt[Rn] && (on[_n + mn] = Wt[Rn], ++Pn), kn++;
-                                if (Cn[kn - Sn] !== Cn[kn] && (on[_n + mn] = Cn[kn] ? 2 : 4, ++Pn), Pn > Bt)
+                                    Rn = (Rn >> 2) + (Cn[kn + 1] ? 4 : 0) + (Cn[kn - yn + 1] ? 8 : 0), Wt[Rn] && (on[_n + mn] = Wt[Rn], ++Pn), kn++;
+                                if (Cn[kn - yn] !== Cn[kn] && (on[_n + mn] = Cn[kn] ? 2 : 4, ++Pn), Pn > Bt)
                                     return null;
                             }
-                            for (kn = Sn * (Dt - 1), _n = rn * Yt, Cn[kn] !== 0 && (on[_n] = 8, ++Pn), mn = 1; mn < Ht; mn++)
+                            for (kn = yn * (Dt - 1), _n = rn * Yt, Cn[kn] !== 0 && (on[_n] = 8, ++Pn), mn = 1; mn < Ht; mn++)
                                 Cn[kn] !== Cn[kn + 1] && (on[_n + mn] = Cn[kn] ? 4 : 8, ++Pn), kn++;
                             if (Cn[kn] !== 0 && (on[_n + mn] = 4, ++Pn), Pn > Bt)
                                 return null;
                             const Mn = new Int32Array([0, Yt, -1, 0, -Yt, 0, 0, 0, 1]),
                                 Wn = new Path2D();
                             for (rn = 0; Pn && rn <= Dt; rn++) {
                                 let Rn = rn * Yt;
-                                const yn = Rn + Ht;
-                                for (; Rn < yn && !on[Rn];)
+                                const Fn = Rn + Ht;
+                                for (; Rn < Fn && !on[Rn];)
                                     Rn++;
-                                if (Rn === yn)
+                                if (Rn === Fn)
                                     continue;
                                 Wn.moveTo(Rn % Yt, rn);
-                                const jn = Rn;
+                                const En = Rn;
                                 let An = on[Rn];
                                 do {
-                                    const bn = Mn[An];
+                                    const gn = Mn[An];
                                     do
-                                        Rn += bn;
+                                        Rn += gn;
                                     while (!on[Rn]);
                                     const xn = on[Rn];
                                     xn !== 5 && xn !== 10 ? (An = xn, on[Rn] = 0) : (An = xn & 51 * An >> 4, on[Rn] &= An >> 2 | An << 2), Wn.lineTo(Rn % Yt, Rn / Yt | 0), on[Rn] || --Pn;
-                                } while (jn !== Rn);
+                                } while (En !== Rn);
                                 --rn;
                             }
                             return Cn = null, on = null,
                                 function(Rn) {
                                     Rn.save(), Rn.scale(1 / Ht, -1 / Dt), Rn.translate(0, -Dt), Rn.fill(Wn), Rn.beginPath(), Rn.restore();
                                 };
                         }
@@ -40891,18 +40891,18 @@
                                 const Bt = yt.Util.applyTransform(Dt, Ht),
                                     Wt = yt.Util.applyTransform(Dt.slice(2), Ht);
                                 this.minX = Math.min(this.minX, Bt[0], Wt[0]), this.minY = Math.min(this.minY, Bt[1], Wt[1]), this.maxX = Math.max(this.maxX, Bt[0], Wt[0]), this.maxY = Math.max(this.maxY, Bt[1], Wt[1]);
                             }
                             updateScalingPathMinMax(Ht, Dt) {
                                 yt.Util.scaleMinMax(Ht, Dt), this.minX = Math.min(this.minX, Dt[0]), this.maxX = Math.max(this.maxX, Dt[1]), this.minY = Math.min(this.minY, Dt[2]), this.maxY = Math.max(this.maxY, Dt[3]);
                             }
-                            updateCurvePathMinMax(Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, Sn) {
+                            updateCurvePathMinMax(Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, yn) {
                                 const Cn = yt.Util.bezierBoundingBox(Dt, Bt, Wt, Yt, on, rn, mn, _n);
-                                if (Sn) {
-                                    Sn[0] = Math.min(Sn[0], Cn[0], Cn[2]), Sn[1] = Math.max(Sn[1], Cn[0], Cn[2]), Sn[2] = Math.min(Sn[2], Cn[1], Cn[3]), Sn[3] = Math.max(Sn[3], Cn[1], Cn[3]);
+                                if (yn) {
+                                    yn[0] = Math.min(yn[0], Cn[0], Cn[2]), yn[1] = Math.max(yn[1], Cn[0], Cn[2]), yn[2] = Math.min(yn[2], Cn[1], Cn[3]), yn[3] = Math.max(yn[3], Cn[1], Cn[3]);
                                     return;
                                 }
                                 this.updateRectMinMax(Ht, Cn);
                             }
                             getPathBoundingBox(Ht = xt.PathType.FILL, Dt = null) {
                                 const Bt = [this.minX, this.minY, this.maxX, this.maxY];
                                 if (Ht === xt.PathType.STROKE) {
@@ -40938,49 +40938,49 @@
                                 Bt = Ht.width,
                                 Wt = Dt % kt,
                                 Yt = (Dt - Wt) / kt,
                                 on = Wt === 0 ? Yt : Yt + 1,
                                 rn = Xt.createImageData(Bt, kt);
                             let mn = 0,
                                 _n;
-                            const Sn = Ht.data,
+                            const yn = Ht.data,
                                 Cn = rn.data;
                             let kn, Pn, Mn, Wn;
                             if (Ht.kind === yt.ImageKind.GRAYSCALE_1BPP) {
-                                const Rn = Sn.byteLength,
-                                    yn = new Uint32Array(Cn.buffer, 0, Cn.byteLength >> 2),
-                                    jn = yn.length,
+                                const Rn = yn.byteLength,
+                                    Fn = new Uint32Array(Cn.buffer, 0, Cn.byteLength >> 2),
+                                    En = Fn.length,
                                     An = Bt + 7 >> 3,
-                                    bn = 4294967295,
+                                    gn = 4294967295,
                                     xn = yt.FeatureTest.isLittleEndian ? 4278190080 : 255;
                                 for (kn = 0; kn < on; kn++) {
                                     for (Mn = kn < Yt ? kt : Wt, _n = 0, Pn = 0; Pn < Mn; Pn++) {
                                         const zn = Rn - mn;
                                         let On = 0;
                                         const Un = zn > An ? Bt : zn * 8 - 7,
                                             Gn = Un & -8;
                                         let Zn = 0,
                                             Yn = 0;
                                         for (; On < Gn; On += 8)
-                                            Yn = Sn[mn++], yn[_n++] = Yn & 128 ? bn : xn, yn[_n++] = Yn & 64 ? bn : xn, yn[_n++] = Yn & 32 ? bn : xn, yn[_n++] = Yn & 16 ? bn : xn, yn[_n++] = Yn & 8 ? bn : xn, yn[_n++] = Yn & 4 ? bn : xn, yn[_n++] = Yn & 2 ? bn : xn, yn[_n++] = Yn & 1 ? bn : xn;
+                                            Yn = yn[mn++], Fn[_n++] = Yn & 128 ? gn : xn, Fn[_n++] = Yn & 64 ? gn : xn, Fn[_n++] = Yn & 32 ? gn : xn, Fn[_n++] = Yn & 16 ? gn : xn, Fn[_n++] = Yn & 8 ? gn : xn, Fn[_n++] = Yn & 4 ? gn : xn, Fn[_n++] = Yn & 2 ? gn : xn, Fn[_n++] = Yn & 1 ? gn : xn;
                                         for (; On < Un; On++)
-                                            Zn === 0 && (Yn = Sn[mn++], Zn = 128), yn[_n++] = Yn & Zn ? bn : xn, Zn >>= 1;
+                                            Zn === 0 && (Yn = yn[mn++], Zn = 128), Fn[_n++] = Yn & Zn ? gn : xn, Zn >>= 1;
                                     }
-                                    for (; _n < jn;)
-                                        yn[_n++] = 0;
+                                    for (; _n < En;)
+                                        Fn[_n++] = 0;
                                     Xt.putImageData(rn, 0, kn * kt);
                                 }
                             } else if (Ht.kind === yt.ImageKind.RGBA_32BPP) {
                                 for (Pn = 0, Wn = Bt * kt * 4, kn = 0; kn < Yt; kn++)
-                                    Cn.set(Sn.subarray(mn, mn + Wn)), mn += Wn, Xt.putImageData(rn, 0, Pn), Pn += kt;
-                                kn < on && (Wn = Bt * Wt * 4, Cn.set(Sn.subarray(mn, mn + Wn)), Xt.putImageData(rn, 0, Pn));
+                                    Cn.set(yn.subarray(mn, mn + Wn)), mn += Wn, Xt.putImageData(rn, 0, Pn), Pn += kt;
+                                kn < on && (Wn = Bt * Wt * 4, Cn.set(yn.subarray(mn, mn + Wn)), Xt.putImageData(rn, 0, Pn));
                             } else if (Ht.kind === yt.ImageKind.RGB_24BPP)
                                 for (Mn = kt, Wn = Bt * Mn, kn = 0; kn < on; kn++) {
                                     for (kn >= Yt && (Mn = Wt, Wn = Bt * Mn), _n = 0, Pn = Wn; Pn--;)
-                                        Cn[_n++] = Sn[mn++], Cn[_n++] = Sn[mn++], Cn[_n++] = Sn[mn++], Cn[_n++] = 255;
+                                        Cn[_n++] = yn[mn++], Cn[_n++] = yn[mn++], Cn[_n++] = yn[mn++], Cn[_n++] = 255;
                                     Xt.putImageData(rn, 0, kn * kt);
                                 }
                             else
                                 throw new Error(`bad image kind: ${Ht.kind}`);
                         }
 
                         function zt(Xt, Ht) {
@@ -40992,23 +40992,23 @@
                                 Bt = Ht.width,
                                 Wt = Dt % kt,
                                 Yt = (Dt - Wt) / kt,
                                 on = Wt === 0 ? Yt : Yt + 1,
                                 rn = Xt.createImageData(Bt, kt);
                             let mn = 0;
                             const _n = Ht.data,
-                                Sn = rn.data;
+                                yn = rn.data;
                             for (let Cn = 0; Cn < on; Cn++) {
                                 const kn = Cn < Yt ? kt : Wt;
                                 ({
                                     srcPos: mn
                                 } = (0, wt.convertBlackAndWhiteToRGBA)({
                                     src: _n,
                                     srcPos: mn,
-                                    dest: Sn,
+                                    dest: yn,
                                     width: Bt,
                                     height: kn,
                                     nonBlackColor: 0
                                 })), Xt.putImageData(rn, 0, Cn * kt);
                             }
                         }
 
@@ -41054,26 +41054,26 @@
                             const Bt = Xt.length;
                             for (let Wt = 3; Wt < Bt; Wt += 4) {
                                 const Yt = Xt[Wt - 3] * 77 + Xt[Wt - 2] * 152 + Xt[Wt - 1] * 28;
                                 Ht[Wt] = Dt ? Ht[Wt] * Dt[Yt >> 8] >> 8 : Ht[Wt] * Yt >> 16;
                             }
                         }
 
-                        function Kt(Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, Sn) {
+                        function Kt(Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, yn) {
                             const Cn = !!Yt,
                                 kn = Cn ? Yt[0] : 0,
                                 Pn = Cn ? Yt[1] : 0,
                                 Mn = Cn ? Yt[2] : 0,
                                 Wn = Wt === "Luminosity" ? en : cn,
                                 Rn = Math.min(Bt, Math.ceil(1048576 / Dt));
-                            for (let yn = 0; yn < Bt; yn += Rn) {
-                                const jn = Math.min(Rn, Bt - yn),
-                                    An = Xt.getImageData(rn - _n, yn + (mn - Sn), Dt, jn),
-                                    bn = Ht.getImageData(rn, yn + mn, Dt, jn);
-                                Cn && Gt(An.data, kn, Pn, Mn), Wn(An.data, bn.data, on), Ht.putImageData(bn, rn, yn + mn);
+                            for (let Fn = 0; Fn < Bt; Fn += Rn) {
+                                const En = Math.min(Rn, Bt - Fn),
+                                    An = Xt.getImageData(rn - _n, Fn + (mn - yn), Dt, En),
+                                    gn = Ht.getImageData(rn, Fn + mn, Dt, En);
+                                Cn && Gt(An.data, kn, Pn, Mn), Wn(An.data, gn.data, on), Ht.putImageData(gn, rn, Fn + mn);
                             }
                         }
 
                         function an(Xt, Ht, Dt, Bt) {
                             const Wt = Bt[0],
                                 Yt = Bt[1],
                                 on = Bt[2] - Wt,
@@ -41120,15 +41120,15 @@
                                     const Yt = Ht.argsArray,
                                         on = Ht.fnArray;
                                     let rn = Dt || 0;
                                     const mn = Yt.length;
                                     if (mn === rn)
                                         return rn;
                                     const _n = mn - rn > Lt && typeof Bt == "function",
-                                        Sn = _n ? Date.now() + Mt : 0;
+                                        yn = _n ? Date.now() + Mt : 0;
                                     let Cn = 0;
                                     const kn = this.commonObjs,
                                         Pn = this.objs;
                                     let Mn;
                                     for (;;) {
                                         if (Wt !== void 0 && rn === Wt.nextBreakPoint)
                                             return Wt.breakIt(rn, Bt), rn;
@@ -41139,15 +41139,15 @@
                                                 const Rn = Wn.startsWith("g_") ? kn : Pn;
                                                 if (!Rn.has(Wn))
                                                     return Rn.get(Wn, Bt), rn;
                                             }
                                         if (rn++, rn === mn)
                                             return rn;
                                         if (_n && ++Cn > Lt) {
-                                            if (Date.now() > Sn)
+                                            if (Date.now() > yn)
                                                 return Bt(), rn;
                                             Cn = 0;
                                         }
                                     }
                                 }
                                 endDrawing() {
                                     tn(this, mt, gt).call(this), this.cachedCanvases.clear(), this.cachedPatterns.clear();
@@ -41162,19 +41162,19 @@
                                     const Bt = Ht.width,
                                         Wt = Ht.height;
                                     let Yt = Math.max(Math.hypot(Dt[0], Dt[1]), 1),
                                         on = Math.max(Math.hypot(Dt[2], Dt[3]), 1),
                                         rn = Bt,
                                         mn = Wt,
                                         _n = "prescale1",
-                                        Sn, Cn;
+                                        yn, Cn;
                                     for (; Yt > 2 && rn > 1 || on > 2 && mn > 1;) {
                                         let kn = rn,
                                             Pn = mn;
-                                        Yt > 2 && rn > 1 && (kn = rn >= 16384 ? Math.floor(rn / 2) - 1 || 1 : Math.ceil(rn / 2), Yt /= rn / kn), on > 2 && mn > 1 && (Pn = mn >= 16384 ? Math.floor(mn / 2) - 1 || 1 : Math.ceil(mn) / 2, on /= mn / Pn), Sn = this.cachedCanvases.getCanvas(_n, kn, Pn), Cn = Sn.context, Cn.clearRect(0, 0, kn, Pn), Cn.drawImage(Ht, 0, 0, rn, mn, 0, 0, kn, Pn), Ht = Sn.canvas, rn = kn, mn = Pn, _n = _n === "prescale1" ? "prescale2" : "prescale1";
+                                        Yt > 2 && rn > 1 && (kn = rn >= 16384 ? Math.floor(rn / 2) - 1 || 1 : Math.ceil(rn / 2), Yt /= rn / kn), on > 2 && mn > 1 && (Pn = mn >= 16384 ? Math.floor(mn / 2) - 1 || 1 : Math.ceil(mn) / 2, on /= mn / Pn), yn = this.cachedCanvases.getCanvas(_n, kn, Pn), Cn = yn.context, Cn.clearRect(0, 0, kn, Pn), Cn.drawImage(Ht, 0, 0, rn, mn, 0, 0, kn, Pn), Ht = yn.canvas, rn = kn, mn = Pn, _n = _n === "prescale1" ? "prescale2" : "prescale1";
                                     }
                                     return {
                                         img: Ht,
                                         paintWidth: rn,
                                         paintHeight: mn
                                     };
                                 }
@@ -41183,47 +41183,47 @@
                                         {
                                             width: Bt,
                                             height: Wt
                                         } = Ht,
                                         Yt = this.current.fillColor,
                                         on = this.current.patternFill,
                                         rn = (0, Et.getCurrentTransform)(Dt);
-                                    let mn, _n, Sn, Cn;
+                                    let mn, _n, yn, Cn;
                                     if ((Ht.bitmap || Ht.data) && Ht.count > 1) {
                                         const On = Ht.bitmap || Ht.data.buffer;
                                         _n = JSON.stringify(on ? rn : [rn.slice(0, 4), Yt]), mn = this._cachedBitmapsMap.get(On), mn || (mn = /* @__PURE__ */ new Map(), this._cachedBitmapsMap.set(On, mn));
                                         const Un = mn.get(_n);
                                         if (Un && !on) {
                                             const Gn = Math.round(Math.min(rn[0], rn[2]) + rn[4]),
                                                 Zn = Math.round(Math.min(rn[1], rn[3]) + rn[5]);
                                             return {
                                                 canvas: Un,
                                                 offsetX: Gn,
                                                 offsetY: Zn
                                             };
                                         }
-                                        Sn = Un;
+                                        yn = Un;
                                     }
-                                    Sn || (Cn = this.cachedCanvases.getCanvas("maskCanvas", Bt, Wt), zt(Cn.context, Ht));
+                                    yn || (Cn = this.cachedCanvases.getCanvas("maskCanvas", Bt, Wt), zt(Cn.context, Ht));
                                     let kn = yt.Util.transform(rn, [1 / Bt, 0, 0, -1 / Wt, 0, 0]);
                                     kn = yt.Util.transform(kn, [1, 0, 0, 1, 0, -Wt]);
                                     const Pn = yt.Util.applyTransform([0, 0], kn),
                                         Mn = yt.Util.applyTransform([Bt, Wt], kn),
                                         Wn = yt.Util.normalizeRect([Pn[0], Pn[1], Mn[0], Mn[1]]),
                                         Rn = Math.round(Wn[2] - Wn[0]) || 1,
-                                        yn = Math.round(Wn[3] - Wn[1]) || 1,
-                                        jn = this.cachedCanvases.getCanvas("fillCanvas", Rn, yn),
-                                        An = jn.context,
-                                        bn = Math.min(Pn[0], Mn[0]),
+                                        Fn = Math.round(Wn[3] - Wn[1]) || 1,
+                                        En = this.cachedCanvases.getCanvas("fillCanvas", Rn, Fn),
+                                        An = En.context,
+                                        gn = Math.min(Pn[0], Mn[0]),
                                         xn = Math.min(Pn[1], Mn[1]);
-                                    An.translate(-bn, -xn), An.transform(...kn), Sn || (Sn = this._scaleImage(Cn.canvas, (0, Et.getCurrentTransformInverse)(An)), Sn = Sn.img, mn && on && mn.set(_n, Sn)), An.imageSmoothingEnabled = Qt((0, Et.getCurrentTransform)(An), Ht.interpolate), Ot(An, Sn, 0, 0, Sn.width, Sn.height, 0, 0, Bt, Wt), An.globalCompositeOperation = "source-in";
-                                    const zn = yt.Util.transform((0, Et.getCurrentTransformInverse)(An), [1, 0, 0, 1, -bn, -xn]);
-                                    return An.fillStyle = on ? Yt.getPattern(Dt, this, zn, xt.PathType.FILL) : Yt, An.fillRect(0, 0, Bt, Wt), mn && !on && (this.cachedCanvases.delete("fillCanvas"), mn.set(_n, jn.canvas)), {
-                                        canvas: jn.canvas,
-                                        offsetX: Math.round(bn),
+                                    An.translate(-gn, -xn), An.transform(...kn), yn || (yn = this._scaleImage(Cn.canvas, (0, Et.getCurrentTransformInverse)(An)), yn = yn.img, mn && on && mn.set(_n, yn)), An.imageSmoothingEnabled = Qt((0, Et.getCurrentTransform)(An), Ht.interpolate), Ot(An, yn, 0, 0, yn.width, yn.height, 0, 0, Bt, Wt), An.globalCompositeOperation = "source-in";
+                                    const zn = yt.Util.transform((0, Et.getCurrentTransformInverse)(An), [1, 0, 0, 1, -gn, -xn]);
+                                    return An.fillStyle = on ? Yt.getPattern(Dt, this, zn, xt.PathType.FILL) : Yt, An.fillRect(0, 0, Bt, Wt), mn && !on && (this.cachedCanvases.delete("fillCanvas"), mn.set(_n, En.canvas)), {
+                                        canvas: En.canvas,
+                                        offsetX: Math.round(gn),
                                         offsetY: Math.round(xn)
                                     };
                                 }
                                 setLineWidth(Ht) {
                                     Ht !== this.current.lineWidth && (this._cachedScaleForStroking[0] = -1), this.current.lineWidth = Ht, this.ctx.lineWidth = Ht;
                                 }
                                 setLineCap(Ht) {
@@ -41333,47 +41333,47 @@
                                 }
                                 constructPath(Ht, Dt, Bt) {
                                     const Wt = this.ctx,
                                         Yt = this.current;
                                     let on = Yt.x,
                                         rn = Yt.y,
                                         mn, _n;
-                                    const Sn = (0, Et.getCurrentTransform)(Wt),
-                                        Cn = Sn[0] === 0 && Sn[3] === 0 || Sn[1] === 0 && Sn[2] === 0,
+                                    const yn = (0, Et.getCurrentTransform)(Wt),
+                                        Cn = yn[0] === 0 && yn[3] === 0 || yn[1] === 0 && yn[2] === 0,
                                         kn = Cn ? Bt.slice(0) : null;
                                     for (let Pn = 0, Mn = 0, Wn = Ht.length; Pn < Wn; Pn++)
                                         switch (Ht[Pn] | 0) {
                                             case yt.OPS.rectangle:
                                                 on = Dt[Mn++], rn = Dt[Mn++];
                                                 const Rn = Dt[Mn++],
-                                                    yn = Dt[Mn++],
-                                                    jn = on + Rn,
-                                                    An = rn + yn;
-                                                Wt.moveTo(on, rn), Rn === 0 || yn === 0 ? Wt.lineTo(jn, An) : (Wt.lineTo(jn, rn), Wt.lineTo(jn, An), Wt.lineTo(on, An)), Cn || Yt.updateRectMinMax(Sn, [on, rn, jn, An]), Wt.closePath();
+                                                    Fn = Dt[Mn++],
+                                                    En = on + Rn,
+                                                    An = rn + Fn;
+                                                Wt.moveTo(on, rn), Rn === 0 || Fn === 0 ? Wt.lineTo(En, An) : (Wt.lineTo(En, rn), Wt.lineTo(En, An), Wt.lineTo(on, An)), Cn || Yt.updateRectMinMax(yn, [on, rn, En, An]), Wt.closePath();
                                                 break;
                                             case yt.OPS.moveTo:
-                                                on = Dt[Mn++], rn = Dt[Mn++], Wt.moveTo(on, rn), Cn || Yt.updatePathMinMax(Sn, on, rn);
+                                                on = Dt[Mn++], rn = Dt[Mn++], Wt.moveTo(on, rn), Cn || Yt.updatePathMinMax(yn, on, rn);
                                                 break;
                                             case yt.OPS.lineTo:
-                                                on = Dt[Mn++], rn = Dt[Mn++], Wt.lineTo(on, rn), Cn || Yt.updatePathMinMax(Sn, on, rn);
+                                                on = Dt[Mn++], rn = Dt[Mn++], Wt.lineTo(on, rn), Cn || Yt.updatePathMinMax(yn, on, rn);
                                                 break;
                                             case yt.OPS.curveTo:
-                                                mn = on, _n = rn, on = Dt[Mn + 4], rn = Dt[Mn + 5], Wt.bezierCurveTo(Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3], on, rn), Yt.updateCurvePathMinMax(Sn, mn, _n, Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3], on, rn, kn), Mn += 6;
+                                                mn = on, _n = rn, on = Dt[Mn + 4], rn = Dt[Mn + 5], Wt.bezierCurveTo(Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3], on, rn), Yt.updateCurvePathMinMax(yn, mn, _n, Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3], on, rn, kn), Mn += 6;
                                                 break;
                                             case yt.OPS.curveTo2:
-                                                mn = on, _n = rn, Wt.bezierCurveTo(on, rn, Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3]), Yt.updateCurvePathMinMax(Sn, mn, _n, on, rn, Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3], kn), on = Dt[Mn + 2], rn = Dt[Mn + 3], Mn += 4;
+                                                mn = on, _n = rn, Wt.bezierCurveTo(on, rn, Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3]), Yt.updateCurvePathMinMax(yn, mn, _n, on, rn, Dt[Mn], Dt[Mn + 1], Dt[Mn + 2], Dt[Mn + 3], kn), on = Dt[Mn + 2], rn = Dt[Mn + 3], Mn += 4;
                                                 break;
                                             case yt.OPS.curveTo3:
-                                                mn = on, _n = rn, on = Dt[Mn + 2], rn = Dt[Mn + 3], Wt.bezierCurveTo(Dt[Mn], Dt[Mn + 1], on, rn, on, rn), Yt.updateCurvePathMinMax(Sn, mn, _n, Dt[Mn], Dt[Mn + 1], on, rn, on, rn, kn), Mn += 4;
+                                                mn = on, _n = rn, on = Dt[Mn + 2], rn = Dt[Mn + 3], Wt.bezierCurveTo(Dt[Mn], Dt[Mn + 1], on, rn, on, rn), Yt.updateCurvePathMinMax(yn, mn, _n, Dt[Mn], Dt[Mn + 1], on, rn, on, rn, kn), Mn += 4;
                                                 break;
                                             case yt.OPS.closePath:
                                                 Wt.closePath();
                                                 break;
                                         }
-                                    Cn && Yt.updateScalingPathMinMax(Sn, kn), Yt.setCurrentPoint(on, rn);
+                                    Cn && Yt.updateScalingPathMinMax(yn, kn), Yt.setCurrentPoint(on, rn);
                                 }
                                 closePath() {
                                     this.ctx.closePath();
                                 }
                                 stroke(Ht = !0) {
                                     const Dt = this.ctx,
                                         Bt = this.current.strokeColor;
@@ -41451,16 +41451,16 @@
                                     if (Yt.fontMatrix = Wt.fontMatrix || yt.FONT_IDENTITY_MATRIX, (Yt.fontMatrix[0] === 0 || Yt.fontMatrix[3] === 0) && (0, yt.warn)("Invalid font matrix for font " + Ht), Dt < 0 ? (Dt = -Dt, Yt.fontDirection = -1) : Yt.fontDirection = 1, this.current.font = Wt, this.current.fontSize = Dt, Wt.isType3Font)
                                         return;
                                     const on = Wt.loadedName || "sans-serif",
                                         rn = ((Bt = Wt.systemFontInfo) == null ? void 0 : Bt.css) || `"${on}", ${Wt.fallbackName}`;
                                     let mn = "normal";
                                     Wt.black ? mn = "900" : Wt.bold && (mn = "bold");
                                     const _n = Wt.italic ? "italic" : "normal";
-                                    let Sn = Dt;
-                                    Dt < $t ? Sn = $t : Dt > Ct && (Sn = Ct), this.current.fontSizeScale = Dt / Sn, this.ctx.font = `${_n} ${mn} ${Sn}px ${rn}`;
+                                    let yn = Dt;
+                                    Dt < $t ? yn = $t : Dt > Ct && (yn = Ct), this.current.fontSizeScale = Dt / yn, this.ctx.font = `${_n} ${mn} ${yn}px ${rn}`;
                                 }
                                 setTextRenderingMode(Ht) {
                                     this.current.textRenderingMode = Ht;
                                 }
                                 setTextRise(Ht) {
                                     this.current.textRise = Ht;
                                 }
@@ -41478,19 +41478,19 @@
                                 }
                                 paintChar(Ht, Dt, Bt, Wt) {
                                     const Yt = this.ctx,
                                         on = this.current,
                                         rn = on.font,
                                         mn = on.textRenderingMode,
                                         _n = on.fontSize / on.fontSizeScale,
-                                        Sn = mn & yt.TextRenderingMode.FILL_STROKE_MASK,
+                                        yn = mn & yt.TextRenderingMode.FILL_STROKE_MASK,
                                         Cn = !!(mn & yt.TextRenderingMode.ADD_TO_PATH_FLAG),
                                         kn = on.patternFill && !rn.missingFile;
                                     let Pn;
-                                    (rn.disableFontFace || Cn || kn) && (Pn = rn.getPathGenerator(this.commonObjs, Ht)), rn.disableFontFace || kn ? (Yt.save(), Yt.translate(Dt, Bt), Yt.beginPath(), Pn(Yt, _n), Wt && Yt.setTransform(...Wt), (Sn === yt.TextRenderingMode.FILL || Sn === yt.TextRenderingMode.FILL_STROKE) && Yt.fill(), (Sn === yt.TextRenderingMode.STROKE || Sn === yt.TextRenderingMode.FILL_STROKE) && Yt.stroke(), Yt.restore()) : ((Sn === yt.TextRenderingMode.FILL || Sn === yt.TextRenderingMode.FILL_STROKE) && Yt.fillText(Ht, Dt, Bt), (Sn === yt.TextRenderingMode.STROKE || Sn === yt.TextRenderingMode.FILL_STROKE) && Yt.strokeText(Ht, Dt, Bt)), Cn && (this.pendingTextPaths || (this.pendingTextPaths = [])).push({
+                                    (rn.disableFontFace || Cn || kn) && (Pn = rn.getPathGenerator(this.commonObjs, Ht)), rn.disableFontFace || kn ? (Yt.save(), Yt.translate(Dt, Bt), Yt.beginPath(), Pn(Yt, _n), Wt && Yt.setTransform(...Wt), (yn === yt.TextRenderingMode.FILL || yn === yt.TextRenderingMode.FILL_STROKE) && Yt.fill(), (yn === yt.TextRenderingMode.STROKE || yn === yt.TextRenderingMode.FILL_STROKE) && Yt.stroke(), Yt.restore()) : ((yn === yt.TextRenderingMode.FILL || yn === yt.TextRenderingMode.FILL_STROKE) && Yt.fillText(Ht, Dt, Bt), (yn === yt.TextRenderingMode.STROKE || yn === yt.TextRenderingMode.FILL_STROKE) && Yt.strokeText(Ht, Dt, Bt)), Cn && (this.pendingTextPaths || (this.pendingTextPaths = [])).push({
                                         transform: (0, Et.getCurrentTransform)(Yt),
                                         x: Dt,
                                         y: Bt,
                                         fontSize: _n,
                                         addToPath: Pn
                                     });
                                 }
@@ -41517,112 +41517,112 @@
                                     if (Wt === 0)
                                         return;
                                     const Yt = this.ctx,
                                         on = Dt.fontSizeScale,
                                         rn = Dt.charSpacing,
                                         mn = Dt.wordSpacing,
                                         _n = Dt.fontDirection,
-                                        Sn = Dt.textHScale * _n,
+                                        yn = Dt.textHScale * _n,
                                         Cn = Ht.length,
                                         kn = Bt.vertical,
                                         Pn = kn ? 1 : -1,
                                         Mn = Bt.defaultVMetrics,
                                         Wn = Wt * Dt.fontMatrix[0],
                                         Rn = Dt.textRenderingMode === yt.TextRenderingMode.FILL && !Bt.disableFontFace && !Dt.patternFill;
-                                    Yt.save(), Yt.transform(...Dt.textMatrix), Yt.translate(Dt.x, Dt.y + Dt.textRise), _n > 0 ? Yt.scale(Sn, -1) : Yt.scale(Sn, 1);
-                                    let yn;
+                                    Yt.save(), Yt.transform(...Dt.textMatrix), Yt.translate(Dt.x, Dt.y + Dt.textRise), _n > 0 ? Yt.scale(yn, -1) : Yt.scale(yn, 1);
+                                    let Fn;
                                     if (Dt.patternFill) {
                                         Yt.save();
                                         const zn = Dt.fillColor.getPattern(Yt, this, (0, Et.getCurrentTransformInverse)(Yt), xt.PathType.FILL);
-                                        yn = (0, Et.getCurrentTransform)(Yt), Yt.restore(), Yt.fillStyle = zn;
+                                        Fn = (0, Et.getCurrentTransform)(Yt), Yt.restore(), Yt.fillStyle = zn;
                                     }
-                                    let jn = Dt.lineWidth;
+                                    let En = Dt.lineWidth;
                                     const An = Dt.textMatrixScale;
-                                    if (An === 0 || jn === 0) {
+                                    if (An === 0 || En === 0) {
                                         const zn = Dt.textRenderingMode & yt.TextRenderingMode.FILL_STROKE_MASK;
-                                        (zn === yt.TextRenderingMode.STROKE || zn === yt.TextRenderingMode.FILL_STROKE) && (jn = this.getSinglePixelWidth());
+                                        (zn === yt.TextRenderingMode.STROKE || zn === yt.TextRenderingMode.FILL_STROKE) && (En = this.getSinglePixelWidth());
                                     } else
-                                        jn /= An;
-                                    if (on !== 1 && (Yt.scale(on, on), jn /= on), Yt.lineWidth = jn, Bt.isInvalidPDFjsFont) {
+                                        En /= An;
+                                    if (on !== 1 && (Yt.scale(on, on), En /= on), Yt.lineWidth = En, Bt.isInvalidPDFjsFont) {
                                         const zn = [];
                                         let On = 0;
                                         for (const Un of Ht)
                                             zn.push(Un.unicode), On += Un.width;
-                                        Yt.fillText(zn.join(""), 0, 0), Dt.x += On * Wn * Sn, Yt.restore(), this.compose();
+                                        Yt.fillText(zn.join(""), 0, 0), Dt.x += On * Wn * yn, Yt.restore(), this.compose();
                                         return;
                                     }
-                                    let bn = 0,
+                                    let gn = 0,
                                         xn;
                                     for (xn = 0; xn < Cn; ++xn) {
                                         const zn = Ht[xn];
                                         if (typeof zn == "number") {
-                                            bn += Pn * zn * Wt / 1e3;
+                                            gn += Pn * zn * Wt / 1e3;
                                             continue;
                                         }
                                         let On = !1;
                                         const Un = (zn.isSpace ? mn : 0) + rn,
                                             Gn = zn.fontChar,
                                             Zn = zn.accent;
                                         let Yn, lr, ur = zn.width;
                                         if (kn) {
                                             const sr = zn.vmetric || Mn,
-                                                Fn = -(zn.vmetric ? sr[1] : ur * 0.5) * Wn,
+                                                Dn = -(zn.vmetric ? sr[1] : ur * 0.5) * Wn,
                                                 wn = sr[2] * Wn;
-                                            ur = sr ? -sr[0] : ur, Yn = Fn / on, lr = (bn + wn) / on;
+                                            ur = sr ? -sr[0] : ur, Yn = Dn / on, lr = (gn + wn) / on;
                                         } else
-                                            Yn = bn / on, lr = 0;
+                                            Yn = gn / on, lr = 0;
                                         if (Bt.remeasure && ur > 0) {
                                             const sr = Yt.measureText(Gn).width * 1e3 / Wt * on;
                                             if (ur < sr && this.isFontSubpixelAAEnabled) {
-                                                const Fn = ur / sr;
-                                                On = !0, Yt.save(), Yt.scale(Fn, 1), Yn /= Fn;
+                                                const Dn = ur / sr;
+                                                On = !0, Yt.save(), Yt.scale(Dn, 1), Yn /= Dn;
                                             } else
                                                 ur !== sr && (Yn += (ur - sr) / 2e3 * Wt / on);
                                         }
                                         if (this.contentVisible && (zn.isInFont || Bt.missingFile)) {
                                             if (Rn && !Zn)
                                                 Yt.fillText(Gn, Yn, lr);
-                                            else if (this.paintChar(Gn, Yn, lr, yn), Zn) {
+                                            else if (this.paintChar(Gn, Yn, lr, Fn), Zn) {
                                                 const sr = Yn + Wt * Zn.offset.x / on,
-                                                    Fn = lr - Wt * Zn.offset.y / on;
-                                                this.paintChar(Zn.fontChar, sr, Fn, yn);
+                                                    Dn = lr - Wt * Zn.offset.y / on;
+                                                this.paintChar(Zn.fontChar, sr, Dn, Fn);
                                             }
                                         }
                                         const nr = kn ? ur * Wn - Un * _n : ur * Wn + Un * _n;
-                                        bn += nr, On && Yt.restore();
+                                        gn += nr, On && Yt.restore();
                                     }
-                                    kn ? Dt.y -= bn : Dt.x += bn * Sn, Yt.restore(), this.compose();
+                                    kn ? Dt.y -= gn : Dt.x += gn * yn, Yt.restore(), this.compose();
                                 }
                                 showType3Text(Ht) {
                                     const Dt = this.ctx,
                                         Bt = this.current,
                                         Wt = Bt.font,
                                         Yt = Bt.fontSize,
                                         on = Bt.fontDirection,
                                         rn = Wt.vertical ? 1 : -1,
                                         mn = Bt.charSpacing,
                                         _n = Bt.wordSpacing,
-                                        Sn = Bt.textHScale * on,
+                                        yn = Bt.textHScale * on,
                                         Cn = Bt.fontMatrix || yt.FONT_IDENTITY_MATRIX,
                                         kn = Ht.length,
                                         Pn = Bt.textRenderingMode === yt.TextRenderingMode.INVISIBLE;
-                                    let Mn, Wn, Rn, yn;
+                                    let Mn, Wn, Rn, Fn;
                                     if (!(Pn || Yt === 0)) {
-                                        for (this._cachedScaleForStroking[0] = -1, this._cachedGetSinglePixelWidth = null, Dt.save(), Dt.transform(...Bt.textMatrix), Dt.translate(Bt.x, Bt.y), Dt.scale(Sn, on), Mn = 0; Mn < kn; ++Mn) {
+                                        for (this._cachedScaleForStroking[0] = -1, this._cachedGetSinglePixelWidth = null, Dt.save(), Dt.transform(...Bt.textMatrix), Dt.translate(Bt.x, Bt.y), Dt.scale(yn, on), Mn = 0; Mn < kn; ++Mn) {
                                             if (Wn = Ht[Mn], typeof Wn == "number") {
-                                                yn = rn * Wn * Yt / 1e3, this.ctx.translate(yn, 0), Bt.x += yn * Sn;
+                                                Fn = rn * Wn * Yt / 1e3, this.ctx.translate(Fn, 0), Bt.x += Fn * yn;
                                                 continue;
                                             }
-                                            const jn = (Wn.isSpace ? _n : 0) + mn,
+                                            const En = (Wn.isSpace ? _n : 0) + mn,
                                                 An = Wt.charProcOperatorList[Wn.operatorListId];
                                             if (!An) {
                                                 (0, yt.warn)(`Type3 character "${Wn.operatorListId}" is not available.`);
                                                 continue;
                                             }
-                                            this.contentVisible && (this.processingType3 = Wn, this.save(), Dt.scale(Yt, Yt), Dt.transform(...Cn), this.executeOperatorList(An), this.restore()), Rn = yt.Util.applyTransform([Wn.width, 0], Cn)[0] * Yt + jn, Dt.translate(Rn, 0), Bt.x += Rn * Sn;
+                                            this.contentVisible && (this.processingType3 = Wn, this.save(), Dt.scale(Yt, Yt), Dt.transform(...Cn), this.executeOperatorList(An), this.restore()), Rn = yt.Util.applyTransform([Wn.width, 0], Cn)[0] * Yt + En, Dt.translate(Rn, 0), Bt.x += Rn * yn;
                                         }
                                         Dt.restore(), this.processingType3 = null;
                                     }
                                 }
                                 setCharWidth(Ht, Dt) {}
                                 setCharWidthAndBounds(Ht, Dt, Bt, Wt, Yt, on) {
                                     this.ctx.rect(Bt, Wt, Yt - Bt, on - Wt), this.ctx.clip(), this.endPath();
@@ -41669,16 +41669,16 @@
                                     const Bt = this._getPattern(Ht);
                                     Dt.fillStyle = Bt.getPattern(Dt, this, (0, Et.getCurrentTransformInverse)(Dt), xt.PathType.SHADING);
                                     const Wt = (0, Et.getCurrentTransformInverse)(Dt);
                                     if (Wt) {
                                         const {
                                             width: Yt,
                                             height: on
-                                        } = Dt.canvas, [rn, mn, _n, Sn] = yt.Util.getAxialAlignedBoundingBox([0, 0, Yt, on], Wt);
-                                        this.ctx.fillRect(rn, mn, _n - rn, Sn - mn);
+                                        } = Dt.canvas, [rn, mn, _n, yn] = yt.Util.getAxialAlignedBoundingBox([0, 0, Yt, on], Wt);
+                                        this.ctx.fillRect(rn, mn, _n - rn, yn - mn);
                                     } else
                                         this.ctx.fillRect(-1e10, -1e10, 2e10, 2e10);
                                     this.compose(this.current.getClippedPathBoundingBox()), this.restore();
                                 }
                                 beginInlineImage() {
                                     (0, yt.unreachable)("Should not call beginInlineImage");
                                 }
@@ -41707,33 +41707,33 @@
                                     let Wt = yt.Util.getAxialAlignedBoundingBox(Ht.bbox, (0, Et.getCurrentTransform)(Dt));
                                     const Yt = [0, 0, Dt.canvas.width, Dt.canvas.height];
                                     Wt = yt.Util.intersect(Wt, Yt) || [0, 0, 0, 0];
                                     const on = Math.floor(Wt[0]),
                                         rn = Math.floor(Wt[1]);
                                     let mn = Math.max(Math.ceil(Wt[2]) - on, 1),
                                         _n = Math.max(Math.ceil(Wt[3]) - rn, 1),
-                                        Sn = 1,
+                                        yn = 1,
                                         Cn = 1;
-                                    mn > Rt && (Sn = mn / Rt, mn = Rt), _n > Rt && (Cn = _n / Rt, _n = Rt), this.current.startNewPathAndClipBox([0, 0, mn, _n]);
+                                    mn > Rt && (yn = mn / Rt, mn = Rt), _n > Rt && (Cn = _n / Rt, _n = Rt), this.current.startNewPathAndClipBox([0, 0, mn, _n]);
                                     let kn = "groupAt" + this.groupLevel;
                                     Ht.smask && (kn += "_smask_" + this.smaskCounter++ % 2);
                                     const Pn = this.cachedCanvases.getCanvas(kn, mn, _n),
                                         Mn = Pn.context;
-                                    Mn.scale(1 / Sn, 1 / Cn), Mn.translate(-on, -rn), Mn.transform(...Bt), Ht.smask ? this.smaskStack.push({
+                                    Mn.scale(1 / yn, 1 / Cn), Mn.translate(-on, -rn), Mn.transform(...Bt), Ht.smask ? this.smaskStack.push({
                                         canvas: Pn.canvas,
                                         context: Mn,
                                         offsetX: on,
                                         offsetY: rn,
-                                        scaleX: Sn,
+                                        scaleX: yn,
                                         scaleY: Cn,
                                         subtype: Ht.smask.subtype,
                                         backdrop: Ht.smask.backdrop,
                                         transferMap: Ht.smask.transferMap || null,
                                         startTransformInverse: null
-                                    }) : (Dt.setTransform(1, 0, 0, 1, 0, 0), Dt.translate(on, rn), Dt.scale(Sn, Cn), Dt.save()), jt(Dt, Mn), this.ctx = Mn, this.setGState([
+                                    }) : (Dt.setTransform(1, 0, 0, 1, 0, 0), Dt.translate(on, rn), Dt.scale(yn, Cn), Dt.save()), jt(Dt, Mn), this.ctx = Mn, this.setGState([
                                         ["BM", "source-over"],
                                         ["ca", 1],
                                         ["CA", 1]
                                     ]), this.groupStack.push(Dt), this.groupLevel++;
                                 }
                                 endGroup(Ht) {
                                     if (!this.contentVisible)
@@ -41754,16 +41754,16 @@
                                 beginAnnotation(Ht, Dt, Bt, Wt, Yt) {
                                     if (tn(this, mt, gt).call(this), Vt(this.ctx), this.ctx.save(), this.save(), this.baseTransform && this.ctx.setTransform(...this.baseTransform), Array.isArray(Dt) && Dt.length === 4) {
                                         const on = Dt[2] - Dt[0],
                                             rn = Dt[3] - Dt[1];
                                         if (Yt && this.annotationCanvasMap) {
                                             Bt = Bt.slice(), Bt[4] -= Dt[0], Bt[5] -= Dt[1], Dt = Dt.slice(), Dt[0] = Dt[1] = 0, Dt[2] = on, Dt[3] = rn;
                                             const [mn, _n] = yt.Util.singularValueDecompose2dScale((0, Et.getCurrentTransform)(this.ctx)), {
-                                                viewportScale: Sn
-                                            } = this, Cn = Math.ceil(on * this.outputScaleX * Sn), kn = Math.ceil(rn * this.outputScaleY * Sn);
+                                                viewportScale: yn
+                                            } = this, Cn = Math.ceil(on * this.outputScaleX * yn), kn = Math.ceil(rn * this.outputScaleY * yn);
                                             this.annotationCanvas = this.canvasFactory.create(Cn, kn);
                                             const {
                                                 canvas: Pn,
                                                 context: Mn
                                             } = this.annotationCanvas;
                                             this.annotationCanvasMap.set(Ht, Pn), this.annotationCanvas.savedCtx = this.ctx, this.ctx = Mn, this.ctx.save(), this.ctx.setTransform(mn, 0, 0, -_n, 0, rn * _n), Vt(this.ctx);
                                         } else
@@ -41795,16 +41795,16 @@
                                     Ht = this.getObject(Ht.data, Ht);
                                     const rn = this.ctx;
                                     rn.save();
                                     const mn = (0, Et.getCurrentTransform)(rn);
                                     rn.transform(Dt, Bt, Wt, Yt, 0, 0);
                                     const _n = this._createMaskCanvas(Ht);
                                     rn.setTransform(1, 0, 0, 1, _n.offsetX - mn[4], _n.offsetY - mn[5]);
-                                    for (let Sn = 0, Cn = on.length; Sn < Cn; Sn += 2) {
-                                        const kn = yt.Util.transform(mn, [Dt, Bt, Wt, Yt, on[Sn], on[Sn + 1]]),
+                                    for (let yn = 0, Cn = on.length; yn < Cn; yn += 2) {
+                                        const kn = yt.Util.transform(mn, [Dt, Bt, Wt, Yt, on[yn], on[yn + 1]]),
                                             [Pn, Mn] = yt.Util.applyTransform([0, 0], kn);
                                         rn.drawImage(_n.canvas, Pn, Mn);
                                     }
                                     rn.restore(), this.compose();
                                 }
                                 paintImageMaskXObjectGroup(Ht) {
                                     if (!this.contentVisible)
@@ -41814,18 +41814,18 @@
                                         Wt = this.current.patternFill;
                                     for (const Yt of Ht) {
                                         const {
                                             data: on,
                                             width: rn,
                                             height: mn,
                                             transform: _n
-                                        } = Yt, Sn = this.cachedCanvases.getCanvas("maskCanvas", rn, mn), Cn = Sn.context;
+                                        } = Yt, yn = this.cachedCanvases.getCanvas("maskCanvas", rn, mn), Cn = yn.context;
                                         Cn.save();
                                         const kn = this.getObject(on, Yt);
-                                        zt(Cn, kn), Cn.globalCompositeOperation = "source-in", Cn.fillStyle = Wt ? Bt.getPattern(Cn, this, (0, Et.getCurrentTransformInverse)(Dt), xt.PathType.FILL) : Bt, Cn.fillRect(0, 0, rn, mn), Cn.restore(), Dt.save(), Dt.transform(..._n), Dt.scale(1, -1), Ot(Dt, Sn.canvas, 0, 0, rn, mn, 0, -1, 1, 1), Dt.restore();
+                                        zt(Cn, kn), Cn.globalCompositeOperation = "source-in", Cn.fillStyle = Wt ? Bt.getPattern(Cn, this, (0, Et.getCurrentTransformInverse)(Dt), xt.PathType.FILL) : Bt, Cn.fillRect(0, 0, rn, mn), Cn.restore(), Dt.save(), Dt.transform(..._n), Dt.scale(1, -1), Ot(Dt, yn.canvas, 0, 0, rn, mn, 0, -1, 1, 1), Dt.restore();
                                     }
                                     this.compose();
                                 }
                                 paintImageXObject(Ht) {
                                     if (!this.contentVisible)
                                         return;
                                     const Dt = this.getObject(Ht);
@@ -41842,15 +41842,15 @@
                                     if (!Yt) {
                                         (0, yt.warn)("Dependent image isn't ready yet");
                                         return;
                                     }
                                     const on = Yt.width,
                                         rn = Yt.height,
                                         mn = [];
-                                    for (let _n = 0, Sn = Wt.length; _n < Sn; _n += 2)
+                                    for (let _n = 0, yn = Wt.length; _n < yn; _n += 2)
                                         mn.push({
                                             transform: [Dt, 0, 0, Bt, Wt[_n], Wt[_n + 1]],
                                             x: 0,
                                             y: 0,
                                             w: on,
                                             h: rn
                                         });
@@ -41967,33 +41967,33 @@
                                         if (Bt === 0 && Wt === 0) {
                                             const mn = Math.abs(Dt),
                                                 _n = Math.abs(Yt);
                                             if (mn === _n)
                                                 if (Ht === 0)
                                                     on = rn = 1 / mn;
                                                 else {
-                                                    const Sn = mn * Ht;
-                                                    on = rn = Sn < 1 ? 1 / Sn : 1;
+                                                    const yn = mn * Ht;
+                                                    on = rn = yn < 1 ? 1 / yn : 1;
                                                 }
                                             else if (Ht === 0)
                                                 on = 1 / mn, rn = 1 / _n;
                                             else {
-                                                const Sn = mn * Ht,
+                                                const yn = mn * Ht,
                                                     Cn = _n * Ht;
-                                                on = Sn < 1 ? 1 / Sn : 1, rn = Cn < 1 ? 1 / Cn : 1;
+                                                on = yn < 1 ? 1 / yn : 1, rn = Cn < 1 ? 1 / Cn : 1;
                                             }
                                         } else {
                                             const mn = Math.abs(Dt * Yt - Bt * Wt),
                                                 _n = Math.hypot(Dt, Bt),
-                                                Sn = Math.hypot(Wt, Yt);
+                                                yn = Math.hypot(Wt, Yt);
                                             if (Ht === 0)
-                                                on = Sn / mn, rn = _n / mn;
+                                                on = yn / mn, rn = _n / mn;
                                             else {
                                                 const Cn = Ht * mn;
-                                                on = Sn > Cn ? Sn / Cn : 1, rn = _n > Cn ? _n / Cn : 1;
+                                                on = yn > Cn ? yn / Cn : 1, rn = _n > Cn ? _n / Cn : 1;
                                             }
                                         }
                                         this._cachedScaleForStroking[0] = on, this._cachedScaleForStroking[1] = rn;
                                     }
                                     return this._cachedScaleForStroking;
                                 }
                                 rescaleAndStroke(Ht) {
@@ -42119,30 +42119,30 @@
                                 Ht = Vt[Ft + 1],
                                 Dt = Vt[Ft + 2],
                                 Bt = Vt[zt],
                                 Wt = Vt[zt + 1],
                                 Yt = Vt[zt + 2],
                                 on = Math.round(an),
                                 rn = Math.round(pn);
-                            let mn, _n, Sn, Cn, kn, Pn, Mn, Wn;
+                            let mn, _n, yn, Cn, kn, Pn, Mn, Wn;
                             for (let Rn = on; Rn <= rn; Rn++) {
                                 if (Rn < Zt) {
                                     const xn = Rn < an ? 0 : (an - Rn) / (an - Zt);
-                                    mn = Kt - (Kt - Qt) * xn, _n = hn - (hn - Xt) * xn, Sn = un - (un - Ht) * xn, Cn = ln - (ln - Dt) * xn;
+                                    mn = Kt - (Kt - Qt) * xn, _n = hn - (hn - Xt) * xn, yn = un - (un - Ht) * xn, Cn = ln - (ln - Dt) * xn;
                                 } else {
                                     let xn;
-                                    Rn > pn ? xn = 1 : Zt === pn ? xn = 0 : xn = (Zt - Rn) / (Zt - pn), mn = Qt - (Qt - Jt) * xn, _n = Xt - (Xt - Bt) * xn, Sn = Ht - (Ht - Wt) * xn, Cn = Dt - (Dt - Yt) * xn;
+                                    Rn > pn ? xn = 1 : Zt === pn ? xn = 0 : xn = (Zt - Rn) / (Zt - pn), mn = Qt - (Qt - Jt) * xn, _n = Xt - (Xt - Bt) * xn, yn = Ht - (Ht - Wt) * xn, Cn = Dt - (Dt - Yt) * xn;
                                 }
-                                let yn;
-                                Rn < an ? yn = 0 : Rn > pn ? yn = 1 : yn = (an - Rn) / (an - pn), kn = Kt - (Kt - Jt) * yn, Pn = hn - (hn - Bt) * yn, Mn = un - (un - Wt) * yn, Wn = ln - (ln - Yt) * yn;
-                                const jn = Math.round(Math.min(mn, kn)),
+                                let Fn;
+                                Rn < an ? Fn = 0 : Rn > pn ? Fn = 1 : Fn = (an - Rn) / (an - pn), kn = Kt - (Kt - Jt) * Fn, Pn = hn - (hn - Bt) * Fn, Mn = un - (un - Wt) * Fn, Wn = ln - (ln - Yt) * Fn;
+                                const En = Math.round(Math.min(mn, kn)),
                                     An = Math.round(Math.max(mn, kn));
-                                let bn = cn * Rn + jn * 4;
-                                for (let xn = jn; xn <= An; xn++)
-                                    yn = (mn - xn) / (mn - kn), yn < 0 ? yn = 0 : yn > 1 && (yn = 1), Gt[bn++] = _n - (_n - Pn) * yn | 0, Gt[bn++] = Sn - (Sn - Mn) * yn | 0, Gt[bn++] = Cn - (Cn - Wn) * yn | 0, Gt[bn++] = 255;
+                                let gn = cn * Rn + En * 4;
+                                for (let xn = En; xn <= An; xn++)
+                                    Fn = (mn - xn) / (mn - kn), Fn < 0 ? Fn = 0 : Fn > 1 && (Fn = 1), Gt[gn++] = _n - (_n - Pn) * Fn | 0, Gt[gn++] = yn - (yn - Mn) * Fn | 0, Gt[gn++] = Cn - (Cn - Wn) * Fn | 0, Gt[gn++] = 255;
                             }
                         }
 
                         function wt(kt, At, Tt) {
                             const Ot = At.coords,
                                 It = At.colors;
                             let Nt, Ft;
@@ -45850,24 +45850,24 @@
                     /***/
                     (_e, it, ft) => {
                         var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt, cn, en, Kt, an, Qt, Zt, Jt, pn, hn, un, ln, Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn;
                         Object.defineProperty(it, "__esModule", {
                             value: !0
                         }), it.StampAnnotationElement = it.InkAnnotationElement = it.FreeTextAnnotationElement = it.AnnotationLayer = void 0;
                         var _n = ft(1),
-                            Sn = ft(6),
+                            yn = ft(6),
                             Cn = ft(3),
                             kn = ft(30),
                             Pn = ft(31),
                             Mn = ft(32);
                         const Wn = 1e3,
                             Rn = 9,
-                            yn = /* @__PURE__ */ new WeakSet();
+                            Fn = /* @__PURE__ */ new WeakSet();
 
-                        function jn(rr) {
+                        function En(rr) {
                             return {
                                 width: rr[2] - rr[0],
                                 height: rr[3] - rr[1]
                             };
                         }
                         class An {
                             static create(nn) {
@@ -45889,17 +45889,17 @@
                                         }
                                         return new Un(nn);
                                     case _n.AnnotationType.POPUP:
                                         return new sr(nn);
                                     case _n.AnnotationType.FREETEXT:
                                         return new wn(nn);
                                     case _n.AnnotationType.LINE:
-                                        return new En(nn);
+                                        return new Sn(nn);
                                     case _n.AnnotationType.SQUARE:
-                                        return new Dn(nn);
+                                        return new jn(nn);
                                     case _n.AnnotationType.CIRCLE:
                                         return new cr(nn);
                                     case _n.AnnotationType.POLYLINE:
                                         return new Tn(nn);
                                     case _n.AnnotationType.CARET:
                                         return new Qn(nn);
                                     case _n.AnnotationType.INK:
@@ -45919,21 +45919,21 @@
                                     case _n.AnnotationType.FILEATTACHMENT:
                                         return new Jn(nn);
                                     default:
                                         return new xn(nn);
                                 }
                             }
                         }
-                        const bn = class Mo {
+                        const gn = class Mo {
                             constructor(nn, {
                                 isRenderable: qt = !1,
                                 ignoreBorder: dn = !1,
-                                createQuadrilaterals: gn = !1
+                                createQuadrilaterals: vn = !1
                             } = {}) {
-                                Ut(this, mt, !1), this.isRenderable = qt, this.data = nn.data, this.layer = nn.layer, this.linkService = nn.linkService, this.downloadManager = nn.downloadManager, this.imageResourcesPath = nn.imageResourcesPath, this.renderForms = nn.renderForms, this.svgFactory = nn.svgFactory, this.annotationStorage = nn.annotationStorage, this.enableScripting = nn.enableScripting, this.hasJSActions = nn.hasJSActions, this._fieldObjects = nn.fieldObjects, this.parent = nn.parent, qt && (this.container = this._createContainer(dn)), gn && this._createQuadrilaterals();
+                                Ut(this, mt, !1), this.isRenderable = qt, this.data = nn.data, this.layer = nn.layer, this.linkService = nn.linkService, this.downloadManager = nn.downloadManager, this.imageResourcesPath = nn.imageResourcesPath, this.renderForms = nn.renderForms, this.svgFactory = nn.svgFactory, this.annotationStorage = nn.annotationStorage, this.enableScripting = nn.enableScripting, this.hasJSActions = nn.hasJSActions, this._fieldObjects = nn.fieldObjects, this.parent = nn.parent, qt && (this.container = this._createContainer(dn)), vn && this._createQuadrilaterals();
                             }
                             static _hasPopupData({
                                 titleObj: nn,
                                 contentsObj: qt,
                                 richText: dn
                             }) {
                                 return !!(nn != null && nn.str || qt != null && qt.str || dn != null && dn.str);
@@ -45942,100 +45942,100 @@
                                 return Mo._hasPopupData(this.data);
                             }
                             _createContainer(nn) {
                                 const {
                                     data: qt,
                                     parent: {
                                         page: dn,
-                                        viewport: gn
+                                        viewport: vn
                                     }
-                                } = this, vn = document.createElement("section");
-                                vn.setAttribute("data-annotation-id", qt.id), this instanceof Un || (vn.tabIndex = Wn), vn.style.zIndex = this.parent.zIndex++, this.data.popupRef && vn.setAttribute("aria-haspopup", "dialog"), qt.noRotate && vn.classList.add("norotate");
+                                } = this, bn = document.createElement("section");
+                                bn.setAttribute("data-annotation-id", qt.id), this instanceof Un || (bn.tabIndex = Wn), bn.style.zIndex = this.parent.zIndex++, this.data.popupRef && bn.setAttribute("aria-haspopup", "dialog"), qt.noRotate && bn.classList.add("norotate");
                                 const {
                                     pageWidth: $n,
                                     pageHeight: Ln,
                                     pageX: Hn,
                                     pageY: Bn
-                                } = gn.rawDims;
+                                } = vn.rawDims;
                                 if (!qt.rect || this instanceof sr) {
                                     const {
                                         rotation: dr
                                     } = qt;
-                                    return !qt.hasOwnCanvas && dr !== 0 && this.setRotation(dr, vn), vn;
+                                    return !qt.hasOwnCanvas && dr !== 0 && this.setRotation(dr, bn), bn;
                                 }
                                 const {
                                     width: qn,
                                     height: ir
-                                } = jn(qt.rect), er = _n.Util.normalizeRect([qt.rect[0], dn.view[3] - qt.rect[1] + dn.view[1], qt.rect[2], dn.view[3] - qt.rect[3] + dn.view[1]]);
+                                } = En(qt.rect), er = _n.Util.normalizeRect([qt.rect[0], dn.view[3] - qt.rect[1] + dn.view[1], qt.rect[2], dn.view[3] - qt.rect[3] + dn.view[1]]);
                                 if (!nn && qt.borderStyle.width > 0) {
-                                    vn.style.borderWidth = `${qt.borderStyle.width}px`;
+                                    bn.style.borderWidth = `${qt.borderStyle.width}px`;
                                     const dr = qt.borderStyle.horizontalCornerRadius,
                                         mr = qt.borderStyle.verticalCornerRadius;
                                     if (dr > 0 || mr > 0) {
                                         const br = `calc(${dr}px * var(--scale-factor)) / calc(${mr}px * var(--scale-factor))`;
-                                        vn.style.borderRadius = br;
+                                        bn.style.borderRadius = br;
                                     } else if (this instanceof lr) {
                                         const br = `calc(${qn}px * var(--scale-factor)) / calc(${ir}px * var(--scale-factor))`;
-                                        vn.style.borderRadius = br;
+                                        bn.style.borderRadius = br;
                                     }
                                     switch (qt.borderStyle.style) {
                                         case _n.AnnotationBorderStyleType.SOLID:
-                                            vn.style.borderStyle = "solid";
+                                            bn.style.borderStyle = "solid";
                                             break;
                                         case _n.AnnotationBorderStyleType.DASHED:
-                                            vn.style.borderStyle = "dashed";
+                                            bn.style.borderStyle = "dashed";
                                             break;
                                         case _n.AnnotationBorderStyleType.BEVELED:
                                             (0, _n.warn)("Unimplemented border style: beveled");
                                             break;
                                         case _n.AnnotationBorderStyleType.INSET:
                                             (0, _n.warn)("Unimplemented border style: inset");
                                             break;
                                         case _n.AnnotationBorderStyleType.UNDERLINE:
-                                            vn.style.borderBottomStyle = "solid";
+                                            bn.style.borderBottomStyle = "solid";
                                             break;
                                     }
                                     const pr = qt.borderColor || null;
-                                    pr ? (sn(this, mt, !0), vn.style.borderColor = _n.Util.makeHexColor(pr[0] | 0, pr[1] | 0, pr[2] | 0)) : vn.style.borderWidth = 0;
+                                    pr ? (sn(this, mt, !0), bn.style.borderColor = _n.Util.makeHexColor(pr[0] | 0, pr[1] | 0, pr[2] | 0)) : bn.style.borderWidth = 0;
                                 }
-                                vn.style.left = `${100 * (er[0] - Hn) / $n}%`, vn.style.top = `${100 * (er[1] - Bn) / Ln}%`;
+                                bn.style.left = `${100 * (er[0] - Hn) / $n}%`, bn.style.top = `${100 * (er[1] - Bn) / Ln}%`;
                                 const {
                                     rotation: ar
                                 } = qt;
-                                return qt.hasOwnCanvas || ar === 0 ? (vn.style.width = `${100 * qn / $n}%`, vn.style.height = `${100 * ir / Ln}%`) : this.setRotation(ar, vn), vn;
+                                return qt.hasOwnCanvas || ar === 0 ? (bn.style.width = `${100 * qn / $n}%`, bn.style.height = `${100 * ir / Ln}%`) : this.setRotation(ar, bn), bn;
                             }
                             setRotation(nn, qt = this.container) {
                                 if (!this.data.rect)
                                     return;
                                 const {
                                     pageWidth: dn,
-                                    pageHeight: gn
+                                    pageHeight: vn
                                 } = this.parent.viewport.rawDims, {
-                                    width: vn,
+                                    width: bn,
                                     height: $n
-                                } = jn(this.data.rect);
+                                } = En(this.data.rect);
                                 let Ln, Hn;
-                                nn % 180 === 0 ? (Ln = 100 * vn / dn, Hn = 100 * $n / gn) : (Ln = 100 * $n / dn, Hn = 100 * vn / gn), qt.style.width = `${Ln}%`, qt.style.height = `${Hn}%`, qt.setAttribute("data-main-rotation", (360 - nn) % 360);
+                                nn % 180 === 0 ? (Ln = 100 * bn / dn, Hn = 100 * $n / vn) : (Ln = 100 * $n / dn, Hn = 100 * bn / vn), qt.style.width = `${Ln}%`, qt.style.height = `${Hn}%`, qt.setAttribute("data-main-rotation", (360 - nn) % 360);
                             }
                             get _commonActions() {
-                                const nn = (qt, dn, gn) => {
-                                    const vn = gn.detail[qt],
-                                        $n = vn[0],
-                                        Ln = vn.slice(1);
-                                    gn.target.style[dn] = kn.ColorConverters[`${$n}_HTML`](Ln), this.annotationStorage.setValue(this.data.id, {
+                                const nn = (qt, dn, vn) => {
+                                    const bn = vn.detail[qt],
+                                        $n = bn[0],
+                                        Ln = bn.slice(1);
+                                    vn.target.style[dn] = kn.ColorConverters[`${$n}_HTML`](Ln), this.annotationStorage.setValue(this.data.id, {
                                         [dn]: kn.ColorConverters[`${$n}_rgb`](Ln)
                                     });
                                 };
                                 return (0, _n.shadow)(this, "_commonActions", {
                                     display: (qt) => {
                                         const {
                                             display: dn
-                                        } = qt.detail, gn = dn % 2 === 1;
-                                        this.container.style.visibility = gn ? "hidden" : "visible", this.annotationStorage.setValue(this.data.id, {
-                                            noView: gn,
+                                        } = qt.detail, vn = dn % 2 === 1;
+                                        this.container.style.visibility = vn ? "hidden" : "visible", this.annotationStorage.setValue(this.data.id, {
+                                            noView: vn,
                                             noPrint: dn === 1 || dn === 2
                                         });
                                     },
                                     print: (qt) => {
                                         this.annotationStorage.setValue(this.data.id, {
                                             noPrint: !qt.detail.print
                                         });
@@ -46087,72 +46087,72 @@
                                             rotation: dn
                                         });
                                     }
                                 });
                             }
                             _dispatchEventFromSandbox(nn, qt) {
                                 const dn = this._commonActions;
-                                for (const gn of Object.keys(qt.detail)) {
-                                    const vn = nn[gn] || dn[gn];
-                                    vn == null || vn(qt);
+                                for (const vn of Object.keys(qt.detail)) {
+                                    const bn = nn[vn] || dn[vn];
+                                    bn == null || bn(qt);
                                 }
                             }
                             _setDefaultPropertiesFromJS(nn) {
                                 if (!this.enableScripting)
                                     return;
                                 const qt = this.annotationStorage.getRawValue(this.data.id);
                                 if (!qt)
                                     return;
                                 const dn = this._commonActions;
-                                for (const [gn, vn] of Object.entries(qt)) {
-                                    const $n = dn[gn];
+                                for (const [vn, bn] of Object.entries(qt)) {
+                                    const $n = dn[vn];
                                     if ($n) {
                                         const Ln = {
                                             detail: {
-                                                [gn]: vn
+                                                [vn]: bn
                                             },
                                             target: nn
                                         };
-                                        $n(Ln), delete qt[gn];
+                                        $n(Ln), delete qt[vn];
                                     }
                                 }
                             }
                             _createQuadrilaterals() {
                                 if (!this.container)
                                     return;
                                 const {
                                     quadPoints: nn
                                 } = this.data;
                                 if (!nn)
                                     return;
-                                const [qt, dn, gn, vn] = this.data.rect;
+                                const [qt, dn, vn, bn] = this.data.rect;
                                 if (nn.length === 1) {
                                     const [, {
                                         x: mr,
                                         y: pr
                                     }, {
                                         x: br,
                                         y: _r
                                     }] = nn[0];
-                                    if (gn === mr && vn === pr && qt === br && dn === _r)
+                                    if (vn === mr && bn === pr && qt === br && dn === _r)
                                         return;
                                 }
                                 const {
                                     style: $n
                                 } = this.container;
                                 let Ln;
                                 if (St(this, mt)) {
                                     const {
                                         borderColor: mr,
                                         borderWidth: pr
                                     } = $n;
                                     $n.borderWidth = 0, Ln = ["url('data:image/svg+xml;utf8,", '<svg xmlns="http://www.w3.org/2000/svg"', ' preserveAspectRatio="none" viewBox="0 0 1 1">', `<g fill="transparent" stroke="${mr}" stroke-width="${pr}">`], this.container.classList.add("hasBorder");
                                 }
-                                const Hn = gn - qt,
-                                    Bn = vn - dn,
+                                const Hn = vn - qt,
+                                    Bn = bn - dn,
                                     {
                                         svgFactory: qn
                                     } = this,
                                     ir = qn.createElement("svg");
                                 ir.classList.add("quadrilateralsContainer"), ir.setAttribute("width", 0), ir.setAttribute("height", 0);
                                 const er = qn.createElement("defs");
                                 ir.append(er);
@@ -46164,15 +46164,15 @@
                                         y: pr
                                     }, {
                                         x: br,
                                         y: _r
                                     }] of nn) {
                                     const yr = qn.createElement("rect"),
                                         Pr = (br - qt) / Hn,
-                                        Cr = (vn - pr) / Bn,
+                                        Cr = (bn - pr) / Bn,
                                         kr = (mr - br) / Hn,
                                         Dr = (pr - _r) / Bn;
                                     yr.setAttribute("x", Pr), yr.setAttribute("y", Cr), yr.setAttribute("width", kr), yr.setAttribute("height", Dr), ar.append(yr), Ln == null || Ln.push(`<rect vector-effect="non-scaling-stroke" x="${Pr}" y="${Cr}" width="${kr}" height="${Dr}"/>`);
                                 }
                                 St(this, mt) && (Ln.push("</g></svg>')"), $n.backgroundImage = Ln.join("")), this.container.append(ir), this.container.style.clipPath = `url(#${dr})`;
                             }
                             _createPopup() {
@@ -46200,46 +46200,46 @@
                             }
                             render() {
                                 (0, _n.unreachable)("Abstract method `AnnotationElement.render` called");
                             }
                             _getElementsByName(nn, qt = null) {
                                 const dn = [];
                                 if (this._fieldObjects) {
-                                    const gn = this._fieldObjects[nn];
-                                    if (gn)
+                                    const vn = this._fieldObjects[nn];
+                                    if (vn)
                                         for (const {
-                                                page: vn,
+                                                page: bn,
                                                 id: $n,
                                                 exportValues: Ln
                                             }
-                                            of gn) {
-                                            if (vn === -1 || $n === qt)
+                                            of vn) {
+                                            if (bn === -1 || $n === qt)
                                                 continue;
                                             const Hn = typeof Ln == "string" ? Ln : null,
                                                 Bn = document.querySelector(`[data-element-id="${$n}"]`);
-                                            if (Bn && !yn.has(Bn)) {
+                                            if (Bn && !Fn.has(Bn)) {
                                                 (0, _n.warn)(`_getElementsByName - element not allowed: ${$n}`);
                                                 continue;
                                             }
                                             dn.push({
                                                 id: $n,
                                                 exportValue: Hn,
                                                 domElement: Bn
                                             });
                                         }
                                     return dn;
                                 }
-                                for (const gn of document.getElementsByName(nn)) {
+                                for (const vn of document.getElementsByName(nn)) {
                                     const {
-                                        exportValue: vn
-                                    } = gn, $n = gn.getAttribute("data-element-id");
-                                    $n !== qt && yn.has(gn) && dn.push({
+                                        exportValue: bn
+                                    } = vn, $n = vn.getAttribute("data-element-id");
+                                    $n !== qt && Fn.has(vn) && dn.push({
                                         id: $n,
-                                        exportValue: vn,
-                                        domElement: gn
+                                        exportValue: bn,
+                                        domElement: vn
                                     });
                                 }
                                 return dn;
                             }
                             show() {
                                 var nn;
                                 this.container && (this.container.hidden = !1), (nn = this.popup) == null || nn.maybeShow();
@@ -46273,31 +46273,31 @@
                                         mode: nn,
                                         editId: qt
                                     });
                                 });
                             }
                         };
                         mt = /* @__PURE__ */ new WeakMap();
-                        let xn = bn;
+                        let xn = gn;
                         class zn extends xn {
                             constructor(nn, qt = null) {
                                 super(nn, {
                                     isRenderable: !0,
                                     ignoreBorder: !!(qt != null && qt.ignoreBorder),
                                     createQuadrilaterals: !0
                                 }), Ut(this, gt), Ut(this, _t), this.isTooltipOnly = nn.data.isTooltipOnly;
                             }
                             render() {
                                 const {
                                     data: nn,
                                     linkService: qt
                                 } = this, dn = document.createElement("a");
                                 dn.setAttribute("data-element-id", nn.id);
-                                let gn = !1;
-                                return nn.url ? (qt.addLinkAttributes(dn, nn.url, nn.newWindow), gn = !0) : nn.action ? (this._bindNamedAction(dn, nn.action), gn = !0) : nn.attachment ? (this._bindAttachment(dn, nn.attachment), gn = !0) : nn.setOCGState ? (tn(this, _t, yt).call(this, dn, nn.setOCGState), gn = !0) : nn.dest ? (this._bindLink(dn, nn.dest), gn = !0) : (nn.actions && (nn.actions.Action || nn.actions["Mouse Up"] || nn.actions["Mouse Down"]) && this.enableScripting && this.hasJSActions && (this._bindJSAction(dn, nn), gn = !0), nn.resetForm ? (this._bindResetFormAction(dn, nn.resetForm), gn = !0) : this.isTooltipOnly && !gn && (this._bindLink(dn, ""), gn = !0)), this.container.classList.add("linkAnnotation"), gn && this.container.append(dn), this.container;
+                                let vn = !1;
+                                return nn.url ? (qt.addLinkAttributes(dn, nn.url, nn.newWindow), vn = !0) : nn.action ? (this._bindNamedAction(dn, nn.action), vn = !0) : nn.attachment ? (this._bindAttachment(dn, nn.attachment), vn = !0) : nn.setOCGState ? (tn(this, _t, yt).call(this, dn, nn.setOCGState), vn = !0) : nn.dest ? (this._bindLink(dn, nn.dest), vn = !0) : (nn.actions && (nn.actions.Action || nn.actions["Mouse Up"] || nn.actions["Mouse Down"]) && this.enableScripting && this.hasJSActions && (this._bindJSAction(dn, nn), vn = !0), nn.resetForm ? (this._bindResetFormAction(dn, nn.resetForm), vn = !0) : this.isTooltipOnly && !vn && (this._bindLink(dn, ""), vn = !0)), this.container.classList.add("linkAnnotation"), vn && this.container.append(dn), this.container;
                             }
                             _bindLink(nn, qt) {
                                 nn.href = this.linkService.getDestinationHash(qt), nn.onclick = () => (qt && this.linkService.goToDestination(qt), !1), (qt || qt === "") && tn(this, gt, bt).call(this);
                             }
                             _bindNamedAction(nn, qt) {
                                 nn.href = this.linkService.getAnchorUrl(""), nn.onclick = () => (this.linkService.executeNamedAction(qt), !1), tn(this, gt, bt).call(this);
                             }
@@ -46310,46 +46310,46 @@
                             _bindJSAction(nn, qt) {
                                 nn.href = this.linkService.getAnchorUrl("");
                                 const dn = /* @__PURE__ */ new Map([
                                     ["Action", "onclick"],
                                     ["Mouse Up", "onmouseup"],
                                     ["Mouse Down", "onmousedown"]
                                 ]);
-                                for (const gn of Object.keys(qt.actions)) {
-                                    const vn = dn.get(gn);
-                                    vn && (nn[vn] = () => {
+                                for (const vn of Object.keys(qt.actions)) {
+                                    const bn = dn.get(vn);
+                                    bn && (nn[bn] = () => {
                                         var $n;
                                         return ($n = this.linkService.eventBus) == null || $n.dispatch("dispatcheventinsandbox", {
                                             source: this,
                                             detail: {
                                                 id: qt.id,
-                                                name: gn
+                                                name: vn
                                             }
                                         }), !1;
                                     });
                                 }
                                 nn.onclick || (nn.onclick = () => !1), tn(this, gt, bt).call(this);
                             }
                             _bindResetFormAction(nn, qt) {
                                 const dn = nn.onclick;
                                 if (dn || (nn.href = this.linkService.getAnchorUrl("")), tn(this, gt, bt).call(this), !this._fieldObjects) {
                                     (0, _n.warn)('_bindResetFormAction - "resetForm" action not supported, ensure that the `fieldObjects` parameter is provided.'), dn || (nn.onclick = () => !1);
                                     return;
                                 }
                                 nn.onclick = () => {
-                                    var gn;
+                                    var vn;
                                     dn == null || dn();
                                     const {
-                                        fields: vn,
+                                        fields: bn,
                                         refs: $n,
                                         include: Ln
                                     } = qt, Hn = [];
-                                    if (vn.length !== 0 || $n.length !== 0) {
+                                    if (bn.length !== 0 || $n.length !== 0) {
                                         const ir = new Set($n);
-                                        for (const er of vn) {
+                                        for (const er of bn) {
                                             const ar = this._fieldObjects[er] || [];
                                             for (const {
                                                     id: dr
                                                 }
                                                 of ar)
                                                 ir.add(dr);
                                         }
@@ -46390,23 +46390,23 @@
                                                 break;
                                             }
                                             default:
                                                 continue;
                                         }
                                         const ar = document.querySelector(`[data-element-id="${er}"]`);
                                         if (ar) {
-                                            if (!yn.has(ar)) {
+                                            if (!Fn.has(ar)) {
                                                 (0, _n.warn)(`_bindResetFormAction - element not allowed: ${er}`);
                                                 continue;
                                             }
                                         } else
                                             continue;
                                         ar.dispatchEvent(new Event("resetform"));
                                     }
-                                    return this.enableScripting && ((gn = this.linkService.eventBus) == null || gn.dispatch("dispatcheventinsandbox", {
+                                    return this.enableScripting && ((vn = this.linkService.eventBus) == null || vn.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: "app",
                                             ids: qn,
                                             name: "ResetForm"
                                         }
                                     })), !1;
@@ -46443,23 +46443,23 @@
                             _getKeyModifier(nn) {
                                 const {
                                     isWin: qt,
                                     isMac: dn
                                 } = _n.FeatureTest.platform;
                                 return qt && nn.ctrlKey || dn && nn.metaKey;
                             }
-                            _setEventListener(nn, qt, dn, gn, vn) {
+                            _setEventListener(nn, qt, dn, vn, bn) {
                                 dn.includes("mouse") ? nn.addEventListener(dn, ($n) => {
                                     var Ln;
                                     (Ln = this.linkService.eventBus) == null || Ln.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: this.data.id,
-                                            name: gn,
-                                            value: vn($n),
+                                            name: vn,
+                                            value: bn($n),
                                             shift: $n.shiftKey,
                                             modifier: this._getKeyModifier($n)
                                         }
                                     });
                                 }) : nn.addEventListener(dn, ($n) => {
                                     var Ln;
                                     if (dn === "blur") {
@@ -46467,134 +46467,134 @@
                                             return;
                                         qt.focused = !1;
                                     } else if (dn === "focus") {
                                         if (qt.focused)
                                             return;
                                         qt.focused = !0;
                                     }
-                                    vn && ((Ln = this.linkService.eventBus) == null || Ln.dispatch("dispatcheventinsandbox", {
+                                    bn && ((Ln = this.linkService.eventBus) == null || Ln.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: this.data.id,
-                                            name: gn,
-                                            value: vn($n)
+                                            name: vn,
+                                            value: bn($n)
                                         }
                                     }));
                                 });
                             }
-                            _setEventListeners(nn, qt, dn, gn) {
-                                var vn, $n, Ln;
+                            _setEventListeners(nn, qt, dn, vn) {
+                                var bn, $n, Ln;
                                 for (const [Hn, Bn] of dn)
-                                    (Bn === "Action" || (vn = this.data.actions) != null && vn[Bn]) && ((Bn === "Focus" || Bn === "Blur") && (qt || (qt = {
+                                    (Bn === "Action" || (bn = this.data.actions) != null && bn[Bn]) && ((Bn === "Focus" || Bn === "Blur") && (qt || (qt = {
                                         focused: !1
-                                    })), this._setEventListener(nn, qt, Hn, Bn, gn), Bn === "Focus" && !(($n = this.data.actions) != null && $n.Blur) ? this._setEventListener(nn, qt, "blur", "Blur", null) : Bn === "Blur" && !((Ln = this.data.actions) != null && Ln.Focus) && this._setEventListener(nn, qt, "focus", "Focus", null));
+                                    })), this._setEventListener(nn, qt, Hn, Bn, vn), Bn === "Focus" && !(($n = this.data.actions) != null && $n.Blur) ? this._setEventListener(nn, qt, "blur", "Blur", null) : Bn === "Blur" && !((Ln = this.data.actions) != null && Ln.Focus) && this._setEventListener(nn, qt, "focus", "Focus", null));
                             }
                             _setBackgroundColor(nn) {
                                 const qt = this.data.backgroundColor || null;
                                 nn.style.backgroundColor = qt === null ? "transparent" : _n.Util.makeHexColor(qt[0], qt[1], qt[2]);
                             }
                             _setTextStyle(nn) {
                                 const qt = ["left", "center", "right"],
                                     {
                                         fontColor: dn
                                     } = this.data.defaultAppearanceData,
-                                    gn = this.data.defaultAppearanceData.fontSize || Rn,
-                                    vn = nn.style;
+                                    vn = this.data.defaultAppearanceData.fontSize || Rn,
+                                    bn = nn.style;
                                 let $n;
                                 const Ln = 2,
                                     Hn = (Bn) => Math.round(10 * Bn) / 10;
                                 if (this.data.multiLine) {
                                     const Bn = Math.abs(this.data.rect[3] - this.data.rect[1] - Ln),
-                                        qn = Math.round(Bn / (_n.LINE_FACTOR * gn)) || 1,
+                                        qn = Math.round(Bn / (_n.LINE_FACTOR * vn)) || 1,
                                         ir = Bn / qn;
-                                    $n = Math.min(gn, Hn(ir / _n.LINE_FACTOR));
+                                    $n = Math.min(vn, Hn(ir / _n.LINE_FACTOR));
                                 } else {
                                     const Bn = Math.abs(this.data.rect[3] - this.data.rect[1] - Ln);
-                                    $n = Math.min(gn, Hn(Bn / _n.LINE_FACTOR));
+                                    $n = Math.min(vn, Hn(Bn / _n.LINE_FACTOR));
                                 }
-                                vn.fontSize = `calc(${$n}px * var(--scale-factor))`, vn.color = _n.Util.makeHexColor(dn[0], dn[1], dn[2]), this.data.textAlignment !== null && (vn.textAlign = qt[this.data.textAlignment]);
+                                bn.fontSize = `calc(${$n}px * var(--scale-factor))`, bn.color = _n.Util.makeHexColor(dn[0], dn[1], dn[2]), this.data.textAlignment !== null && (bn.textAlign = qt[this.data.textAlignment]);
                             }
                             _setRequired(nn, qt) {
                                 qt ? nn.setAttribute("required", !0) : nn.removeAttribute("required"), nn.setAttribute("aria-required", qt);
                             }
                         }
                         class Gn extends Un {
                             constructor(nn) {
                                 const qt = nn.renderForms || !nn.data.hasAppearance && !!nn.data.fieldValue;
                                 super(nn, {
                                     isRenderable: qt
                                 });
                             }
-                            setPropertyOnSiblings(nn, qt, dn, gn) {
-                                const vn = this.annotationStorage;
+                            setPropertyOnSiblings(nn, qt, dn, vn) {
+                                const bn = this.annotationStorage;
                                 for (const $n of this._getElementsByName(nn.name, nn.id))
-                                    $n.domElement && ($n.domElement[qt] = dn), vn.setValue($n.id, {
-                                        [gn]: dn
+                                    $n.domElement && ($n.domElement[qt] = dn), bn.setValue($n.id, {
+                                        [vn]: dn
                                     });
                             }
                             render() {
                                 var nn, qt;
                                 const dn = this.annotationStorage,
-                                    gn = this.data.id;
+                                    vn = this.data.id;
                                 this.container.classList.add("textWidgetAnnotation");
-                                let vn = null;
+                                let bn = null;
                                 if (this.renderForms) {
-                                    const $n = dn.getValue(gn, {
+                                    const $n = dn.getValue(vn, {
                                         value: this.data.fieldValue
                                     });
                                     let Ln = $n.value || "";
-                                    const Hn = dn.getValue(gn, {
+                                    const Hn = dn.getValue(vn, {
                                         charLimit: this.data.maxLen
                                     }).charLimit;
                                     Hn && Ln.length > Hn && (Ln = Ln.slice(0, Hn));
                                     let Bn = $n.formattedValue || ((nn = this.data.textContent) == null ? void 0 : nn.join(`
 `)) || null;
                                     Bn && this.data.comb && (Bn = Bn.replaceAll(/\s+/g, ""));
                                     const qn = {
                                         userValue: Ln,
                                         formattedValue: Bn,
                                         lastCommittedValue: null,
                                         commitKey: 1,
                                         focused: !1
                                     };
-                                    this.data.multiLine ? (vn = document.createElement("textarea"), vn.textContent = Bn ?? Ln, this.data.doNotScroll && (vn.style.overflowY = "hidden")) : (vn = document.createElement("input"), vn.type = "text", vn.setAttribute("value", Bn ?? Ln), this.data.doNotScroll && (vn.style.overflowX = "hidden")), this.data.hasOwnCanvas && (vn.hidden = !0), yn.add(vn), vn.setAttribute("data-element-id", gn), vn.disabled = this.data.readOnly, vn.name = this.data.fieldName, vn.tabIndex = Wn, this._setRequired(vn, this.data.required), Hn && (vn.maxLength = Hn), vn.addEventListener("input", (er) => {
-                                        dn.setValue(gn, {
+                                    this.data.multiLine ? (bn = document.createElement("textarea"), bn.textContent = Bn ?? Ln, this.data.doNotScroll && (bn.style.overflowY = "hidden")) : (bn = document.createElement("input"), bn.type = "text", bn.setAttribute("value", Bn ?? Ln), this.data.doNotScroll && (bn.style.overflowX = "hidden")), this.data.hasOwnCanvas && (bn.hidden = !0), Fn.add(bn), bn.setAttribute("data-element-id", vn), bn.disabled = this.data.readOnly, bn.name = this.data.fieldName, bn.tabIndex = Wn, this._setRequired(bn, this.data.required), Hn && (bn.maxLength = Hn), bn.addEventListener("input", (er) => {
+                                        dn.setValue(vn, {
                                             value: er.target.value
-                                        }), this.setPropertyOnSiblings(vn, "value", er.target.value, "value"), qn.formattedValue = null;
-                                    }), vn.addEventListener("resetform", (er) => {
+                                        }), this.setPropertyOnSiblings(bn, "value", er.target.value, "value"), qn.formattedValue = null;
+                                    }), bn.addEventListener("resetform", (er) => {
                                         const ar = this.data.defaultFieldValue ?? "";
-                                        vn.value = qn.userValue = ar, qn.formattedValue = null;
+                                        bn.value = qn.userValue = ar, qn.formattedValue = null;
                                     });
                                     let ir = (er) => {
                                         const {
                                             formattedValue: ar
                                         } = qn;
                                         ar != null && (er.target.value = ar), er.target.scrollLeft = 0;
                                     };
                                     if (this.enableScripting && this.hasJSActions) {
-                                        vn.addEventListener("focus", (ar) => {
+                                        bn.addEventListener("focus", (ar) => {
                                             if (qn.focused)
                                                 return;
                                             const {
                                                 target: dr
                                             } = ar;
                                             qn.userValue && (dr.value = qn.userValue), qn.lastCommittedValue = dr.value, qn.commitKey = 1, qn.focused = !0;
-                                        }), vn.addEventListener("updatefromsandbox", (ar) => {
+                                        }), bn.addEventListener("updatefromsandbox", (ar) => {
                                             this.showElementAndHideCanvas(ar.target);
                                             const dr = {
                                                 value(mr) {
-                                                    qn.userValue = mr.detail.value ?? "", dn.setValue(gn, {
+                                                    qn.userValue = mr.detail.value ?? "", dn.setValue(vn, {
                                                         value: qn.userValue.toString()
                                                     }), mr.target.value = qn.userValue;
                                                 },
                                                 formattedValue(mr) {
                                                     const {
                                                         formattedValue: pr
                                                     } = mr.detail;
-                                                    qn.formattedValue = pr, pr != null && mr.target !== document.activeElement && (mr.target.value = pr), dn.setValue(gn, {
+                                                    qn.formattedValue = pr, pr != null && mr.target !== document.activeElement && (mr.target.value = pr), dn.setValue(vn, {
                                                         formattedValue: pr
                                                     });
                                                 },
                                                 selRange(mr) {
                                                     mr.target.setSelectionRange(...mr.detail.selRange);
                                                 },
                                                 charLimit: (mr) => {
@@ -46606,75 +46606,75 @@
                                                     } = mr;
                                                     if (br === 0) {
                                                         _r.removeAttribute("maxLength");
                                                         return;
                                                     }
                                                     _r.setAttribute("maxLength", br);
                                                     let yr = qn.userValue;
-                                                    !yr || yr.length <= br || (yr = yr.slice(0, br), _r.value = qn.userValue = yr, dn.setValue(gn, {
+                                                    !yr || yr.length <= br || (yr = yr.slice(0, br), _r.value = qn.userValue = yr, dn.setValue(vn, {
                                                         value: yr
                                                     }), (pr = this.linkService.eventBus) == null || pr.dispatch("dispatcheventinsandbox", {
                                                         source: this,
                                                         detail: {
-                                                            id: gn,
+                                                            id: vn,
                                                             name: "Keystroke",
                                                             value: yr,
                                                             willCommit: !0,
                                                             commitKey: 1,
                                                             selStart: _r.selectionStart,
                                                             selEnd: _r.selectionEnd
                                                         }
                                                     }));
                                                 }
                                             };
                                             this._dispatchEventFromSandbox(dr, ar);
-                                        }), vn.addEventListener("keydown", (ar) => {
+                                        }), bn.addEventListener("keydown", (ar) => {
                                             var dr;
                                             qn.commitKey = 1;
                                             let mr = -1;
                                             if (ar.key === "Escape" ? mr = 0 : ar.key === "Enter" && !this.data.multiLine ? mr = 2 : ar.key === "Tab" && (qn.commitKey = 3), mr === -1)
                                                 return;
                                             const {
                                                 value: pr
                                             } = ar.target;
                                             qn.lastCommittedValue !== pr && (qn.lastCommittedValue = pr, qn.userValue = pr, (dr = this.linkService.eventBus) == null || dr.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
-                                                    id: gn,
+                                                    id: vn,
                                                     name: "Keystroke",
                                                     value: pr,
                                                     willCommit: !0,
                                                     commitKey: mr,
                                                     selStart: ar.target.selectionStart,
                                                     selEnd: ar.target.selectionEnd
                                                 }
                                             }));
                                         });
                                         const er = ir;
-                                        ir = null, vn.addEventListener("blur", (ar) => {
+                                        ir = null, bn.addEventListener("blur", (ar) => {
                                             var dr;
                                             if (!qn.focused || !ar.relatedTarget)
                                                 return;
                                             qn.focused = !1;
                                             const {
                                                 value: mr
                                             } = ar.target;
                                             qn.userValue = mr, qn.lastCommittedValue !== mr && ((dr = this.linkService.eventBus) == null || dr.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
-                                                    id: gn,
+                                                    id: vn,
                                                     name: "Keystroke",
                                                     value: mr,
                                                     willCommit: !0,
                                                     commitKey: qn.commitKey,
                                                     selStart: ar.target.selectionStart,
                                                     selEnd: ar.target.selectionEnd
                                                 }
                                             })), er(ar);
-                                        }), (qt = this.data.actions) != null && qt.Keystroke && vn.addEventListener("beforeinput", (ar) => {
+                                        }), (qt = this.data.actions) != null && qt.Keystroke && bn.addEventListener("beforeinput", (ar) => {
                                             var dr;
                                             qn.lastCommittedValue = null;
                                             const {
                                                 data: mr,
                                                 target: pr
                                             } = ar, {
                                                 value: br,
@@ -46700,39 +46700,39 @@
                                                 case "deleteContentForward":
                                                     _r === yr && (Cr += 1);
                                                     break;
                                             }
                                             ar.preventDefault(), (dr = this.linkService.eventBus) == null || dr.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
-                                                    id: gn,
+                                                    id: vn,
                                                     name: "Keystroke",
                                                     value: br,
                                                     change: mr || "",
                                                     willCommit: !1,
                                                     selStart: Pr,
                                                     selEnd: Cr
                                                 }
                                             });
-                                        }), this._setEventListeners(vn, qn, [
+                                        }), this._setEventListeners(bn, qn, [
                                             ["focus", "Focus"],
                                             ["blur", "Blur"],
                                             ["mousedown", "Mouse Down"],
                                             ["mouseenter", "Mouse Enter"],
                                             ["mouseleave", "Mouse Exit"],
                                             ["mouseup", "Mouse Up"]
                                         ], (ar) => ar.target.value);
                                     }
-                                    if (ir && vn.addEventListener("blur", ir), this.data.comb) {
+                                    if (ir && bn.addEventListener("blur", ir), this.data.comb) {
                                         const er = (this.data.rect[2] - this.data.rect[0]) / Hn;
-                                        vn.classList.add("comb"), vn.style.letterSpacing = `calc(${er}px * var(--scale-factor) - 1ch)`;
+                                        bn.classList.add("comb"), bn.style.letterSpacing = `calc(${er}px * var(--scale-factor) - 1ch)`;
                                     }
                                 } else
-                                    vn = document.createElement("div"), vn.textContent = this.data.fieldValue, vn.style.verticalAlign = "middle", vn.style.display = "table-cell";
-                                return this._setTextStyle(vn), this._setBackgroundColor(vn), this._setDefaultPropertiesFromJS(vn), this.container.append(vn), this.container;
+                                    bn = document.createElement("div"), bn.textContent = this.data.fieldValue, bn.style.verticalAlign = "middle", bn.style.display = "table-cell";
+                                return this._setTextStyle(bn), this._setBackgroundColor(bn), this._setDefaultPropertiesFromJS(bn), this.container.append(bn), this.container;
                             }
                         }
                         class Zn extends Un {
                             constructor(nn) {
                                 super(nn, {
                                     isRenderable: !!nn.data.hasOwnCanvas
                                 });
@@ -46744,119 +46744,119 @@
                                     isRenderable: nn.renderForms
                                 });
                             }
                             render() {
                                 const nn = this.annotationStorage,
                                     qt = this.data,
                                     dn = qt.id;
-                                let gn = nn.getValue(dn, {
+                                let vn = nn.getValue(dn, {
                                     value: qt.exportValue === qt.fieldValue
                                 }).value;
-                                typeof gn == "string" && (gn = gn !== "Off", nn.setValue(dn, {
-                                    value: gn
+                                typeof vn == "string" && (vn = vn !== "Off", nn.setValue(dn, {
+                                    value: vn
                                 })), this.container.classList.add("buttonWidgetAnnotation", "checkBox");
-                                const vn = document.createElement("input");
-                                return yn.add(vn), vn.setAttribute("data-element-id", dn), vn.disabled = qt.readOnly, this._setRequired(vn, this.data.required), vn.type = "checkbox", vn.name = qt.fieldName, gn && vn.setAttribute("checked", !0), vn.setAttribute("exportValue", qt.exportValue), vn.tabIndex = Wn, vn.addEventListener("change", ($n) => {
+                                const bn = document.createElement("input");
+                                return Fn.add(bn), bn.setAttribute("data-element-id", dn), bn.disabled = qt.readOnly, this._setRequired(bn, this.data.required), bn.type = "checkbox", bn.name = qt.fieldName, vn && bn.setAttribute("checked", !0), bn.setAttribute("exportValue", qt.exportValue), bn.tabIndex = Wn, bn.addEventListener("change", ($n) => {
                                     const {
                                         name: Ln,
                                         checked: Hn
                                     } = $n.target;
                                     for (const Bn of this._getElementsByName(Ln, dn)) {
                                         const qn = Hn && Bn.exportValue === qt.exportValue;
                                         Bn.domElement && (Bn.domElement.checked = qn), nn.setValue(Bn.id, {
                                             value: qn
                                         });
                                     }
                                     nn.setValue(dn, {
                                         value: Hn
                                     });
-                                }), vn.addEventListener("resetform", ($n) => {
+                                }), bn.addEventListener("resetform", ($n) => {
                                     const Ln = qt.defaultFieldValue || "Off";
                                     $n.target.checked = Ln === qt.exportValue;
-                                }), this.enableScripting && this.hasJSActions && (vn.addEventListener("updatefromsandbox", ($n) => {
+                                }), this.enableScripting && this.hasJSActions && (bn.addEventListener("updatefromsandbox", ($n) => {
                                     const Ln = {
                                         value(Hn) {
                                             Hn.target.checked = Hn.detail.value !== "Off", nn.setValue(dn, {
                                                 value: Hn.target.checked
                                             });
                                         }
                                     };
                                     this._dispatchEventFromSandbox(Ln, $n);
-                                }), this._setEventListeners(vn, null, [
+                                }), this._setEventListeners(bn, null, [
                                     ["change", "Validate"],
                                     ["change", "Action"],
                                     ["focus", "Focus"],
                                     ["blur", "Blur"],
                                     ["mousedown", "Mouse Down"],
                                     ["mouseenter", "Mouse Enter"],
                                     ["mouseleave", "Mouse Exit"],
                                     ["mouseup", "Mouse Up"]
-                                ], ($n) => $n.target.checked)), this._setBackgroundColor(vn), this._setDefaultPropertiesFromJS(vn), this.container.append(vn), this.container;
+                                ], ($n) => $n.target.checked)), this._setBackgroundColor(bn), this._setDefaultPropertiesFromJS(bn), this.container.append(bn), this.container;
                             }
                         }
                         class lr extends Un {
                             constructor(nn) {
                                 super(nn, {
                                     isRenderable: nn.renderForms
                                 });
                             }
                             render() {
                                 this.container.classList.add("buttonWidgetAnnotation", "radioButton");
                                 const nn = this.annotationStorage,
                                     qt = this.data,
                                     dn = qt.id;
-                                let gn = nn.getValue(dn, {
+                                let vn = nn.getValue(dn, {
                                     value: qt.fieldValue === qt.buttonValue
                                 }).value;
-                                typeof gn == "string" && (gn = gn !== qt.buttonValue, nn.setValue(dn, {
-                                    value: gn
+                                typeof vn == "string" && (vn = vn !== qt.buttonValue, nn.setValue(dn, {
+                                    value: vn
                                 }));
-                                const vn = document.createElement("input");
-                                if (yn.add(vn), vn.setAttribute("data-element-id", dn), vn.disabled = qt.readOnly, this._setRequired(vn, this.data.required), vn.type = "radio", vn.name = qt.fieldName, gn && vn.setAttribute("checked", !0), vn.tabIndex = Wn, vn.addEventListener("change", ($n) => {
+                                const bn = document.createElement("input");
+                                if (Fn.add(bn), bn.setAttribute("data-element-id", dn), bn.disabled = qt.readOnly, this._setRequired(bn, this.data.required), bn.type = "radio", bn.name = qt.fieldName, vn && bn.setAttribute("checked", !0), bn.tabIndex = Wn, bn.addEventListener("change", ($n) => {
                                         const {
                                             name: Ln,
                                             checked: Hn
                                         } = $n.target;
                                         for (const Bn of this._getElementsByName(Ln, dn))
                                             nn.setValue(Bn.id, {
                                                 value: !1
                                             });
                                         nn.setValue(dn, {
                                             value: Hn
                                         });
-                                    }), vn.addEventListener("resetform", ($n) => {
+                                    }), bn.addEventListener("resetform", ($n) => {
                                         const Ln = qt.defaultFieldValue;
                                         $n.target.checked = Ln != null && Ln === qt.buttonValue;
                                     }), this.enableScripting && this.hasJSActions) {
                                     const $n = qt.buttonValue;
-                                    vn.addEventListener("updatefromsandbox", (Ln) => {
+                                    bn.addEventListener("updatefromsandbox", (Ln) => {
                                         const Hn = {
                                             value: (Bn) => {
                                                 const qn = $n === Bn.detail.value;
                                                 for (const ir of this._getElementsByName(Bn.target.name)) {
                                                     const er = qn && ir.id === dn;
                                                     ir.domElement && (ir.domElement.checked = er), nn.setValue(ir.id, {
                                                         value: er
                                                     });
                                                 }
                                             }
                                         };
                                         this._dispatchEventFromSandbox(Hn, Ln);
-                                    }), this._setEventListeners(vn, null, [
+                                    }), this._setEventListeners(bn, null, [
                                         ["change", "Validate"],
                                         ["change", "Action"],
                                         ["focus", "Focus"],
                                         ["blur", "Blur"],
                                         ["mousedown", "Mouse Down"],
                                         ["mouseenter", "Mouse Enter"],
                                         ["mouseleave", "Mouse Exit"],
                                         ["mouseup", "Mouse Up"]
                                     ], (Ln) => Ln.target.checked);
                                 }
-                                return this._setBackgroundColor(vn), this._setDefaultPropertiesFromJS(vn), this.container.append(vn), this.container;
+                                return this._setBackgroundColor(bn), this._setDefaultPropertiesFromJS(bn), this.container.append(bn), this.container;
                             }
                         }
                         class ur extends zn {
                             constructor(nn) {
                                 super(nn, {
                                     ignoreBorder: nn.data.hasAppearance
                                 });
@@ -46879,105 +46879,105 @@
                             render() {
                                 this.container.classList.add("choiceWidgetAnnotation");
                                 const nn = this.annotationStorage,
                                     qt = this.data.id,
                                     dn = nn.getValue(qt, {
                                         value: this.data.fieldValue
                                     }),
-                                    gn = document.createElement("select");
-                                yn.add(gn), gn.setAttribute("data-element-id", qt), gn.disabled = this.data.readOnly, this._setRequired(gn, this.data.required), gn.name = this.data.fieldName, gn.tabIndex = Wn;
-                                let vn = this.data.combo && this.data.options.length > 0;
-                                this.data.combo || (gn.size = this.data.options.length, this.data.multiSelect && (gn.multiple = !0)), gn.addEventListener("resetform", (qn) => {
+                                    vn = document.createElement("select");
+                                Fn.add(vn), vn.setAttribute("data-element-id", qt), vn.disabled = this.data.readOnly, this._setRequired(vn, this.data.required), vn.name = this.data.fieldName, vn.tabIndex = Wn;
+                                let bn = this.data.combo && this.data.options.length > 0;
+                                this.data.combo || (vn.size = this.data.options.length, this.data.multiSelect && (vn.multiple = !0)), vn.addEventListener("resetform", (qn) => {
                                     const ir = this.data.defaultFieldValue;
-                                    for (const er of gn.options)
+                                    for (const er of vn.options)
                                         er.selected = er.value === ir;
                                 });
                                 for (const qn of this.data.options) {
                                     const ir = document.createElement("option");
-                                    ir.textContent = qn.displayValue, ir.value = qn.exportValue, dn.value.includes(qn.exportValue) && (ir.setAttribute("selected", !0), vn = !1), gn.append(ir);
+                                    ir.textContent = qn.displayValue, ir.value = qn.exportValue, dn.value.includes(qn.exportValue) && (ir.setAttribute("selected", !0), bn = !1), vn.append(ir);
                                 }
                                 let $n = null;
-                                if (vn) {
+                                if (bn) {
                                     const qn = document.createElement("option");
-                                    qn.value = " ", qn.setAttribute("hidden", !0), qn.setAttribute("selected", !0), gn.prepend(qn), $n = () => {
-                                        qn.remove(), gn.removeEventListener("input", $n), $n = null;
-                                    }, gn.addEventListener("input", $n);
+                                    qn.value = " ", qn.setAttribute("hidden", !0), qn.setAttribute("selected", !0), vn.prepend(qn), $n = () => {
+                                        qn.remove(), vn.removeEventListener("input", $n), $n = null;
+                                    }, vn.addEventListener("input", $n);
                                 }
                                 const Ln = (qn) => {
                                     const ir = qn ? "value" : "textContent",
                                         {
                                             options: er,
                                             multiple: ar
-                                        } = gn;
+                                        } = vn;
                                     return ar ? Array.prototype.filter.call(er, (dr) => dr.selected).map((dr) => dr[ir]) : er.selectedIndex === -1 ? null : er[er.selectedIndex][ir];
                                 };
                                 let Hn = Ln(!1);
                                 const Bn = (qn) => {
                                     const ir = qn.target.options;
                                     return Array.prototype.map.call(ir, (er) => ({
                                         displayValue: er.textContent,
                                         exportValue: er.value
                                     }));
                                 };
-                                return this.enableScripting && this.hasJSActions ? (gn.addEventListener("updatefromsandbox", (qn) => {
+                                return this.enableScripting && this.hasJSActions ? (vn.addEventListener("updatefromsandbox", (qn) => {
                                     const ir = {
                                         value(er) {
                                             $n == null || $n();
                                             const ar = er.detail.value,
                                                 dr = new Set(Array.isArray(ar) ? ar : [ar]);
-                                            for (const mr of gn.options)
+                                            for (const mr of vn.options)
                                                 mr.selected = dr.has(mr.value);
                                             nn.setValue(qt, {
                                                 value: Ln(!0)
                                             }), Hn = Ln(!1);
                                         },
                                         multipleSelection(er) {
-                                            gn.multiple = !0;
+                                            vn.multiple = !0;
                                         },
                                         remove(er) {
-                                            const ar = gn.options,
+                                            const ar = vn.options,
                                                 dr = er.detail.remove;
-                                            ar[dr].selected = !1, gn.remove(dr), ar.length > 0 && Array.prototype.findIndex.call(ar, (mr) => mr.selected) === -1 && (ar[0].selected = !0), nn.setValue(qt, {
+                                            ar[dr].selected = !1, vn.remove(dr), ar.length > 0 && Array.prototype.findIndex.call(ar, (mr) => mr.selected) === -1 && (ar[0].selected = !0), nn.setValue(qt, {
                                                 value: Ln(!0),
                                                 items: Bn(er)
                                             }), Hn = Ln(!1);
                                         },
                                         clear(er) {
-                                            for (; gn.length !== 0;)
-                                                gn.remove(0);
+                                            for (; vn.length !== 0;)
+                                                vn.remove(0);
                                             nn.setValue(qt, {
                                                 value: null,
                                                 items: []
                                             }), Hn = Ln(!1);
                                         },
                                         insert(er) {
                                             const {
                                                 index: ar,
                                                 displayValue: dr,
                                                 exportValue: mr
-                                            } = er.detail.insert, pr = gn.children[ar], br = document.createElement("option");
-                                            br.textContent = dr, br.value = mr, pr ? pr.before(br) : gn.append(br), nn.setValue(qt, {
+                                            } = er.detail.insert, pr = vn.children[ar], br = document.createElement("option");
+                                            br.textContent = dr, br.value = mr, pr ? pr.before(br) : vn.append(br), nn.setValue(qt, {
                                                 value: Ln(!0),
                                                 items: Bn(er)
                                             }), Hn = Ln(!1);
                                         },
                                         items(er) {
                                             const {
                                                 items: ar
                                             } = er.detail;
-                                            for (; gn.length !== 0;)
-                                                gn.remove(0);
+                                            for (; vn.length !== 0;)
+                                                vn.remove(0);
                                             for (const dr of ar) {
                                                 const {
                                                     displayValue: mr,
                                                     exportValue: pr
                                                 } = dr, br = document.createElement("option");
-                                                br.textContent = mr, br.value = pr, gn.append(br);
+                                                br.textContent = mr, br.value = pr, vn.append(br);
                                             }
-                                            gn.options.length > 0 && (gn.options[0].selected = !0), nn.setValue(qt, {
+                                            vn.options.length > 0 && (vn.options[0].selected = !0), nn.setValue(qt, {
                                                 value: Ln(!0),
                                                 items: Bn(er)
                                             }), Hn = Ln(!1);
                                         },
                                         indices(er) {
                                             const ar = new Set(er.detail.indices);
                                             for (const dr of er.target.options)
@@ -46987,15 +46987,15 @@
                                             }), Hn = Ln(!1);
                                         },
                                         editable(er) {
                                             er.target.disabled = !er.detail.editable;
                                         }
                                     };
                                     this._dispatchEventFromSandbox(ir, qn);
-                                }), gn.addEventListener("input", (qn) => {
+                                }), vn.addEventListener("input", (qn) => {
                                     var ir;
                                     const er = Ln(!0);
                                     nn.setValue(qt, {
                                         value: er
                                     }), qn.preventDefault(), (ir = this.linkService.eventBus) == null || ir.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
@@ -47004,43 +47004,43 @@
                                             value: Hn,
                                             changeEx: er,
                                             willCommit: !1,
                                             commitKey: 1,
                                             keyDown: !1
                                         }
                                     });
-                                }), this._setEventListeners(gn, null, [
+                                }), this._setEventListeners(vn, null, [
                                     ["focus", "Focus"],
                                     ["blur", "Blur"],
                                     ["mousedown", "Mouse Down"],
                                     ["mouseenter", "Mouse Enter"],
                                     ["mouseleave", "Mouse Exit"],
                                     ["mouseup", "Mouse Up"],
                                     ["input", "Action"],
                                     ["input", "Validate"]
-                                ], (qn) => qn.target.value)) : gn.addEventListener("input", function(qn) {
+                                ], (qn) => qn.target.value)) : vn.addEventListener("input", function(qn) {
                                     nn.setValue(qt, {
                                         value: Ln(!0)
                                     });
-                                }), this.data.combo && this._setTextStyle(gn), this._setBackgroundColor(gn), this._setDefaultPropertiesFromJS(gn), this.container.append(gn), this.container;
+                                }), this.data.combo && this._setTextStyle(vn), this._setBackgroundColor(vn), this._setDefaultPropertiesFromJS(vn), this.container.append(vn), this.container;
                             }
                         }
                         class sr extends xn {
                             constructor(nn) {
                                 const {
                                     data: qt,
                                     elements: dn
                                 } = nn;
                                 super(nn, {
                                     isRenderable: xn._hasPopupData(qt)
                                 }), this.elements = dn;
                             }
                             render() {
                                 this.container.classList.add("popupAnnotation");
-                                const nn = new Fn({
+                                const nn = new Dn({
                                         container: this.container,
                                         color: this.data.color,
                                         titleObj: this.data.titleObj,
                                         modificationDate: this.data.modificationDate,
                                         contentsObj: this.data.contentsObj,
                                         richText: this.data.richText,
                                         rect: this.data.rect,
@@ -47051,32 +47051,32 @@
                                     }),
                                     qt = [];
                                 for (const dn of this.elements)
                                     dn.popup = nn, qt.push(dn.data.id), dn.addHighlightArea();
                                 return this.container.setAttribute("aria-controls", qt.map((dn) => `${_n.AnnotationPrefix}${dn}`).join(",")), this.container;
                             }
                         }
-                        class Fn {
+                        class Dn {
                             constructor({
                                 container: nn,
                                 color: qt,
                                 elements: dn,
-                                titleObj: gn,
-                                modificationDate: vn,
+                                titleObj: vn,
+                                modificationDate: bn,
                                 contentsObj: $n,
                                 richText: Ln,
                                 parent: Hn,
                                 rect: Bn,
                                 parentRect: qn,
                                 open: ir
                             }) {
                                 Ut(this, jt), Ut(this, Gt), Ut(this, en), Ut(this, an), Ut(this, Et, null), Ut(this, xt, tn(this, jt, Vt).bind(this)), Ut(this, wt, tn(this, an, Qt).bind(this)), Ut(this, $t, tn(this, en, Kt).bind(this)), Ut(this, Ct, tn(this, Gt, cn).bind(this)), Ut(this, Rt, null), Ut(this, Mt, null), Ut(this, Lt, null), Ut(this, Pt, null), Ut(this, kt, null), Ut(this, At, null), Ut(this, Tt, !1), Ut(this, Ot, null), Ut(this, It, null), Ut(this, Nt, null), Ut(this, Ft, null), Ut(this, zt, !1);
                                 var er;
-                                sn(this, Mt, nn), sn(this, Ft, gn), sn(this, Lt, $n), sn(this, Nt, Ln), sn(this, kt, Hn), sn(this, Rt, qt), sn(this, It, Bn), sn(this, At, qn), sn(this, Pt, dn);
-                                const ar = Sn.PDFDateString.toDateObject(vn);
+                                sn(this, Mt, nn), sn(this, Ft, vn), sn(this, Lt, $n), sn(this, Nt, Ln), sn(this, kt, Hn), sn(this, Rt, qt), sn(this, It, Bn), sn(this, At, qn), sn(this, Pt, dn);
+                                const ar = yn.PDFDateString.toDateObject(bn);
                                 ar && sn(this, Et, Hn.l10n.get("annotation_date_string", {
                                     date: ar.toLocaleDateString(),
                                     time: ar.toLocaleTimeString()
                                 })), this.trigger = dn.flatMap((dr) => dr.getElementsToTriggerPopup());
                                 for (const dr of this.trigger)
                                     dr.addEventListener("click", St(this, Ct)), dr.addEventListener("mouseenter", St(this, $t)), dr.addEventListener("mouseleave", St(this, wt)), dr.classList.add("popupTriggerArea");
                                 for (const dr of dn)
@@ -47090,16 +47090,16 @@
                                     page: {
                                         view: nn
                                     },
                                     viewport: {
                                         rawDims: {
                                             pageWidth: qt,
                                             pageHeight: dn,
-                                            pageX: gn,
-                                            pageY: vn
+                                            pageX: vn,
+                                            pageY: bn
                                         }
                                     }
                                 } = St(this, kt), $n = sn(this, Ot, document.createElement("div"));
                                 if ($n.className = "popup", St(this, Rt)) {
                                     const _r = $n.style.outlineColor = _n.Util.makeHexColor(...St(this, Rt));
                                     CSS.supports("background-color", "color-mix(in srgb, red 30%, white)") ? $n.style.backgroundColor = `color-mix(in srgb, ${_r} 30%, white)` : $n.style.backgroundColor = _n.Util.makeHexColor(...St(this, Rt).map((yr) => Math.floor(0.7 * (255 - yr) + yr)));
                                 }
@@ -47137,26 +47137,26 @@
                                 const ar = _n.Util.normalizeRect([er[0], nn[3] - er[1] + nn[1], er[2], nn[3] - er[3] + nn[1]]),
                                     dr = ir ? er[2] - er[0] + 5 : 0,
                                     mr = ar[0] + dr,
                                     pr = ar[1],
                                     {
                                         style: br
                                     } = St(this, Mt);
-                                br.left = `${100 * (mr - gn) / qt}%`, br.top = `${100 * (pr - vn) / dn}%`, St(this, Mt).append($n);
+                                br.left = `${100 * (mr - vn) / qt}%`, br.top = `${100 * (pr - bn) / dn}%`, St(this, Mt).append($n);
                             }
                             _formatContents({
                                 str: nn,
                                 dir: qt
                             }) {
                                 const dn = document.createElement("p");
                                 dn.classList.add("popupContent"), dn.dir = qt;
-                                const gn = nn.split(/(?:\r\n?|\n)/);
-                                for (let vn = 0, $n = gn.length; vn < $n; ++vn) {
-                                    const Ln = gn[vn];
-                                    dn.append(document.createTextNode(Ln)), vn < $n - 1 && dn.append(document.createElement("br"));
+                                const vn = nn.split(/(?:\r\n?|\n)/);
+                                for (let bn = 0, $n = vn.length; bn < $n; ++bn) {
+                                    const Ln = vn[bn];
+                                    dn.append(document.createTextNode(Ln)), bn < $n - 1 && dn.append(document.createElement("br"));
                                 }
                                 return dn;
                             }
                             forceHide() {
                                 sn(this, zt, this.isVisible), St(this, zt) && (St(this, Mt).hidden = !0);
                             }
                             maybeShow() {
@@ -47192,58 +47192,58 @@
                                     }
                                     this.container.append(nn);
                                 }
                                 return !this.data.popupRef && this.hasPopupData && this._createPopup(), this._editOnDoubleClick(), this.container;
                             }
                         }
                         it.FreeTextAnnotationElement = wn;
-                        class En extends xn {
+                        class Sn extends xn {
                             constructor(nn) {
                                 super(nn, {
                                     isRenderable: !0,
                                     ignoreBorder: !0
                                 }), Ut(this, Zt, null);
                             }
                             render() {
                                 this.container.classList.add("lineAnnotation");
                                 const nn = this.data,
                                     {
                                         width: qt,
                                         height: dn
-                                    } = jn(nn.rect),
-                                    gn = this.svgFactory.create(qt, dn, !0),
-                                    vn = sn(this, Zt, this.svgFactory.createElement("svg:line"));
-                                return vn.setAttribute("x1", nn.rect[2] - nn.lineCoordinates[0]), vn.setAttribute("y1", nn.rect[3] - nn.lineCoordinates[1]), vn.setAttribute("x2", nn.rect[2] - nn.lineCoordinates[2]), vn.setAttribute("y2", nn.rect[3] - nn.lineCoordinates[3]), vn.setAttribute("stroke-width", nn.borderStyle.width || 1), vn.setAttribute("stroke", "transparent"), vn.setAttribute("fill", "transparent"), gn.append(vn), this.container.append(gn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                    } = En(nn.rect),
+                                    vn = this.svgFactory.create(qt, dn, !0),
+                                    bn = sn(this, Zt, this.svgFactory.createElement("svg:line"));
+                                return bn.setAttribute("x1", nn.rect[2] - nn.lineCoordinates[0]), bn.setAttribute("y1", nn.rect[3] - nn.lineCoordinates[1]), bn.setAttribute("x2", nn.rect[2] - nn.lineCoordinates[2]), bn.setAttribute("y2", nn.rect[3] - nn.lineCoordinates[3]), bn.setAttribute("stroke-width", nn.borderStyle.width || 1), bn.setAttribute("stroke", "transparent"), bn.setAttribute("fill", "transparent"), vn.append(bn), this.container.append(vn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return St(this, Zt);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
                         }
                         Zt = /* @__PURE__ */ new WeakMap();
-                        class Dn extends xn {
+                        class jn extends xn {
                             constructor(nn) {
                                 super(nn, {
                                     isRenderable: !0,
                                     ignoreBorder: !0
                                 }), Ut(this, Jt, null);
                             }
                             render() {
                                 this.container.classList.add("squareAnnotation");
                                 const nn = this.data,
                                     {
                                         width: qt,
                                         height: dn
-                                    } = jn(nn.rect),
-                                    gn = this.svgFactory.create(qt, dn, !0),
-                                    vn = nn.borderStyle.width,
+                                    } = En(nn.rect),
+                                    vn = this.svgFactory.create(qt, dn, !0),
+                                    bn = nn.borderStyle.width,
                                     $n = sn(this, Jt, this.svgFactory.createElement("svg:rect"));
-                                return $n.setAttribute("x", vn / 2), $n.setAttribute("y", vn / 2), $n.setAttribute("width", qt - vn), $n.setAttribute("height", dn - vn), $n.setAttribute("stroke-width", vn || 1), $n.setAttribute("stroke", "transparent"), $n.setAttribute("fill", "transparent"), gn.append($n), this.container.append(gn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                return $n.setAttribute("x", bn / 2), $n.setAttribute("y", bn / 2), $n.setAttribute("width", qt - bn), $n.setAttribute("height", dn - bn), $n.setAttribute("stroke-width", bn || 1), $n.setAttribute("stroke", "transparent"), $n.setAttribute("fill", "transparent"), vn.append($n), this.container.append(vn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return St(this, Jt);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -47258,19 +47258,19 @@
                             }
                             render() {
                                 this.container.classList.add("circleAnnotation");
                                 const nn = this.data,
                                     {
                                         width: qt,
                                         height: dn
-                                    } = jn(nn.rect),
-                                    gn = this.svgFactory.create(qt, dn, !0),
-                                    vn = nn.borderStyle.width,
+                                    } = En(nn.rect),
+                                    vn = this.svgFactory.create(qt, dn, !0),
+                                    bn = nn.borderStyle.width,
                                     $n = sn(this, pn, this.svgFactory.createElement("svg:ellipse"));
-                                return $n.setAttribute("cx", qt / 2), $n.setAttribute("cy", dn / 2), $n.setAttribute("rx", qt / 2 - vn / 2), $n.setAttribute("ry", dn / 2 - vn / 2), $n.setAttribute("stroke-width", vn || 1), $n.setAttribute("stroke", "transparent"), $n.setAttribute("fill", "transparent"), gn.append($n), this.container.append(gn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                return $n.setAttribute("cx", qt / 2), $n.setAttribute("cy", dn / 2), $n.setAttribute("rx", qt / 2 - bn / 2), $n.setAttribute("ry", dn / 2 - bn / 2), $n.setAttribute("stroke-width", bn || 1), $n.setAttribute("stroke", "transparent"), $n.setAttribute("fill", "transparent"), vn.append($n), this.container.append(vn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return St(this, pn);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -47285,25 +47285,25 @@
                             }
                             render() {
                                 this.container.classList.add(this.containerClassName);
                                 const nn = this.data,
                                     {
                                         width: qt,
                                         height: dn
-                                    } = jn(nn.rect),
-                                    gn = this.svgFactory.create(qt, dn, !0);
-                                let vn = [];
+                                    } = En(nn.rect),
+                                    vn = this.svgFactory.create(qt, dn, !0);
+                                let bn = [];
                                 for (const Ln of nn.vertices) {
                                     const Hn = Ln.x - nn.rect[0],
                                         Bn = nn.rect[3] - Ln.y;
-                                    vn.push(Hn + "," + Bn);
+                                    bn.push(Hn + "," + Bn);
                                 }
-                                vn = vn.join(" ");
+                                bn = bn.join(" ");
                                 const $n = sn(this, hn, this.svgFactory.createElement(this.svgElementName));
-                                return $n.setAttribute("points", vn), $n.setAttribute("stroke-width", nn.borderStyle.width || 1), $n.setAttribute("stroke", "transparent"), $n.setAttribute("fill", "transparent"), gn.append($n), this.container.append(gn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                return $n.setAttribute("points", bn), $n.setAttribute("stroke-width", nn.borderStyle.width || 1), $n.setAttribute("stroke", "transparent"), $n.setAttribute("fill", "transparent"), vn.append($n), this.container.append(vn), !nn.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return St(this, hn);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -47334,28 +47334,28 @@
                             }
                             render() {
                                 this.container.classList.add(this.containerClassName);
                                 const nn = this.data,
                                     {
                                         width: qt,
                                         height: dn
-                                    } = jn(nn.rect),
-                                    gn = this.svgFactory.create(qt, dn, !0);
-                                for (const vn of nn.inkLists) {
+                                    } = En(nn.rect),
+                                    vn = this.svgFactory.create(qt, dn, !0);
+                                for (const bn of nn.inkLists) {
                                     let $n = [];
-                                    for (const Hn of vn) {
+                                    for (const Hn of bn) {
                                         const Bn = Hn.x - nn.rect[0],
                                             qn = nn.rect[3] - Hn.y;
                                         $n.push(`${Bn},${qn}`);
                                     }
                                     $n = $n.join(" ");
                                     const Ln = this.svgFactory.createElement(this.svgElementName);
-                                    St(this, un).push(Ln), Ln.setAttribute("points", $n), Ln.setAttribute("stroke-width", nn.borderStyle.width || 1), Ln.setAttribute("stroke", "transparent"), Ln.setAttribute("fill", "transparent"), !nn.popupRef && this.hasPopupData && this._createPopup(), gn.append(Ln);
+                                    St(this, un).push(Ln), Ln.setAttribute("points", $n), Ln.setAttribute("stroke-width", nn.borderStyle.width || 1), Ln.setAttribute("stroke", "transparent"), Ln.setAttribute("fill", "transparent"), !nn.popupRef && this.hasPopupData && this._createPopup(), vn.append(Ln);
                                 }
-                                return this.container.append(gn), this.container;
+                                return this.container.append(vn), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return St(this, un);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -47425,35 +47425,35 @@
                             constructor(nn) {
                                 var qt;
                                 super(nn, {
                                     isRenderable: !0
                                 }), Ut(this, Xt), Ut(this, ln, null);
                                 const {
                                     filename: dn,
-                                    content: gn
+                                    content: vn
                                 } = this.data.file;
-                                this.filename = (0, Sn.getFilenameFromUrl)(dn, !0), this.content = gn, (qt = this.linkService.eventBus) == null || qt.dispatch("fileattachmentannotation", {
+                                this.filename = (0, yn.getFilenameFromUrl)(dn, !0), this.content = vn, (qt = this.linkService.eventBus) == null || qt.dispatch("fileattachmentannotation", {
                                     source: this,
                                     filename: dn,
-                                    content: gn
+                                    content: vn
                                 });
                             }
                             render() {
                                 this.container.classList.add("fileAttachmentAnnotation");
                                 const {
                                     container: nn,
                                     data: qt
                                 } = this;
                                 let dn;
                                 qt.hasAppearance || qt.fillAlpha === 0 ? dn = document.createElement("div") : (dn = document.createElement("img"), dn.src = `${this.imageResourcesPath}annotation-${/paperclip/i.test(qt.name) ? "paperclip" : "pushpin"}.svg`, qt.fillAlpha && qt.fillAlpha < 1 && (dn.style = `filter: opacity(${Math.round(qt.fillAlpha * 100)}%);`)), dn.addEventListener("dblclick", tn(this, Xt, Ht).bind(this)), sn(this, ln, dn);
                                 const {
-                                    isMac: gn
+                                    isMac: vn
                                 } = _n.FeatureTest.platform;
-                                return nn.addEventListener("keydown", (vn) => {
-                                    vn.key === "Enter" && (gn ? vn.metaKey : vn.ctrlKey) && tn(this, Xt, Ht).call(this);
+                                return nn.addEventListener("keydown", (bn) => {
+                                    bn.key === "Enter" && (vn ? bn.metaKey : bn.ctrlKey) && tn(this, Xt, Ht).call(this);
                                 }), !qt.popupRef && this.hasPopupData ? this._createPopup() : dn.classList.add("popupTriggerArea"), nn.append(dn), nn;
                             }
                             getElementsToTriggerPopup() {
                                 return St(this, ln);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
@@ -47464,77 +47464,77 @@
                             (rr = this.downloadManager) == null || rr.openOrDownloadData(this.container, this.content, this.filename);
                         };
                         class gr {
                             constructor({
                                 div: nn,
                                 accessibilityManager: qt,
                                 annotationCanvasMap: dn,
-                                l10n: gn,
-                                page: vn,
+                                l10n: vn,
+                                page: bn,
                                 viewport: $n
                             }) {
-                                Ut(this, Yt), Ut(this, rn), Ut(this, Dt, null), Ut(this, Bt, null), Ut(this, Wt, /* @__PURE__ */ new Map()), this.div = nn, sn(this, Dt, qt), sn(this, Bt, dn), this.l10n = gn, this.page = vn, this.viewport = $n, this.zIndex = 0, this.l10n || (this.l10n = Pn.NullL10n);
+                                Ut(this, Yt), Ut(this, rn), Ut(this, Dt, null), Ut(this, Bt, null), Ut(this, Wt, /* @__PURE__ */ new Map()), this.div = nn, sn(this, Dt, qt), sn(this, Bt, dn), this.l10n = vn, this.page = bn, this.viewport = $n, this.zIndex = 0, this.l10n || (this.l10n = Pn.NullL10n);
                             }
                             async render(nn) {
                                 const {
                                     annotations: qt
                                 } = nn, dn = this.div;
-                                (0, Sn.setLayerDimensions)(dn, this.viewport);
-                                const gn = /* @__PURE__ */ new Map(),
-                                    vn = {
+                                (0, yn.setLayerDimensions)(dn, this.viewport);
+                                const vn = /* @__PURE__ */ new Map(),
+                                    bn = {
                                         data: null,
                                         layer: dn,
                                         linkService: nn.linkService,
                                         downloadManager: nn.downloadManager,
                                         imageResourcesPath: nn.imageResourcesPath || "",
                                         renderForms: nn.renderForms !== !1,
-                                        svgFactory: new Sn.DOMSVGFactory(),
+                                        svgFactory: new yn.DOMSVGFactory(),
                                         annotationStorage: nn.annotationStorage || new Cn.AnnotationStorage(),
                                         enableScripting: nn.enableScripting === !0,
                                         hasJSActions: nn.hasJSActions,
                                         fieldObjects: nn.fieldObjects,
                                         parent: this,
                                         elements: null
                                     };
                                 for (const $n of qt) {
                                     if ($n.noHTML)
                                         continue;
                                     const Ln = $n.annotationType === _n.AnnotationType.POPUP;
                                     if (Ln) {
-                                        const qn = gn.get($n.id);
+                                        const qn = vn.get($n.id);
                                         if (!qn)
                                             continue;
-                                        vn.elements = qn;
+                                        bn.elements = qn;
                                     } else {
                                         const {
                                             width: qn,
                                             height: ir
-                                        } = jn($n.rect);
+                                        } = En($n.rect);
                                         if (qn <= 0 || ir <= 0)
                                             continue;
                                     }
-                                    vn.data = $n;
-                                    const Hn = An.create(vn);
+                                    bn.data = $n;
+                                    const Hn = An.create(bn);
                                     if (!Hn.isRenderable)
                                         continue;
                                     if (!Ln && $n.popupRef) {
-                                        const qn = gn.get($n.popupRef);
-                                        qn ? qn.push(Hn) : gn.set($n.popupRef, [Hn]);
+                                        const qn = vn.get($n.popupRef);
+                                        qn ? qn.push(Hn) : vn.set($n.popupRef, [Hn]);
                                     }
                                     Hn.annotationEditorType > 0 && St(this, Wt).set(Hn.data.id, Hn);
                                     const Bn = Hn.render();
                                     $n.hidden && (Bn.style.visibility = "hidden"), tn(this, Yt, on).call(this, Bn, $n.id);
                                 }
                                 tn(this, rn, mn).call(this), await this.l10n.translate(dn);
                             }
                             update({
                                 viewport: nn
                             }) {
                                 const qt = this.div;
-                                this.viewport = nn, (0, Sn.setLayerDimensions)(qt, {
+                                this.viewport = nn, (0, yn.setLayerDimensions)(qt, {
                                     rotation: nn.rotation
                                 }), tn(this, rn, mn).call(this), qt.hidden = !1;
                             }
                             getEditableAnnotations() {
                                 return Array.from(St(this, Wt).values());
                             }
                             getEditableAnnotation(nn) {
@@ -47550,17 +47550,17 @@
                                 return;
                             const rr = this.div;
                             for (const [nn, qt] of St(this, Bt)) {
                                 const dn = rr.querySelector(`[data-annotation-id="${nn}"]`);
                                 if (!dn)
                                     continue;
                                 const {
-                                    firstChild: gn
+                                    firstChild: vn
                                 } = dn;
-                                gn ? gn.nodeName === "CANVAS" ? gn.replaceWith(qt) : gn.before(qt) : dn.append(qt);
+                                vn ? vn.nodeName === "CANVAS" ? vn.replaceWith(qt) : vn.before(qt) : dn.append(qt);
                             }
                             St(this, Bt).clear();
                         }, it.AnnotationLayer = gr;
                     },
                     /* 30 */
                     /***/
                     (_e, it) => {
@@ -47871,29 +47871,29 @@
                             }
                         }
                         it.XfaLayer = gt;
                     },
                     /* 33 */
                     /***/
                     (_e, it, ft) => {
-                        var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt, cn, en, Kt, an, Qt, Zt, Jt, pn, hn, un, ln, Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, Sn, Cn, kn, Pn, Mn, Wn, Rn, yn, jn, An, bn, xn, zn, On, Un, Gn, Zn, Yn, lr, ur;
+                        var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt, cn, en, Kt, an, Qt, Zt, Jt, pn, hn, un, ln, Xt, Ht, Dt, Bt, Wt, Yt, on, rn, mn, _n, yn, Cn, kn, Pn, Mn, Wn, Rn, Fn, En, An, gn, xn, zn, On, Un, Gn, Zn, Yn, lr, ur;
                         Object.defineProperty(it, "__esModule", {
                             value: !0
                         }), it.InkEditor = void 0;
                         var nr = ft(1),
                             sr = ft(4),
-                            Fn = ft(29),
+                            Dn = ft(29),
                             wn = ft(6),
-                            En = ft(5);
-                        const Dn = class zr extends sr.AnnotationEditor {
+                            Sn = ft(5);
+                        const jn = class zr extends sr.AnnotationEditor {
                             constructor(In) {
                                 super({
                                     ...In,
                                     name: "inkEditor"
-                                }), Ut(this, kt), Ut(this, Tt), Ut(this, It), Ut(this, Ft), Ut(this, jt), Ut(this, Gt), Ut(this, en), Ut(this, an), Ut(this, Zt), Ut(this, pn), Ut(this, un), Ut(this, Xt), Ut(this, Dt), Ut(this, Wt), Ut(this, on), Ut(this, mn), Ut(this, Sn), Ut(this, kn), Ut(this, Mn), Ut(this, zn), Ut(this, Un), Ut(this, Zn), Ut(this, lr), Ut(this, mt, 0), Ut(this, gt, 0), Ut(this, bt, this.canvasPointermove.bind(this)), Ut(this, _t, this.canvasPointerleave.bind(this)), Ut(this, yt, this.canvasPointerup.bind(this)), Ut(this, Et, this.canvasPointerdown.bind(this)), Ut(this, xt, new Path2D()), Ut(this, wt, !1), Ut(this, $t, !1), Ut(this, Ct, !1), Ut(this, Rt, null), Ut(this, Mt, 0), Ut(this, Lt, 0), Ut(this, Pt, null), this.color = In.color || null, this.thickness = In.thickness || null, this.opacity = In.opacity || null, this.paths = [], this.bezierPath2D = [], this.allRawPaths = [], this.currentPath = [], this.scaleFactor = 1, this.translationX = this.translationY = 0, this.x = 0, this.y = 0, this._willKeepAspectRatio = !0;
+                                }), Ut(this, kt), Ut(this, Tt), Ut(this, It), Ut(this, Ft), Ut(this, jt), Ut(this, Gt), Ut(this, en), Ut(this, an), Ut(this, Zt), Ut(this, pn), Ut(this, un), Ut(this, Xt), Ut(this, Dt), Ut(this, Wt), Ut(this, on), Ut(this, mn), Ut(this, yn), Ut(this, kn), Ut(this, Mn), Ut(this, zn), Ut(this, Un), Ut(this, Zn), Ut(this, lr), Ut(this, mt, 0), Ut(this, gt, 0), Ut(this, bt, this.canvasPointermove.bind(this)), Ut(this, _t, this.canvasPointerleave.bind(this)), Ut(this, yt, this.canvasPointerup.bind(this)), Ut(this, Et, this.canvasPointerdown.bind(this)), Ut(this, xt, new Path2D()), Ut(this, wt, !1), Ut(this, $t, !1), Ut(this, Ct, !1), Ut(this, Rt, null), Ut(this, Mt, 0), Ut(this, Lt, 0), Ut(this, Pt, null), this.color = In.color || null, this.thickness = In.thickness || null, this.opacity = In.opacity || null, this.paths = [], this.bezierPath2D = [], this.allRawPaths = [], this.currentPath = [], this.scaleFactor = 1, this.translationX = this.translationY = 0, this.x = 0, this.y = 0, this._willKeepAspectRatio = !0;
                             }
                             static initialize(In) {
                                 sr.AnnotationEditor.initialize(In, {
                                     strings: ["editor_ink_canvas_aria_label", "editor_ink2_aria_label"]
                                 });
                             }
                             static updateDefaultParams(In, Qn) {
@@ -47933,15 +47933,15 @@
                                 return [
                                     [nr.AnnotationEditorParamsType.INK_THICKNESS, this.thickness || zr._defaultThickness],
                                     [nr.AnnotationEditorParamsType.INK_COLOR, this.color || zr._defaultColor || sr.AnnotationEditor._defaultLineColor],
                                     [nr.AnnotationEditorParamsType.INK_OPACITY, Math.round(100 * (this.opacity ?? zr._defaultOpacity))]
                                 ];
                             }
                             rebuild() {
-                                this.parent && (super.rebuild(), this.div !== null && (this.canvas || (tn(this, on, rn).call(this), tn(this, mn, _n).call(this)), this.isAttachedToDOM || (this.parent.add(this), tn(this, Sn, Cn).call(this)), tn(this, lr, ur).call(this)));
+                                this.parent && (super.rebuild(), this.div !== null && (this.canvas || (tn(this, on, rn).call(this), tn(this, mn, _n).call(this)), this.isAttachedToDOM || (this.parent.add(this), tn(this, yn, Cn).call(this)), tn(this, lr, ur).call(this)));
                             }
                             remove() {
                                 this.canvas !== null && (this.isEmpty() || this.commit(), this.canvas.width = this.canvas.height = 0, this.canvas.remove(), this.canvas = null, St(this, Rt).disconnect(), sn(this, Rt, null), super.remove());
                             }
                             setParent(In) {
                                 !this.parent && In ? this._uiManager.removeShouldRescale(this) : this.parent && In === null && this._uiManager.addShouldRescale(this), super.setParent(In);
                             }
@@ -47991,46 +47991,46 @@
                                 this.width && (In = this.x, Qn = this.y), super.render(), sr.AnnotationEditor._l10nPromise.get("editor_ink2_aria_label").then((Nn) => {
                                     var Kn;
                                     return (Kn = this.div) == null ? void 0 : Kn.setAttribute("aria-label", Nn);
                                 });
                                 const [or, Xn, Vn, hr] = tn(this, Ft, zt).call(this);
                                 if (this.setAt(or, Xn, 0, 0), this.setDims(Vn, hr), tn(this, on, rn).call(this), this.width) {
                                     const [Nn, Kn] = this.parentDimensions;
-                                    this.setAspectRatio(this.width * Nn, this.height * Kn), this.setAt(In * Nn, Qn * Kn, this.width * Nn, this.height * Kn), sn(this, Ct, !0), tn(this, Sn, Cn).call(this), this.setDims(this.width * Nn, this.height * Kn), tn(this, Dt, Bt).call(this), this.div.classList.add("disabled");
+                                    this.setAspectRatio(this.width * Nn, this.height * Kn), this.setAt(In * Nn, Qn * Kn, this.width * Nn, this.height * Kn), sn(this, Ct, !0), tn(this, yn, Cn).call(this), this.setDims(this.width * Nn, this.height * Kn), tn(this, Dt, Bt).call(this), this.div.classList.add("disabled");
                                 } else
                                     this.div.classList.add("editing"), this.enableEditMode();
                                 return tn(this, mn, _n).call(this), this.div;
                             }
                             setDimensions(In, Qn) {
                                 const or = Math.round(In),
                                     Xn = Math.round(Qn);
                                 if (St(this, Mt) === or && St(this, Lt) === Xn)
                                     return;
                                 sn(this, Mt, or), sn(this, Lt, Xn), this.canvas.style.visibility = "hidden";
                                 const [Vn, hr] = this.parentDimensions;
-                                this.width = In / Vn, this.height = Qn / hr, this.fixAndSetPosition(), St(this, wt) && tn(this, kn, Pn).call(this, In, Qn), tn(this, Sn, Cn).call(this), tn(this, Dt, Bt).call(this), this.canvas.style.visibility = "visible", this.fixDims();
+                                this.width = In / Vn, this.height = Qn / hr, this.fixAndSetPosition(), St(this, wt) && tn(this, kn, Pn).call(this, In, Qn), tn(this, yn, Cn).call(this), tn(this, Dt, Bt).call(this), this.canvas.style.visibility = "visible", this.fixDims();
                             }
                             static deserialize(In, Qn, or) {
                                 var Xn, Vn, hr;
-                                if (In instanceof Fn.InkAnnotationElement)
+                                if (In instanceof Dn.InkAnnotationElement)
                                     return null;
                                 const Nn = super.deserialize(In, Qn, or);
                                 Nn.thickness = In.thickness, Nn.color = nr.Util.makeHexColor(...In.color), Nn.opacity = In.opacity;
                                 const [Kn, Jn] = Nn.pageDimensions, gr = Nn.width * Kn, rr = Nn.height * Jn, nn = Nn.parentScale, qt = In.thickness / 2;
                                 sn(Nn, wt, !0), sn(Nn, Mt, Math.round(gr)), sn(Nn, Lt, Math.round(rr));
                                 const {
                                     paths: dn,
-                                    rect: gn,
-                                    rotation: vn
+                                    rect: vn,
+                                    rotation: bn
                                 } = In;
                                 for (let {
                                         bezier: Ln
                                     }
                                     of dn) {
-                                    Ln = tn(Xn = zr, bn, xn).call(Xn, Ln, gn, vn);
+                                    Ln = tn(Xn = zr, gn, xn).call(Xn, Ln, vn, bn);
                                     const Hn = [];
                                     Nn.paths.push(Hn);
                                     let Bn = nn * (Ln[0] - qt),
                                         qn = nn * (Ln[1] - qt);
                                     for (let er = 2, ar = Ln.length; er < ar; er += 6) {
                                         const dr = nn * (Ln[er] - qt),
                                             mr = nn * (Ln[er + 1] - qt),
@@ -48041,15 +48041,15 @@
                                         Hn.push([
                                             [Bn, qn],
                                             [dr, mr],
                                             [pr, br],
                                             [_r, yr]
                                         ]), Bn = _r, qn = yr;
                                     }
-                                    const ir = tn(this, Rn, yn).call(this, Hn);
+                                    const ir = tn(this, Rn, Fn).call(this, Hn);
                                     Nn.bezierPath2D.push(ir);
                                 }
                                 const $n = tn(Vn = Nn, Un, Gn).call(Vn);
                                 return sn(Nn, gt, Math.max(sr.AnnotationEditor.MIN_SIZE, $n[2] - $n[0])), sn(Nn, mt, Math.max(sr.AnnotationEditor.MIN_SIZE, $n[3] - $n[1])), tn(hr = Nn, kn, Pn).call(hr, gr, rr), Nn;
                             }
                             serialize() {
                                 if (this.isEmpty())
@@ -48132,17 +48132,17 @@
                                 ctx: Tn,
                                 color: In,
                                 opacity: Qn,
                                 thickness: or,
                                 parentScale: Xn,
                                 scaleFactor: Vn
                             } = this;
-                            Tn.lineWidth = or * Xn / Vn, Tn.lineCap = "round", Tn.lineJoin = "round", Tn.miterLimit = 10, Tn.strokeStyle = `${In}${(0, En.opacityToHex)(Qn)}`;
+                            Tn.lineWidth = or * Xn / Vn, Tn.lineCap = "round", Tn.lineJoin = "round", Tn.miterLimit = 10, Tn.strokeStyle = `${In}${(0, Sn.opacityToHex)(Qn)}`;
                         }, Gt = /* @__PURE__ */ new WeakSet(), cn = function(Tn, In) {
-                            this.canvas.addEventListener("contextmenu", wn.noContextMenu), this.canvas.addEventListener("pointerleave", St(this, _t)), this.canvas.addEventListener("pointermove", St(this, bt)), this.canvas.addEventListener("pointerup", St(this, yt)), this.canvas.removeEventListener("pointerdown", St(this, Et)), this.isEditing = !0, St(this, Ct) || (sn(this, Ct, !0), tn(this, Sn, Cn).call(this), this.thickness || (this.thickness = Dn._defaultThickness), this.color || (this.color = Dn._defaultColor || sr.AnnotationEditor._defaultLineColor), this.opacity ?? (this.opacity = Dn._defaultOpacity)), this.currentPath.push([Tn, In]), sn(this, $t, !1), tn(this, jt, Vt).call(this), sn(this, Pt, () => {
+                            this.canvas.addEventListener("contextmenu", wn.noContextMenu), this.canvas.addEventListener("pointerleave", St(this, _t)), this.canvas.addEventListener("pointermove", St(this, bt)), this.canvas.addEventListener("pointerup", St(this, yt)), this.canvas.removeEventListener("pointerdown", St(this, Et)), this.isEditing = !0, St(this, Ct) || (sn(this, Ct, !0), tn(this, yn, Cn).call(this), this.thickness || (this.thickness = jn._defaultThickness), this.color || (this.color = jn._defaultColor || sr.AnnotationEditor._defaultLineColor), this.opacity ?? (this.opacity = jn._defaultOpacity)), this.currentPath.push([Tn, In]), sn(this, $t, !1), tn(this, jt, Vt).call(this), sn(this, Pt, () => {
                                 tn(this, pn, hn).call(this), St(this, Pt) && window.requestAnimationFrame(St(this, Pt));
                             }), window.requestAnimationFrame(St(this, Pt));
                         }, en = /* @__PURE__ */ new WeakSet(), Kt = function(Tn, In) {
                             const [Qn, or] = this.currentPath.at(-1);
                             if (this.currentPath.length > 1 && Tn === Qn && In === or)
                                 return;
                             const Xn = this.currentPath;
@@ -48209,18 +48209,18 @@
                             if (Tn.length <= 2)
                                 return [
                                     [Tn[0], Tn[0], Tn.at(-1), Tn.at(-1)]
                                 ];
                             const In = [];
                             let Qn, [or, Xn] = Tn[0];
                             for (Qn = 1; Qn < Tn.length - 2; Qn++) {
-                                const [rr, nn] = Tn[Qn], [qt, dn] = Tn[Qn + 1], gn = (rr + qt) / 2, vn = (nn + dn) / 2, $n = [or + 2 * (rr - or) / 3, Xn + 2 * (nn - Xn) / 3], Ln = [gn + 2 * (rr - gn) / 3, vn + 2 * (nn - vn) / 3];
+                                const [rr, nn] = Tn[Qn], [qt, dn] = Tn[Qn + 1], vn = (rr + qt) / 2, bn = (nn + dn) / 2, $n = [or + 2 * (rr - or) / 3, Xn + 2 * (nn - Xn) / 3], Ln = [vn + 2 * (rr - vn) / 3, bn + 2 * (nn - bn) / 3];
                                 In.push([
-                                    [or, Xn], $n, Ln, [gn, vn]
-                                ]), [or, Xn] = [gn, vn];
+                                    [or, Xn], $n, Ln, [vn, bn]
+                                ]), [or, Xn] = [vn, bn];
                             }
                             const [Vn, hr] = Tn[Qn], [Nn, Kn] = Tn[Qn + 1], Jn = [or + 2 * (Vn - or) / 3, Xn + 2 * (hr - Xn) / 3], gr = [Nn + 2 * (Vn - Nn) / 3, Kn + 2 * (hr - Kn) / 3];
                             return In.push([
                                 [or, Xn], Jn, gr, [Nn, Kn]
                             ]), In;
                         }, Dt = /* @__PURE__ */ new WeakSet(), Bt = function() {
                             if (this.isEmpty()) {
@@ -48245,35 +48245,35 @@
                                 return (In = this.canvas) == null ? void 0 : In.setAttribute("aria-label", Tn);
                             }), this.div.append(this.canvas), this.ctx = this.canvas.getContext("2d");
                         }, mn = /* @__PURE__ */ new WeakSet(), _n = function() {
                             sn(this, Rt, new ResizeObserver((Tn) => {
                                 const In = Tn[0].contentRect;
                                 In.width && In.height && this.setDimensions(In.width, In.height);
                             })), St(this, Rt).observe(this.div);
-                        }, Sn = /* @__PURE__ */ new WeakSet(), Cn = function() {
+                        }, yn = /* @__PURE__ */ new WeakSet(), Cn = function() {
                             if (!St(this, Ct))
                                 return;
                             const [Tn, In] = this.parentDimensions;
                             this.canvas.width = Math.ceil(this.width * Tn), this.canvas.height = Math.ceil(this.height * In), tn(this, Mn, Wn).call(this);
                         }, kn = /* @__PURE__ */ new WeakSet(), Pn = function(Tn, In) {
                             const Qn = tn(this, Zn, Yn).call(this),
                                 or = (Tn - Qn) / St(this, gt),
                                 Xn = (In - Qn) / St(this, mt);
                             this.scaleFactor = Math.min(or, Xn);
                         }, Mn = /* @__PURE__ */ new WeakSet(), Wn = function() {
                             const Tn = tn(this, Zn, Yn).call(this) / 2;
                             this.ctx.setTransform(this.scaleFactor, 0, 0, this.scaleFactor, this.translationX * this.scaleFactor + Tn, this.translationY * this.scaleFactor + Tn);
-                        }, Rn = /* @__PURE__ */ new WeakSet(), yn = function(Tn) {
+                        }, Rn = /* @__PURE__ */ new WeakSet(), Fn = function(Tn) {
                             const In = new Path2D();
                             for (let Qn = 0, or = Tn.length; Qn < or; Qn++) {
                                 const [Xn, Vn, hr, Nn] = Tn[Qn];
                                 Qn === 0 && In.moveTo(...Xn), In.bezierCurveTo(Vn[0], Vn[1], hr[0], hr[1], Nn[0], Nn[1]);
                             }
                             return In;
-                        }, jn = /* @__PURE__ */ new WeakSet(), An = function(Tn, In, Qn) {
+                        }, En = /* @__PURE__ */ new WeakSet(), An = function(Tn, In, Qn) {
                             const [or, Xn, Vn, hr] = In;
                             switch (Qn) {
                                 case 0:
                                     for (let Nn = 0, Kn = Tn.length; Nn < Kn; Nn += 2)
                                         Tn[Nn] += or, Tn[Nn + 1] = hr - Tn[Nn + 1];
                                     break;
                                 case 90:
@@ -48292,15 +48292,15 @@
                                         Tn[Nn] = Vn - Tn[Nn + 1], Tn[Nn + 1] = hr - Jn;
                                     }
                                     break;
                                 default:
                                     throw new Error("Invalid rotation");
                             }
                             return Tn;
-                        }, bn = /* @__PURE__ */ new WeakSet(), xn = function(Tn, In, Qn) {
+                        }, gn = /* @__PURE__ */ new WeakSet(), xn = function(Tn, In, Qn) {
                             const [or, Xn, Vn, hr] = In;
                             switch (Qn) {
                                 case 0:
                                     for (let Nn = 0, Kn = Tn.length; Nn < Kn; Nn += 2)
                                         Tn[Nn] -= or, Tn[Nn + 1] = hr - Tn[Nn + 1];
                                     break;
                                 case 90:
@@ -48329,20 +48329,20 @@
                                 Nn = this.thickness / 2,
                                 Kn = Tn * In + Nn,
                                 Jn = Tn * Qn + Nn;
                             for (const gr of this.paths) {
                                 const rr = [],
                                     nn = [];
                                 for (let qt = 0, dn = gr.length; qt < dn; qt++) {
-                                    const [gn, vn, $n, Ln] = gr[qt], Hn = Tn * gn[0] + Kn, Bn = Tn * gn[1] + Jn, qn = Tn * vn[0] + Kn, ir = Tn * vn[1] + Jn, er = Tn * $n[0] + Kn, ar = Tn * $n[1] + Jn, dr = Tn * Ln[0] + Kn, mr = Tn * Ln[1] + Jn;
+                                    const [vn, bn, $n, Ln] = gr[qt], Hn = Tn * vn[0] + Kn, Bn = Tn * vn[1] + Jn, qn = Tn * bn[0] + Kn, ir = Tn * bn[1] + Jn, er = Tn * $n[0] + Kn, ar = Tn * $n[1] + Jn, dr = Tn * Ln[0] + Kn, mr = Tn * Ln[1] + Jn;
                                     qt === 0 && (rr.push(Hn, Bn), nn.push(Hn, Bn)), rr.push(qn, ir, er, ar, dr, mr), nn.push(qn, ir), qt === dn - 1 && nn.push(dr, mr);
                                 }
                                 hr.push({
-                                    bezier: tn(Xn = Dn, jn, An).call(Xn, rr, or, this.rotation),
-                                    points: tn(Vn = Dn, jn, An).call(Vn, nn, or, this.rotation)
+                                    bezier: tn(Xn = jn, En, An).call(Xn, rr, or, this.rotation),
+                                    points: tn(Vn = jn, En, An).call(Vn, nn, or, this.rotation)
                                 });
                             }
                             return hr;
                         }, Un = /* @__PURE__ */ new WeakSet(), Gn = function() {
                             let Tn = 1 / 0,
                                 In = -1 / 0,
                                 Qn = 1 / 0,
@@ -48367,19 +48367,19 @@
                             sn(this, gt, Math.max(sr.AnnotationEditor.MIN_SIZE, In[2] - In[0])), sn(this, mt, Math.max(sr.AnnotationEditor.MIN_SIZE, In[3] - In[1]));
                             const or = Math.ceil(Qn + St(this, gt) * this.scaleFactor),
                                 Xn = Math.ceil(Qn + St(this, mt) * this.scaleFactor),
                                 [Vn, hr] = this.parentDimensions;
                             this.width = or / Vn, this.height = Xn / hr, this.setAspectRatio(or, Xn);
                             const Nn = this.translationX,
                                 Kn = this.translationY;
-                            this.translationX = -In[0], this.translationY = -In[1], tn(this, Sn, Cn).call(this), tn(this, Dt, Bt).call(this), sn(this, Mt, or), sn(this, Lt, Xn), this.setDims(or, Xn);
+                            this.translationX = -In[0], this.translationY = -In[1], tn(this, yn, Cn).call(this), tn(this, Dt, Bt).call(this), sn(this, Mt, or), sn(this, Lt, Xn), this.setDims(or, Xn);
                             const Jn = Tn ? Qn / this.scaleFactor / 2 : 0;
                             this.translate(Nn - this.translationX - Jn, Kn - this.translationY - Jn);
-                        }, Ut(Dn, Rn), Ut(Dn, jn), Ut(Dn, bn), tr(Dn, "_defaultColor", null), tr(Dn, "_defaultOpacity", 1), tr(Dn, "_defaultThickness", 1), tr(Dn, "_type", "ink");
-                        let cr = Dn;
+                        }, Ut(jn, Rn), Ut(jn, En), Ut(jn, gn), tr(jn, "_defaultColor", null), tr(jn, "_defaultOpacity", 1), tr(jn, "_defaultThickness", 1), tr(jn, "_type", "ink");
+                        let cr = jn;
                         it.InkEditor = cr;
                     },
                     /* 34 */
                     /***/
                     (_e, it, ft) => {
                         var mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt, Pt, kt, At, Tt, Ot, It, Nt, Ft, zt, jt, Vt, Gt, cn, en, Kt;
                         Object.defineProperty(it, "__esModule", {
@@ -56848,32 +56848,32 @@
     } = globals,
     {
         getContext
     } = window.__gradio__svelte__internal;
 
 function get_each_context(_e, it, ft) {
     const mt = _e.slice();
-    return mt[53] = it[ft], mt;
+    return mt[54] = it[ft], mt;
 }
 
 function create_if_block_5(_e) {
     let it, ft;
     const mt = [{
             autoscroll: (
                 /*gradio*/
-                _e[3].autoscroll
+                _e[2].autoscroll
             )
         }, {
             i18n: (
                 /*gradio*/
-                _e[3].i18n
+                _e[2].i18n
             )
         },
         /*loading_status*/
-        _e[18]
+        _e[17]
     ];
     let gt = {};
     for (let bt = 0; bt < mt.length; bt += 1)
         gt = assign(gt, mt[bt]);
     return it = new Static({
         props: gt
     }), {
@@ -56881,33 +56881,33 @@
             create_component(it.$$.fragment);
         },
         m(bt, _t) {
             mount_component(it, bt, _t), ft = !0;
         },
         p(bt, _t) {
             const yt = _t[0] & /*gradio, loading_status*/
-                262152 ? get_spread_update(mt, [
+                131076 ? get_spread_update(mt, [
                     _t[0] & /*gradio*/
-                    8 && {
+                    4 && {
                         autoscroll: (
                             /*gradio*/
-                            bt[3].autoscroll
+                            bt[2].autoscroll
                         )
                     },
                     _t[0] & /*gradio*/
-                    8 && {
+                    4 && {
                         i18n: (
                             /*gradio*/
-                            bt[3].i18n
+                            bt[2].i18n
                         )
                     },
                     _t[0] & /*loading_status*/
-                    262144 && get_spread_object(
+                    131072 && get_spread_object(
                         /*loading_status*/
-                        bt[18]
+                        bt[17]
                     )
                 ]) : {};
             it.$set(yt);
         },
         i(bt) {
             ft || (transition_in(it.$$.fragment, bt), ft = !0);
         },
@@ -56922,19 +56922,19 @@
 
 function create_if_block_4(_e) {
     let it, ft;
     return it = new BlockTitle({
         props: {
             show_label: (
                 /*show_label*/
-                _e[11]
+                _e[10]
             ),
             info: (
                 /*info*/
-                _e[5]
+                _e[4]
             ),
             $$slots: {
                 default: [create_default_slot_1]
             },
             $$scope: {
                 ctx: _e
             }
@@ -56945,20 +56945,20 @@
         },
         m(mt, gt) {
             mount_component(it, mt, gt), ft = !0;
         },
         p(mt, gt) {
             const bt = {};
             gt[0] & /*show_label*/
-                2048 && (bt.show_label = /*show_label*/
-                    mt[11]), gt[0] & /*info*/
-                32 && (bt.info = /*info*/
-                    mt[5]), gt[0] & /*label*/
-                16 | gt[1] & /*$$scope*/
-                33554432 && (bt.$$scope = {
+                1024 && (bt.show_label = /*show_label*/
+                    mt[10]), gt[0] & /*info*/
+                16 && (bt.info = /*info*/
+                    mt[4]), gt[0] & /*label*/
+                8 | gt[1] & /*$$scope*/
+                67108864 && (bt.$$scope = {
                     dirty: gt,
                     ctx: mt
                 }), it.$set(bt);
         },
         i(mt) {
             ft || (transition_in(it.$$.fragment, mt), ft = !0);
         },
@@ -56973,87 +56973,87 @@
 
 function create_default_slot_1(_e) {
     let it;
     return {
         c() {
             it = text(
                 /*label*/
-                _e[4]
+                _e[3]
             );
         },
         m(ft, mt) {
             insert(ft, it, mt);
         },
         p(ft, mt) {
             mt[0] & /*label*/
-                16 && set_data(
+                8 && set_data(
                     it,
                     /*label*/
-                    ft[4]
+                    ft[3]
                 );
         },
         d(ft) {
             ft && detach(it);
         }
     };
 }
 
 function create_if_block_3(_e) {
     let it, ft, mt, gt;
     const bt = [
         /*_webcam_props*/
-        _e[27], {
+        _e[26], {
             i18n: (
                 /*gradio*/
-                _e[3].i18n
+                _e[2].i18n
             )
         }, {
             disabled: ! /*interactive*/
-                _e[23]
+                _e[22]
         }
     ];
     let _t = {};
     for (let yt = 0; yt < bt.length; yt += 1)
         _t = assign(_t, bt[yt]);
     return ft = new Webcam_1({
         props: _t
     }), ft.$on(
         "error",
         /*error_handler_1*/
-        _e[46]
+        _e[47]
     ), ft.$on(
         "change",
         /*change_handler_3*/
-        _e[47]
+        _e[48]
     ), {
         c() {
             it = element("span"), create_component(ft.$$.fragment), mt = space(), attr(it, "class", "tool-button svelte-9felha");
         },
         m(yt, Et) {
             insert(yt, it, Et), mount_component(ft, it, null), append(it, mt), gt = !0;
         },
         p(yt, Et) {
             const xt = Et[0] & /*_webcam_props, gradio, interactive*/
-                142606344 ? get_spread_update(bt, [
+                71303172 ? get_spread_update(bt, [
                     Et[0] & /*_webcam_props*/
-                    134217728 && get_spread_object(
+                    67108864 && get_spread_object(
                         /*_webcam_props*/
-                        yt[27]
+                        yt[26]
                     ),
                     Et[0] & /*gradio*/
-                    8 && {
+                    4 && {
                         i18n: (
                             /*gradio*/
-                            yt[3].i18n
+                            yt[2].i18n
                         )
                     },
                     Et[0] & /*interactive*/
-                    8388608 && {
+                    4194304 && {
                         disabled: ! /*interactive*/
-                            yt[23]
+                            yt[22]
                     }
                 ]) : {};
             ft.$set(xt);
         },
         i(yt) {
             gt || (transition_in(ft.$$.fragment, yt), gt = !0);
         },
@@ -57068,41 +57068,41 @@
 
 function create_if_block_2(_e) {
     let it, ft, mt, gt;
     return ft = new AudioRecorder({
         props: {
             i18n: (
                 /*gradio*/
-                _e[3].i18n
+                _e[2].i18n
             ),
             disabled: ! /*interactive*/
-                _e[23]
+                _e[22]
         }
     }), ft.$on(
         "error",
         /*error_handler*/
-        _e[44]
+        _e[45]
     ), ft.$on(
         "change",
         /*change_handler_2*/
-        _e[45]
+        _e[46]
     ), {
         c() {
             it = element("span"), create_component(ft.$$.fragment), mt = space(), attr(it, "class", "tool-button svelte-9felha");
         },
         m(bt, _t) {
             insert(bt, it, _t), mount_component(ft, it, null), append(it, mt), gt = !0;
         },
         p(bt, _t) {
             const yt = {};
             _t[0] & /*gradio*/
-                8 && (yt.i18n = /*gradio*/
-                    bt[3].i18n), _t[0] & /*interactive*/
-                8388608 && (yt.disabled = ! /*interactive*/
-                    bt[23]), ft.$set(yt);
+                4 && (yt.i18n = /*gradio*/
+                    bt[2].i18n), _t[0] & /*interactive*/
+                4194304 && (yt.disabled = ! /*interactive*/
+                    bt[22]), ft.$set(yt);
         },
         i(bt) {
             gt || (transition_in(ft.$$.fragment, bt), gt = !0);
         },
         o(bt) {
             transition_out(ft.$$.fragment, bt), gt = !1;
         },
@@ -57114,47 +57114,47 @@
 
 function create_if_block_1(_e) {
     let it, ft, mt, gt;
     return ft = new UploadButton({
         props: {
             props: (
                 /*_upload_button_props*/
-                _e[26]
+                _e[25]
             ),
             disabled: ! /*interactive*/
-                _e[23],
+                _e[22],
             i18n: (
                 /*gradio*/
-                _e[3].i18n
+                _e[2].i18n
             )
         }
     }), ft.$on(
         "change",
         /*change_handler_1*/
-        _e[42]
+        _e[43]
     ), ft.$on(
         "click",
         /*click_handler*/
-        _e[43]
+        _e[44]
     ), {
         c() {
             it = element("span"), create_component(ft.$$.fragment), mt = space(), attr(it, "class", "tool-button upload-button svelte-9felha");
         },
         m(bt, _t) {
             insert(bt, it, _t), mount_component(ft, it, null), append(it, mt), gt = !0;
         },
         p(bt, _t) {
             const yt = {};
             _t[0] & /*_upload_button_props*/
-                67108864 && (yt.props = /*_upload_button_props*/
-                    bt[26]), _t[0] & /*interactive*/
-                8388608 && (yt.disabled = ! /*interactive*/
-                    bt[23]), _t[0] & /*gradio*/
-                8 && (yt.i18n = /*gradio*/
-                    bt[3].i18n), ft.$set(yt);
+                33554432 && (yt.props = /*_upload_button_props*/
+                    bt[25]), _t[0] & /*interactive*/
+                4194304 && (yt.disabled = ! /*interactive*/
+                    bt[22]), _t[0] & /*gradio*/
+                4 && (yt.i18n = /*gradio*/
+                    bt[2].i18n), ft.$set(yt);
         },
         i(bt) {
             gt || (transition_in(ft.$$.fragment, bt), gt = !0);
         },
         o(bt) {
             transition_out(ft.$$.fragment, bt), gt = !1;
         },
@@ -57168,19 +57168,19 @@
     let it, ft, mt, gt;
     const bt = [create_if_block_1, create_if_block_2, create_if_block_3],
         _t = [];
 
     function yt(Et, xt) {
         return (
             /*source*/
-            Et[53] === "upload" ? 0 : (
+            Et[54] === "upload" ? 0 : (
                 /*source*/
-                Et[53] === "microphone" ? 1 : (
+                Et[54] === "microphone" ? 1 : (
                     /*source*/
-                    Et[53] === "webcam" ? 2 : -1
+                    Et[54] === "webcam" ? 2 : -1
                 )
             )
         );
     }
     return ~(it = yt(_e)) && (ft = _t[it] = bt[it](_e)), {
         c() {
             ft && ft.c(), mt = empty();
@@ -57208,77 +57208,77 @@
 
 function create_if_block(_e) {
     let it, ft;
     return it = new FilePreview({
         props: {
             loading: (
                 /*uploading*/
-                _e[30]
+                _e[29]
             ),
             proxy_url: (
                 /*proxy_url*/
-                _e[25]
+                _e[24]
             ),
             root: (
                 /*root*/
-                _e[24]
+                _e[23]
             ),
             theme: (
                 /*gradio*/
-                _e[3].theme
+                _e[2].theme
             ),
             i18n: (
                 /*gradio*/
-                _e[3].i18n
+                _e[2].i18n
             ),
             value: (
                 /*value*/
-                _e[1].files
+                _e[0].files
             ),
             props: (
                 /*_file_preview_props*/
-                _e[29]
+                _e[28]
             ),
             disabled: ! /*interactive*/
-                _e[23]
+                _e[22]
         }
     }), it.$on(
         "select",
         /*select_handler*/
-        _e[49]
+        _e[50]
     ), it.$on(
         "delete",
         /*delete_handler*/
-        _e[50]
+        _e[51]
     ), {
         c() {
             create_component(it.$$.fragment);
         },
         m(mt, gt) {
             mount_component(it, mt, gt), ft = !0;
         },
         p(mt, gt) {
             const bt = {};
             gt[0] & /*uploading*/
-                1073741824 && (bt.loading = /*uploading*/
-                    mt[30]), gt[0] & /*proxy_url*/
-                33554432 && (bt.proxy_url = /*proxy_url*/
-                    mt[25]), gt[0] & /*root*/
-                16777216 && (bt.root = /*root*/
-                    mt[24]), gt[0] & /*gradio*/
-                8 && (bt.theme = /*gradio*/
-                    mt[3].theme), gt[0] & /*gradio*/
-                8 && (bt.i18n = /*gradio*/
-                    mt[3].i18n), gt[0] & /*value*/
-                2 && (bt.value = /*value*/
-                    mt[1].files), gt[0] & /*_file_preview_props*/
-                536870912 && (bt.props = /*_file_preview_props*/
-                    mt[29]), gt[0] & /*interactive*/
-                8388608 && (bt.disabled = ! /*interactive*/
-                    mt[23]), it.$set(bt);
+                536870912 && (bt.loading = /*uploading*/
+                    mt[29]), gt[0] & /*proxy_url*/
+                16777216 && (bt.proxy_url = /*proxy_url*/
+                    mt[24]), gt[0] & /*root*/
+                8388608 && (bt.root = /*root*/
+                    mt[23]), gt[0] & /*gradio*/
+                4 && (bt.theme = /*gradio*/
+                    mt[2].theme), gt[0] & /*gradio*/
+                4 && (bt.i18n = /*gradio*/
+                    mt[2].i18n), gt[0] & /*value*/
+                1 && (bt.value = /*value*/
+                    mt[0].files), gt[0] & /*_file_preview_props*/
+                268435456 && (bt.props = /*_file_preview_props*/
+                    mt[28]), gt[0] & /*interactive*/
+                4194304 && (bt.disabled = ! /*interactive*/
+                    mt[22]), it.$set(bt);
         },
         i(mt) {
             ft || (transition_in(it.$$.fragment, mt), ft = !0);
         },
         o(mt) {
             transition_out(it.$$.fragment, mt), ft = !1;
         },
@@ -57288,141 +57288,141 @@
     };
 }
 
 function create_default_slot(_e) {
     var Ft;
     let it, ft, mt, gt, bt, _t, yt, Et, xt, wt, $t, Ct, Rt, Mt, Lt = (
             /*loading_status*/
-            _e[18] && create_if_block_5(_e)
+            _e[17] && create_if_block_5(_e)
         ),
         Pt = (
             /*show_label*/
-            _e[11] && /*label*/
-            _e[4] && create_if_block_4(_e)
+            _e[10] && /*label*/
+            _e[3] && create_if_block_4(_e)
         );
 
     function kt(zt) {
-        _e[35](zt);
+        _e[36](zt);
     }
     let At = {
         value: (
             /*value*/
-            _e[1].text
+            _e[0].text
         ),
         show_label: (
             /*show_label*/
-            _e[11]
+            _e[10]
         ),
         lines: (
             /*lines*/
-            _e[9]
+            _e[8]
         ),
         type: (
             /*type*/
-            _e[13]
+            _e[12]
         ),
         rtl: (
             /*rtl*/
-            _e[19]
+            _e[18]
         ),
         text_align: (
             /*text_align*/
-            _e[20]
+            _e[19]
         ),
-        max_lines: /*max_lines*/ _e[12] ? (
+        max_lines: /*max_lines*/ _e[11] ? (
             /*max_lines*/
-            _e[12]
+            _e[11]
         ) : (
             /*lines*/
-            _e[9] + 1
+            _e[8] + 1
         ),
         placeholder: (
             /*placeholder*/
-            _e[10]
+            _e[9]
         ),
         show_copy_button: (
             /*show_copy_button*/
-            _e[17]
+            _e[16]
         ),
         autofocus: (
             /*autofocus*/
-            _e[21]
+            _e[20]
         ),
         container: (
             /*container*/
-            _e[14]
+            _e[13]
         ),
         autoscroll: (
             /*autoscroll*/
-            _e[22]
+            _e[21]
         ),
         disabled: ! /*interactive*/
-            _e[23]
+            _e[22]
     };
     /*value_is_output*/
-    _e[2] !== void 0 && (At.value_is_output = /*value_is_output*/
-        _e[2]), gt = new Input({
+    _e[1] !== void 0 && (At.value_is_output = /*value_is_output*/
+        _e[1]), gt = new Input({
         props: At
     }), binding_callbacks.push(() => bind(gt, "value_is_output", kt)), gt.$on(
         "change",
         /*change_handler*/
-        _e[36]
+        _e[37]
     ), gt.$on(
         "input",
         /*input_handler*/
-        _e[37]
+        _e[38]
     ), gt.$on(
         "submit",
         /*submit_handler*/
-        _e[38]
+        _e[39]
     ), gt.$on(
         "blur",
         /*blur_handler*/
-        _e[39]
+        _e[40]
     ), gt.$on(
         "select",
         /*select_handler_1*/
-        _e[40]
+        _e[41]
     ), gt.$on(
         "focus",
         /*focus_handler*/
-        _e[41]
+        _e[42]
     );
     let Tt = ensure_array_like(
-            /*sources*/
-            _e[0]
+            /*_sources*/
+            _e[30]
         ),
         Ot = [];
     for (let zt = 0; zt < Tt.length; zt += 1)
         Ot[zt] = create_each_block(get_each_context(_e, Tt, zt));
     const It = (zt) => transition_out(Ot[zt], 1, 1, () => {
         Ot[zt] = null;
     });
     $t = new SubmitButton({
         props: {
             props: (
                 /*_submit_button_props*/
-                _e[28]
+                _e[27]
             ),
             i18n: (
                 /*gradio*/
-                _e[3].i18n
+                _e[2].i18n
             ),
             disabled: ! /*interactive*/
-                _e[23] || /*uploading*/
-                _e[30]
+                _e[22] || /*uploading*/
+                _e[29]
         }
     }), $t.$on(
         "click",
         /*click_handler_1*/
-        _e[48]
+        _e[49]
     );
     let Nt = (
         /*value*/
-        ((Ft = _e[1].files) == null ? void 0 : Ft.length) && create_if_block(_e)
+        ((Ft = _e[0].files) == null ? void 0 : Ft.length) && create_if_block(_e)
     );
     return {
         c() {
             Lt && Lt.c(), it = space(), Pt && Pt.c(), ft = space(), mt = element("div"), create_component(gt.$$.fragment), _t = space(), yt = element("div"), Et = element("span");
             for (let zt = 0; zt < Ot.length; zt += 1)
                 Ot[zt].c();
             xt = space(), wt = element("span"), create_component($t.$$.fragment), Ct = space(), Nt && Nt.c(), Rt = empty(), attr(mt, "class", "input-content svelte-9felha"), attr(Et, "class", "input-tools svelte-9felha"), attr(wt, "class", "submit-button svelte-9felha"), attr(yt, "class", "controls svelte-9felha");
@@ -57432,84 +57432,84 @@
             for (let Vt = 0; Vt < Ot.length; Vt += 1)
                 Ot[Vt] && Ot[Vt].m(Et, null);
             append(yt, xt), append(yt, wt), mount_component($t, wt, null), insert(zt, Ct, jt), Nt && Nt.m(zt, jt), insert(zt, Rt, jt), Mt = !0;
         },
         p(zt, jt) {
             var cn;
             /*loading_status*/
-            zt[18] ? Lt ? (Lt.p(zt, jt), jt[0] & /*loading_status*/
-                    262144 && transition_in(Lt, 1)) : (Lt = create_if_block_5(zt), Lt.c(), transition_in(Lt, 1), Lt.m(it.parentNode, it)) : Lt && (group_outros(), transition_out(Lt, 1, 1, () => {
+            zt[17] ? Lt ? (Lt.p(zt, jt), jt[0] & /*loading_status*/
+                    131072 && transition_in(Lt, 1)) : (Lt = create_if_block_5(zt), Lt.c(), transition_in(Lt, 1), Lt.m(it.parentNode, it)) : Lt && (group_outros(), transition_out(Lt, 1, 1, () => {
                     Lt = null;
                 }), check_outros()), /*show_label*/
-                zt[11] && /*label*/
-                zt[4] ? Pt ? (Pt.p(zt, jt), jt[0] & /*show_label, label*/
-                    2064 && transition_in(Pt, 1)) : (Pt = create_if_block_4(zt), Pt.c(), transition_in(Pt, 1), Pt.m(ft.parentNode, ft)) : Pt && (group_outros(), transition_out(Pt, 1, 1, () => {
+                zt[10] && /*label*/
+                zt[3] ? Pt ? (Pt.p(zt, jt), jt[0] & /*show_label, label*/
+                    1032 && transition_in(Pt, 1)) : (Pt = create_if_block_4(zt), Pt.c(), transition_in(Pt, 1), Pt.m(ft.parentNode, ft)) : Pt && (group_outros(), transition_out(Pt, 1, 1, () => {
                     Pt = null;
                 }), check_outros());
             const Vt = {};
             if (jt[0] & /*value*/
-                2 && (Vt.value = /*value*/
-                    zt[1].text), jt[0] & /*show_label*/
-                2048 && (Vt.show_label = /*show_label*/
-                    zt[11]), jt[0] & /*lines*/
-                512 && (Vt.lines = /*lines*/
-                    zt[9]), jt[0] & /*type*/
-                8192 && (Vt.type = /*type*/
-                    zt[13]), jt[0] & /*rtl*/
-                524288 && (Vt.rtl = /*rtl*/
-                    zt[19]), jt[0] & /*text_align*/
-                1048576 && (Vt.text_align = /*text_align*/
-                    zt[20]), jt[0] & /*max_lines, lines*/
-                4608 && (Vt.max_lines = /*max_lines*/
-                    zt[12] ? (
+                1 && (Vt.value = /*value*/
+                    zt[0].text), jt[0] & /*show_label*/
+                1024 && (Vt.show_label = /*show_label*/
+                    zt[10]), jt[0] & /*lines*/
+                256 && (Vt.lines = /*lines*/
+                    zt[8]), jt[0] & /*type*/
+                4096 && (Vt.type = /*type*/
+                    zt[12]), jt[0] & /*rtl*/
+                262144 && (Vt.rtl = /*rtl*/
+                    zt[18]), jt[0] & /*text_align*/
+                524288 && (Vt.text_align = /*text_align*/
+                    zt[19]), jt[0] & /*max_lines, lines*/
+                2304 && (Vt.max_lines = /*max_lines*/
+                    zt[11] ? (
                         /*max_lines*/
-                        zt[12]
+                        zt[11]
                     ) : (
                         /*lines*/
-                        zt[9] + 1
+                        zt[8] + 1
                     )), jt[0] & /*placeholder*/
-                1024 && (Vt.placeholder = /*placeholder*/
-                    zt[10]), jt[0] & /*show_copy_button*/
-                131072 && (Vt.show_copy_button = /*show_copy_button*/
-                    zt[17]), jt[0] & /*autofocus*/
-                2097152 && (Vt.autofocus = /*autofocus*/
-                    zt[21]), jt[0] & /*container*/
-                16384 && (Vt.container = /*container*/
-                    zt[14]), jt[0] & /*autoscroll*/
-                4194304 && (Vt.autoscroll = /*autoscroll*/
-                    zt[22]), jt[0] & /*interactive*/
-                8388608 && (Vt.disabled = ! /*interactive*/
-                    zt[23]), !bt && jt[0] & /*value_is_output*/
-                4 && (bt = !0, Vt.value_is_output = /*value_is_output*/
-                    zt[2], add_flush_callback(() => bt = !1)), gt.$set(Vt), jt[0] & /*_upload_button_props, interactive, gradio, value, sources, _webcam_props*/
-                209715211) {
+                512 && (Vt.placeholder = /*placeholder*/
+                    zt[9]), jt[0] & /*show_copy_button*/
+                65536 && (Vt.show_copy_button = /*show_copy_button*/
+                    zt[16]), jt[0] & /*autofocus*/
+                1048576 && (Vt.autofocus = /*autofocus*/
+                    zt[20]), jt[0] & /*container*/
+                8192 && (Vt.container = /*container*/
+                    zt[13]), jt[0] & /*autoscroll*/
+                2097152 && (Vt.autoscroll = /*autoscroll*/
+                    zt[21]), jt[0] & /*interactive*/
+                4194304 && (Vt.disabled = ! /*interactive*/
+                    zt[22]), !bt && jt[0] & /*value_is_output*/
+                2 && (bt = !0, Vt.value_is_output = /*value_is_output*/
+                    zt[1], add_flush_callback(() => bt = !1)), gt.$set(Vt), jt[0] & /*_upload_button_props, interactive, gradio, value, _sources, _webcam_props*/
+                1178599429) {
                 Tt = ensure_array_like(
-                    /*sources*/
-                    zt[0]
+                    /*_sources*/
+                    zt[30]
                 );
                 let en;
                 for (en = 0; en < Tt.length; en += 1) {
                     const Kt = get_each_context(zt, Tt, en);
                     Ot[en] ? (Ot[en].p(Kt, jt), transition_in(Ot[en], 1)) : (Ot[en] = create_each_block(Kt), Ot[en].c(), transition_in(Ot[en], 1), Ot[en].m(Et, null));
                 }
                 for (group_outros(), en = Tt.length; en < Ot.length; en += 1)
                     It(en);
                 check_outros();
             }
             const Gt = {};
             jt[0] & /*_submit_button_props*/
-                268435456 && (Gt.props = /*_submit_button_props*/
-                    zt[28]), jt[0] & /*gradio*/
-                8 && (Gt.i18n = /*gradio*/
-                    zt[3].i18n), jt[0] & /*interactive, uploading*/
-                1082130432 && (Gt.disabled = ! /*interactive*/
-                    zt[23] || /*uploading*/
-                    zt[30]), $t.$set(Gt), /*value*/
-                (cn = zt[1].files) != null && cn.length ? Nt ? (Nt.p(zt, jt), jt[0] & /*value*/
-                    2 && transition_in(Nt, 1)) : (Nt = create_if_block(zt), Nt.c(), transition_in(Nt, 1), Nt.m(Rt.parentNode, Rt)) : Nt && (group_outros(), transition_out(Nt, 1, 1, () => {
+                134217728 && (Gt.props = /*_submit_button_props*/
+                    zt[27]), jt[0] & /*gradio*/
+                4 && (Gt.i18n = /*gradio*/
+                    zt[2].i18n), jt[0] & /*interactive, uploading*/
+                541065216 && (Gt.disabled = ! /*interactive*/
+                    zt[22] || /*uploading*/
+                    zt[29]), $t.$set(Gt), /*value*/
+                (cn = zt[0].files) != null && cn.length ? Nt ? (Nt.p(zt, jt), jt[0] & /*value*/
+                    1 && transition_in(Nt, 1)) : (Nt = create_if_block(zt), Nt.c(), transition_in(Nt, 1), Nt.m(Rt.parentNode, Rt)) : Nt && (group_outros(), transition_out(Nt, 1, 1, () => {
                     Nt = null;
                 }), check_outros());
         },
         i(zt) {
             if (!Mt) {
                 transition_in(Lt), transition_in(Pt), transition_in(gt.$$.fragment, zt);
                 for (let jt = 0; jt < Tt.length; jt += 1)
@@ -57531,40 +57531,40 @@
 
 function create_fragment(_e) {
     let it, ft;
     return it = new Block({
         props: {
             visible: (
                 /*visible*/
-                _e[8]
+                _e[7]
             ),
             elem_id: (
                 /*elem_id*/
-                _e[6]
+                _e[5]
             ),
             elem_classes: (
                 /*elem_classes*/
-                _e[7]
+                _e[6]
             ),
             scale: (
                 /*scale*/
-                _e[15]
+                _e[14]
             ),
             min_width: (
                 /*min_width*/
-                _e[16]
+                _e[15]
             ),
             allow_overflow: !1,
             container: (
                 /*container*/
-                _e[14]
+                _e[13]
             ),
             padding: (
                 /*container*/
-                _e[14]
+                _e[13]
             ),
             $$slots: {
                 default: [create_default_slot]
             },
             $$scope: {
                 ctx: _e
             }
@@ -57575,30 +57575,30 @@
         },
         m(mt, gt) {
             mount_component(it, mt, gt), ft = !0;
         },
         p(mt, gt) {
             const bt = {};
             gt[0] & /*visible*/
-                256 && (bt.visible = /*visible*/
-                    mt[8]), gt[0] & /*elem_id*/
-                64 && (bt.elem_id = /*elem_id*/
-                    mt[6]), gt[0] & /*elem_classes*/
-                128 && (bt.elem_classes = /*elem_classes*/
-                    mt[7]), gt[0] & /*scale*/
-                32768 && (bt.scale = /*scale*/
-                    mt[15]), gt[0] & /*min_width*/
-                65536 && (bt.min_width = /*min_width*/
-                    mt[16]), gt[0] & /*container*/
-                16384 && (bt.container = /*container*/
-                    mt[14]), gt[0] & /*container*/
-                16384 && (bt.padding = /*container*/
-                    mt[14]), gt[0] & /*uploading, proxy_url, root, gradio, value, _file_preview_props, interactive, _submit_button_props, sources, _upload_button_props, _webcam_props, show_label, lines, type, rtl, text_align, max_lines, placeholder, show_copy_button, autofocus, container, autoscroll, value_is_output, info, label, loading_status*/
-                2147384895 | gt[1] & /*$$scope*/
-                33554432 && (bt.$$scope = {
+                128 && (bt.visible = /*visible*/
+                    mt[7]), gt[0] & /*elem_id*/
+                32 && (bt.elem_id = /*elem_id*/
+                    mt[5]), gt[0] & /*elem_classes*/
+                64 && (bt.elem_classes = /*elem_classes*/
+                    mt[6]), gt[0] & /*scale*/
+                16384 && (bt.scale = /*scale*/
+                    mt[14]), gt[0] & /*min_width*/
+                32768 && (bt.min_width = /*min_width*/
+                    mt[15]), gt[0] & /*container*/
+                8192 && (bt.container = /*container*/
+                    mt[13]), gt[0] & /*container*/
+                8192 && (bt.padding = /*container*/
+                    mt[13]), gt[0] & /*uploading, proxy_url, root, gradio, value, _file_preview_props, interactive, _submit_button_props, _sources, _upload_button_props, _webcam_props, show_label, lines, type, rtl, text_align, max_lines, placeholder, show_copy_button, autofocus, container, autoscroll, value_is_output, info, label, loading_status*/
+                2147434271 | gt[1] & /*$$scope*/
+                67108864 && (bt.$$scope = {
                     dirty: gt,
                     ctx: mt
                 }), it.$set(bt);
         },
         i(mt) {
             ft || (transition_in(it.$$.fragment, mt), ft = !0);
         },
@@ -57621,489 +57621,524 @@
             return;
         gt === "access" || gt === "optionalAccess" ? (it = ft, ft = bt(ft)) : (gt === "call" || gt === "optionalCall") && (ft = bt((..._t) => ft.call(it, ..._t)), it = void 0);
     }
     return ft;
 }
 
 function instance(_e, it, ft) {
-    let {
-        gradio: mt
-    } = it, {
-        label: gt = ""
-    } = it, {
-        info: bt = void 0
-    } = it, {
-        elem_id: _t = ""
-    } = it, {
-        elem_classes: yt = []
-    } = it, {
-        visible: Et = !0
-    } = it, {
-        value: xt = {
-            text: "",
-            files: []
-        }
-    } = it, {
-        lines: wt
-    } = it, {
-        placeholder: $t = ""
-    } = it, {
-        show_label: Ct
-    } = it, {
-        max_lines: Rt
-    } = it, {
-        type: Mt = "text"
-    } = it, {
-        container: Lt = !0
-    } = it, {
-        scale: Pt = null
-    } = it, {
-        min_width: kt = void 0
-    } = it, {
-        show_copy_button: At = !1
-    } = it, {
-        loading_status: Tt = void 0
-    } = it, {
-        value_is_output: Ot = !1
-    } = it, {
-        rtl: It = !1
-    } = it, {
-        text_align: Nt = void 0
-    } = it, {
-        autofocus: Ft = !1
-    } = it, {
-        autoscroll: zt = !0
-    } = it, {
-        interactive: jt
-    } = it, {
-        sources: Vt = ["upload"]
-    } = it, {
-        root: Gt = ""
-    } = it, {
-        proxy_url: cn = ""
-    } = it, {
-        upload_button_props: en = {}
-    } = it, Kt = {}, {
-        webcam_props: an = {}
-    } = it, Qt = {}, {
-        submit_button_props: Zt = {}
-    } = it, Jt = {}, {
-        file_preview_props: pn = {}
-    } = it, hn = {}, un = !1;
-    const ln = getContext("upload_files");
+    let mt, {
+            gradio: gt
+        } = it,
+        {
+            label: bt = ""
+        } = it,
+        {
+            info: _t = void 0
+        } = it,
+        {
+            elem_id: yt = ""
+        } = it,
+        {
+            elem_classes: Et = []
+        } = it,
+        {
+            visible: xt = !0
+        } = it,
+        {
+            value: wt = {
+                text: "",
+                files: []
+            }
+        } = it,
+        {
+            lines: $t
+        } = it,
+        {
+            placeholder: Ct = ""
+        } = it,
+        {
+            show_label: Rt
+        } = it,
+        {
+            max_lines: Mt
+        } = it,
+        {
+            type: Lt = "text"
+        } = it,
+        {
+            container: Pt = !0
+        } = it,
+        {
+            scale: kt = null
+        } = it,
+        {
+            min_width: At = void 0
+        } = it,
+        {
+            show_copy_button: Tt = !1
+        } = it,
+        {
+            loading_status: Ot = void 0
+        } = it,
+        {
+            value_is_output: It = !1
+        } = it,
+        {
+            rtl: Nt = !1
+        } = it,
+        {
+            text_align: Ft = void 0
+        } = it,
+        {
+            autofocus: zt = !1
+        } = it,
+        {
+            autoscroll: jt = !0
+        } = it,
+        {
+            interactive: Vt
+        } = it,
+        {
+            sources: Gt = ["upload"]
+        } = it,
+        {
+            root: cn = ""
+        } = it,
+        {
+            proxy_url: en = ""
+        } = it,
+        {
+            upload_button_props: Kt = {}
+        } = it,
+        an = {},
+        {
+            webcam_props: Qt = {}
+        } = it,
+        Zt = {},
+        {
+            submit_button_props: Jt = {}
+        } = it,
+        pn = {},
+        {
+            file_preview_props: hn = {}
+        } = it,
+        un = {},
+        ln = !1;
+    const Xt = getContext("upload_files");
     setContextValue({
-        upload: async (yn) => {
+        upload: async (En) => {
             try {
-                ft(30, un = !0);
-                const jn = await upload(await prepare_files(yn), Gt, void 0, ln);
-                return _optionalChain([jn, "optionalAccess", (An) => An.filter, "call", (An) => An(Boolean)]) || [];
+                ft(29, ln = !0);
+                const An = await upload(await prepare_files(En), cn, void 0, Xt);
+                return _optionalChain([An, "optionalAccess", (gn) => gn.filter, "call", (gn) => gn(Boolean)]) || [];
             } catch {
                 return [];
             } finally {
-                ft(30, un = !1);
+                ft(29, ln = !1);
             }
         }
     });
 
-    function Ht(yn) {
-        Ot = yn, ft(2, Ot);
+    function Dt(En) {
+        It = En, ft(1, It);
     }
-    const Dt = (yn) => {
-            ft(1, xt.text = yn.detail, xt), mt.dispatch("change", xt);
+    const Bt = (En) => {
+            ft(0, wt.text = En.detail, wt), gt.dispatch("change", wt);
         },
-        Bt = () => mt.dispatch("input"),
-        Wt = () => {
-            un || mt.dispatch("submit");
+        Wt = () => gt.dispatch("input"),
+        Yt = () => {
+            ln || gt.dispatch("submit");
         },
-        Yt = () => mt.dispatch("blur"),
-        on = (yn) => mt.dispatch("select", yn.detail),
-        rn = () => mt.dispatch("focus"),
-        mn = (yn) => {
-            Kt.file_count === "single" ? ft(1, xt.files = yn.detail, xt) : ft(1, xt.files = [...xt.files, ...yn.detail], xt), mt.dispatch("upload"), mt.dispatch("change", xt);
+        on = () => gt.dispatch("blur"),
+        rn = (En) => gt.dispatch("select", En.detail),
+        mn = () => gt.dispatch("focus"),
+        _n = (En) => {
+            an.file_count === "single" ? ft(0, wt.files = En.detail, wt) : ft(0, wt.files = [...wt.files, ...En.detail], wt), gt.dispatch("upload"), gt.dispatch("change", wt);
         };
 
-    function _n(yn) {
-        bubble.call(this, _e, yn);
+    function yn(En) {
+        bubble.call(this, _e, En);
     }
-    const Sn = (yn) => {
-            mt.dispatch("error", yn.detail);
+    const Cn = (En) => {
+            gt.dispatch("error", En.detail);
         },
-        Cn = (yn) => {
-            Kt.file_count === "single" ? ft(1, xt.files = [yn.detail], xt) : ft(1, xt.files = [...xt.files, yn.detail], xt), mt.dispatch("upload"), mt.dispatch("change", xt);
+        kn = (En) => {
+            an.file_count === "single" ? ft(0, wt.files = [En.detail], wt) : ft(0, wt.files = [...wt.files, En.detail], wt), gt.dispatch("upload"), gt.dispatch("change", wt);
         },
-        kn = (yn) => {
-            mt.dispatch("error", yn.detail);
+        Pn = (En) => {
+            gt.dispatch("error", En.detail);
         },
-        Pn = (yn) => {
-            Kt.file_count === "single" ? ft(1, xt.files = [yn.detail], xt) : ft(1, xt.files = [...xt.files, yn.detail], xt), mt.dispatch("upload"), mt.dispatch("change", xt);
+        Mn = (En) => {
+            an.file_count === "single" ? ft(0, wt.files = [En.detail], wt) : ft(0, wt.files = [...wt.files, En.detail], wt), gt.dispatch("upload"), gt.dispatch("change", wt);
         },
-        Mn = () => mt.dispatch("submit");
+        Wn = () => gt.dispatch("submit");
 
-    function Wn(yn) {
-        bubble.call(this, _e, yn);
+    function Rn(En) {
+        bubble.call(this, _e, En);
     }
-    const Rn = (yn) => {
-        ft(1, xt.files = xt.files.filter((jn, An) => An !== yn.detail), xt), mt.dispatch("change", xt);
+    const Fn = (En) => {
+        ft(0, wt.files = wt.files.filter((An, gn) => gn !== En.detail), wt), gt.dispatch("change", wt);
     };
-    return _e.$$set = (yn) => {
-        "gradio" in yn && ft(3, mt = yn.gradio), "label" in yn && ft(4, gt = yn.label), "info" in yn && ft(5, bt = yn.info), "elem_id" in yn && ft(6, _t = yn.elem_id), "elem_classes" in yn && ft(7, yt = yn.elem_classes), "visible" in yn && ft(8, Et = yn.visible), "value" in yn && ft(1, xt = yn.value), "lines" in yn && ft(9, wt = yn.lines), "placeholder" in yn && ft(10, $t = yn.placeholder), "show_label" in yn && ft(11, Ct = yn.show_label), "max_lines" in yn && ft(12, Rt = yn.max_lines), "type" in yn && ft(13, Mt = yn.type), "container" in yn && ft(14, Lt = yn.container), "scale" in yn && ft(15, Pt = yn.scale), "min_width" in yn && ft(16, kt = yn.min_width), "show_copy_button" in yn && ft(17, At = yn.show_copy_button), "loading_status" in yn && ft(18, Tt = yn.loading_status), "value_is_output" in yn && ft(2, Ot = yn.value_is_output), "rtl" in yn && ft(19, It = yn.rtl), "text_align" in yn && ft(20, Nt = yn.text_align), "autofocus" in yn && ft(21, Ft = yn.autofocus), "autoscroll" in yn && ft(22, zt = yn.autoscroll), "interactive" in yn && ft(23, jt = yn.interactive), "sources" in yn && ft(0, Vt = yn.sources), "root" in yn && ft(24, Gt = yn.root), "proxy_url" in yn && ft(25, cn = yn.proxy_url), "upload_button_props" in yn && ft(31, en = yn.upload_button_props), "webcam_props" in yn && ft(32, an = yn.webcam_props), "submit_button_props" in yn && ft(33, Zt = yn.submit_button_props), "file_preview_props" in yn && ft(34, pn = yn.file_preview_props);
+    return _e.$$set = (En) => {
+        "gradio" in En && ft(2, gt = En.gradio), "label" in En && ft(3, bt = En.label), "info" in En && ft(4, _t = En.info), "elem_id" in En && ft(5, yt = En.elem_id), "elem_classes" in En && ft(6, Et = En.elem_classes), "visible" in En && ft(7, xt = En.visible), "value" in En && ft(0, wt = En.value), "lines" in En && ft(8, $t = En.lines), "placeholder" in En && ft(9, Ct = En.placeholder), "show_label" in En && ft(10, Rt = En.show_label), "max_lines" in En && ft(11, Mt = En.max_lines), "type" in En && ft(12, Lt = En.type), "container" in En && ft(13, Pt = En.container), "scale" in En && ft(14, kt = En.scale), "min_width" in En && ft(15, At = En.min_width), "show_copy_button" in En && ft(16, Tt = En.show_copy_button), "loading_status" in En && ft(17, Ot = En.loading_status), "value_is_output" in En && ft(1, It = En.value_is_output), "rtl" in En && ft(18, Nt = En.rtl), "text_align" in En && ft(19, Ft = En.text_align), "autofocus" in En && ft(20, zt = En.autofocus), "autoscroll" in En && ft(21, jt = En.autoscroll), "interactive" in En && ft(22, Vt = En.interactive), "sources" in En && ft(31, Gt = En.sources), "root" in En && ft(23, cn = En.root), "proxy_url" in En && ft(24, en = En.proxy_url), "upload_button_props" in En && ft(32, Kt = En.upload_button_props), "webcam_props" in En && ft(33, Qt = En.webcam_props), "submit_button_props" in En && ft(34, Jt = En.submit_button_props), "file_preview_props" in En && ft(35, hn = En.file_preview_props);
     }, _e.$$.update = () => {
-        _e.$$.dirty[0] & /*sources*/
-            1 && ft(0, Vt = Array.from(new Set(Vt))), _e.$$.dirty[0] & /*_upload_button_props*/
-            67108864 | _e.$$.dirty[1] & /*upload_button_props*/
-            1 && ft(26, Kt = {
-                ...Kt,
-                ...en
+        _e.$$.dirty[1] & /*sources*/
+            1 && ft(30, mt = Array.from(new Set(Gt))), _e.$$.dirty[0] & /*_upload_button_props*/
+            33554432 | _e.$$.dirty[1] & /*upload_button_props*/
+            2 && ft(25, an = {
+                ...an,
+                ...Kt
             }), _e.$$.dirty[0] & /*_webcam_props*/
-            134217728 | _e.$$.dirty[1] & /*webcam_props*/
-            2 && ft(27, Qt = {
-                ...Qt,
-                ...an
+            67108864 | _e.$$.dirty[1] & /*webcam_props*/
+            4 && ft(26, Zt = {
+                ...Zt,
+                ...Qt
             }), _e.$$.dirty[0] & /*_submit_button_props*/
-            268435456 | _e.$$.dirty[1] & /*submit_button_props*/
-            4 && ft(28, Jt = {
-                ...Jt,
-                ...Zt
+            134217728 | _e.$$.dirty[1] & /*submit_button_props*/
+            8 && ft(27, pn = {
+                ...pn,
+                ...Jt
             }), _e.$$.dirty[0] & /*_file_preview_props*/
-            536870912 | _e.$$.dirty[1] & /*file_preview_props*/
-            8 && ft(29, hn = {
-                ...hn,
-                ...pn
+            268435456 | _e.$$.dirty[1] & /*file_preview_props*/
+            16 && ft(28, un = {
+                ...un,
+                ...hn
             });
     }, [
-        Vt,
-        xt,
-        Ot,
-        mt,
+        wt,
+        It,
         gt,
         bt,
         _t,
         yt,
         Et,
-        wt,
+        xt,
         $t,
         Ct,
         Rt,
         Mt,
         Lt,
         Pt,
         kt,
         At,
         Tt,
-        It,
+        Ot,
         Nt,
         Ft,
         zt,
         jt,
-        Gt,
+        Vt,
         cn,
-        Kt,
-        Qt,
-        Jt,
-        hn,
-        un,
         en,
         an,
         Zt,
         pn,
-        Ht,
+        un,
+        ln,
+        mt,
+        Gt,
+        Kt,
+        Qt,
+        Jt,
+        hn,
         Dt,
         Bt,
         Wt,
         Yt,
         on,
         rn,
         mn,
         _n,
-        Sn,
+        yn,
         Cn,
         kn,
         Pn,
         Mn,
         Wn,
-        Rn
+        Rn,
+        Fn
     ];
 }
 class Index extends SvelteComponent {
     constructor(it) {
         super(), init(
             this,
             it,
             instance,
             create_fragment,
             safe_not_equal, {
-                gradio: 3,
-                label: 4,
-                info: 5,
-                elem_id: 6,
-                elem_classes: 7,
-                visible: 8,
-                value: 1,
-                lines: 9,
-                placeholder: 10,
-                show_label: 11,
-                max_lines: 12,
-                type: 13,
-                container: 14,
-                scale: 15,
-                min_width: 16,
-                show_copy_button: 17,
-                loading_status: 18,
-                value_is_output: 2,
-                rtl: 19,
-                text_align: 20,
-                autofocus: 21,
-                autoscroll: 22,
-                interactive: 23,
-                sources: 0,
-                root: 24,
-                proxy_url: 25,
-                upload_button_props: 31,
-                webcam_props: 32,
-                submit_button_props: 33,
-                file_preview_props: 34
+                gradio: 2,
+                label: 3,
+                info: 4,
+                elem_id: 5,
+                elem_classes: 6,
+                visible: 7,
+                value: 0,
+                lines: 8,
+                placeholder: 9,
+                show_label: 10,
+                max_lines: 11,
+                type: 12,
+                container: 13,
+                scale: 14,
+                min_width: 15,
+                show_copy_button: 16,
+                loading_status: 17,
+                value_is_output: 1,
+                rtl: 18,
+                text_align: 19,
+                autofocus: 20,
+                autoscroll: 21,
+                interactive: 22,
+                sources: 31,
+                root: 23,
+                proxy_url: 24,
+                upload_button_props: 32,
+                webcam_props: 33,
+                submit_button_props: 34,
+                file_preview_props: 35
             },
             null,
             [-1, -1]
         );
     }
     get gradio() {
-        return this.$$.ctx[3];
+        return this.$$.ctx[2];
     }
     set gradio(it) {
         this.$$set({
             gradio: it
         }), flush();
     }
     get label() {
-        return this.$$.ctx[4];
+        return this.$$.ctx[3];
     }
     set label(it) {
         this.$$set({
             label: it
         }), flush();
     }
     get info() {
-        return this.$$.ctx[5];
+        return this.$$.ctx[4];
     }
     set info(it) {
         this.$$set({
             info: it
         }), flush();
     }
     get elem_id() {
-        return this.$$.ctx[6];
+        return this.$$.ctx[5];
     }
     set elem_id(it) {
         this.$$set({
             elem_id: it
         }), flush();
     }
     get elem_classes() {
-        return this.$$.ctx[7];
+        return this.$$.ctx[6];
     }
     set elem_classes(it) {
         this.$$set({
             elem_classes: it
         }), flush();
     }
     get visible() {
-        return this.$$.ctx[8];
+        return this.$$.ctx[7];
     }
     set visible(it) {
         this.$$set({
             visible: it
         }), flush();
     }
     get value() {
-        return this.$$.ctx[1];
+        return this.$$.ctx[0];
     }
     set value(it) {
         this.$$set({
             value: it
         }), flush();
     }
     get lines() {
-        return this.$$.ctx[9];
+        return this.$$.ctx[8];
     }
     set lines(it) {
         this.$$set({
             lines: it
         }), flush();
     }
     get placeholder() {
-        return this.$$.ctx[10];
+        return this.$$.ctx[9];
     }
     set placeholder(it) {
         this.$$set({
             placeholder: it
         }), flush();
     }
     get show_label() {
-        return this.$$.ctx[11];
+        return this.$$.ctx[10];
     }
     set show_label(it) {
         this.$$set({
             show_label: it
         }), flush();
     }
     get max_lines() {
-        return this.$$.ctx[12];
+        return this.$$.ctx[11];
     }
     set max_lines(it) {
         this.$$set({
             max_lines: it
         }), flush();
     }
     get type() {
-        return this.$$.ctx[13];
+        return this.$$.ctx[12];
     }
     set type(it) {
         this.$$set({
             type: it
         }), flush();
     }
     get container() {
-        return this.$$.ctx[14];
+        return this.$$.ctx[13];
     }
     set container(it) {
         this.$$set({
             container: it
         }), flush();
     }
     get scale() {
-        return this.$$.ctx[15];
+        return this.$$.ctx[14];
     }
     set scale(it) {
         this.$$set({
             scale: it
         }), flush();
     }
     get min_width() {
-        return this.$$.ctx[16];
+        return this.$$.ctx[15];
     }
     set min_width(it) {
         this.$$set({
             min_width: it
         }), flush();
     }
     get show_copy_button() {
-        return this.$$.ctx[17];
+        return this.$$.ctx[16];
     }
     set show_copy_button(it) {
         this.$$set({
             show_copy_button: it
         }), flush();
     }
     get loading_status() {
-        return this.$$.ctx[18];
+        return this.$$.ctx[17];
     }
     set loading_status(it) {
         this.$$set({
             loading_status: it
         }), flush();
     }
     get value_is_output() {
-        return this.$$.ctx[2];
+        return this.$$.ctx[1];
     }
     set value_is_output(it) {
         this.$$set({
             value_is_output: it
         }), flush();
     }
     get rtl() {
-        return this.$$.ctx[19];
+        return this.$$.ctx[18];
     }
     set rtl(it) {
         this.$$set({
             rtl: it
         }), flush();
     }
     get text_align() {
-        return this.$$.ctx[20];
+        return this.$$.ctx[19];
     }
     set text_align(it) {
         this.$$set({
             text_align: it
         }), flush();
     }
     get autofocus() {
-        return this.$$.ctx[21];
+        return this.$$.ctx[20];
     }
     set autofocus(it) {
         this.$$set({
             autofocus: it
         }), flush();
     }
     get autoscroll() {
-        return this.$$.ctx[22];
+        return this.$$.ctx[21];
     }
     set autoscroll(it) {
         this.$$set({
             autoscroll: it
         }), flush();
     }
     get interactive() {
-        return this.$$.ctx[23];
+        return this.$$.ctx[22];
     }
     set interactive(it) {
         this.$$set({
             interactive: it
         }), flush();
     }
     get sources() {
-        return this.$$.ctx[0];
+        return this.$$.ctx[31];
     }
     set sources(it) {
         this.$$set({
             sources: it
         }), flush();
     }
     get root() {
-        return this.$$.ctx[24];
+        return this.$$.ctx[23];
     }
     set root(it) {
         this.$$set({
             root: it
         }), flush();
     }
     get proxy_url() {
-        return this.$$.ctx[25];
+        return this.$$.ctx[24];
     }
     set proxy_url(it) {
         this.$$set({
             proxy_url: it
         }), flush();
     }
     get upload_button_props() {
-        return this.$$.ctx[31];
+        return this.$$.ctx[32];
     }
     set upload_button_props(it) {
         this.$$set({
             upload_button_props: it
         }), flush();
     }
     get webcam_props() {
-        return this.$$.ctx[32];
+        return this.$$.ctx[33];
     }
     set webcam_props(it) {
         this.$$set({
             webcam_props: it
         }), flush();
     }
     get submit_button_props() {
-        return this.$$.ctx[33];
+        return this.$$.ctx[34];
     }
     set submit_button_props(it) {
         this.$$set({
             submit_button_props: it
         }), flush();
     }
     get file_preview_props() {
-        return this.$$.ctx[34];
+        return this.$$.ctx[35];
     }
     set file_preview_props(it) {
         this.$$set({
             file_preview_props: it
         }), flush();
     }
 }
```

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/style.css` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/component/wrapper-6f348d45-f837cf34.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/component/wrapper-6f348d45-f837cf34.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/MultimodalInput/templates/example/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/MultimodalInput/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/__init__.py` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/__init__.py`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/__init__.pyi` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/templates/component/index.js` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/components/WaterfallGallery/templates/component/style.css` & `modelscope_studio-0.1.7/backend/modelscope_studio/components/WaterfallGallery/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/backend/modelscope_studio/utils/process_links.py` & `modelscope_studio-0.1.7/backend/modelscope_studio/utils/process_links.py`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/.gitignore` & `modelscope_studio-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/LICENSE` & `modelscope_studio-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/README.md` & `modelscope_studio-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `modelscope_studio-0.1.6/pyproject.toml` & `modelscope_studio-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "modelscope_studio"
-version = "0.1.6"
+version = "0.1.7"
 description = "A set of extension component, inluding components for conversational input and display in multimodal scenarios, as well as more components for vertical scenarios."
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = [
   "gradio-custom-component",
@@ -42,14 +42,22 @@
 [tool.hatch.build]
 artifacts = [
   "*.pyi",
   "backend/modelscope_studio/components/Chatbot/templates",
   "backend/modelscope_studio/components/MultimodalInput/templates",
   "backend/modelscope_studio/components/Markdown/templates",
   "backend/modelscope_studio/components/WaterfallGallery/templates",
+  "backend/modelscope_studio/components/Chatbot/templates",
+  "backend/modelscope_studio/components/Markdown/templates",
+  "backend/modelscope_studio/components/MultimodalInput/templates",
+  "backend/modelscope_studio/components/WaterfallGallery/templates",
+  "backend/modelscope_studio/components/Chatbot/templates",
+  "backend/modelscope_studio/components/Markdown/templates",
+  "backend/modelscope_studio/components/MultimodalInput/templates",
+  "backend/modelscope_studio/components/WaterfallGallery/templates",
 ]
 
 [tool.hatch.build.targets.sdist]
 exclude = ["__pycache__"]
 include = ["/backend/modelscope_studio"]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `modelscope_studio-0.1.6/PKG-INFO` & `modelscope_studio-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: modelscope_studio
-Version: 0.1.6
+Version: 0.1.7
 Summary: A set of extension component, inluding components for conversational input and display in multimodal scenarios, as well as more components for vertical scenarios.
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: gradio-custom-component,gradio-template-Chatbot,modelscope-studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

