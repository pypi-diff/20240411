# Comparing `tmp/tarsier-0.5.92.tar.gz` & `tmp/tarsier-0.5.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarsier-0.5.92.tar", max compression
+gzip compressed data, was "tarsier-0.5.93.tar", max compression
```

## Comparing `tarsier-0.5.92.tar` & `tarsier-0.5.93.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-02-20 05:00:45.297770 tarsier-0.5.92/LICENSE
--rw-r--r--   0        0        0     5763 2024-02-20 05:00:45.297770 tarsier-0.5.92/README.md
--rw-r--r--   0        0        0     1392 2024-02-20 05:00:45.297770 tarsier-0.5.92/pyproject.toml
--rw-r--r--   0        0        0      115 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/__init__.py
--rw-r--r--   0        0        0     1575 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/__main__.py
--rw-r--r--   0        0        0      348 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/_utils.py
--rw-r--r--   0        0        0     1029 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/adapter/__init__.py
--rw-r--r--   0        0        0      488 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/adapter/_base.py
--rw-r--r--   0        0        0     2154 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/adapter/playwright.py
--rw-r--r--   0        0        0      941 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/adapter/selenium.py
--rw-r--r--   0        0        0      334 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/adapter/types.py
--rw-r--r--   0        0        0     2780 2024-02-20 05:00:46.633770 tarsier-0.5.92/tarsier/core.py
--rw-r--r--   0        0        0      180 2024-02-20 05:00:46.637770 tarsier-0.5.92/tarsier/ocr/__init__.py
--rw-r--r--   0        0        0     2617 2024-02-20 05:00:46.637770 tarsier-0.5.92/tarsier/ocr/ocr_service.py
--rw-r--r--   0        0        0      490 2024-02-20 05:00:46.637770 tarsier-0.5.92/tarsier/ocr/types.py
--rw-r--r--   0        0        0        0 2024-02-20 05:00:46.637770 tarsier-0.5.92/tarsier/py.typed
--rw-r--r--   0        0        0     4791 2024-02-20 05:00:55.157776 tarsier-0.5.92/tarsier/tag_utils.min.js
--rw-r--r--   0        0        0     7799 2024-02-20 05:00:46.637770 tarsier-0.5.92/tarsier/text_format.py
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 tarsier-0.5.92/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 21:53:35.657099 tarsier-0.5.93/LICENSE
+-rw-r--r--   0        0        0     5763 2024-04-11 21:53:35.657099 tarsier-0.5.93/README.md
+-rw-r--r--   0        0        0     1392 2024-04-11 21:53:35.657099 tarsier-0.5.93/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/__init__.py
+-rw-r--r--   0        0        0     1575 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/__main__.py
+-rw-r--r--   0        0        0      348 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/_utils.py
+-rw-r--r--   0        0        0     1029 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/adapter/__init__.py
+-rw-r--r--   0        0        0      488 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/adapter/_base.py
+-rw-r--r--   0        0        0     2154 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/adapter/playwright.py
+-rw-r--r--   0        0        0      941 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/adapter/selenium.py
+-rw-r--r--   0        0        0      334 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/adapter/types.py
+-rw-r--r--   0        0        0     2780 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/core.py
+-rw-r--r--   0        0        0      180 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/ocr/__init__.py
+-rw-r--r--   0        0        0     2617 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/ocr/ocr_service.py
+-rw-r--r--   0        0        0      490 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/ocr/types.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/py.typed
+-rw-r--r--   0        0        0     5723 2024-04-11 21:53:44.541099 tarsier-0.5.93/tarsier/tag_utils.min.js
+-rw-r--r--   0        0        0     7799 2024-04-11 21:53:36.977099 tarsier-0.5.93/tarsier/text_format.py
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 tarsier-0.5.93/PKG-INFO
```

### Comparing `tarsier-0.5.92/LICENSE` & `tarsier-0.5.93/LICENSE`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/README.md` & `tarsier-0.5.93/README.md`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/pyproject.toml` & `tarsier-0.5.93/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tarsier"
-version = "0.5.92"
+version = "0.5.93"
 description = "Vision utilities for web interaction agents"
 authors = ["Rohan Pandey", "Adam Watkins", "Asim Shrestha"]
 readme = "README.md"
 include = ["tarsier/**/*.min.js"]
 exclude = ["tarsier/**/*.ts", "tarsier_snapshots", "tarsier_snapshots/*"]
