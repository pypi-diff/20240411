# Comparing `tmp/cumo-0.32.0.tar.gz` & `tmp/cumo-0.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumo-0.32.0.tar", max compression
+gzip compressed data, was "cumo-0.33.0.tar", max compression
```

## Comparing `cumo-0.32.0.tar` & `cumo-0.33.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1275 2024-03-21 11:24:39.298661 cumo-0.32.0/README.md
--rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/.gitignore
--rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/__init__.py
--rw-r--r--   0        0        0     3683 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/__main__.py
--rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/.gitignore
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/__init__.py
--rw-r--r--   0        0        0     1675 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/_internal/down_sample.py
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/members/__init__.py
--rw-r--r--   0        0        0     8722 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/_internal/members/camera.py
--rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/members/capture_screen.py
--rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/members/custom_control.py
--rw-r--r--   0        0        0     5927 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/_internal/members/event_handler.py
--rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/members/internal_utils.py
--rw-r--r--   0        0        0     6396 2023-09-11 09:15:41.832883 cumo-0.32.0/cumo/_internal/members/keyboard_event_handler.py
--rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_internal/members/remove_object.py
--rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.32.0/cumo/_internal/members/send_object.py
--rw-r--r--   0        0        0    10336 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/_internal/members/set_custom_control.py
--rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.32.0/cumo/_internal/members/set_enable.py
--rw-r--r--   0        0        0     1256 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/_internal/members/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 11:24:00.917259 cumo-0.32.0/cumo/_internal/protobuf/__init__.py
--rw-r--r--   0        0        0     3923 2024-03-21 11:24:00.917259 cumo-0.32.0/cumo/_internal/protobuf/client_pb2.py
--rw-r--r--   0        0        0    10387 2024-03-21 11:24:00.917259 cumo-0.32.0/cumo/_internal/protobuf/client_pb2.pyi
--rw-r--r--   0        0        0    12303 2024-03-21 11:24:00.056055 cumo-0.32.0/cumo/_internal/protobuf/server_pb2.py
--rw-r--r--   0        0        0    40121 2024-03-21 11:24:00.056055 cumo-0.32.0/cumo/_internal/protobuf/server_pb2.pyi
--rw-r--r--   0        0        0     4200 2024-03-21 11:15:04.876331 cumo-0.32.0/cumo/_internal/server.py
--rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_vendor/pypcd/LICENSE
--rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/_vendor/pypcd/pypcd.py
--rw-r--r--   0        0        0     1119 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/camera_state.py
--rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.32.0/cumo/keyboard_event.py
--rw-r--r--   0        0        0     3554 2023-09-13 10:26:38.801824 cumo-0.32.0/cumo/pointcloudviewer.py
--rw-r--r--   0        0        0  5077059 2024-03-21 11:24:39.298661 cumo-0.32.0/cumo/public/bundle-97e7bef4.js
--rw-r--r--   0        0        0   243028 2024-03-21 11:24:39.298661 cumo-0.32.0/cumo/public/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      515 2024-03-21 11:24:39.298661 cumo-0.32.0/cumo/public/index-31f52342.css
--rw-r--r--   0        0        0      281 2024-03-21 11:24:39.298661 cumo-0.32.0/cumo/public/index.html
--rw-r--r--   0        0        0     1219 2024-03-21 11:17:50.006048 cumo-0.32.0/pyproject.toml
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.32.0/PKG-INFO
+-rw-r--r--   0        0        0     1275 2024-04-11 11:47:47.357491 cumo-0.33.0/README.md
+-rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/.gitignore
+-rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/__init__.py
+-rw-r--r--   0        0        0     3683 2024-04-11 11:47:04.668132 cumo-0.33.0/cumo/__main__.py
+-rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/.gitignore
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/__init__.py
+-rw-r--r--   0        0        0     1675 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/_internal/down_sample.py
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/members/__init__.py
+-rw-r--r--   0        0        0     8722 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/_internal/members/camera.py
+-rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/members/capture_screen.py
+-rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/members/custom_control.py
+-rw-r--r--   0        0        0     5927 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/_internal/members/event_handler.py
+-rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/members/internal_utils.py
+-rw-r--r--   0        0        0     6396 2023-09-11 09:15:41.832883 cumo-0.33.0/cumo/_internal/members/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_internal/members/remove_object.py
+-rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.33.0/cumo/_internal/members/send_object.py
+-rw-r--r--   0        0        0    10336 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/_internal/members/set_custom_control.py
+-rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.33.0/cumo/_internal/members/set_enable.py
+-rw-r--r--   0        0        0     1256 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/_internal/members/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:47:13.438572 cumo-0.33.0/cumo/_internal/protobuf/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-11 11:47:13.428572 cumo-0.33.0/cumo/_internal/protobuf/client_pb2.py
+-rw-r--r--   0        0        0    10387 2024-04-11 11:47:13.428572 cumo-0.33.0/cumo/_internal/protobuf/client_pb2.pyi
+-rw-r--r--   0        0        0    12303 2024-04-11 11:47:12.828542 cumo-0.33.0/cumo/_internal/protobuf/server_pb2.py
+-rw-r--r--   0        0        0    40121 2024-04-11 11:47:12.828542 cumo-0.33.0/cumo/_internal/protobuf/server_pb2.pyi
+-rw-r--r--   0        0        0     4200 2024-03-21 11:15:04.876331 cumo-0.33.0/cumo/_internal/server.py
+-rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_vendor/pypcd/LICENSE
+-rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/_vendor/pypcd/pypcd.py
+-rw-r--r--   0        0        0     1119 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/camera_state.py
+-rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.33.0/cumo/keyboard_event.py
+-rw-r--r--   0        0        0     3554 2023-09-13 10:26:38.801824 cumo-0.33.0/cumo/pointcloudviewer.py
+-rw-r--r--   0        0        0  5077279 2024-04-11 11:47:47.347491 cumo-0.33.0/cumo/public/bundle-0c935839.js
+-rw-r--r--   0        0        0   243028 2024-04-11 11:47:47.347491 cumo-0.33.0/cumo/public/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      515 2024-04-11 11:47:47.347491 cumo-0.33.0/cumo/public/index-31f52342.css
+-rw-r--r--   0        0        0      281 2024-04-11 11:47:47.347491 cumo-0.33.0/cumo/public/index.html
+-rw-r--r--   0        0        0     1219 2024-04-11 11:44:45.303456 cumo-0.33.0/pyproject.toml
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.33.0/PKG-INFO
```

### Comparing `cumo-0.32.0/README.md` & `cumo-0.33.0/README.md`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/__main__.py` & `cumo-0.33.0/cumo/__main__.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/down_sample.py` & `cumo-0.33.0/cumo/_internal/down_sample.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/camera.py` & `cumo-0.33.0/cumo/_internal/members/camera.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/capture_screen.py` & `cumo-0.33.0/cumo/_internal/members/capture_screen.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/custom_control.py` & `cumo-0.33.0/cumo/_internal/members/custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/event_handler.py` & `cumo-0.33.0/cumo/_internal/members/event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/internal_utils.py` & `cumo-0.33.0/cumo/_internal/members/internal_utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/keyboard_event_handler.py` & `cumo-0.33.0/cumo/_internal/members/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/remove_object.py` & `cumo-0.33.0/cumo/_internal/members/remove_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/send_object.py` & `cumo-0.33.0/cumo/_internal/members/send_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/set_custom_control.py` & `cumo-0.33.0/cumo/_internal/members/set_custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/set_enable.py` & `cumo-0.33.0/cumo/_internal/members/set_enable.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/members/utils.py` & `cumo-0.33.0/cumo/_internal/members/utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/protobuf/client_pb2.py` & `cumo-0.33.0/cumo/_internal/protobuf/client_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/protobuf/client_pb2.pyi` & `cumo-0.33.0/cumo/_internal/protobuf/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/protobuf/server_pb2.py` & `cumo-0.33.0/cumo/_internal/protobuf/server_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/protobuf/server_pb2.pyi` & `cumo-0.33.0/cumo/_internal/protobuf/server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_internal/server.py` & `cumo-0.33.0/cumo/_internal/server.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_vendor/pypcd/LICENSE` & `cumo-0.33.0/cumo/_vendor/pypcd/LICENSE`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/_vendor/pypcd/pypcd.py` & `cumo-0.33.0/cumo/_vendor/pypcd/pypcd.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/camera_state.py` & `cumo-0.33.0/cumo/camera_state.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/keyboard_event.py` & `cumo-0.33.0/cumo/keyboard_event.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/pointcloudviewer.py` & `cumo-0.33.0/cumo/pointcloudviewer.py`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/public/bundle-97e7bef4.js` & `cumo-0.33.0/cumo/public/bundle-0c935839.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -114736,19 +114736,20 @@
         he(this, "__position");
         he(this, "__elem");
         he(this, "__coordType");
         this.__position = r, this.__elem = t, this.__coordType = s, this.__elem.style.position = "absolute", this.uuid = n
     }
     render(t, r) {
         let s, n;
+        const o = t.getClientRects()[0];
         if (this.__coordType === CoordinateType.WORLD_COORDINATE) {
-            const o = Vector3.Project(this.__position, Matrix.Identity(), r.getTransformMatrix(), new Viewport(0, 0, t.width, t.height));
-            s = o.x, n = o.y
+            const c = Vector3.Project(this.__position, Matrix.IdentityReadOnly, r.getTransformMatrix(), new Viewport(0, 0, t.width, t.height));
+            s = c.x / window.devicePixelRatio, n = c.y / window.devicePixelRatio
         } else console.assert(this.__coordType === CoordinateType.SCREEN_COORDINATE), s = this.__position.x, n = this.__position.y;
-        this.__elem.style.top = "" + n + "px", this.__elem.style.left = "" + s + "px"
+        this.__elem.style.top = "" + (n + o.top) + "px", this.__elem.style.left = "" + (s + o.left) + "px"
     }
     dispose() {
         this.__elem.remove()
     }
 }
 class Lineset {
     constructor(t, r, s, n, o) {
@@ -114759,36 +114760,36 @@
             const h = s[c + 0],
                 d = s[c + 1],
                 p = s[c + 2];
             this.colorsStr[Math.floor(c / 3)] = "rgb(" + h + "," + d + "," + p + ")"
         }
         this.UUID = o.toUpperCase()
     }
-    render(t, r, s) {
-        const n = Frustum.GetPlanes(s),
-            o = new Viewport(0, 0, t.domElement.width, t.domElement.height),
-            c = new Vector3,
-            h = new Vector3;
+    render(t, r) {
+        const s = Frustum.GetPlanes(r),
+            n = new Viewport(0, 0, t.domElement.width, t.domElement.height),
+            o = new Vector3,
+            c = new Vector3;
         t.ctx.save();
-        for (let d = 0; d * 2 + 1 < this.indices.length; d++) {
-            const p = this.indices[d * 2 + 0],
-                g = this.indices[d * 2 + 1],
-                _ = this.positions[p * 3 + 0],
-                m = this.positions[p * 3 + 1],
-                C = this.positions[p * 3 + 2],
-                S = this.positions[g * 3 + 0],
-                b = this.positions[g * 3 + 1],
-                x = this.positions[g * 3 + 2];
-            if (c.set(_, m, C), h.set(S, b, x), !trimLineEndPoint(c, h, n) || !trimLineEndPoint(h, c, n)) continue;
-            Vector3.ProjectToRef(c, Matrix.IdentityReadOnly, s, o, c), Vector3.ProjectToRef(h, Matrix.IdentityReadOnly, s, o, h);
-            const y = c.x,
-                v = c.y,
-                P = h.x,
-                M = h.y;
-            t.ctx.beginPath(), t.ctx.lineWidth = d < this.widths.length ? this.widths[d] : 1, t.ctx.strokeStyle = d < this.colorsStr.length ? this.colorsStr[d] : "white", t.ctx.moveTo(y, v), t.ctx.lineTo(P, M), t.ctx.stroke()
+        for (let h = 0; h * 2 + 1 < this.indices.length; h++) {
+            const d = this.indices[h * 2 + 0],
+                p = this.indices[h * 2 + 1],
+                g = this.positions[d * 3 + 0],
+                _ = this.positions[d * 3 + 1],
+                m = this.positions[d * 3 + 2],
+                C = this.positions[p * 3 + 0],
+                S = this.positions[p * 3 + 1],
+                b = this.positions[p * 3 + 2];
+            if (o.set(g, _, m), c.set(C, S, b), !trimLineEndPoint(o, c, s) || !trimLineEndPoint(c, o, s)) continue;
+            Vector3.ProjectToRef(o, Matrix.IdentityReadOnly, r, n, o), Vector3.ProjectToRef(c, Matrix.IdentityReadOnly, r, n, c);
+            const x = o.x,
+                y = o.y,
+                v = c.x,
+                P = c.y;
+            t.ctx.beginPath(), t.ctx.lineWidth = h < this.widths.length ? this.widths[h] : 1, t.ctx.strokeStyle = h < this.colorsStr.length ? this.colorsStr[h] : "white", t.ctx.moveTo(x, y), t.ctx.lineTo(v, P), t.ctx.stroke()
         }
         t.ctx.restore()
     }
 }
 
 function trimLineEndPoint(l, t, r) {
     if (Frustum.IsPointInFrustum(l, r)) return !0;
@@ -116324,15 +116325,15 @@
             for (let b = 0; b < C; b++) S[b * 4 + 0] = m[b * 3 + 2], S[b * 4 + 1] = m[b * 3 + 1], S[b * 4 + 2] = m[b * 3 + 0], S[b * 4 + 3] = 1;
             h.set(S, VertexBuffer.ColorKind)
         } else sendFailure(l, t, `unsupported element size: ${g.BYTES_PER_ELEMENT}`)
     }
     const d = new StandardMaterial(t, r.scene);
     d.emissiveColor = new Color3(1, 1, 1), d.disableLighting = !0, d.pointsCloud = !0, d.pointSize = s.pointSize;
     const p = new Mesh(t, r.scene);
-    h.applyToMesh(p, !0), p.material = d, sendSuccess(l, t, t)
+    p.renderingGroupId = 1, h.applyToMesh(p, !0), p.material = d, sendSuccess(l, t, t)
 }
 
 function handleImage(l, t, r, s) {
     if (s === void 0) {
         sendFailure(l, t, "failed to get image");
         return
     }
@@ -123710,15 +123711,20 @@
         if (this.camera === null || !this.enabled) return;
         const t = this.camera.absoluteRotation.clone();
         this.target.subtractToRef(this.camera.position, this.eye);
         const r = this.eye.clone();
         r.normalize();
         const s = this.camera.upVector.clone(),
             n = this.camera.upVector.clone();
-        if (n.normalize(), 1 - Math.abs(Vector3.Dot(r, n)) < EPS && (n.set(0, 1, 0), n.applyRotationQuaternionInPlace(this.camera.rotationQuaternion), this.camera.upVector.copyFrom(n)), this.noRotate || this.rotateCamera(), this.noZoom || this.zoomCamera(), this.noPan || this.panCamera(), this.noRoll || this.rollCamera(), this.target.subtractToRef(this.eye, this.camera.position), this.checkDistances(), this.noRoll && this.camera.upVector.copyFrom(s), this.camera.setTarget(this.target), this.noRoll && 1 - Math.abs(Vector3.Dot(r, this.camera.upVector)) < .1) {
+        if (n.normalize(), 1 - Math.abs(Vector3.Dot(r, n)) < EPS) {
+            n.set(0, 1, 0);
+            const c = new Quaternion;
+            c.fromRotationMatrix(this.camera.getWorldMatrix()), n.applyRotationQuaternionInPlace(c), this.camera.upVector.copyFrom(n)
+        }
+        if (this.noRotate || this.rotateCamera(), this.noZoom || this.zoomCamera(), this.noPan || this.panCamera(), this.noRoll || this.rollCamera(), this.target.subtractToRef(this.eye, this.camera.position), this.checkDistances(), this.noRoll && this.camera.upVector.copyFrom(s), this.camera.setTarget(this.target), this.noRoll && 1 - Math.abs(Vector3.Dot(r, this.camera.upVector)) < .1) {
             const c = this.camera.absoluteRotation.clone();
             c.multiplyInPlace(t.invert());
             const h = new Vector3(c.x, c.y, c.z),
                 d = this.camera.upVector.clone().normalize(),
                 p = Vector3.Dot(h, d);
             h.copyFrom(d).scaleInPlace(p);
             const g = new Quaternion(h.x, h.y, h.z, c.w);
@@ -123915,15 +123921,15 @@
         this.container = t;
         const r = 1e-5,
             s = 1e5;
         this.canvas = document.createElement("canvas"), t.appendChild(this.canvas), this.engine = new Engine(this.canvas, !0, {
             adaptToDeviceRatio: !0
         }), this.scene = new Scene(this.engine), this.scene.clearColor = new Color4(0, 0, 0), this.scene.lightsEnabled = !1, this.camera = new FreeCamera("camera", new Vector3(-1, -1, -1), this.scene), this.camera.fov = this.config.camera.perspective.fov / 180 * Math.PI, this.camera.fovMode = Camera.FOVMODE_HORIZONTAL_FIXED, this.camera.maxZ = s, this.camera.minZ = r, this.cameraInput = new CustomCameraInput, this.camera.inputs.clear(), this.camera.inputs.add(this.cameraInput), this.camera.attachControl(), this.canvas2d = new Canvas2D, this.canvas.style.position = "absolute", this.canvas.style.width = "100vw", this.canvas.style.height = "100vh", this.canvas.width = window.innerWidth * window.devicePixelRatio, this.canvas.height = window.innerHeight * window.devicePixelRatio, this.canvas2d.domElement.style.pointerEvents = "none", t.appendChild(this.canvas2d.domElement);
         const n = () => {
-            this.canvas.width = window.innerWidth * window.devicePixelRatio, this.canvas.height = window.innerHeight * window.devicePixelRatio, this.engine.resize()
+            this.canvas.width = window.innerWidth * window.devicePixelRatio, this.canvas.height = window.innerHeight * window.devicePixelRatio, this.engine.setHardwareScalingLevel(1 / window.devicePixelRatio), this.engine.resize(!0)
         };
         window.addEventListener("resize", n);
         let o = null;
         const c = () => {
             o !== null && o();
             const p = window.matchMedia(`window and (resolution: ${window.devicePixelRatio}dppx)`);
             p.addEventListener("change", c), o = () => {
@@ -123948,15 +123954,15 @@
     }
     render() {
         if (!this.enabled) return;
         this.scene.render();
         for (let r = 0; r < this.overlays.length; r++) this.overlays[r].render(this.canvas, this.scene);
         this.canvas2d.ctx.clearRect(0, 0, this.canvas2d.domElement.width, this.canvas2d.domElement.height);
         const t = this.camera.getTransformationMatrix();
-        for (let r = 0; r < this.linesets.length; r++) this.linesets[r].render(this.canvas2d, this.scene, t)
+        for (let r = 0; r < this.linesets.length; r++) this.linesets[r].render(this.canvas2d, t)
     }
     switchCamera(t) {
         const r = t ? Camera.PERSPECTIVE_CAMERA : Camera.ORTHOGRAPHIC_CAMERA;
         this.camera.mode = r, t !== this.config.camera.usePerspective && (this.config.camera.usePerspective = t, this.gui.updateDisplay())
     }
 }
 const WEBSOCKET_URL_ENDPOINT = "/websocket_url",
```

### Comparing `cumo-0.32.0/cumo/public/bundle.js.LICENSE.txt` & `cumo-0.33.0/cumo/public/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/cumo/public/index-31f52342.css` & `cumo-0.33.0/cumo/public/index-31f52342.css`

 * *Files identical despite different names*

### Comparing `cumo-0.32.0/pyproject.toml` & `cumo-0.33.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 readme = "README.md"
 name = "cumo"
-version = "0.32.0"
+version = "0.33.0"
 description = "Webブラウザ上に点群を描画する python ライブラリ"
 authors = ["Kurusugawa Computer"]
 license = "BSD"
 keywords = ["point-cloud", "pcd"]
 repository = "https://github.com/kurusugawa-computer/cumo"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

### Comparing `cumo-0.32.0/PKG-INFO` & `cumo-0.33.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumo
-Version: 0.32.0
+Version: 0.33.0
 Summary: Webブラウザ上に点群を描画する python ライブラリ
 Home-page: https://github.com/kurusugawa-computer/cumo
 License: BSD
 Keywords: point-cloud,pcd
 Author: Kurusugawa Computer
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