```

### Comparing `tarsier-0.5.92/tarsier/__main__.py` & `tarsier-0.5.93/tarsier/__main__.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/tarsier/adapter/__init__.py` & `tarsier-0.5.93/tarsier/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/tarsier/adapter/playwright.py` & `tarsier-0.5.93/tarsier/adapter/playwright.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/tarsier/adapter/selenium.py` & `tarsier-0.5.93/tarsier/adapter/selenium.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/tarsier/core.py` & `tarsier-0.5.93/tarsier/core.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/tarsier/ocr/ocr_service.py` & `tarsier-0.5.93/tarsier/ocr/ocr_service.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/tarsier/tag_utils.min.js` & `tarsier-0.5.93/tarsier/tag_utils.min.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,142 +1,155 @@
 "use strict";
 const tarsierId = "__tarsier_id",
     tarsierSelector = `#${tarsierId}`,
     elIsClean = t => {
         const i = t.getBoundingClientRect(),
-            o = window.getComputedStyle(t),
-            e = o.visibility === "hidden" || o.display === "none" || t.hidden || t.disabled,
-            r = o.opacity === "0",
-            n = i.width === 0 || i.height === 0,
-            s = t.tagName === "SCRIPT" || t.tagName === "STYLE";
-        return !e && !r && !n && !s
+            n = window.getComputedStyle(t),
+            e = n.visibility === "hidden" || n.display === "none" || t.hidden || t.disabled,
+            s = n.opacity === "0",
+            o = i.width === 0 || i.height === 0,
+            a = t.tagName === "SCRIPT" || t.tagName === "STYLE";
+        return !e && !s && !o && !a
     },
     inputs = ["a", "button", "textarea", "select", "details", "label"],
     isInteractable = t => inputs.includes(t.tagName.toLowerCase()) || t.tagName.toLowerCase() === "input" && t.type !== "hidden" || t.role === "button",
     text_input_types = ["text", "password", "email", "search", "url", "tel", "number"],
     isTextInsertable = t => t.tagName.toLowerCase() === "textarea" || t.tagName.toLowerCase() === "input" && text_input_types.includes(t.type),
     emptyTagWhitelist = ["input", "textarea", "select", "button"],
     isEmpty = t => {
         const i = t.tagName.toLowerCase();
         if (emptyTagWhitelist.includes(i) || t.childElementCount > 0) return !1;
         if ("innerText" in t && t.innerText.trim().length === 0) {
-            const o = t.querySelector("svg"),
+            const n = t.querySelector("svg"),
                 e = t.querySelector("img");
-            return o || e ? !1 : isElementInViewport(t)
+            return n || e ? !1 : isElementInViewport(t)
         }
         return !1
     };
 
 function isElementInViewport(t) {
     const i = t.getBoundingClientRect();
     return i.top >= 0 && i.left >= 0 && i.bottom <= (window.innerHeight || document.documentElement.clientHeight) && i.right <= (window.innerWidth || document.documentElement.clientWidth)
 }
 
 function getElementXPath(t) {
     let i = [],
-        o = "";
-    for (t && t.ownerDocument !== window.document && (o = `iframe[${t.getAttribute("iframe_index")}]`); t;) {
+        n = "";
+    for (t && t.ownerDocument !== window.document && (n = `iframe[${t.getAttribute("iframe_index")}]`); t;) {
         if (!t.tagName) {
             t = t.parentNode;
             continue
         }
         let e = t.tagName.toLowerCase(),
-            r = 1,
-            n = t.previousElementSibling;
-        for (; n;) n.tagName === t.tagName && r++, n = n.previousElementSibling;
-        let s = t.nextElementSibling,
-            a = !1;
-        for (; s;) {
-            if (s.tagName === t.tagName) {
-                a = !0;
+            s = 1,
+            o = t.previousElementSibling;
+        for (; o;) o.tagName === t.tagName && s++, o = o.previousElementSibling;
+        let a = t.nextElementSibling,
+            r = !1;
+        for (; a;) {
+            if (a.tagName === t.tagName) {
+                r = !0;
                 break
             }
-            s = s.nextElementSibling
+            a = a.nextElementSibling
         }
-        if ((r > 1 || a) && (e += `[${r}]`), t.id) {
+        if ((s > 1 || r) && (e += `[${s}]`), t.id) {
             if (e += `[@id="${t.id}"]`, i.length > 3) return i.unshift(e), "//" + i.join("/")
         } else if (t.className) {
             const l = Array.from(t.classList);
             e += `[@class="${t.className}"]`
         }
         i.unshift(e), t = t.parentNode
     }
-    return o + "//" + i.join("/")
+    return n + "//" + i.join("/")
 }
 
 function create_tagged_span(t, i) {
-    let o;
-    isInteractable(i) ? isTextInsertable(i) ? o = `[#${t}]` : i.tagName.toLowerCase() == "a" ? o = `[@${t}]` : o = `[$${t}]` : o = `[${t}]`;
+    let n;
+    isInteractable(i) ? isTextInsertable(i) ? n = `[#${t}]` : i.tagName.toLowerCase() == "a" ? n = `[@${t}]` : n = `[$${t}]` : n = `[${t}]`;
     let e = document.createElement("span");
-    return e.id = tarsierId, e.style.position = "relative", e.style.display = "inline", e.style.color = "white", e.style.backgroundColor = "red", e.style.padding = "1.5px", e.style.borderRadius = "3px", e.style.fontWeight = "bold", e.style.fontSize = "15px", e.style.fontFamily = "Arial", e.style.margin = "1px", e.style.lineHeight = "1.25", e.style.letterSpacing = "2px", e.style.zIndex = "2140000046", e.style.clip = "auto", e.style.height = "fit-content", e.style.width = "fit-content", e.style.minHeight = "fit-content", e.style.minWidth = "fit-content", e.style.maxHeight = "unset", e.style.maxWidth = "unset", e.textContent = o, e.style.webkitTextFillColor = "white", e.style.textShadow = "", e.style.textDecoration = "none", e
+    return e.id = tarsierId, e.style.position = "relative", e.style.display = "inline", e.style.color = "white", e.style.backgroundColor = "red", e.style.padding = "1.5px", e.style.borderRadius = "3px", e.style.fontWeight = "bold", e.style.fontSize = "15px", e.style.fontFamily = "Arial", e.style.margin = "1px", e.style.lineHeight = "1.25", e.style.letterSpacing = "2px", e.style.zIndex = "2140000046", e.style.clip = "auto", e.style.height = "fit-content", e.style.width = "fit-content", e.style.minHeight = "fit-content", e.style.minWidth = "fit-content", e.style.maxHeight = "unset", e.style.maxWidth = "unset", e.textContent = n, e.style.webkitTextFillColor = "white", e.style.textShadow = "", e.style.textDecoration = "none", e
 }
 window.tagifyWebpage = (t = !1) => {
-    window.removeTags();
+    window.removeTags(), hideMapElements();
     let i = 0,
-        o = {},
+        n = {},
         e = [...document.body.querySelectorAll("*")];
-    const r = document.getElementsByTagName("iframe");
-    for (let n = 0; n < r.length; n++) try {
-        const s = r[n];
-        console.log("iframe!", r[n]);
-        const l = [...(s.contentDocument || s.contentWindow?.document).querySelectorAll("*")];
-        l.forEach(c => c.setAttribute("iframe_index", n)), e.push(...l)
-    } catch (s) {
-        console.error("Cross-origin iframe:", s)
+    const s = document.getElementsByTagName("iframe");
+    for (let o = 0; o < s.length; o++) try {
+        const a = s[o];
+        console.log("iframe!", s[o]);
+        const l = [...(a.contentDocument || a.contentWindow?.document).querySelectorAll("*")];
+        l.forEach(c => c.setAttribute("iframe_index", o)), e.push(...l)
+    } catch (a) {
+        console.error("Cross-origin iframe:", a)
     }
-    e.map(n => {
-        isInteractable(n) && (n.childNodes.forEach(s => {
-            const a = e.indexOf(s);
-            a > -1 && e.splice(a, 1)
-        }), n.querySelectorAll("*").forEach(s => {
-            const a = e.indexOf(s);
-            a > -1 && isInteractable(s) && e.splice(a, 1)
+    e.map(o => {
+        isInteractable(o) && (o.childNodes.forEach(a => {
+            const r = e.indexOf(a);
+            r > -1 && e.splice(r, 1)
+        }), o.querySelectorAll("*").forEach(a => {
+            const r = e.indexOf(a);
+            r > -1 && isInteractable(a) && e.splice(r, 1)
         }))
     });
-    for (let n of e)
-        if (!(isEmpty(n) || !elIsClean(n))) {
-            if (isInteractable(n)) o[i] = getElementXPath(n), i++;
+    for (let o of e)
+        if (!(isEmpty(o) || !elIsClean(o))) {
+            if (isInteractable(o)) n[i] = getElementXPath(o), i++;
             else if (t)
-                for (let s of Array.from(n.childNodes)) s.nodeType === Node.TEXT_NODE && /\S/.test(s.textContent || "") && (o[i] = getElementXPath(n), i++)
+                for (let a of Array.from(o.childNodes)) a.nodeType === Node.TEXT_NODE && /\S/.test(a.textContent || "") && (n[i] = getElementXPath(o), i++)
         } i = 0;
-    for (let n of e) {
-        if (isEmpty(n) || !elIsClean(n)) continue;
-        let s = create_tagged_span(i, n);
-        if (isInteractable(n)) isTextInsertable(n) && n.parentElement ? n.parentElement.insertBefore(s, n) : n.prepend(s), i++;
+    for (let o of e) {
+        if (isEmpty(o) || !elIsClean(o)) continue;
+        let a = create_tagged_span(i, o);
+        if (isInteractable(o)) isTextInsertable(o) && o.parentElement ? o.parentElement.insertBefore(a, o) : o.prepend(a), i++;
         else if (t) {
-            for (let a of Array.from(n.childNodes))
-                if (a.nodeType === Node.TEXT_NODE && /\S/.test(a.textContent || "")) {
-                    let l = create_tagged_span(i, n);
-                    n.insertBefore(l, a), i++
+            for (let r of Array.from(o.childNodes))
+                if (r.nodeType === Node.TEXT_NODE && /\S/.test(r.textContent || "")) {
+                    let l = create_tagged_span(i, o);
+                    o.insertBefore(l, r), i++
                 }
         }
     }
-    return absolutelyPositionMissingTags(), o
+    return absolutelyPositionMissingTags(), n
 };
 
 function absolutelyPositionMissingTags() {
-    document.querySelectorAll(tarsierSelector).forEach(o => {
-        const e = o.parentElement,
-            r = e.getBoundingClientRect(),
-            n = o.getBoundingClientRect(),
-            s = {
-                x: (r.left + r.right) / 2,
-                y: (r.top + r.bottom) / 2
-            },
+    document.querySelectorAll(tarsierSelector).forEach(n => {
+        const e = n.parentElement,
+            s = e.getBoundingClientRect(),
+            o = n.getBoundingClientRect(),
             a = {
-                x: (n.left + n.right) / 2,
-                y: (n.top + n.bottom) / 2
+                x: (s.left + s.right) / 2,
+                y: (s.top + s.bottom) / 2
+            },
+            r = {
+                x: (o.left + o.right) / 2,
+                y: (o.top + o.bottom) / 2
             },
-            l = Math.abs(s.x - a.x),
-            c = Math.abs(s.y - a.y);
-        if (l > 500 || c > 500 || !elIsClean(o)) {
-            o.style.position = "absolute";
-            let d = Math.max(0, r.left - (n.right + 3 - n.left));
-            d = Math.min(d, window.innerWidth - (n.right - n.left));
-            let f = Math.max(0, r.top + 3);
-            f = Math.min(f, Math.max(window.innerHeight, document.documentElement.scrollHeight) - (n.bottom - n.top)), o.style.left = `${d}px`, o.style.top = `${f}px`, e.removeChild(o), document.body.appendChild(o)
+            l = Math.abs(a.x - r.x),
+            c = Math.abs(a.y - r.y);
+        if (l > 500 || c > 500 || !elIsClean(n)) {
+            n.style.position = "absolute";
+            let d = Math.max(0, s.left - (o.right + 3 - o.left));
+            d = Math.min(d, window.innerWidth - (o.right - o.left));
+            let p = Math.max(0, s.top + 3);
+            p = Math.min(p, Math.max(window.innerHeight, document.documentElement.scrollHeight) - (o.bottom - o.top)), n.style.left = `${d}px`, n.style.top = `${p}px`, e.removeChild(n), document.body.appendChild(n)
         }
     })
 }
 window.removeTags = () => {
-    document.querySelectorAll(tarsierSelector).forEach(i => i.remove())
-};
+    document.querySelectorAll(tarsierSelector).forEach(i => i.remove()), showMapElements()
+};
+const GOOGLE_MAPS_OPACITY_CONTROL = "__reworkd_google_maps_opacity",
+    hideMapElements = () => {
+        const t = ['iframe[src*="google.com/maps"]', 'iframe[id*="gmap_canvas"]', ".maplibregl-map", ".mapboxgl-map", ".leaflet-container", 'img[src*="maps.googleapis.com"]', '[aria-label="Map"]', ".cmp-location-map__map", '.map-view[data-role="mapView"]', ".google_Map-wrapper", ".google_map-wrapper", ".googleMap-wrapper", ".googlemap-wrapper", ".ls-map-canvas", ".gmapcluster", "#googleMap", "#googleMaps", "#googlemaps", "#googlemap", "#google_map", "#google_maps", "#MapId", ".geolocation-map-wrapper", ".locatorMap"];
+        document.querySelectorAll(t.join(", ")).forEach(i => {
+            const n = window.getComputedStyle(i).opacity;
+            i.setAttribute("data-original-opacity", n), i.style.opacity = "0"
+        })
+    },
+    showMapElements = () => {
+        document.querySelectorAll(`[${GOOGLE_MAPS_OPACITY_CONTROL}]`).forEach(i => {
+            i.style.opacity = i.getAttribute("data-original-opacity") || "1"
+        })
+    };
```

### Comparing `tarsier-0.5.92/tarsier/text_format.py` & `tarsier-0.5.93/tarsier/text_format.py`

 * *Files identical despite different names*

### Comparing `tarsier-0.5.92/PKG-INFO` & `tarsier-0.5.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarsier
-Version: 0.5.92
+Version: 0.5.93
 Summary: Vision utilities for web interaction agents
 Author: Rohan Pandey
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-cloud-vision (>=3.4.5,<4.0.0)
```

