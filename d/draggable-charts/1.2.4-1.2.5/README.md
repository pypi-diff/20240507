# Comparing `tmp/draggable-charts-1.2.4.tar.gz` & `tmp/draggable-charts-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-charts-1.2.4.tar", last modified: Tue May  7 02:18:43 2024, max compression
+gzip compressed data, was "draggable-charts-1.2.5.tar", last modified: Tue May  7 03:21:34 2024, max compression
```

## Comparing `draggable-charts-1.2.4.tar` & `draggable-charts-1.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.931822 draggable-charts-1.2.4/
--rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.4/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6106 2024-05-07 02:18:43.929897 draggable-charts-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.848160 draggable-charts-1.2.4/draggable_charts/
--rw-rw-rw-   0        0        0       41 2024-05-07 02:17:05.000000 draggable-charts-1.2.4/draggable_charts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.829598 draggable-charts-1.2.4/draggable_charts/frontend/
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.876085 draggable-charts-1.2.4/draggable_charts/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-05-07 02:16:50.000000 draggable-charts-1.2.4/draggable_charts/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.4/draggable_charts/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-05-07 02:16:50.000000 draggable-charts-1.2.4/draggable_charts/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.830595 draggable-charts-1.2.4/draggable_charts/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.889051 draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/
--rw-rw-rw-   0        0        0   602564 2024-05-07 02:16:50.000000 draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/main.c3c91322.js
--rw-rw-rw-   0        0        0     1831 2024-05-07 02:16:50.000000 draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/main.c3c91322.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2574332 2024-05-07 02:16:50.000000 draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/main.c3c91322.js.map
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.908445 draggable-charts-1.2.4/draggable_charts/utils/
--rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.4/draggable_charts/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.4/draggable_charts/utils/callback.py
--rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.4/draggable_charts/utils/component_func.py
--rw-rw-rw-   0        0        0     2626 2024-05-06 23:57:39.000000 draggable-charts-1.2.4/draggable_charts/utils/options.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.926814 draggable-charts-1.2.4/draggable_charts/widgets/
--rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.4/draggable_charts/widgets/__init__.py
--rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.4/draggable_charts/widgets/bezierchart.py
--rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.4/draggable_charts/widgets/cubicbezierchart.py
--rw-rw-rw-   0        0        0     4720 2024-05-07 01:53:09.000000 draggable-charts-1.2.4/draggable_charts/widgets/linechart.py
--rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.4/draggable_charts/widgets/scatterchart.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:18:43.864117 draggable-charts-1.2.4/draggable_charts.egg-info/
--rw-rw-rw-   0        0        0     6106 2024-05-07 02:18:43.000000 draggable-charts-1.2.4/draggable_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2024-05-07 02:18:43.000000 draggable-charts-1.2.4/draggable_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 02:18:43.000000 draggable-charts-1.2.4/draggable_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-07 02:18:43.000000 draggable-charts-1.2.4/draggable_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 02:18:43.000000 draggable-charts-1.2.4/draggable_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 02:18:43.932799 draggable-charts-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1115 2024-05-07 02:18:22.000000 draggable-charts-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.190616 draggable-charts-1.2.5/
+-rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6106 2024-05-07 03:21:34.186322 draggable-charts-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:33.981090 draggable-charts-1.2.5/draggable_charts/
+-rw-rw-rw-   0        0        0       41 2024-05-07 03:18:24.000000 draggable-charts-1.2.5/draggable_charts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:33.934858 draggable-charts-1.2.5/draggable_charts/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.044910 draggable-charts-1.2.5/draggable_charts/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:33.936756 draggable-charts-1.2.5/draggable_charts/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.079817 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   604810 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js
+-rw-rw-rw-   0        0        0     1831 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2584548 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.map
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.128206 draggable-charts-1.2.5/draggable_charts/utils/
+-rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.5/draggable_charts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.5/draggable_charts/utils/callback.py
+-rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.5/draggable_charts/utils/component_func.py
+-rw-rw-rw-   0        0        0     2626 2024-05-06 23:57:39.000000 draggable-charts-1.2.5/draggable_charts/utils/options.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.175081 draggable-charts-1.2.5/draggable_charts/widgets/
+-rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.5/draggable_charts/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.5/draggable_charts/widgets/bezierchart.py
+-rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.5/draggable_charts/widgets/cubicbezierchart.py
+-rw-rw-rw-   0        0        0     4720 2024-05-07 01:53:09.000000 draggable-charts-1.2.5/draggable_charts/widgets/linechart.py
+-rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.5/draggable_charts/widgets/scatterchart.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.015988 draggable-charts-1.2.5/draggable_charts.egg-info/
+-rw-rw-rw-   0        0        0     6106 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:21:34.192626 draggable-charts-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2024-05-07 03:20:13.000000 draggable-charts-1.2.5/setup.py
```

### Comparing `draggable-charts-1.2.4/LICENSE` & `draggable-charts-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/PKG-INFO` & `draggable-charts-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.2.4/README.md` & `draggable-charts-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/frontend/build/bootstrap.min.css` & `draggable-charts-1.2.5/draggable_charts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/main.c3c91322.js` & `draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.c3c91322.js.LICENSE.txt */
+/*! For license information please see main.41dd267d.js.LICENSE.txt */
 (() => {
     var e = {
             895: (t, e, n) => {
                 var i;
                 ! function(r, s, o, a) {
                     "use strict";
                     var l, c = ["", "webkit", "Moz", "MS", "ms", "o"],
@@ -147,18 +147,18 @@
                         V = 25,
                         j = 1,
                         W = 4,
                         H = 8,
                         Y = 1,
                         $ = 2,
                         X = 4,
-                        q = 8,
-                        K = 16,
+                        K = 8,
+                        q = 16,
                         Q = $ | X,
-                        G = q | K,
+                        G = K | q,
                         Z = Q | G,
                         J = ["x", "y"],
                         tt = ["clientX", "clientY"];
 
                     function et(t, e) {
                         var n = this;
                         this.manager = t, this.callback = e, this.element = t.element, this.target = t.options.inputTarget, this.domHandler = function(e) {
@@ -250,15 +250,15 @@
                         return {
                             x: e / t || 0,
                             y: n / t || 0
                         }
                     }
 
                     function ot(t, e) {
-                        return t === e ? Y : f(t) >= f(e) ? t < 0 ? $ : X : e < 0 ? q : K
+                        return t === e ? Y : f(t) >= f(e) ? t < 0 ? $ : X : e < 0 ? K : q
                     }
 
                     function at(t, e, n) {
                         n || (n = J);
                         var i = e[n[0]] - t[n[0]],
                             r = e[n[1]] - t[n[1]];
                         return Math.sqrt(i * i + r * r)
@@ -528,15 +528,15 @@
                     }
 
                     function Wt(t) {
                         return 16 & t ? "cancel" : 8 & t ? "end" : 4 & t ? "move" : 2 & t ? "start" : ""
                     }
 
                     function Ht(t) {
-                        return t == K ? "down" : t == q ? "up" : t == $ ? "left" : t == X ? "right" : ""
+                        return t == q ? "down" : t == K ? "up" : t == $ ? "left" : t == X ? "right" : ""
                     }
 
                     function Yt(t, e) {
                         var n = e.manager;
                         return n ? n.get(t) : t
                     }
 
@@ -544,19 +544,19 @@
                         jt.apply(this, arguments)
                     }
 
                     function Xt() {
                         $t.apply(this, arguments), this.pX = null, this.pY = null
                     }
 
-                    function qt() {
+                    function Kt() {
                         $t.apply(this, arguments)
                     }
 
-                    function Kt() {
+                    function qt() {
                         jt.apply(this, arguments), this._timer = null, this._input = null
                     }
 
                     function Qt() {
                         $t.apply(this, arguments)
                     }
 
@@ -659,25 +659,25 @@
                         directionTest: function(t) {
                             var e = this.options,
                                 n = !0,
                                 i = t.distance,
                                 r = t.direction,
                                 s = t.deltaX,
                                 o = t.deltaY;
-                            return r & e.direction || (e.direction & Q ? (r = 0 === s ? Y : s < 0 ? $ : X, n = s != this.pX, i = Math.abs(t.deltaX)) : (r = 0 === o ? Y : o < 0 ? q : K, n = o != this.pY, i = Math.abs(t.deltaY))), t.direction = r, n && i > e.threshold && r & e.direction
+                            return r & e.direction || (e.direction & Q ? (r = 0 === s ? Y : s < 0 ? $ : X, n = s != this.pX, i = Math.abs(t.deltaX)) : (r = 0 === o ? Y : o < 0 ? K : q, n = o != this.pY, i = Math.abs(t.deltaY))), t.direction = r, n && i > e.threshold && r & e.direction
                         },
                         attrTest: function(t) {
                             return $t.prototype.attrTest.call(this, t) && (2 & this.state || !(2 & this.state) && this.directionTest(t))
                         },
                         emit: function(t) {
                             this.pX = t.deltaX, this.pY = t.deltaY;
                             var e = Ht(t.direction);
                             e && (t.additionalEvent = this.options.event + e), this._super.emit.call(this, t)
                         }
-                    }), _(qt, $t, {
+                    }), _(Kt, $t, {
                         defaults: {
                             event: "pinch",
                             threshold: 0,
                             pointers: 2
                         },
                         getTouchAction: function() {
                             return [Lt]
@@ -688,15 +688,15 @@
                         emit: function(t) {
                             if (1 !== t.scale) {
                                 var e = t.scale < 1 ? "in" : "out";
                                 t.additionalEvent = this.options.event + e
                             }
                             this._super.emit.call(this, t)
                         }
-                    }), _(Kt, jt, {
+                    }), _(qt, jt, {
                         defaults: {
                             event: "press",
                             pointers: 1,
                             time: 251,
                             threshold: 9
                         },
                         getTouchAction: function() {
@@ -797,15 +797,15 @@
                         enable: !0,
                         inputTarget: null,
                         inputClass: null,
                         preset: [
                             [Qt, {
                                 enable: !1
                             }],
-                            [qt, {
+                            [Kt, {
                                     enable: !1
                                 },
                                 ["rotate"]
                             ],
                             [Gt, {
                                 direction: Q
                             }],
@@ -817,15 +817,15 @@
                             [Zt],
                             [Zt, {
                                     event: "doubletap",
                                     taps: 2
                                 },
                                 ["tap"]
                             ],
-                            [Kt]
+                            [qt]
                         ],
                         cssProps: {
                             userSelect: "none",
                             touchSelect: "none",
                             touchCallout: "none",
                             contentZooming: "none",
                             userDrag: "none",
@@ -927,16 +927,16 @@
                         STATE_ENDED: 8,
                         STATE_RECOGNIZED: 8,
                         STATE_CANCELLED: 16,
                         STATE_FAILED: Vt,
                         DIRECTION_NONE: Y,
                         DIRECTION_LEFT: $,
                         DIRECTION_RIGHT: X,
-                        DIRECTION_UP: q,
-                        DIRECTION_DOWN: K,
+                        DIRECTION_UP: K,
+                        DIRECTION_DOWN: q,
                         DIRECTION_HORIZONTAL: Q,
                         DIRECTION_VERTICAL: G,
                         DIRECTION_ALL: Z,
                         Manager: te,
                         Input: et,
                         TouchAction: Rt,
                         TouchInput: St,
@@ -945,17 +945,17 @@
                         TouchMouseInput: Mt,
                         SingleTouchInput: vt,
                         Recognizer: jt,
                         AttrRecognizer: $t,
                         Tap: Zt,
                         Pan: Xt,
                         Swipe: Gt,
-                        Pinch: qt,
+                        Pinch: Kt,
                         Rotate: Qt,
-                        Press: Kt,
+                        Press: qt,
                         on: k,
                         off: M,
                         each: y,
                         merge: x,
                         extend: v,
                         assign: l,
                         inherit: _,
@@ -1034,14 +1034,93 @@
                                 } catch (v) {}
                             }
                         }
                     }
                     return e
                 }
             },
+            373: (t, e, n) => {
+                "use strict";
+                const i = n(359),
+                    r = n(176),
+                    s = 1e3;
+
+                function* o(t) {
+                    let e = s;
+                    for (;;) {
+                        const n = t / e;
+                        if (n < 1) return;
+                        yield n, e *= s
+                    }
+                }
+
+                function a(t, e) {
+                    var n, s;
+                    const a = e ? {
+                        ...i.defaultOptions,
+                        ...e
+                    } : i.defaultOptions;
+                    if (!Array.isArray(a.units) || !a.units.length) throw new Error("Option `units` must be a non-empty array");
+                    let l;
+                    try {
+                        l = r.parseValue(t)
+                    } catch (m) {
+                        return m instanceof Error && console.warn("WARN: ".concat(m.message, " (millify)")), String(t)
+                    }
+                    const c = l < 0 ? "-" : "";
+                    l = Math.abs(l);
+                    let u = 0;
+                    for (const i of o(l)) l = i, u += 1;
+                    if (u >= a.units.length) return t.toString();
+                    let h = r.roundTo(l, a.precision);
+                    for (const i of o(h)) h = i, u += 1;
+                    const d = null !== (n = a.units[u]) && void 0 !== n ? n : "",
+                        f = a.lowercase ? d.toLowerCase() : d,
+                        p = a.space ? " " : "",
+                        g = h.toLocaleString(null !== (s = a.locales) && void 0 !== s ? s : r.getLocales(), {
+                            minimumFractionDigits: r.getFractionDigits(h)
+                        });
+                    return "".concat(c).concat(g).concat(p).concat(f)
+                }
+                e.Ay = a
+            },
+            359: (t, e) => {
+                "use strict";
+                Object.defineProperty(e, "__esModule", {
+                    value: !0
+                }), e.defaultOptions = void 0, e.defaultOptions = {
+                    lowercase: !1,
+                    precision: 1,
+                    space: !1,
+                    units: ["", "K", "M", "B", "T", "P", "E"]
+                }
+            },
+            176: (t, e) => {
+                "use strict";
+                Object.defineProperty(e, "__esModule", {
+                    value: !0
+                }), e.getLocales = e.getFractionDigits = e.roundTo = e.parseValue = void 0, e.parseValue = function(t) {
+                    const e = parseFloat(null === t || void 0 === t ? void 0 : t.toString());
+                    if (isNaN(e)) throw new Error("Input value is not a number");
+                    if (e > Number.MAX_SAFE_INTEGER || e < Number.MIN_SAFE_INTEGER) throw new RangeError("Input value is outside of safe integer range");
+                    return e
+                }, e.roundTo = function(t, e) {
+                    if (!Number.isFinite(t)) throw new Error("Input value is not a finite number");
+                    if (!Number.isInteger(e) || e < 0) throw new Error("Precision is not a positive integer");
+                    return Number.isInteger(t) ? t : parseFloat(t.toFixed(e))
+                }, e.getFractionDigits = function(t) {
+                    var e;
+                    if (Number.isInteger(t)) return 0;
+                    const n = t.toString().split(".")[1];
+                    return null !== (e = null === n || void 0 === n ? void 0 : n.length) && void 0 !== e ? e : 0
+                }, e.getLocales = function() {
+                    var t;
+                    return "undefined" === typeof navigator ? [] : Array.from(null !== (t = navigator.languages) && void 0 !== t ? t : [])
+                }
+            },
             123: t => {
                 "use strict";
                 var e = Object.getOwnPropertySymbols,
                     n = Object.prototype.hasOwnProperty,
                     i = Object.prototype.propertyIsEnumerable;
                 t.exports = function() {
                     try {
@@ -1252,27 +1331,27 @@
                 })), ["capture", "download"].forEach((function(t) {
                     X[t] = new $(t, 4, !1, t, null, !1)
                 })), ["cols", "rows", "size", "span"].forEach((function(t) {
                     X[t] = new $(t, 6, !1, t, null, !1)
                 })), ["rowSpan", "start"].forEach((function(t) {
                     X[t] = new $(t, 5, !1, t.toLowerCase(), null, !1)
                 }));
-                var q = /[\-:]([a-z])/g;
+                var K = /[\-:]([a-z])/g;
 
-                function K(t) {
+                function q(t) {
                     return t[1].toUpperCase()
                 }
                 "accent-height alignment-baseline arabic-form baseline-shift cap-height clip-path clip-rule color-interpolation color-interpolation-filters color-profile color-rendering dominant-baseline enable-background fill-opacity fill-rule flood-color flood-opacity font-family font-size font-size-adjust font-stretch font-style font-variant font-weight glyph-name glyph-orientation-horizontal glyph-orientation-vertical horiz-adv-x horiz-origin-x image-rendering letter-spacing lighting-color marker-end marker-mid marker-start overline-position overline-thickness paint-order panose-1 pointer-events rendering-intent shape-rendering stop-color stop-opacity strikethrough-position strikethrough-thickness stroke-dasharray stroke-dashoffset stroke-linecap stroke-linejoin stroke-miterlimit stroke-opacity stroke-width text-anchor text-decoration text-rendering underline-position underline-thickness unicode-bidi unicode-range units-per-em v-alphabetic v-hanging v-ideographic v-mathematical vector-effect vert-adv-y vert-origin-x vert-origin-y word-spacing writing-mode xmlns:xlink x-height".split(" ").forEach((function(t) {
-                    var e = t.replace(q, K);
+                    var e = t.replace(K, q);
                     X[e] = new $(e, 1, !1, t, null, !1)
                 })), "xlink:actuate xlink:arcrole xlink:role xlink:show xlink:title xlink:type".split(" ").forEach((function(t) {
-                    var e = t.replace(q, K);
+                    var e = t.replace(K, q);
                     X[e] = new $(e, 1, !1, t, "http://www.w3.org/1999/xlink", !1)
                 })), ["xml:base", "xml:lang", "xml:space"].forEach((function(t) {
-                    var e = t.replace(q, K);
+                    var e = t.replace(K, q);
                     X[e] = new $(e, 1, !1, t, "http://www.w3.org/XML/1998/namespace", !1)
                 })), ["tabIndex", "crossOrigin"].forEach((function(t) {
                     X[t] = new $(t, 1, !1, t.toLowerCase(), null, !1)
                 })), X.xlinkHref = new $("xlinkHref", 1, !1, "xlink:href", "http://www.w3.org/1999/xlink", !0), ["src", "href", "action", "formAction"].forEach((function(t) {
                     X[t] = new $(t, 1, !1, t.toLowerCase(), null, !0)
                 }));
                 var Q = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED;
@@ -1619,16 +1698,16 @@
                     var e, n = Wt[t];
                     for (e in n)
                         if (n.hasOwnProperty(e) && e in Yt) return Ht[t] = n[e];
                     return t
                 }
                 I && (Yt = document.createElement("div").style, "AnimationEvent" in window || (delete Wt.animationend.animation, delete Wt.animationiteration.animation, delete Wt.animationstart.animation), "TransitionEvent" in window || delete Wt.transitionend.transition);
                 var Xt = $t("animationend"),
-                    qt = $t("animationiteration"),
-                    Kt = $t("animationstart"),
+                    Kt = $t("animationiteration"),
+                    qt = $t("animationstart"),
                     Qt = $t("transitionend"),
                     Gt = "abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),
                     Zt = new("function" === typeof WeakMap ? WeakMap : Map);
 
                 function Jt(t) {
                     var e = Zt.get(t);
                     return void 0 === e && (e = new Map, Zt.set(t, e)), e
@@ -1823,30 +1902,30 @@
                     }
                 }
 
                 function ge(t, e, n) {
                     if (!n.has(t)) {
                         switch (t) {
                             case "scroll":
-                                Ke(e, "scroll", !0);
+                                qe(e, "scroll", !0);
                                 break;
                             case "focus":
                             case "blur":
-                                Ke(e, "focus", !0), Ke(e, "blur", !0), n.set("blur", null), n.set("focus", null);
+                                qe(e, "focus", !0), qe(e, "blur", !0), n.set("blur", null), n.set("focus", null);
                                 break;
                             case "cancel":
                             case "close":
-                                ue(t) && Ke(e, t, !0);
+                                ue(t) && qe(e, t, !0);
                                 break;
                             case "invalid":
                             case "submit":
                             case "reset":
                                 break;
                             default:
-                                -1 === Gt.indexOf(t) && qe(t, e)
+                                -1 === Gt.indexOf(t) && Ke(t, e)
                         }
                         n.set(t, null)
                     }
                 }
                 var me, ye, be, ve = !1,
                     xe = [],
                     _e = null,
@@ -1954,15 +2033,15 @@
                     }
                     for (null !== _e && ze(_e, t), null !== we && ze(we, t), null !== Se && ze(Se, t), Te.forEach(e), ke.forEach(e), n = 0; n < Me.length; n++)(i = Me[n]).blockedOn === t && (i.blockedOn = null);
                     for (; 0 < Me.length && null === (n = Me[0]).blockedOn;) Ae(n), null === n.blockedOn && Me.shift()
                 }
                 var Be = {},
                     Re = new Map,
                     Ue = new Map,
-                    Ve = ["abort", "abort", Xt, "animationEnd", qt, "animationIteration", Kt, "animationStart", "canplay", "canPlay", "canplaythrough", "canPlayThrough", "durationchange", "durationChange", "emptied", "emptied", "encrypted", "encrypted", "ended", "ended", "error", "error", "gotpointercapture", "gotPointerCapture", "load", "load", "loadeddata", "loadedData", "loadedmetadata", "loadedMetadata", "loadstart", "loadStart", "lostpointercapture", "lostPointerCapture", "playing", "playing", "progress", "progress", "seeking", "seeking", "stalled", "stalled", "suspend", "suspend", "timeupdate", "timeUpdate", Qt, "transitionEnd", "waiting", "waiting"];
+                    Ve = ["abort", "abort", Xt, "animationEnd", Kt, "animationIteration", qt, "animationStart", "canplay", "canPlay", "canplaythrough", "canPlayThrough", "durationchange", "durationChange", "emptied", "emptied", "encrypted", "encrypted", "ended", "ended", "error", "error", "gotpointercapture", "gotPointerCapture", "load", "load", "loadeddata", "loadedData", "loadedmetadata", "loadedMetadata", "loadstart", "loadStart", "lostpointercapture", "lostPointerCapture", "playing", "playing", "progress", "progress", "seeking", "seeking", "stalled", "stalled", "suspend", "suspend", "timeupdate", "timeUpdate", Qt, "transitionEnd", "waiting", "waiting"];
 
                 function je(t, e) {
                     for (var n = 0; n < t.length; n += 2) {
                         var i = t[n],
                             r = t[n + 1],
                             s = "on" + (r[0].toUpperCase() + r.slice(1));
                         s = {
@@ -1977,19 +2056,19 @@
                 }
                 je("blur blur cancel cancel click click close close contextmenu contextMenu copy copy cut cut auxclick auxClick dblclick doubleClick dragend dragEnd dragstart dragStart drop drop focus focus input input invalid invalid keydown keyDown keypress keyPress keyup keyUp mousedown mouseDown mouseup mouseUp paste paste pause pause play play pointercancel pointerCancel pointerdown pointerDown pointerup pointerUp ratechange rateChange reset reset seeked seeked submit submit touchcancel touchCancel touchend touchEnd touchstart touchStart volumechange volumeChange".split(" "), 0), je("drag drag dragenter dragEnter dragexit dragExit dragleave dragLeave dragover dragOver mousemove mouseMove mouseout mouseOut mouseover mouseOver pointermove pointerMove pointerout pointerOut pointerover pointerOver scroll scroll toggle toggle touchmove touchMove wheel wheel".split(" "), 1), je(Ve, 2);
                 for (var We = "change selectionchange textInput compositionstart compositionend compositionupdate".split(" "), He = 0; He < We.length; He++) Ue.set(We[He], 0);
                 var Ye = s.unstable_UserBlockingPriority,
                     $e = s.unstable_runWithPriority,
                     Xe = !0;
 
-                function qe(t, e) {
-                    Ke(e, t, !1)
+                function Ke(t, e) {
+                    qe(e, t, !1)
                 }
 
-                function Ke(t, e, n) {
+                function qe(t, e, n) {
                     var i = Ue.get(e);
                     switch (void 0 === i ? 2 : i) {
                         case 0:
                             i = Qe.bind(null, e, 1, t);
                             break;
                         case 1:
                             i = Ge.bind(null, e, 1, t);
@@ -2402,25 +2481,25 @@
                         s = r.length;
                     for (t = 0; t < i && n[t] === r[t]; t++);
                     var o = i - t;
                     for (e = 1; e <= o && n[i - e] === r[s - e]; e++);
                     return $n = r.slice(t, 1 < e ? 1 - e : void 0)
                 }
 
-                function qn() {
+                function Kn() {
                     return !0
                 }
 
-                function Kn() {
+                function qn() {
                     return !1
                 }
 
                 function Qn(t, e, n, i) {
                     for (var r in this.dispatchConfig = t, this._targetInst = e, this.nativeEvent = n, t = this.constructor.Interface) t.hasOwnProperty(r) && ((e = t[r]) ? this[r] = e(n) : "target" === r ? this.target = i : this[r] = n[r]);
-                    return this.isDefaultPrevented = (null != n.defaultPrevented ? n.defaultPrevented : !1 === n.returnValue) ? qn : Kn, this.isPropagationStopped = Kn, this
+                    return this.isDefaultPrevented = (null != n.defaultPrevented ? n.defaultPrevented : !1 === n.returnValue) ? Kn : qn, this.isPropagationStopped = qn, this
                 }
 
                 function Gn(t, e, n, i) {
                     if (this.eventPool.length) {
                         var r = this.eventPool.pop();
                         return this.call(r, t, e, n, i), r
                     }
@@ -2435,28 +2514,28 @@
                 function Jn(t) {
                     t.eventPool = [], t.getPooled = Gn, t.release = Zn
                 }
                 r(Qn.prototype, {
                     preventDefault: function() {
                         this.defaultPrevented = !0;
                         var t = this.nativeEvent;
-                        t && (t.preventDefault ? t.preventDefault() : "unknown" !== typeof t.returnValue && (t.returnValue = !1), this.isDefaultPrevented = qn)
+                        t && (t.preventDefault ? t.preventDefault() : "unknown" !== typeof t.returnValue && (t.returnValue = !1), this.isDefaultPrevented = Kn)
                     },
                     stopPropagation: function() {
                         var t = this.nativeEvent;
-                        t && (t.stopPropagation ? t.stopPropagation() : "unknown" !== typeof t.cancelBubble && (t.cancelBubble = !0), this.isPropagationStopped = qn)
+                        t && (t.stopPropagation ? t.stopPropagation() : "unknown" !== typeof t.cancelBubble && (t.cancelBubble = !0), this.isPropagationStopped = Kn)
                     },
                     persist: function() {
-                        this.isPersistent = qn
+                        this.isPersistent = Kn
                     },
-                    isPersistent: Kn,
+                    isPersistent: qn,
                     destructor: function() {
                         var t, e = this.constructor.Interface;
                         for (t in e) this[t] = null;
-                        this.nativeEvent = this._targetInst = this.dispatchConfig = null, this.isPropagationStopped = this.isDefaultPrevented = Kn, this._dispatchInstances = this._dispatchListeners = null
+                        this.nativeEvent = this._targetInst = this.dispatchConfig = null, this.isPropagationStopped = this.isDefaultPrevented = qn, this._dispatchInstances = this._dispatchListeners = null
                     }
                 }), Qn.Interface = {
                     type: null,
                     target: null,
                     currentTarget: function() {
                         return null
                     },
@@ -2829,30 +2908,30 @@
                             phasedRegistrationNames: {
                                 bubbled: "onSelect",
                                 captured: "onSelectCapture"
                             },
                             dependencies: "blur contextmenu dragend focus keydown keyup mousedown mouseup selectionchange".split(" ")
                         }
                     },
-                    qi = null,
                     Ki = null,
+                    qi = null,
                     Qi = null,
                     Gi = !1;
 
                 function Zi(t, e) {
                     var n = e.window === e ? e.document : 9 === e.nodeType ? e : e.ownerDocument;
-                    return Gi || null == qi || qi !== hn(n) ? null : ("selectionStart" in (n = qi) && mn(n) ? n = {
+                    return Gi || null == Ki || Ki !== hn(n) ? null : ("selectionStart" in (n = Ki) && mn(n) ? n = {
                         start: n.selectionStart,
                         end: n.selectionEnd
                     } : n = {
                         anchorNode: (n = (n.ownerDocument && n.ownerDocument.defaultView || window).getSelection()).anchorNode,
                         anchorOffset: n.anchorOffset,
                         focusNode: n.focusNode,
                         focusOffset: n.focusOffset
-                    }, Qi && Yi(Qi, n) ? null : (Qi = n, (t = Qn.getPooled(Xi.select, Ki, t, e)).type = "select", t.target = qi, Wn(t), t))
+                    }, Qi && Yi(Qi, n) ? null : (Qi = n, (t = Qn.getPooled(Xi.select, qi, t, e)).type = "select", t.target = Ki, Wn(t), t))
                 }
                 var Ji = {
                         eventTypes: Xi,
                         extractEvents: function(t, e, n, i, r, s) {
                             if (!(s = !(r = s || (i.window === i ? i.document : 9 === i.nodeType ? i : i.ownerDocument)))) {
                                 t: {
                                     r = Jt(r),
@@ -2864,18 +2943,18 @@
                                         } r = !0
                                 }
                                 s = !r
                             }
                             if (s) return null;
                             switch (r = e ? Ln(e) : window, t) {
                                 case "focus":
-                                    (gi(r) || "true" === r.contentEditable) && (qi = r, Ki = e, Qi = null);
+                                    (gi(r) || "true" === r.contentEditable) && (Ki = r, qi = e, Qi = null);
                                     break;
                                 case "blur":
-                                    Qi = Ki = qi = null;
+                                    Qi = qi = Ki = null;
                                     break;
                                 case "mousedown":
                                     Gi = !0;
                                     break;
                                 case "contextmenu":
                                 case "mouseup":
                                 case "dragend":
@@ -3054,16 +3133,16 @@
                                 case "touchcancel":
                                 case "touchend":
                                 case "touchmove":
                                 case "touchstart":
                                     t = lr;
                                     break;
                                 case Xt:
-                                case qt:
                                 case Kt:
+                                case qt:
                                     t = tr;
                                     break;
                                 case Qt:
                                     t = cr;
                                     break;
                                 case "scroll":
                                     t = Ci;
@@ -3211,19 +3290,19 @@
                         case 95:
                             return Nr;
                         default:
                             throw Error(o(332))
                     }
                 }
 
-                function qr(t, e) {
+                function Kr(t, e) {
                     return t = Xr(t), Ir(t, e)
                 }
 
-                function Kr(t, e, n) {
+                function qr(t, e, n) {
                     return t = Xr(t), Er(t, e, n)
                 }
 
                 function Qr(t) {
                     return null === Vr ? (Vr = [t], jr = Er(Pr, Zr)) : Vr.push(t), Br
                 }
 
@@ -3237,15 +3316,15 @@
 
                 function Zr() {
                     if (!Wr && null !== Vr) {
                         Wr = !0;
                         var t = 0;
                         try {
                             var e = Vr;
-                            qr(99, (function() {
+                            Kr(99, (function() {
                                 for (; t < e.length; t++) {
                                     var n = e[t];
                                     do {
                                         n = n(!0)
                                     } while (null !== n)
                                 }
                             })), Vr = null
@@ -3785,16 +3864,16 @@
                         props: e
                     }
                 }
                 var Hs = Q.ReactCurrentDispatcher,
                     Ys = Q.ReactCurrentBatchConfig,
                     $s = 0,
                     Xs = null,
-                    qs = null,
                     Ks = null,
+                    qs = null,
                     Qs = !1;
 
                 function Gs() {
                     throw Error(o(321))
                 }
 
                 function Zs(t, e) {
@@ -3805,62 +3884,62 @@
                 }
 
                 function Js(t, e, n, i, r, s) {
                     if ($s = s, Xs = e, e.memoizedState = null, e.updateQueue = null, e.expirationTime = 0, Hs.current = null === t || null === t.memoizedState ? So : To, t = n(i, r), e.expirationTime === $s) {
                         s = 0;
                         do {
                             if (e.expirationTime = 0, !(25 > s)) throw Error(o(301));
-                            s += 1, Ks = qs = null, e.updateQueue = null, Hs.current = ko, t = n(i, r)
+                            s += 1, qs = Ks = null, e.updateQueue = null, Hs.current = ko, t = n(i, r)
                         } while (e.expirationTime === $s)
                     }
-                    if (Hs.current = wo, e = null !== qs && null !== qs.next, $s = 0, Ks = qs = Xs = null, Qs = !1, e) throw Error(o(300));
+                    if (Hs.current = wo, e = null !== Ks && null !== Ks.next, $s = 0, qs = Ks = Xs = null, Qs = !1, e) throw Error(o(300));
                     return t
                 }
 
                 function to() {
                     var t = {
                         memoizedState: null,
                         baseState: null,
                         baseQueue: null,
                         queue: null,
                         next: null
                     };
-                    return null === Ks ? Xs.memoizedState = Ks = t : Ks = Ks.next = t, Ks
+                    return null === qs ? Xs.memoizedState = qs = t : qs = qs.next = t, qs
                 }
 
                 function eo() {
-                    if (null === qs) {
+                    if (null === Ks) {
                         var t = Xs.alternate;
                         t = null !== t ? t.memoizedState : null
-                    } else t = qs.next;
-                    var e = null === Ks ? Xs.memoizedState : Ks.next;
-                    if (null !== e) Ks = e, qs = t;
+                    } else t = Ks.next;
+                    var e = null === qs ? Xs.memoizedState : qs.next;
+                    if (null !== e) qs = e, Ks = t;
                     else {
                         if (null === t) throw Error(o(310));
                         t = {
-                            memoizedState: (qs = t).memoizedState,
-                            baseState: qs.baseState,
-                            baseQueue: qs.baseQueue,
-                            queue: qs.queue,
+                            memoizedState: (Ks = t).memoizedState,
+                            baseState: Ks.baseState,
+                            baseQueue: Ks.baseQueue,
+                            queue: Ks.queue,
                             next: null
-                        }, null === Ks ? Xs.memoizedState = Ks = t : Ks = Ks.next = t
+                        }, null === qs ? Xs.memoizedState = qs = t : qs = qs.next = t
                     }
-                    return Ks
+                    return qs
                 }
 
                 function no(t, e) {
                     return "function" === typeof e ? e(t) : e
                 }
 
                 function io(t) {
                     var e = eo(),
                         n = e.queue;
                     if (null === n) throw Error(o(311));
                     n.lastRenderedReducer = t;
-                    var i = qs,
+                    var i = Ks,
                         r = i.baseQueue,
                         s = n.pending;
                     if (null !== s) {
                         if (null !== r) {
                             var a = r.next;
                             r.next = s.next, s.next = a
                         }
@@ -3947,16 +4026,16 @@
                     Xs.effectTag |= t, r.memoizedState = oo(1 | e, n, void 0, void 0 === i ? null : i)
                 }
 
                 function co(t, e, n, i) {
                     var r = eo();
                     i = void 0 === i ? null : i;
                     var s = void 0;
-                    if (null !== qs) {
-                        var o = qs.memoizedState;
+                    if (null !== Ks) {
+                        var o = Ks.memoizedState;
                         if (s = o.destroy, null !== i && Zs(i, o.deps)) return void oo(e, n, s, i)
                     }
                     Xs.effectTag |= t, r.memoizedState = oo(1 | e, n, s, i)
                 }
 
                 function uo(t, e) {
                     return lo(516, 4, t, e)
@@ -4000,17 +4079,17 @@
                     e = void 0 === e ? null : e;
                     var i = n.memoizedState;
                     return null !== i && null !== e && Zs(e, i[1]) ? i[0] : (t = t(), n.memoizedState = [t, e], t)
                 }
 
                 function xo(t, e, n) {
                     var i = $r();
-                    qr(98 > i ? 98 : i, (function() {
+                    Kr(98 > i ? 98 : i, (function() {
                         t(!0)
-                    })), qr(97 < i ? 97 : i, (function() {
+                    })), Kr(97 < i ? 97 : i, (function() {
                         var i = Ys.suspense;
                         Ys.suspense = void 0 === e ? null : e;
                         try {
                             t(!1), n()
                         } finally {
                             Ys.suspense = i
                         }
@@ -4314,15 +4393,15 @@
                     return e.effectTag |= 1, null !== t && o ? (e.child = Os(e, t.child, null, s), e.child = Os(e, null, a, s)) : No(t, e, a, s), e.memoizedState = i.state, r && Mr(e, n, !0), e.child
                 }
 
                 function Yo(t) {
                     var e = t.stateNode;
                     e.pendingContext ? Sr(0, e.pendingContext, e.pendingContext !== e.context) : e.context && Sr(0, e.context, !1), Ns(t, e.containerInfo)
                 }
-                var $o, Xo, qo, Ko, Qo = {
+                var $o, Xo, Ko, qo, Qo = {
                     dehydrated: null,
                     retryTime: 0
                 };
 
                 function Go(t, e, n) {
                     var i, r = e.mode,
                         s = e.pendingProps,
@@ -4463,57 +4542,57 @@
                         case 17:
                             return _r(e.type) && wr(), null;
                         case 3:
                             return Bs(), pr(br), pr(yr), (n = e.stateNode).pendingContext && (n.context = n.pendingContext, n.pendingContext = null), null !== t && null !== t.child || !Po(e) || (e.effectTag |= 4), Xo(e), null;
                         case 5:
                             Us(e), n = zs(Ls.current);
                             var s = e.type;
-                            if (null !== t && null != e.stateNode) qo(t, e, s, i, n), t.ref !== e.ref && (e.effectTag |= 128);
+                            if (null !== t && null != e.stateNode) Ko(t, e, s, i, n), t.ref !== e.ref && (e.effectTag |= 128);
                             else {
                                 if (!i) {
                                     if (null === e.stateNode) throw Error(o(166));
                                     return null
                                 }
                                 if (t = zs(Ps.current), Po(e)) {
                                     i = e.stateNode, s = e.type;
                                     var a = e.memoizedProps;
                                     switch (i[On] = e, i[Cn] = a, s) {
                                         case "iframe":
                                         case "object":
                                         case "embed":
-                                            qe("load", i);
+                                            Ke("load", i);
                                             break;
                                         case "video":
                                         case "audio":
-                                            for (t = 0; t < Gt.length; t++) qe(Gt[t], i);
+                                            for (t = 0; t < Gt.length; t++) Ke(Gt[t], i);
                                             break;
                                         case "source":
-                                            qe("error", i);
+                                            Ke("error", i);
                                             break;
                                         case "img":
                                         case "image":
                                         case "link":
-                                            qe("error", i), qe("load", i);
+                                            Ke("error", i), Ke("load", i);
                                             break;
                                         case "form":
-                                            qe("reset", i), qe("submit", i);
+                                            Ke("reset", i), Ke("submit", i);
                                             break;
                                         case "details":
-                                            qe("toggle", i);
+                                            Ke("toggle", i);
                                             break;
                                         case "input":
-                                            St(i, a), qe("invalid", i), cn(n, "onChange");
+                                            St(i, a), Ke("invalid", i), cn(n, "onChange");
                                             break;
                                         case "select":
                                             i._wrapperState = {
                                                 wasMultiple: !!a.multiple
-                                            }, qe("invalid", i), cn(n, "onChange");
+                                            }, Ke("invalid", i), cn(n, "onChange");
                                             break;
                                         case "textarea":
-                                            Ct(i, a), qe("invalid", i), cn(n, "onChange")
+                                            Ct(i, a), Ke("invalid", i), cn(n, "onChange")
                                     }
                                     for (var l in on(s, a), t = null, a)
                                         if (a.hasOwnProperty(l)) {
                                             var c = a[l];
                                             "children" === l ? "string" === typeof c ? i.textContent !== c && (t = ["children", c]) : "number" === typeof c && i.textContent !== "" + c && (t = ["children", "" + c]) : T.hasOwnProperty(l) && null != c && cn(n, l)
                                         } switch (s) {
                                         case "input":
@@ -4532,50 +4611,50 @@
                                 } else {
                                     switch (l = 9 === n.nodeType ? n : n.ownerDocument, t === ln && (t = zt(s)), t === ln ? "script" === s ? ((t = l.createElement("div")).innerHTML = "<script><\/script>", t = t.removeChild(t.firstChild)) : "string" === typeof i.is ? t = l.createElement(s, {
                                             is: i.is
                                         }) : (t = l.createElement(s), "select" === s && (l = t, i.multiple ? l.multiple = !0 : i.size && (l.size = i.size))) : t = l.createElementNS(t, s), t[On] = e, t[Cn] = i, $o(t, e, !1, !1), e.stateNode = t, l = an(s, i), s) {
                                         case "iframe":
                                         case "object":
                                         case "embed":
-                                            qe("load", t), c = i;
+                                            Ke("load", t), c = i;
                                             break;
                                         case "video":
                                         case "audio":
-                                            for (c = 0; c < Gt.length; c++) qe(Gt[c], t);
+                                            for (c = 0; c < Gt.length; c++) Ke(Gt[c], t);
                                             c = i;
                                             break;
                                         case "source":
-                                            qe("error", t), c = i;
+                                            Ke("error", t), c = i;
                                             break;
                                         case "img":
                                         case "image":
                                         case "link":
-                                            qe("error", t), qe("load", t), c = i;
+                                            Ke("error", t), Ke("load", t), c = i;
                                             break;
                                         case "form":
-                                            qe("reset", t), qe("submit", t), c = i;
+                                            Ke("reset", t), Ke("submit", t), c = i;
                                             break;
                                         case "details":
-                                            qe("toggle", t), c = i;
+                                            Ke("toggle", t), c = i;
                                             break;
                                         case "input":
-                                            St(t, i), c = wt(t, i), qe("invalid", t), cn(n, "onChange");
+                                            St(t, i), c = wt(t, i), Ke("invalid", t), cn(n, "onChange");
                                             break;
                                         case "option":
                                             c = Et(t, i);
                                             break;
                                         case "select":
                                             t._wrapperState = {
                                                 wasMultiple: !!i.multiple
                                             }, c = r({}, i, {
                                                 value: void 0
-                                            }), qe("invalid", t), cn(n, "onChange");
+                                            }), Ke("invalid", t), cn(n, "onChange");
                                             break;
                                         case "textarea":
-                                            Ct(t, i), c = Ot(t, i), qe("invalid", t), cn(n, "onChange");
+                                            Ct(t, i), c = Ot(t, i), Ke("invalid", t), cn(n, "onChange");
                                             break;
                                         default:
                                             c = i
                                     }
                                     on(s, c);
                                     var u = c;
                                     for (a in u)
@@ -4600,22 +4679,22 @@
                                     }
                                     Sn(s, i) && (e.effectTag |= 4)
                                 }
                                 null !== e.ref && (e.effectTag |= 128)
                             }
                             return null;
                         case 6:
-                            if (t && null != e.stateNode) Ko(t, e, t.memoizedProps, i);
+                            if (t && null != e.stateNode) qo(t, e, t.memoizedProps, i);
                             else {
                                 if ("string" !== typeof i && null === e.stateNode) throw Error(o(166));
                                 n = zs(Ls.current), zs(Ps.current), Po(e) ? (n = e.stateNode, i = e.memoizedProps, n[On] = e, n.nodeValue !== i && (e.effectTag |= 4)) : ((n = (9 === n.nodeType ? n : n.ownerDocument).createTextNode(i))[On] = e, e.stateNode = n)
                             }
                             return null;
                         case 13:
-                            return pr(Vs), i = e.memoizedState, 0 !== (64 & e.effectTag) ? (e.expirationTime = n, e) : (n = null !== i, i = !1, null === t ? void 0 !== e.memoizedProps.fallback && Po(e) : (i = null !== (s = t.memoizedState), n || null === s || null !== (s = t.child.sibling) && (null !== (a = e.firstEffect) ? (e.firstEffect = s, s.nextEffect = a) : (e.firstEffect = e.lastEffect = s, s.nextEffect = null), s.effectTag = 8)), n && !i && 0 !== (2 & e.mode) && (null === t && !0 !== e.memoizedProps.unstable_avoidThisFallback || 0 !== (1 & Vs.current) ? Wa === Pa && (Wa = za) : (Wa !== Pa && Wa !== za || (Wa = Na), 0 !== qa && null !== Ua && (Ql(Ua, ja), Gl(Ua, qa)))), (n || i) && (e.effectTag |= 4), null);
+                            return pr(Vs), i = e.memoizedState, 0 !== (64 & e.effectTag) ? (e.expirationTime = n, e) : (n = null !== i, i = !1, null === t ? void 0 !== e.memoizedProps.fallback && Po(e) : (i = null !== (s = t.memoizedState), n || null === s || null !== (s = t.child.sibling) && (null !== (a = e.firstEffect) ? (e.firstEffect = s, s.nextEffect = a) : (e.firstEffect = e.lastEffect = s, s.nextEffect = null), s.effectTag = 8)), n && !i && 0 !== (2 & e.mode) && (null === t && !0 !== e.memoizedProps.unstable_avoidThisFallback || 0 !== (1 & Vs.current) ? Wa === Pa && (Wa = za) : (Wa !== Pa && Wa !== za || (Wa = Na), 0 !== Ka && null !== Ua && (Ql(Ua, ja), Gl(Ua, Ka)))), (n || i) && (e.effectTag |= 4), null);
                         case 4:
                             return Bs(), Xo(e), null;
                         case 10:
                             return os(e), null;
                         case 19:
                             if (pr(Vs), null === (i = e.memoizedState)) return null;
                             if (s = 0 !== (64 & e.effectTag), null === (a = i.rendering)) {
@@ -4685,15 +4764,15 @@
                         if (n === e) break;
                         for (; null === n.sibling;) {
                             if (null === n.return || n.return === e) return;
                             n = n.return
                         }
                         n.sibling.return = n.return, n = n.sibling
                     }
-                }, Xo = function() {}, qo = function(t, e, n, i, s) {
+                }, Xo = function() {}, Ko = function(t, e, n, i, s) {
                     var o = t.memoizedProps;
                     if (o !== i) {
                         var a, l, c = e.stateNode;
                         switch (zs(Ps.current), t = null, n) {
                             case "input":
                                 o = wt(c, o), i = wt(c, i), t = [];
                                 break;
@@ -4726,15 +4805,15 @@
                                         for (l in c) !c.hasOwnProperty(l) || u && u.hasOwnProperty(l) || (n || (n = {}), n[l] = "");
                                         for (l in u) u.hasOwnProperty(l) && c[l] !== u[l] && (n || (n = {}), n[l] = u[l])
                                     } else n || (t || (t = []), t.push(a, n)), n = u;
                             else "dangerouslySetInnerHTML" === a ? (u = u ? u.__html : void 0, c = c ? c.__html : void 0, null != u && c !== u && (t = t || []).push(a, u)) : "children" === a ? c === u || "string" !== typeof u && "number" !== typeof u || (t = t || []).push(a, "" + u) : "suppressContentEditableWarning" !== a && "suppressHydrationWarning" !== a && (T.hasOwnProperty(a) ? (null != u && cn(s, a), t || c === u || (t = [])) : (t = t || []).push(a, u))
                         }
                         n && (t = t || []).push("style", n), s = t, (e.updateQueue = s) && (e.effectTag |= 4)
                     }
-                }, Ko = function(t, e, n, i) {
+                }, qo = function(t, e, n, i) {
                     n !== i && (e.effectTag |= 4)
                 };
                 var oa = "function" === typeof WeakSet ? WeakSet : Set;
 
                 function aa(t, e) {
                     var n = e.source,
                         i = e.stack;
@@ -4852,15 +4931,15 @@
                         case 0:
                         case 11:
                         case 14:
                         case 15:
                         case 22:
                             if (null !== (t = e.updateQueue) && null !== (t = t.lastEffect)) {
                                 var i = t.next;
-                                qr(97 < n ? 97 : n, (function() {
+                                Kr(97 < n ? 97 : n, (function() {
                                     var t = i;
                                     do {
                                         var n = t.destroy;
                                         if (void 0 !== n) {
                                             var r = e;
                                             try {
                                                 n()
@@ -5137,16 +5216,16 @@
                     Va = null,
                     ja = 0,
                     Wa = Pa,
                     Ha = null,
                     Ya = 1073741823,
                     $a = 1073741823,
                     Xa = null,
-                    qa = 0,
-                    Ka = !1,
+                    Ka = 0,
+                    qa = !1,
                     Qa = 0,
                     Ga = 500,
                     Za = null,
                     Ja = !1,
                     tl = null,
                     el = null,
                     nl = !1,
@@ -5214,15 +5293,15 @@
                         }
                     return null !== r && (Ua === r && (Sl(e), Wa === Na && Ql(r, ja)), Gl(r, e)), r
                 }
 
                 function fl(t) {
                     var e = t.lastExpiredTime;
                     if (0 !== e) return e;
-                    if (!Kl(t, e = t.firstPendingTime)) return e;
+                    if (!ql(t, e = t.firstPendingTime)) return e;
                     var n = t.lastPingedTime;
                     return 2 >= (t = n > (t = t.nextKnownPendingLevel) ? n : t) && e !== t ? 0 : t
                 }
 
                 function pl(t) {
                     if (0 !== t.lastExpiredTime) t.callbackExpirationTime = 1073741823, t.callbackPriority = 99, t.callbackNode = Qr(ml.bind(null, t));
                     else {
@@ -5232,15 +5311,15 @@
                         else {
                             var i = cl();
                             if (1073741823 === e ? i = 99 : 1 === e || 2 === e ? i = 95 : i = 0 >= (i = 10 * (1073741821 - e) - 10 * (1073741821 - i)) ? 99 : 250 >= i ? 98 : 5250 >= i ? 97 : 95, null !== n) {
                                 var r = t.callbackPriority;
                                 if (t.callbackExpirationTime === e && r >= i) return;
                                 n !== Br && Dr(n)
                             }
-                            t.callbackExpirationTime = e, t.callbackPriority = i, e = 1073741823 === e ? Qr(ml.bind(null, t)) : Kr(i, gl.bind(null, t), {
+                            t.callbackExpirationTime = e, t.callbackPriority = i, e = 1073741823 === e ? Qr(ml.bind(null, t)) : qr(i, gl.bind(null, t), {
                                 timeout: 10 * (1073741821 - e) - Yr()
                             }), t.callbackNode = e
                         }
                     }
                 }
 
                 function gl(t, e) {
@@ -5263,15 +5342,15 @@
                                 case Fa:
                                     throw Error(o(345));
                                 case La:
                                     Zl(t, 2 < n ? 2 : n);
                                     break;
                                 case za:
                                     if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), 1073741823 === Ya && 10 < (r = Qa + Ga - Yr())) {
-                                        if (Ka) {
+                                        if (qa) {
                                             var s = t.lastPingedTime;
                                             if (0 === s || s >= n) {
                                                 t.lastPingedTime = n, vl(t, n);
                                                 break
                                             }
                                         }
                                         if (0 !== (s = fl(t)) && s !== n) break;
@@ -5281,15 +5360,15 @@
                                         }
                                         t.timeoutHandle = kn(Dl.bind(null, t), r);
                                         break
                                     }
                                     Dl(t);
                                     break;
                                 case Na:
-                                    if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), Ka && (0 === (r = t.lastPingedTime) || r >= n)) {
+                                    if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), qa && (0 === (r = t.lastPingedTime) || r >= n)) {
                                         t.lastPingedTime = n, vl(t, n);
                                         break
                                     }
                                     if (0 !== (r = fl(t)) && r !== n) break;
                                     if (0 !== i && i !== n) {
                                         t.lastPingedTime = i;
                                         break
@@ -5383,26 +5462,26 @@
                                     pr(Vs);
                                     break;
                                 case 10:
                                     os(i)
                             }
                             n = n.return
                         }
-                    Ua = t, Va = Wl(t.current, null), ja = e, Wa = Pa, Ha = null, $a = Ya = 1073741823, Xa = null, qa = 0, Ka = !1
+                    Ua = t, Va = Wl(t.current, null), ja = e, Wa = Pa, Ha = null, $a = Ya = 1073741823, Xa = null, Ka = 0, qa = !1
                 }
 
                 function xl(t, e) {
                     for (;;) {
                         try {
                             if (ss(), Hs.current = wo, Qs)
                                 for (var n = Xs.memoizedState; null !== n;) {
                                     var i = n.queue;
                                     null !== i && (i.pending = null), n = n.next
                                 }
-                            if ($s = 0, Ks = qs = Xs = null, Qs = !1, null === Va || null === Va.return) return Wa = Fa, Ha = e, Va = null;
+                            if ($s = 0, qs = Ks = Xs = null, Qs = !1, null === Va || null === Va.return) return Wa = Fa, Ha = e, Va = null;
                             t: {
                                 var r = t,
                                     s = Va.return,
                                     o = Va,
                                     a = e;
                                 if (e = ja, o.effectTag |= 2048, o.firstEffect = o.lastEffect = null, null !== a && "object" === typeof a && "function" === typeof a.then) {
                                     var l = a;
@@ -5485,15 +5564,15 @@
                 }
 
                 function wl(t, e) {
                     t < Ya && 2 < t && (Ya = t), null !== e && t < $a && 2 < t && ($a = t, Xa = e)
                 }
 
                 function Sl(t) {
-                    t > qa && (qa = t)
+                    t > Ka && (Ka = t)
                 }
 
                 function Tl() {
                     for (; null !== Va;) Va = Ml(Va)
                 }
 
                 function kl() {
@@ -5533,15 +5612,15 @@
                 function El(t) {
                     var e = t.expirationTime;
                     return e > (t = t.childExpirationTime) ? e : t
                 }
 
                 function Dl(t) {
                     var e = $r();
-                    return qr(99, Ol.bind(null, t, e)), null
+                    return Kr(99, Ol.bind(null, t, e)), null
                 }
 
                 function Ol(t, e) {
                     do {
                         Al()
                     } while (null !== il);
                     if ((Ra & (Ca | Aa)) !== Da) throw Error(o(327));
@@ -5688,24 +5767,24 @@
                     if (0 === (e = t.firstPendingTime) && (el = null), 1073741823 === e ? t === al ? ol++ : (ol = 0, al = t) : ol = 0, "function" === typeof Bl && Bl(n.stateNode, i), pl(t), Ja) throw Ja = !1, t = tl, tl = null, t;
                     return (Ra & Oa) !== Da || Gr(), null
                 }
 
                 function Cl() {
                     for (; null !== Za;) {
                         var t = Za.effectTag;
-                        0 !== (256 & t) && ca(Za.alternate, Za), 0 === (512 & t) || nl || (nl = !0, Kr(97, (function() {
+                        0 !== (256 & t) && ca(Za.alternate, Za), 0 === (512 & t) || nl || (nl = !0, qr(97, (function() {
                             return Al(), null
                         }))), Za = Za.nextEffect
                     }
                 }
 
                 function Al() {
                     if (90 !== rl) {
                         var t = 97 < rl ? 97 : rl;
-                        return rl = 90, qr(t, Pl)
+                        return rl = 90, Kr(t, Pl)
                     }
                 }
 
                 function Pl() {
                     if (null === il) return !1;
                     var t = il;
                     if (il = null, (Ra & (Ca | Aa)) !== Da) throw Error(o(331));
@@ -5750,15 +5829,15 @@
                             }
                             n = n.return
                         }
                 }
 
                 function zl(t, e, n) {
                     var i = t.pingCache;
-                    null !== i && i.delete(e), Ua === t && ja === n ? Wa === Na || Wa === za && 1073741823 === Ya && Yr() - Qa < Ga ? vl(t, ja) : Ka = !0 : Kl(t, n) && (0 !== (e = t.lastPingedTime) && e < n || (t.lastPingedTime = n, pl(t)))
+                    null !== i && i.delete(e), Ua === t && ja === n ? Wa === Na || Wa === za && 1073741823 === Ya && Yr() - Qa < Ga ? vl(t, ja) : qa = !0 : ql(t, n) && (0 !== (e = t.lastPingedTime) && e < n || (t.lastPingedTime = n, pl(t)))
                 }
 
                 function Nl(t, e) {
                     var n = t.stateNode;
                     null !== n && n.delete(e), 0 === (e = 0) && (e = ul(e = cl(), t, null)), null !== (t = dl(t, e)) && pl(t)
                 }
                 ka = function(t, e, n) {
@@ -6017,19 +6096,19 @@
                     return (e = Vl(4, null !== t.children ? t.children : [], t.key, e)).expirationTime = n, e.stateNode = {
                         containerInfo: t.containerInfo,
                         pendingChildren: null,
                         implementation: t.implementation
                     }, e
                 }
 
-                function ql(t, e, n) {
+                function Kl(t, e, n) {
                     this.tag = e, this.current = null, this.containerInfo = t, this.pingCache = this.pendingChildren = null, this.finishedExpirationTime = 0, this.finishedWork = null, this.timeoutHandle = -1, this.pendingContext = this.context = null, this.hydrate = n, this.callbackNode = null, this.callbackPriority = 90, this.lastExpiredTime = this.lastPingedTime = this.nextKnownPendingLevel = this.lastSuspendedTime = this.firstSuspendedTime = this.firstPendingTime = 0
                 }
 
-                function Kl(t, e) {
+                function ql(t, e) {
                     var n = t.firstSuspendedTime;
                     return t = t.lastSuspendedTime, 0 !== n && n >= e && t <= e
                 }
 
                 function Ql(t, e) {
                     var n = t.firstSuspendedTime,
                         i = t.lastSuspendedTime;
@@ -6094,15 +6173,15 @@
                 }
 
                 function nc(t, e) {
                     ec(t, e), (t = t.alternate) && ec(t, e)
                 }
 
                 function ic(t, e, n) {
-                    var i = new ql(t, e, n = null != n && !0 === n.hydrate),
+                    var i = new Kl(t, e, n = null != n && !0 === n.hydrate),
                         r = Vl(3, null, null, 2 === e ? 7 : 1 === e ? 3 : 0);
                     i.current = r, r.stateNode = i, hs(r), t[An] = i.current, n && 0 !== e && function(t, e) {
                         var n = Jt(e);
                         Ie.forEach((function(t) {
                             ge(t, e, n)
                         })), Ee.forEach((function(t) {
                             ge(t, e, n)
@@ -6202,15 +6281,15 @@
                         case "select":
                             null != (e = n.value) && Dt(t, !!n.multiple, e, !1)
                     }
                 }, F = yl, L = function(t, e, n, i, r) {
                     var s = Ra;
                     Ra |= 4;
                     try {
-                        return qr(98, t.bind(null, e, n, i, r))
+                        return Kr(98, t.bind(null, e, n, i, r))
                     } finally {
                         (Ra = s) === Da && Gr()
                     }
                 }, z = function() {
                     (Ra & (1 | Ca | Aa)) === Da && (function() {
                         if (null !== sl) {
                             var t = sl;
@@ -6286,15 +6365,15 @@
                     }
                     return t = null === (t = ie(e)) ? null : t.stateNode
                 }, e.flushSync = function(t, e) {
                     if ((Ra & (Ca | Aa)) !== Da) throw Error(o(187));
                     var n = Ra;
                     Ra |= 1;
                     try {
-                        return qr(99, t.bind(null, e))
+                        return Kr(99, t.bind(null, e))
                     } finally {
                         Ra = n, Gr()
                     }
                 }, e.hydrate = function(t, e, n) {
                     if (!rc(e)) throw Error(o(200));
                     return sc(null, t, e, !0, n)
                 }, e.render = function(t, e, n) {
@@ -7283,15 +7362,15 @@
                 i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : e.byteLength;
             const r = t.byteLength,
                 s = new Uint8Array(t.buffer, t.byteOffset, r),
                 o = new Uint8Array(e.buffer, e.byteOffset, Math.min(i, r));
             return s.set(o, n), t
         }
 
-        function q(t, e) {
+        function K(t, e) {
             const n = function(t) {
                     const e = t[0] ? [t[0]] : [];
                     let n, i, r, s;
                     for (let o, a, l = 0, c = 0, u = t.length; ++l < u;) o = e[c], a = t[l], !o || !a || o.buffer !== a.buffer || a.byteOffset < o.byteOffset ? a && (e[++c] = a) : (({
                         byteOffset: n,
                         byteLength: r
                     } = o), ({
@@ -7310,31 +7389,31 @@
                     break
                 }
                 X(o || (o = new Uint8Array(c)), s, a), a += s.length
             }
             return [o || new Uint8Array(0), n.slice(l), i - (o ? o.byteLength : 0)]
         }
 
-        function K(t, e) {
+        function q(t, e) {
             let n = E(e) ? e.value : e;
-            return n instanceof t ? t === Uint8Array ? new t(n.buffer, n.byteOffset, n.byteLength) : n : n ? ("string" === typeof n && (n = Y(n)), n instanceof ArrayBuffer || n instanceof $ ? new t(n) : F(n) ? K(t, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new t(0) : new t(n.buffer, n.byteOffset, n.byteLength / t.BYTES_PER_ELEMENT) : t.from(n)) : new t(0)
+            return n instanceof t ? t === Uint8Array ? new t(n.buffer, n.byteOffset, n.byteLength) : n : n ? ("string" === typeof n && (n = Y(n)), n instanceof ArrayBuffer || n instanceof $ ? new t(n) : F(n) ? q(t, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new t(0) : new t(n.buffer, n.byteOffset, n.byteLength / t.BYTES_PER_ELEMENT) : t.from(n)) : new t(0)
         }
-        const Q = t => K(Int32Array, t),
-            G = t => K(Uint8Array, t),
+        const Q = t => q(Int32Array, t),
+            G = t => q(Uint8Array, t),
             Z = t => (t.next(), t);
 
         function* J(t, e) {
             const n = function*(t) {
                     yield t
                 },
                 i = "string" === typeof e || ArrayBuffer.isView(e) || e instanceof ArrayBuffer || e instanceof $ ? n(e) : k(e) ? e : n(e);
             return yield* Z(function*(e) {
                 let n = null;
                 do {
-                    n = e.next(yield K(t, n))
+                    n = e.next(yield q(t, n))
                 } while (!n.done)
             }(i[Symbol.iterator]())), new t
         }
 
         function tt(t, e) {
             return R(this, arguments, (function*() {
                 if (T(e)) return yield B(yield B(yield* U(V(tt(t, yield B(e))))));
@@ -7353,15 +7432,15 @@
                             }(t[Symbol.iterator]())))))
                         }))
                     }(e) : M(e) ? e : n(e);
                 return yield B(yield* U(V(Z(function(e) {
                     return R(this, arguments, (function*() {
                         let n = null;
                         do {
-                            n = yield B(e.next(yield yield B(K(t, n))))
+                            n = yield B(e.next(yield yield B(q(t, n))))
                         } while (!n.done)
                     }))
                 }(i[Symbol.asyncIterator]()))))), yield B(new t)
             }))
         }
 
         function et(t, e, n) {
@@ -7371,15 +7450,15 @@
             }
             return n
         }
         const nt = Symbol.for("isArrowBigNum");
 
         function it(t) {
             for (var e = arguments.length, n = new Array(e > 1 ? e - 1 : 0), i = 1; i < e; i++) n[i - 1] = arguments[i];
-            return 0 === n.length ? Object.setPrototypeOf(K(this.TypedArray, t), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(t, ...n), this.constructor.prototype)
+            return 0 === n.length ? Object.setPrototypeOf(q(this.TypedArray, t), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(t, ...n), this.constructor.prototype)
         }
 
         function rt() {
             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
             return it.apply(this, e)
         }
 
@@ -7850,27 +7929,27 @@
                 return c.Union
             }
             toString() {
                 return "".concat(this[Symbol.toStringTag], "<").concat(this.children.map((t => "".concat(t.type))).join(" | "), ">")
             }
         }
         Mt = Symbol.toStringTag, Xt[Mt] = (t => (t.mode = null, t.typeIds = null, t.children = null, t.typeIdToChildIndex = null, t.ArrayType = Int8Array, t[Symbol.toStringTag] = "Union"))(Xt.prototype);
-        class qt extends At {
+        class Kt extends At {
             constructor(t) {
                 super(), this.byteWidth = t
             }
             get typeId() {
                 return c.FixedSizeBinary
             }
             toString() {
                 return "FixedSizeBinary[".concat(this.byteWidth, "]")
             }
         }
-        It = Symbol.toStringTag, qt[It] = (t => (t.byteWidth = null, t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "FixedSizeBinary"))(qt.prototype);
-        class Kt extends At {
+        It = Symbol.toStringTag, Kt[It] = (t => (t.byteWidth = null, t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "FixedSizeBinary"))(Kt.prototype);
+        class qt extends At {
             constructor(t, e) {
                 super(), this.listSize = t, this.children = [e]
             }
             get typeId() {
                 return c.FixedSizeList
             }
             get valueType() {
@@ -7882,15 +7961,15 @@
             get ArrayType() {
                 return this.valueType.ArrayType
             }
             toString() {
                 return "FixedSizeList[".concat(this.listSize, "]<").concat(this.valueType, ">")
             }
         }
-        Et = Symbol.toStringTag, Kt[Et] = (t => (t.children = null, t.listSize = null, t[Symbol.toStringTag] = "FixedSizeList"))(Kt.prototype);
+        Et = Symbol.toStringTag, qt[Et] = (t => (t.children = null, t.listSize = null, t[Symbol.toStringTag] = "FixedSizeList"))(qt.prototype);
         class Qt extends At {
             constructor(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                 super(), this.children = [t], this.keysSorted = e
             }
             get typeId() {
                 return c.Map
@@ -8685,21 +8764,21 @@
             },
             Xe = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            qe = (t, e) => {
+            Ke = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            Ke = (t, e) => {
+            qe = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
             Qe = (t, e) => {
                 let {
@@ -8786,21 +8865,21 @@
                     return $e(t, e)
             }
         })), Fe.prototype.visitTimestampSecond = Le(We), Fe.prototype.visitTimestampMillisecond = Le(He), Fe.prototype.visitTimestampMicrosecond = Le(Ye), Fe.prototype.visitTimestampNanosecond = Le($e), Fe.prototype.visitTime = Le(((t, e) => {
             switch (t.type.unit) {
                 case o.SECOND:
                     return Xe(t, e);
                 case o.MILLISECOND:
-                    return qe(t, e);
-                case o.MICROSECOND:
                     return Ke(t, e);
+                case o.MICROSECOND:
+                    return qe(t, e);
                 case o.NANOSECOND:
                     return Qe(t, e)
             }
-        })), Fe.prototype.visitTimeSecond = Le(Xe), Fe.prototype.visitTimeMillisecond = Le(qe), Fe.prototype.visitTimeMicrosecond = Le(Ke), Fe.prototype.visitTimeNanosecond = Le(Qe), Fe.prototype.visitDecimal = Le(((t, e) => {
+        })), Fe.prototype.visitTimeSecond = Le(Xe), Fe.prototype.visitTimeMillisecond = Le(Ke), Fe.prototype.visitTimeMicrosecond = Le(qe), Fe.prototype.visitTimeNanosecond = Le(Qe), Fe.prototype.visitDecimal = Le(((t, e) => {
             let {
                 values: n,
                 stride: i
             } = t;
             return ht.decimal(n.subarray(i * e, i * (e + 1)))
         })), Fe.prototype.visitList = Le(((t, e) => {
             const {
@@ -9374,15 +9453,15 @@
         var Wn;
         const Hn = {},
             Yn = {};
         class $n {
             constructor(t) {
                 var e, n, i;
                 const r = t[0] instanceof $n ? t.flatMap((t => t.data)) : t;
-                if (0 === r.length || r.some((t => !(t instanceof qn)))) throw new TypeError("Vector constructor expects an Array of Data instances.");
+                if (0 === r.length || r.some((t => !(t instanceof Kn)))) throw new TypeError("Vector constructor expects an Array of Data instances.");
                 const s = null === (e = r[0]) || void 0 === e ? void 0 : e.type;
                 switch (r.length) {
                     case 0:
                         this._offsets = [0];
                         break;
                     case 1: {
                         const {
@@ -9581,19 +9660,19 @@
                 }), Object.defineProperty(this, "unmemoize", {
                     value: () => new $n(this.data)
                 }), Object.defineProperty(this, "memoize", {
                     value: () => this
                 })
             }
         }
-        class qn {
+        class Kn {
             constructor(t, e, n, i, r) {
                 let s, o = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : [],
                     a = arguments.length > 6 ? arguments[6] : void 0;
-                this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(n || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), r instanceof qn ? (this.stride = r.stride, this.values = r.values, this.typeIds = r.typeIds, this.nullBitmap = r.nullBitmap, this.valueOffsets = r.valueOffsets) : (this.stride = te(t), r && ((s = r[0]) && (this.valueOffsets = s), (s = r[1]) && (this.values = s), (s = r[2]) && (this.nullBitmap = s), (s = r[3]) && (this.typeIds = s))), this.nullable = 0 !== this._nullCount && this.nullBitmap && this.nullBitmap.byteLength > 0
+                this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(n || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), r instanceof Kn ? (this.stride = r.stride, this.values = r.values, this.typeIds = r.typeIds, this.nullBitmap = r.nullBitmap, this.valueOffsets = r.valueOffsets) : (this.stride = te(t), r && ((s = r[0]) && (this.valueOffsets = s), (s = r[1]) && (this.values = s), (s = r[2]) && (this.nullBitmap = s), (s = r[3]) && (this.typeIds = s))), this.nullable = 0 !== this._nullCount && this.nullBitmap && this.nullBitmap.byteLength > 0
             }
             get typeId() {
                 return this.type.typeId
             }
             get ArrayType() {
                 return this.type.ArrayType
             }
@@ -9641,15 +9720,15 @@
             clone() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.type,
                     e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.offset,
                     n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.length,
                     i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : this._nullCount,
                     r = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : this,
                     s = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : this.children;
-                return new qn(t, e, n, i, r, s, this.dictionary)
+                return new Kn(t, e, n, i, r, s, this.dictionary)
             }
             slice(t, e) {
                 const {
                     stride: n,
                     typeId: i,
                     children: r
                 } = this, s = +(0 === this._nullCount) - 1, o = 16 === i ? n : 1, a = this._sliceBuffers(t, e, n, i);
@@ -9672,137 +9751,137 @@
                 } = this;
                 return (r = s[u.TYPE]) && (s[u.TYPE] = r.subarray(t, t + e)), (r = s[u.OFFSET]) && (s[u.OFFSET] = r.subarray(t, t + e + 1)) || (r = s[u.DATA]) && (s[u.DATA] = 6 === i ? r : r.subarray(n * t, n * (t + e))), s
             }
             _sliceChildren(t, e, n) {
                 return t.map((t => t.slice(e, n)))
             }
         }
-        qn.prototype.children = Object.freeze([]);
-        class Kn extends ee {
+        Kn.prototype.children = Object.freeze([]);
+        class qn extends ee {
             visit(t) {
                 return this.getVisitFn(t.type).call(this, t)
             }
             visitNull(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     length: i = 0
                 } = t;
-                return new qn(e, n, i, 0)
+                return new Kn(e, n, i, 0)
             }
             visitBool(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length >> 3,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitInt(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitFloat(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitUtf8(t) {
                 const {
                     type: e,
                     offset: n = 0
                 } = t, i = G(t.data), r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, o, a, [s, i, r])
+                return new Kn(e, n, o, a, [s, i, r])
             }
             visitBinary(t) {
                 const {
                     type: e,
                     offset: n = 0
                 } = t, i = G(t.data), r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, o, a, [s, i, r])
+                return new Kn(e, n, o, a, [s, i, r])
             }
             visitFixedSizeBinary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitDate(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitTimestamp(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitTime(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitDecimal(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitList(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     child: i
                 } = t, r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, o, a, [s, void 0, r], [i])
+                return new Kn(e, n, o, a, [s, void 0, r], [i])
             }
             visitStruct(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     children: i = []
                 } = t, r = G(t.nullBitmap), {
@@ -9810,83 +9889,83 @@
                         let {
                             length: n
                         } = e;
                         return Math.max(t, n)
                     }), 0),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, void 0, r], i)
+                return new Kn(e, n, s, o, [void 0, void 0, r], i)
             }
             visitUnion(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     children: i = []
-                } = t, r = G(t.nullBitmap), s = K(e.ArrayType, t.typeIds), {
+                } = t, r = G(t.nullBitmap), s = q(e.ArrayType, t.typeIds), {
                     length: o = s.length,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                if (At.isSparseUnion(e)) return new qn(e, n, o, a, [void 0, void 0, r, s], i);
+                if (At.isSparseUnion(e)) return new Kn(e, n, o, a, [void 0, void 0, r, s], i);
                 const l = Q(t.valueOffsets);
-                return new qn(e, n, o, a, [l, void 0, r, s], i)
+                return new Kn(e, n, o, a, [l, void 0, r, s], i)
             }
             visitDictionary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.indices.ArrayType, t.data), {
-                    dictionary: s = new $n([(new Kn).visit({
+                } = t, i = G(t.nullBitmap), r = q(e.indices.ArrayType, t.data), {
+                    dictionary: s = new $n([(new qn).visit({
                         type: e.dictionary
                     })])
                 } = t, {
                     length: o = r.length,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, o, a, [void 0, r, i], [], s)
+                return new Kn(e, n, o, a, [void 0, r, i], [], s)
             }
             visitInterval(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = K(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, r, i])
+                return new Kn(e, n, s, o, [void 0, r, i])
             }
             visitFixedSizeList(t) {
                 const {
                     type: e,
                     offset: n = 0,
-                    child: i = (new Kn).visit({
+                    child: i = (new qn).visit({
                         type: e.valueType
                     })
                 } = t, r = G(t.nullBitmap), {
                     length: s = i.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, s, o, [void 0, void 0, r], [i])
+                return new Kn(e, n, s, o, [void 0, void 0, r], [i])
             }
             visitMap(t) {
                 const {
                     type: e,
                     offset: n = 0,
-                    child: i = (new Kn).visit({
+                    child: i = (new qn).visit({
                         type: e.childType
                     })
                 } = t, r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new qn(e, n, o, a, [s, void 0, r], [i])
+                return new Kn(e, n, o, a, [s, void 0, r], [i])
             }
         }
 
         function Qn(t) {
-            return (new Kn).visit(t)
+            return (new qn).visit(t)
         }
         class Gn {
             constructor() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [],
                     e = arguments.length > 1 ? arguments[1] : void 0,
                     n = arguments.length > 2 ? arguments[2] : void 0;
                 this.fields = t || [], this.metadata = e || new Map, n || (n = ti(t)), this.dictionaries = n
@@ -10051,15 +10130,15 @@
                         if ([, this.data = Qn({
                                 nullCount: 0,
                                 type: new $t(this.schema.fields),
                                 children: this.schema.fields.map((t => Qn({
                                     type: t.type,
                                     nullCount: 0
                                 })))
-                            })] = e, !(this.data instanceof qn)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
+                            })] = e, !(this.data instanceof Kn)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
                         [this.schema, this.data] = mi(this.schema, this.data.children);
                         break;
                     case 1: {
                         const [t] = e, {
                             fields: n,
                             children: i,
                             length: r
@@ -10284,15 +10363,15 @@
                 if (0 === i.length) return this.batches = [], this.schema = new Gn([]), this._offsets = [0], this;
                 let s, o;
                 i[0] instanceof Gn && (s = i.shift()), i[i.length - 1] instanceof Uint32Array && (o = i.pop());
                 const a = t => {
                         if (t) {
                             if (t instanceof gi) return [t];
                             if (t instanceof _i) return t.batches;
-                            if (t instanceof qn) {
+                            if (t instanceof Kn) {
                                 if (t.type instanceof $t) return [new gi(new Gn(t.type.children), t)]
                             } else {
                                 if (Array.isArray(t)) return t.flatMap((t => a(t)));
                                 if ("function" === typeof t[Symbol.iterator]) return [...t].flatMap((t => a(t)));
                                 if ("object" === typeof t) {
                                     const e = Object.keys(t),
                                         n = e.map((e => new $n([t[e]]))),
@@ -11332,21 +11411,21 @@
                 const {
                     metaDataLength: n
                 } = e, i = new Vi(e.offset, 0), r = new Vi(e.bodyLength, 0);
                 return wi.createBlock(t, i, n, r)
             }
         }
         const Xi = {
-                fromIterable: t => qi(function*(t) {
+                fromIterable: t => Ki(function*(t) {
                     let e, n, i, r, s = !1,
                         o = [],
                         a = 0;
 
                     function l() {
-                        return "peek" === i ? q(o, r)[0] : ([n, o, a] = q(o, r), n)
+                        return "peek" === i ? K(o, r)[0] : ([n, o, a] = K(o, r), n)
                     }({
                         cmd: i,
                         size: r
                     } = yield null);
                     const c = (u = t, J(Uint8Array, u))[Symbol.iterator]();
                     var u;
                     try {
@@ -11365,22 +11444,22 @@
                     } catch (h) {
                         (s = !0) && "function" === typeof c.throw && c.throw(h)
                     } finally {
                         !1 === s && "function" === typeof c.return && c.return(null)
                     }
                     return null
                 }(t)),
-                fromAsyncIterable: t => qi(function(t) {
+                fromAsyncIterable: t => Ki(function(t) {
                     return R(this, arguments, (function*() {
                         let e, n, i, r, s = !1,
                             o = [],
                             a = 0;
 
                         function l() {
-                            return "peek" === i ? q(o, r)[0] : ([n, o, a] = q(o, r), n)
+                            return "peek" === i ? K(o, r)[0] : ([n, o, a] = K(o, r), n)
                         }({
                             cmd: i,
                             size: r
                         } = yield yield B(null));
                         const c = (u = t, tt(Uint8Array, u))[Symbol.asyncIterator]();
                         var u;
                         try {
@@ -11400,28 +11479,28 @@
                             (s = !0) && "function" === typeof c.throw && (yield B(c.throw(h)))
                         } finally {
                             !1 === s && "function" === typeof c.return && (yield B(c.return(new Uint8Array(0))))
                         }
                         return yield B(null)
                     }))
                 }(t)),
-                fromDOMStream: t => qi(function(t) {
+                fromDOMStream: t => Ki(function(t) {
                     return R(this, arguments, (function*() {
                         let e, n, i, r = !1,
                             s = !1,
                             o = [],
                             a = 0;
 
                         function l() {
-                            return "peek" === n ? q(o, i)[0] : ([e, o, a] = q(o, i), e)
+                            return "peek" === n ? K(o, i)[0] : ([e, o, a] = K(o, i), e)
                         }({
                             cmd: n,
                             size: i
                         } = yield yield B(null));
-                        const c = new Ki(t);
+                        const c = new qi(t);
                         try {
                             do {
                                 if (({
                                         done: r,
                                         value: e
                                     } = Number.isNaN(i - a) ? yield B(c.read()): yield B(c.read(i - a))), !r && e.byteLength > 0 && (o.push(G(e)), a += e.byteLength), r || i <= a)
                                     do {
@@ -11435,25 +11514,25 @@
                             (s = !0) && (yield B(c.cancel(u)))
                         } finally {
                             !1 === s ? yield B(c.cancel()): t.locked && c.releaseLock()
                         }
                         return yield B(null)
                     }))
                 }(t)),
-                fromNodeStream: t => qi(function(t) {
+                fromNodeStream: t => Ki(function(t) {
                     return R(this, arguments, (function*() {
                         const e = [];
                         let n, i, r, s = "error",
                             o = !1,
                             a = null,
                             l = 0,
                             c = [];
 
                         function u() {
-                            return "peek" === n ? q(c, i)[0] : ([r, c, l] = q(c, i), r)
+                            return "peek" === n ? K(c, i)[0] : ([r, c, l] = K(c, i), r)
                         }
                         if (({
                                 cmd: n,
                                 size: i
                             } = yield yield B(null)), t.isTTY) return yield yield B(new Uint8Array(0)), yield B(null);
                         try {
                             e[0] = Qi(t, "end"), e[1] = Qi(t, "error");
@@ -11490,16 +11569,16 @@
                 toDOMStream(t, e) {
                     throw new Error('"toDOMStream" not available in this environment')
                 },
                 toNodeStream(t, e) {
                     throw new Error('"toNodeStream" not available in this environment')
                 }
             },
-            qi = t => (t.next(), t);
-        class Ki {
+            Ki = t => (t.next(), t);
+        class qi {
             constructor(t) {
                 this.source = t, this.reader = null, this.reader = this.source.getReader(), this.reader.closed.catch((() => {}))
             }
             get closed() {
                 return this.reader ? this.reader.closed.catch((() => {})) : Promise.resolve()
             }
             releaseLock() {
@@ -11654,15 +11733,15 @@
             write(t) {
                 if ((t = G(t)).byteLength > 0) return super.write(t)
             }
             toString() {
                 return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? W(this.toUint8Array(!0)) : this.toUint8Array(!1).then(W)
             }
             toUint8Array() {
-                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? q(this._values)[0] : (() => z(this, void 0, void 0, (function*() {
+                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? K(this._values)[0] : (() => z(this, void 0, void 0, (function*() {
                     var t, e;
                     const n = [];
                     let i = 0;
                     try {
                         for (var r, s = V(this); !(r = yield s.next()).done;) {
                             const t = r.value;
                             n.push(t), i += t.byteLength
@@ -11674,15 +11753,15 @@
                     } finally {
                         try {
                             r && !r.done && (e = s.return) && (yield e.call(s))
                         } finally {
                             if (t) throw t.error
                         }
                     }
-                    return q(n, i)[0]
+                    return K(n, i)[0]
                 })))()
             }
         }
         class nr {
             constructor(t) {
                 t && (this.source = new rr(Xi.fromIterable(t)))
             } [Symbol.iterator]() {
@@ -12421,35 +12500,35 @@
                 } = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.nextBufferRange();
                 return e <= 0 ? new Uint8Array(0) : Mn(this.sources[n])
             }
             readOffsets(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
-                return K(Uint8Array, K(Int32Array, this.sources[e]))
+                return q(Uint8Array, q(Int32Array, this.sources[e]))
             }
             readTypeIds(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
-                return K(Uint8Array, K(t.ArrayType, this.sources[e]))
+                return q(Uint8Array, q(t.ArrayType, this.sources[e]))
             }
             readData(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
                 const {
                     sources: n
                 } = this;
-                return At.isTimestamp(t) || (At.isInt(t) || At.isTime(t)) && 64 === t.bitWidth || At.isDate(t) && t.unit === s.MILLISECOND ? K(Uint8Array, dr.convertArray(n[e])) : At.isDecimal(t) ? K(Uint8Array, fr.convertArray(n[e])) : At.isBinary(t) || At.isFixedSizeBinary(t) ? function(t) {
+                return At.isTimestamp(t) || (At.isInt(t) || At.isTime(t)) && 64 === t.bitWidth || At.isDate(t) && t.unit === s.MILLISECOND ? q(Uint8Array, dr.convertArray(n[e])) : At.isDecimal(t) ? q(Uint8Array, fr.convertArray(n[e])) : At.isBinary(t) || At.isFixedSizeBinary(t) ? function(t) {
                     const e = t.join(""),
                         n = new Uint8Array(e.length / 2);
                     for (let i = 0; i < e.length; i += 2) n[i >> 1] = Number.parseInt(e.slice(i, i + 2), 16);
                     return n
-                }(n[e]) : At.isBool(t) ? Mn(n[e]) : At.isUtf8(t) ? Y(n[e].join("")) : K(Uint8Array, K(t.ArrayType, n[e].map((t => +t))))
+                }(n[e]) : At.isBool(t) ? Mn(n[e]) : At.isUtf8(t) ? Y(n[e].join("")) : q(Uint8Array, q(t.ArrayType, n[e].map((t => +t))))
             }
         }
         var mr, yr, br, vr, xr, _r, wr, Sr;
         ! function(t) {
             t[t.BUFFER = 0] = "BUFFER"
         }(mr || (mr = {})),
         function(t) {
@@ -13273,19 +13352,19 @@
                 return Nr.startFixedSizeList(e), Nr.addListSize(e, t.listSize), Nr.endFixedSizeList(e)
             }
             visitMap(t, e) {
                 return Br.startMap(e), Br.addKeysSorted(e, t.keysSorted), Br.endMap(e)
             }
         };
 
-        function qr(t) {
+        function Kr(t) {
             return new ss(t.count, Qr(t.columns), Gr(t.columns))
         }
 
-        function Kr(t, e) {
+        function qr(t, e) {
             return (t.children || []).filter(Boolean).map((t => Zn.fromJSON(t, e)))
         }
 
         function Qr(t) {
             return (t || []).reduce(((t, e) => {
                 return [...t, new ls(e.count, (n = e.VALIDITY, (n || []).reduce(((t, e) => t + +(0 === e)), 0))), ...Qr(e.children)];
                 var n
@@ -13358,19 +13437,19 @@
                 }
                 case "union": {
                     const i = t.type;
                     return new Xt(n[i.mode], i.typeIds || [], e || [])
                 }
                 case "fixedsizebinary": {
                     const e = t.type;
-                    return new qt(e.byteWidth)
+                    return new Kt(e.byteWidth)
                 }
                 case "fixedsizelist": {
                     const n = t.type;
-                    return new Kt(n.listSize, (e || [])[0])
+                    return new qt(n.listSize, (e || [])[0])
                 }
                 case "map": {
                     const n = t.type;
                     return new Qt((e || [])[0], n.keysSorted)
                 }
             }
             throw new Error('Unrecognized type: "'.concat(i, '"'))
@@ -13570,19 +13649,19 @@
                 }
                 case Ai.Union: {
                     const n = t.type(new Lr);
                     return new Xt(n.mode(), n.typeIdsArray() || [], e || [])
                 }
                 case Ai.FixedSizeBinary: {
                     const e = t.type(new zr);
-                    return new qt(e.byteWidth())
+                    return new Kt(e.byteWidth())
                 }
                 case Ai.FixedSizeList: {
                     const n = t.type(new Nr);
-                    return new Kt(n.listSize(), (e || [])[0])
+                    return new qt(n.listSize(), (e || [])[0])
                 }
                 case Ai.Map: {
                     const n = t.type(new Br);
                     return new Qt((e || [])[0], n.keysSorted())
                 }
             }
             throw new Error('Unrecognized type: "'.concat(Ai[n], '" (').concat(n, ")"))
@@ -13607,15 +13686,15 @@
             return Bi.endField(t)
         }, Zn.decode = function(t, e) {
             let n, i, r, s, o, a;
             e && (a = t.dictionary()) ? e.has(n = a.id().low) ? (s = (s = a.indexType()) ? hs(s) : new Lt, o = new Jt(e.get(n), s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (s = (s = a.indexType()) ? hs(s) : new Lt, e.set(n, r = ds(t, cs(t, e))), o = new Jt(r, s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (r = ds(t, cs(t, e)), i = new Zn(t.name(), r, t.nullable(), us(t)));
             return i || null
         }, Zn.fromJSON = function(t, e) {
             let n, i, r, s, o, a;
-            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Jr(i) : new Lt, a = new Jt(e.get(n), i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (i = (i = s.indexType) ? Jr(i) : new Lt, e.set(n, o = ts(t, Kr(t, e))), a = new Jt(o, i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (o = ts(t, Kr(t, e)), r = new Zn(t.name, o, t.nullable, Zr(t.customMetadata))), r || null
+            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Jr(i) : new Lt, a = new Jt(e.get(n), i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (i = (i = s.indexType) ? Jr(i) : new Lt, e.set(n, o = ts(t, qr(t, e))), a = new Jt(o, i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (o = ts(t, qr(t, e)), r = new Zn(t.name, o, t.nullable, Zr(t.customMetadata))), r || null
         }, Gn.encode = function(t, e) {
             const n = e.fields.map((e => Zn.encode(t, e)));
             Ri.startFieldsVector(t, n.length);
             const i = Ri.createFieldsVector(t, n),
                 r = e.metadata && e.metadata.size > 0 ? Ri.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
@@ -13655,22 +13734,22 @@
                 for (let n, i = -1, r = -1, s = t.nodesLength(); ++i < s;)(n = t.nodes(i)) && (e[++r] = ls.decode(n));
                 return e
             }(t), function(t, n) {
                 const i = [];
                 for (let r, s = -1, o = -1, a = t.buffersLength(); ++s < a;)(r = t.buffers(s)) && (n < e.V4 && (r.bb_pos += 8 * (s + 1)), i[++o] = as.decode(r));
                 return i
             }(t, n))
-        }, ss.fromJSON = qr, os.encode = function(t, e) {
+        }, ss.fromJSON = Kr, os.encode = function(t, e) {
             const n = ss.encode(t, e.data);
             return Er.startDictionaryBatch(t), Er.addId(t, new es(e.id, 0)), Er.addIsDelta(t, e.isDelta), Er.addData(t, n), Er.endDictionaryBatch(t)
         }, os.decode = function(t) {
             let n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : e.V4;
             return new os(ss.decode(t.data(), n), t.id(), t.isDelta())
         }, os.fromJSON = function(t) {
-            return new os(qr(t.data), t.id, t.isDelta)
+            return new os(Kr(t.data), t.id, t.isDelta)
         }, ls.encode = function(t, e) {
             return Mr.createFieldNode(t, new es(e.length, 0), new es(e.nullCount, 0))
         }, ls.decode = function(t) {
             return new ls(t.length(), t.nullCount())
         }, as.encode = function(t, e) {
             return kr.createBuffer(t, new es(e.offset, 0), new es(e.length, 0))
         }, as.decode = function(t) {
@@ -14523,15 +14602,15 @@
                                 n = Math.min(i, o[t]);
                             this.visit(r.slice(a[t], n))
                         }
                 }
             }
             return this
         }, js.prototype.visitInterval = Hs, js.prototype.visitFixedSizeList = $s, js.prototype.visitMap = $s;
-        class qs extends Ji {
+        class Ks extends Ji {
             constructor(t) {
                 super(), this._position = 0, this._started = !1, this._sink = new er, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, S(t) || (t = {
                     autoDestroy: !0,
                     writeLegacyIpcFormat: !1
                 }), this._autoDestroy = "boolean" !== typeof t.autoDestroy || t.autoDestroy, this._writeLegacyIpcFormat = "boolean" === typeof t.writeLegacyIpcFormat && t.writeLegacyIpcFormat
             }
             static throughNode(t) {
@@ -14651,21 +14730,21 @@
                     let t = this._dictionaryDeltaOffsets.get(e) || 0;
                     if (0 === t || (n = null === n || void 0 === n ? void 0 : n.slice(t)).length > 0)
                         for (const i of n.data) this._writeDictionaryBatch(i, e, t > 0), t += i.length
                 }
                 return this
             }
         }
-        class Ks extends qs {
+        class qs extends Ks {
             static writeAll(t, e) {
-                const n = new Ks(e);
+                const n = new qs(e);
                 return T(t) ? t.then((t => n.writeAll(t))) : M(t) ? Zs(n, t) : Gs(n, t)
             }
         }
-        class Qs extends qs {
+        class Qs extends Ks {
             static writeAll(t) {
                 const e = new Qs;
                 return T(t) ? t.then((t => e.writeAll(t))) : M(t) ? Zs(e, t) : Gs(e, t)
             }
             constructor() {
                 super(), this._autoDestroy = !0
             }
@@ -14710,15 +14789,15 @@
 
         function Js(t) {
             const e = Es.from(t);
             return T(e) ? e.then((t => Js(t))) : e.isAsync() ? e.readAll().then((t => new _i(t))) : new _i(e.readAll())
         }
 
         function to(t) {
-            return ("stream" === (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "stream") ? Ks : Qs).writeAll(t).toUint8Array(!0)
+            return ("stream" === (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "stream") ? qs : Qs).writeAll(t).toUint8Array(!0)
         }
         var eo, no = function() {
                 function t(t, e, n, i) {
                     var r = this;
                     this.getCell = function(t, e) {
                         var n = t < r.headerRows && e < r.headerColumns,
                             i = t >= r.headerRows && e < r.headerColumns,
@@ -15478,19 +15557,19 @@
 
         function $o() {}
         const Xo = (() => {
             let t = 0;
             return () => t++
         })();
 
-        function qo(t) {
+        function Ko(t) {
             return null === t || "undefined" === typeof t
         }
 
-        function Ko(t) {
+        function qo(t) {
             if (Array.isArray && Array.isArray(t)) return !0;
             const e = Object.prototype.toString.call(t);
             return "[object" === e.slice(0, 7) && "Array]" === e.slice(-6)
         }
 
         function Qo(t) {
             return null !== t && "[object Object]" === Object.prototype.toString.call(t)
@@ -15511,15 +15590,15 @@
 
         function ea(t, e, n) {
             if (t && "function" === typeof t.call) return t.apply(n, e)
         }
 
         function na(t, e, n, i) {
             let r, s, o;
-            if (Ko(t))
+            if (qo(t))
                 if (s = t.length, i)
                     for (r = s - 1; r >= 0; r--) e.call(n, t[r], r);
                 else
                     for (r = 0; r < s; r++) e.call(n, t[r], r);
             else if (Qo(t))
                 for (o = Object.keys(t), s = o.length, r = 0; r < s; r++) e.call(n, t[o[r]], o[r])
         }
@@ -15529,15 +15608,15 @@
             if (!t || !e || t.length !== e.length) return !1;
             for (n = 0, i = t.length; n < i; ++n)
                 if (r = t[n], s = e[n], r.datasetIndex !== s.datasetIndex || r.index !== s.index) return !1;
             return !0
         }
 
         function ra(t) {
-            if (Ko(t)) return t.map(ra);
+            if (qo(t)) return t.map(ra);
             if (Qo(t)) {
                 const e = Object.create(null),
                     n = Object.keys(t),
                     i = n.length;
                 let r = 0;
                 for (; r < i; ++r) e[n[r]] = ra(t[n[r]]);
                 return e
@@ -15553,15 +15632,15 @@
             if (!sa(t)) return;
             const r = e[t],
                 s = n[t];
             Qo(r) && Qo(s) ? aa(r, s, i) : e[t] = ra(s)
         }
 
         function aa(t, e, n) {
-            const i = Ko(e) ? e : [e],
+            const i = qo(e) ? e : [e],
                 r = i.length;
             if (!Qo(t)) return t;
             const s = (n = n || {}).merger || oa;
             let o;
             for (let a = 0; a < r; ++a) {
                 if (o = i[a], !Qo(o)) continue;
                 const e = Object.keys(o);
@@ -15750,16 +15829,16 @@
             return function() {
                 for (var r = arguments.length, s = new Array(r), o = 0; o < r; o++) s[o] = arguments[o];
                 n = s, i || (i = !0, $a.call(window, (() => {
                     i = !1, t.apply(e, n)
                 })))
             }
         }
-        const qa = t => "start" === t ? "left" : "end" === t ? "right" : "center",
-            Ka = (t, e, n) => "start" === t ? e : "end" === t ? n : (e + n) / 2;
+        const Ka = t => "start" === t ? "left" : "end" === t ? "right" : "center",
+            qa = (t, e, n) => "start" === t ? e : "end" === t ? n : (e + n) / 2;
 
         function Qa(t, e, n) {
             const i = e.length;
             let r = 0,
                 s = i;
             if (t._sorted) {
                 const {
@@ -15871,15 +15950,15 @@
                 e = e || {};
                 const n = t + JSON.stringify(e);
                 let i = al.get(n);
                 return i || (i = new Intl.NumberFormat(t, e), al.set(n, i)), i
             }(e, n).format(t)
         }
         const cl = {
-            values: t => Ko(t) ? t : "" + t,
+            values: t => qo(t) ? t : "" + t,
             numeric(t, e, n) {
                 if (0 === t) return "0";
                 const i = this.chart.options.locale;
                 let r, s = t;
                 if (n.length > 1) {
                     const e = Math.max(Math.abs(n[0].value), Math.abs(n[n.length - 1].value));
                     (e < 1e-4 || e > 1e15) && (r = "scientific"), s = function(t, e) {
@@ -16128,17 +16207,17 @@
             let r = (i = i || {}).data = i.data || {},
                 s = i.garbageCollect = i.garbageCollect || [];
             i.font !== e && (r = i.data = {}, s = i.garbageCollect = [], i.font = e), t.save(), t.font = e;
             let o = 0;
             const a = n.length;
             let l, c, u, h, d;
             for (l = 0; l < a; l++)
-                if (h = n[l], void 0 === h || null === h || Ko(h)) {
-                    if (Ko(h))
-                        for (c = 0, u = h.length; c < u; c++) d = h[c], void 0 === d || null === d || Ko(d) || (o = yl(t, r, s, o, d))
+                if (h = n[l], void 0 === h || null === h || qo(h)) {
+                    if (qo(h))
+                        for (c = 0, u = h.length; c < u; c++) d = h[c], void 0 === d || null === d || qo(d) || (o = yl(t, r, s, o, d))
                 } else o = yl(t, r, s, o, h);
             t.restore();
             const f = s.length / 2;
             if (f > n.length) {
                 for (l = 0; l < f; l++) delete r[s[l]];
                 s.splice(0, f)
             }
@@ -16248,20 +16327,20 @@
         function Dl(t, e) {
             const n = t.fillStyle;
             t.fillStyle = e.color, t.fillRect(e.left, e.top, e.width, e.height), t.fillStyle = n
         }
 
         function Ol(t, e, n, i, r) {
             let s = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : {};
-            const o = Ko(e) ? e : [e],
+            const o = qo(e) ? e : [e],
                 a = s.strokeWidth > 0 && "" !== s.strokeColor;
             let l, c;
             for (t.save(), t.font = r.string, function(t, e) {
-                    e.translation && t.translate(e.translation[0], e.translation[1]), qo(e.rotation) || t.rotate(e.rotation), e.color && (t.fillStyle = e.color), e.textAlign && (t.textAlign = e.textAlign), e.textBaseline && (t.textBaseline = e.textBaseline)
-                }(t, s), l = 0; l < o.length; ++l) c = o[l], s.backdrop && Dl(t, s.backdrop), a && (s.strokeColor && (t.strokeStyle = s.strokeColor), qo(s.strokeWidth) || (t.lineWidth = s.strokeWidth), t.strokeText(c, n, i, s.maxWidth)), t.fillText(c, n, i, s.maxWidth), El(t, n, i, c, s), i += Number(r.lineHeight);
+                    e.translation && t.translate(e.translation[0], e.translation[1]), Ko(e.rotation) || t.rotate(e.rotation), e.color && (t.fillStyle = e.color), e.textAlign && (t.textAlign = e.textAlign), e.textBaseline && (t.textBaseline = e.textBaseline)
+                }(t, s), l = 0; l < o.length; ++l) c = o[l], s.backdrop && Dl(t, s.backdrop), a && (s.strokeColor && (t.strokeStyle = s.strokeColor), Ko(s.strokeWidth) || (t.lineWidth = s.strokeWidth), t.strokeText(c, n, i, s.maxWidth)), t.fillText(c, n, i, s.maxWidth), El(t, n, i, c, s), i += Number(r.lineHeight);
             t.restore()
         }
 
         function Cl(t, e) {
             const {
                 x: n,
                 y: i,
@@ -16325,22 +16404,22 @@
                 lineHeight: Fl(Jo(t.lineHeight, e.lineHeight), n),
                 size: n,
                 style: i,
                 weight: Jo(t.weight, e.weight),
                 string: ""
             };
             return r.string = function(t) {
-                return !t || qo(t.size) || qo(t.family) ? null : (t.style ? t.style + " " : "") + (t.weight ? t.weight + " " : "") + t.size + "px " + t.family
+                return !t || Ko(t.size) || Ko(t.family) ? null : (t.style ? t.style + " " : "") + (t.weight ? t.weight + " " : "") + t.size + "px " + t.family
             }(r), r
         }
 
         function Vl(t, e, n, i) {
             let r, s, o, a = !0;
             for (r = 0, s = t.length; r < s; ++r)
-                if (o = t[r], void 0 !== o && (void 0 !== e && "function" === typeof o && (o = o(e), a = !1), void 0 !== n && Ko(o) && (o = o[n % o.length], a = !1), void 0 !== o)) return i && !a && (i.cacheable = !1), o
+                if (o = t[r], void 0 !== o && (void 0 !== e && "function" === typeof o && (o = o(e), a = !1), void 0 !== n && qo(o) && (o = o[n % o.length], a = !1), void 0 !== o)) return i && !a && (i.cacheable = !1), o
         }
 
         function jl(t, e) {
             return Object.assign(Object.create(t), e)
         }
 
         function Wl(t) {
@@ -16356,15 +16435,15 @@
                 _rootScopes: r,
                 _fallback: n,
                 _getTarget: i,
                 override: i => Wl([i, ...t], e, r, n)
             };
             return new Proxy(s, {
                 deleteProperty: (e, n) => (delete e[n], delete e._keys, delete t[0][n], !0),
-                get: (n, i) => ql(n, i, (() => function(t, e, n, i) {
+                get: (n, i) => Kl(n, i, (() => function(t, e, n, i) {
                     let r;
                     for (const s of e)
                         if (r = tc($l(s, t), n), "undefined" !== typeof r) return Xl(t, r) ? Zl(n, i, t, r) : r
                 }(i, e, t, n))),
                 getOwnPropertyDescriptor: (t, e) => Reflect.getOwnPropertyDescriptor(t._scopes[0], e),
                 getPrototypeOf: () => Reflect.getPrototypeOf(t[0]),
                 has: (t, e) => ec(t).includes(e),
@@ -16385,15 +16464,15 @@
                 _stack: new Set,
                 _descriptors: Yl(t, i),
                 setContext: e => Hl(t, e, n, i),
                 override: r => Hl(t.override(r), e, n, i)
             };
             return new Proxy(r, {
                 deleteProperty: (e, n) => (delete e[n], delete t[n], !0),
-                get: (t, e, n) => ql(t, e, (() => function(t, e, n) {
+                get: (t, e, n) => Kl(t, e, (() => function(t, e, n) {
                     const {
                         _proxy: i,
                         _context: r,
                         _subProxy: s,
                         _descriptors: o
                     } = t;
                     let a = i[e];
@@ -16406,15 +16485,15 @@
                         } = n;
                         if (a.has(t)) throw new Error("Recursion detected: " + Array.from(a).join("->") + "->" + t);
                         a.add(t);
                         let l = e(s, o || i);
                         a.delete(t), Xl(t, l) && (l = Zl(r._scopes, r, t, l));
                         return l
                     }(e, a, t, n));
-                    Ko(a) && a.length && (a = function(t, e, n, i) {
+                    qo(a) && a.length && (a = function(t, e, n, i) {
                         const {
                             _proxy: r,
                             _context: s,
                             _subProxy: o,
                             _descriptors: a
                         } = n;
                         if ("undefined" !== typeof s.index && i(t)) return e[s.index % e.length];
@@ -16460,49 +16539,49 @@
                 isScriptable: pa(n) ? n : () => n,
                 isIndexable: pa(i) ? i : () => i
             }
         }
         const $l = (t, e) => t ? t + da(e) : e,
             Xl = (t, e) => Qo(e) && "adapters" !== t && (null === Object.getPrototypeOf(e) || e.constructor === Object);
 
-        function ql(t, e, n) {
+        function Kl(t, e, n) {
             if (Object.prototype.hasOwnProperty.call(t, e)) return t[e];
             const i = n();
             return t[e] = i, i
         }
 
-        function Kl(t, e, n) {
+        function ql(t, e, n) {
             return pa(t) ? t(e, n) : t
         }
         const Ql = (t, e) => !0 === t ? e : "string" === typeof t ? ha(e, t) : void 0;
 
         function Gl(t, e, n, i, r) {
             for (const s of e) {
                 const e = Ql(n, s);
                 if (e) {
                     t.add(e);
-                    const s = Kl(e._fallback, n, r);
+                    const s = ql(e._fallback, n, r);
                     if ("undefined" !== typeof s && s !== n && s !== i) return s
                 } else if (!1 === e && "undefined" !== typeof i && n !== i) return null
             }
             return !1
         }
 
         function Zl(t, e, n, i) {
             const r = e._rootScopes,
-                s = Kl(e._fallback, n, i),
+                s = ql(e._fallback, n, i),
                 o = [...t, ...r],
                 a = new Set;
             a.add(i);
             let l = Jl(a, o, n, s || n, i);
             return null !== l && (("undefined" === typeof s || s === n || (l = Jl(a, o, s, l, i), null !== l)) && Wl(Array.from(a), [""], r, s, (() => function(t, e, n) {
                 const i = t._getTarget();
                 e in i || (i[e] = {});
                 const r = i[e];
-                if (Ko(r) && Qo(n)) return n;
+                if (qo(r) && Qo(n)) return n;
                 return r || {}
             }(e, n, i))))
         }
 
         function Jl(t, e, n, i, r) {
             for (; n;) n = Gl(t, e, n, i, r);
             return n
@@ -17120,15 +17199,15 @@
                 const e = Object.keys(ml.animation),
                     n = this._properties;
                 Object.getOwnPropertyNames(t).forEach((i => {
                     const r = t[i];
                     if (!Qo(r)) return;
                     const s = {};
                     for (const t of e) s[t] = r[t];
-                    (Ko(r.properties) && r.properties || [i]).forEach((t => {
+                    (qo(r.properties) && r.properties || [i]).forEach((t => {
                         t !== i && n.has(t) || n.set(t, s)
                     }))
                 }))
             }
             _animateOptions(t, e) {
                 const n = e.options,
                     i = function(t, e) {
@@ -17240,15 +17319,15 @@
             for (const r of e.getMatchingVisibleMetas(i).reverse()) {
                 const e = t[r.index];
                 if (n && e > 0 || !n && e < 0) return r.index
             }
             return null
         }
 
-        function qc(t, e) {
+        function Kc(t, e) {
             const {
                 chart: n,
                 _cachedMeta: i
             } = t, r = n._stacks || (n._stacks = {}), {
                 iScale: s,
                 vScale: o,
                 index: a
@@ -17263,15 +17342,15 @@
                         [c]: s
                     } = t;
                 d = (t._stacks || (t._stacks = {}))[c] = $c(r, u, n), d[a] = s, d._top = Xc(d, o, !0, i.type), d._bottom = Xc(d, o, !1, i.type);
                 (d._visualValues || (d._visualValues = {}))[a] = s
             }
         }
 
-        function Kc(t, e) {
+        function qc(t, e) {
             const n = t.scales;
             return Object.keys(n).filter((t => n[t].axis === e)).shift()
         }
 
         function Qc(t, e) {
             const n = t.controller.index,
                 i = t.vScale && t.vScale.axis;
@@ -17298,17 +17377,17 @@
                 this.index !== t && Qc(this._cachedMeta), this.index = t
             }
             linkScales() {
                 const t = this.chart,
                     e = this._cachedMeta,
                     n = this.getDataset(),
                     i = (t, e, n, i) => "x" === t ? e : "r" === t ? i : n,
-                    r = e.xAxisID = Jo(n.xAxisID, Kc(t, "x")),
-                    s = e.yAxisID = Jo(n.yAxisID, Kc(t, "y")),
-                    o = e.rAxisID = Jo(n.rAxisID, Kc(t, "r")),
+                    r = e.xAxisID = Jo(n.xAxisID, qc(t, "x")),
+                    s = e.yAxisID = Jo(n.yAxisID, qc(t, "y")),
+                    o = e.rAxisID = Jo(n.rAxisID, qc(t, "r")),
                     a = e.indexAxis,
                     l = e.iAxisID = i(a, r, s, o),
                     c = e.vAxisID = i(a, s, r, o);
                 e.xScale = this.getScaleForId(r), e.yScale = this.getScaleForId(s), e.rScale = this.getScaleForId(o), e.iScale = this.getScaleForId(l), e.vScale = this.getScaleForId(c)
             }
             getDataset() {
                 return this.chart.data.datasets[this.index]
@@ -17380,15 +17459,15 @@
             }
             buildOrUpdateElements(t) {
                 const e = this._cachedMeta,
                     n = this.getDataset();
                 let i = !1;
                 this._dataCheck();
                 const r = e._stacked;
-                e._stacked = Yc(e.vScale, e), e.stack !== n.stack && (i = !0, Qc(e), e.stack = n.stack), this._resyncElements(t), (i || r !== e._stacked) && qc(this, e._parsed)
+                e._stacked = Yc(e.vScale, e), e.stack !== n.stack && (i = !0, Qc(e), e.stack = n.stack), this._resyncElements(t), (i || r !== e._stacked) && Kc(this, e._parsed)
             }
             configure() {
                 const t = this.chart.config,
                     e = t.datasetScopeKeys(this._type),
                     n = t.getOptionScopes(this.getDataset(), e, !0);
                 this.options = t.createResolver(n, this.getContext()), this._parsing = this.options.parsing, this._cachedDataOpts = {}
             }
@@ -17400,20 +17479,20 @@
                     iScale: r,
                     _stacked: s
                 } = n, o = r.axis;
                 let a, l, c, u = 0 === t && e === i.length || n._sorted,
                     h = t > 0 && n._parsed[t - 1];
                 if (!1 === this._parsing) n._parsed = i, n._sorted = !0, c = i;
                 else {
-                    c = Ko(i[t]) ? this.parseArrayData(n, i, t, e) : Qo(i[t]) ? this.parseObjectData(n, i, t, e) : this.parsePrimitiveData(n, i, t, e);
+                    c = qo(i[t]) ? this.parseArrayData(n, i, t, e) : Qo(i[t]) ? this.parseObjectData(n, i, t, e) : this.parsePrimitiveData(n, i, t, e);
                     const r = () => null === l[o] || h && l[o] < h[o];
                     for (a = 0; a < e; ++a) n._parsed[a + t] = l = c[a], u && (r() && (u = !1), h = l);
                     n._sorted = u
                 }
-                s && qc(this, c)
+                s && Kc(this, c)
             }
             parsePrimitiveData(t, e, n, i) {
                 const {
                     iScale: r,
                     vScale: s
                 } = t, o = r.axis, a = s.axis, l = r.getLabels(), c = r === s, u = new Array(i);
                 let h, d, f;
@@ -17769,15 +17848,15 @@
             };
             for (i = 0, r = n.length; i < r; ++i) s = e.getPixelForValue(n[i]), l();
             for (o = void 0, i = 0, r = e.ticks.length; i < r; ++i) s = e.getPixelForTick(i), l();
             return a
         }
 
         function eu(t, e, n, i) {
-            return Ko(t) ? function(t, e, n, i) {
+            return qo(t) ? function(t, e, n, i) {
                 const r = n.parse(t[0], i),
                     s = n.parse(t[1], i),
                     o = Math.min(r, s),
                     a = Math.max(r, s);
                 let l = o,
                     c = a;
                 Math.abs(o) > Math.abs(a) && (l = a, c = o), e[n.axis] = c, e._custom = {
@@ -17913,15 +17992,15 @@
                     c = this._getRuler(),
                     {
                         sharedOptions: u,
                         includeOptions: h
                     } = this._getSharedOptions(e, i);
                 for (let d = e; d < e + n; d++) {
                     const e = this.getParsed(d),
-                        n = r || qo(e[o.axis]) ? {
+                        n = r || Ko(e[o.axis]) ? {
                             base: a,
                             head: a
                         } : this._calculateBarValuePixels(d),
                         f = this._calculateBarIndexPixels(d, c),
                         p = (e._stacks || {})[o.axis],
                         g = {
                             horizontal: l,
@@ -17939,15 +18018,15 @@
             }
             _getStacks(t, e) {
                 const {
                     iScale: n
                 } = this._cachedMeta, i = n.getMatchingVisibleMetas(this._type).filter((t => t.controller.options.grouped)), r = n.options.stacked, s = [], o = t => {
                     const n = t.controller.getParsed(e),
                         i = n && n[t.vScale.axis];
-                    if (qo(i) || isNaN(i)) return !0
+                    if (Ko(i) || isNaN(i)) return !0
                 };
                 for (const a of i)
                     if ((void 0 === e || !o(a)) && ((!1 === r || -1 === s.indexOf(a.stack) || void 0 === r && void 0 === a.stack) && s.push(a.stack), a.index === t)) break;
                 return s.length || s.push(void 0), s
             }
             _getStackCount(t) {
                 return this._getStacks(void 0, t).length
@@ -17988,15 +18067,15 @@
                         minBarLength: s
                     }
                 } = this, o = r || 0, a = this.getParsed(t), l = a._custom, c = iu(l);
                 let u, h, d = a[e.axis],
                     f = 0,
                     p = n ? this.applyStack(e, a, n) : d;
                 p !== d && (f = p - d, p = d), c && (d = l.barStart, p = l.barEnd - l.barStart, 0 !== d && ka(d) !== ka(l.barEnd) && (f = 0), f += d);
-                const g = qo(r) || c ? f : r;
+                const g = Ko(r) || c ? f : r;
                 let m = e.getPixelForValue(g);
                 if (u = this.chart.getDataVisibility(t) ? e.getPixelForValue(f + p) : m, h = u - m, Math.abs(h) < s) {
                     h = function(t, e, n) {
                         return 0 !== t ? ka(t) : (e.isHorizontal() ? 1 : -1) * (e.min >= n ? 1 : -1)
                     }(h, e, o) * s, d === o && (m -= h / 2);
                     const t = e.getPixelForDecimal(0),
                         r = e.getPixelForDecimal(1),
@@ -18035,15 +18114,15 @@
                                 chunk: Math.abs(a - o) / 2 * l / i,
                                 ratio: n.barPercentage,
                                 start: c
                             }
                         }(t, e, i, n) : function(t, e, n, i) {
                             const r = n.barThickness;
                             let s, o;
-                            return qo(r) ? (s = e.min * n.categoryPercentage, o = n.barPercentage) : (s = r * i, o = 1), {
+                            return Ko(r) ? (s = e.min * n.categoryPercentage, o = n.barPercentage) : (s = r * i, o = 1), {
                                 chunk: s / i,
                                 ratio: o,
                                 start: e.pixels[t] - s / 2
                             }
                         }(t, e, i, n),
                         c = this._getStackIndex(this.index, this._cachedMeta.stack, r ? t : void 0);
                     o = l.start + l.chunk * c + l.chunk / 2, a = Math.min(s, l.chunk * l.ratio)
@@ -18490,15 +18569,15 @@
                     const n = t[x],
                         f = m ? n : {};
                     if (x < e || x >= y) {
                         f.skip = !0;
                         continue
                     }
                     const b = this.getParsed(x),
-                        _ = qo(b[d]),
+                        _ = Ko(b[d]),
                         w = f[h] = s.getPixelForValue(b[h], x),
                         S = f[d] = r || _ ? o.getBasePixel() : o.getPixelForValue(a ? this.applyStack(o, b, a) : b[d], x);
                     f.skip = isNaN(w) || isNaN(S) || _, f.stop = x > 0 && Math.abs(b[h] - v[h]) > g, p && (f.parsed = b, f.raw = l.data[x]), u && (f.options = c || this.resolveDataElementOptions(x, n.active ? "active" : i)), m || this.updateElement(n, x, f, i), v = b
                 }
             }
             getMaxOverflow() {
                 const t = this._cachedMeta,
@@ -18819,15 +18898,15 @@
                     m = Ea(p) ? p : Number.POSITIVE_INFINITY,
                     y = this.chart._animationsDisabled || r || "none" === i;
                 let b = e > 0 && this.getParsed(e - 1);
                 for (let v = e; v < e + n; ++v) {
                     const e = t[v],
                         n = this.getParsed(v),
                         c = y ? e : {},
-                        p = qo(n[f]),
+                        p = Ko(n[f]),
                         x = c[d] = s.getPixelForValue(n[d], v),
                         _ = c[f] = r || p ? o.getBasePixel() : o.getPixelForValue(a ? this.applyStack(o, n, a) : n[f], v);
                     c.skip = isNaN(x) || isNaN(_) || p, c.stop = v > 0 && Math.abs(n[d] - b[d]) > m, g && (c.parsed = n, c.raw = l.data[v]), h && (c.options = u || this.resolveDataElementOptions(v, e.active ? "active" : i)), y || this.updateElement(e, v, c, i), b = n
                 }
                 this.updateSharedOptions(u, i, c)
             }
             getMaxOverflow() {
@@ -19391,28 +19470,28 @@
         }
 
         function Xu(t, e) {
             for (const n of t)
                 if (n === e || n.contains(e)) return !0
         }
 
-        function qu(t, e, n) {
+        function Ku(t, e, n) {
             const i = t.canvas,
                 r = new MutationObserver((t => {
                     let e = !1;
                     for (const n of t) e = e || Xu(n.addedNodes, i), e = e && !Xu(n.removedNodes, i);
                     e && n()
                 }));
             return r.observe(document, {
                 childList: !0,
                 subtree: !0
             }), r
         }
 
-        function Ku(t, e, n) {
+        function qu(t, e, n) {
             const i = t.canvas,
                 r = new MutationObserver((t => {
                     let e = !1;
                     for (const n of t) e = e || Xu(n.removedNodes, i), e = e && !Xu(n.addedNodes, i);
                     e && n()
                 }));
             return r.observe(document, {
@@ -19509,27 +19588,27 @@
             }
             releaseContext(t) {
                 const e = t.canvas;
                 if (!e[ju]) return !1;
                 const n = e[ju].initial;
                 ["height", "width"].forEach((t => {
                     const i = n[t];
-                    qo(i) ? e.removeAttribute(t) : e.setAttribute(t, i)
+                    Ko(i) ? e.removeAttribute(t) : e.setAttribute(t, i)
                 }));
                 const i = n.style || {};
                 return Object.keys(i).forEach((t => {
                     e.style[t] = i[t]
                 })), e.width = e.width, delete e[ju], !0
             }
             addEventListener(t, e, n) {
                 this.removeEventListener(t, e);
                 const i = t.$proxies || (t.$proxies = {}),
                     r = {
-                        attach: qu,
-                        detach: Ku,
+                        attach: Ku,
+                        detach: qu,
                         resize: Ju
                     } [e] || eh;
                 i[e] = r(t, e, n)
             }
             removeEventListener(t, e) {
                 const n = t.$proxies || (t.$proxies = {}),
                     i = n[e];
@@ -19626,16 +19705,16 @@
                     if (t > r) return t
                 }
                 return Math.max(r, 1)
             }(s, e, r);
             if (o > 0) {
                 let t, n;
                 const i = o > 1 ? Math.round((l - a) / (o - 1)) : null;
-                for (sh(e, c, u, qo(i) ? 0 : a - i, a), t = 0, n = o - 1; t < n; t++) sh(e, c, u, s[t], s[t + 1]);
-                return sh(e, c, u, l, qo(i) ? e.length : l + i), c
+                for (sh(e, c, u, Ko(i) ? 0 : a - i, a), t = 0, n = o - 1; t < n; t++) sh(e, c, u, s[t], s[t + 1]);
+                return sh(e, c, u, l, Ko(i) ? e.length : l + i), c
             }
             return sh(e, c, u), c
         }
 
         function sh(t, e, n, i, r) {
             const s = Jo(i, 0),
                 o = Math.min(Jo(r, t.length), t.length);
@@ -19670,19 +19749,19 @@
             return t.drawTicks ? t.tickLength : 0
         }
 
         function hh(t, e) {
             if (!t.display) return 0;
             const n = Ul(t.font, e),
                 i = Rl(t.padding);
-            return (Ko(t.text) ? t.text.length : 1) * n.lineHeight + i.height
+            return (qo(t.text) ? t.text.length : 1) * n.lineHeight + i.height
         }
 
         function dh(t, e, n) {
-            let i = qa(t);
+            let i = Ka(t);
             return (n && "right" !== e || !n && "right" === e) && (i = (t => "left" === t ? "right" : "right" === t ? "left" : t)(i)), i
         }
         class fh extends ih {
             constructor(t) {
                 super(), this.id = t.id, this.type = t.type, this.options = void 0, this.ctx = t.ctx, this.chart = t.chart, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.width = void 0, this.height = void 0, this._margins = {
                     left: 0,
                     right: 0,
@@ -19917,15 +19996,15 @@
                 return "top" === e || "bottom" === e || "x" === t
             }
             isFullSize() {
                 return this.options.fullSize
             }
             _convertTicksToLabels(t) {
                 let e, n;
-                for (this.beforeTickToLabelConversion(), this.generateTickLabels(t), e = 0, n = t.length; e < n; e++) qo(t[e].label) && (t.splice(e, 1), n--, e--);
+                for (this.beforeTickToLabelConversion(), this.generateTickLabels(t), e = 0, n = t.length; e < n; e++) Ko(t[e].label) && (t.splice(e, 1), n--, e--);
                 this.afterTickToLabelConversion()
             }
             _getLabelSizes() {
                 let t = this._labelSizes;
                 if (!t) {
                     const e = this.options.ticks.sampleSize;
                     let n = this.ticks;
@@ -19940,17 +20019,17 @@
                 } = this, s = [], o = [], a = Math.floor(e / ah(e, n));
                 let l, c, u, h, d, f, p, g, m, y, b, v = 0,
                     x = 0;
                 for (l = 0; l < e; l += a) {
                     if (h = t[l].label, d = this._resolveTickFontOptions(l), i.font = f = d.string, p = r[f] = r[f] || {
                             data: {},
                             gc: []
-                        }, g = d.lineHeight, m = y = 0, qo(h) || Ko(h)) {
-                        if (Ko(h))
-                            for (c = 0, u = h.length; c < u; ++c) b = h[c], qo(b) || Ko(b) || (m = yl(i, p.data, p.gc, m, b), y += g)
+                        }, g = d.lineHeight, m = y = 0, Ko(h) || qo(h)) {
+                        if (qo(h))
+                            for (c = 0, u = h.length; c < u; ++c) b = h[c], Ko(b) || qo(b) || (m = yl(i, p.data, p.gc, m, b), y += g)
                     } else m = yl(i, p.data, p.gc, m, h), y = g;
                     s.push(m), o.push(y), v = Math.max(m, v), x = Math.max(y, x)
                 }! function(t, e) {
                     na(t, (t => {
                         const n = t.gc,
                             i = n.length / 2;
                         let r;
@@ -20161,15 +20240,15 @@
                     w = this._getYAxisLabelAlignment(h).textAlign
                 }
                 "y" === e && ("start" === a ? E = "top" : "end" === a && (E = "bottom"));
                 const D = this._getLabelSizes();
                 for (m = 0, y = o.length; m < y; ++m) {
                     b = o[m], v = b.label;
                     const t = r.setContext(this.getContext(m));
-                    S = this.getPixelForTick(m) + r.labelOffset, T = this._resolveTickFontOptions(m), k = T.lineHeight, M = Ko(v) ? v.length : 1;
+                    S = this.getPixelForTick(m) + r.labelOffset, T = this._resolveTickFontOptions(m), k = T.lineHeight, M = qo(v) ? v.length : 1;
                     const e = M / 2,
                         n = t.color,
                         a = t.textStrokeColor,
                         c = t.textStrokeWidth;
                     let h, d = w;
                     if (s ? (x = S, "inner" === w && (d = m === y - 1 ? this.options.reverse ? "left" : "right" : 0 === m ? this.options.reverse ? "right" : "left" : "center"), I = "top" === i ? "near" === l || 0 !== p ? -M * k + k / 2 : "center" === l ? -D.highest.height / 2 - e * k + k : -D.highest.height + k / 2 : "near" === l || 0 !== p ? k / 2 : "center" === l ? D.highest.height / 2 - e * k : D.highest.height - M * k, u && (I *= -1), 0 === p || t.showLabelBackdrop || (x += k / 2 * Math.sin(p))) : (_ = S, I = (1 - M) * k / 2), t.showLabelBackdrop) {
                         const e = Rl(t.backdropPadding),
@@ -20351,15 +20430,15 @@
                     }
                 } = this;
                 if (!n.display) return;
                 const r = Ul(n.font),
                     s = Rl(n.padding),
                     o = n.align;
                 let a = r.lineHeight / 2;
-                "bottom" === e || "center" === e || Qo(e) ? (a += s.bottom, Ko(n.text) && (a += r.lineHeight * (n.text.length - 1))) : a += s.top;
+                "bottom" === e || "center" === e || Qo(e) ? (a += s.bottom, qo(n.text) && (a += r.lineHeight * (n.text.length - 1))) : a += s.top;
                 const {
                     titleX: l,
                     titleY: c,
                     maxWidth: u,
                     rotation: h
                 } = function(t, e, n, i) {
                     const {
@@ -20372,27 +20451,27 @@
                         chartArea: c,
                         scales: u
                     } = l;
                     let h, d, f, p = 0;
                     const g = o - r,
                         m = a - s;
                     if (t.isHorizontal()) {
-                        if (d = Ka(i, s, a), Qo(n)) {
+                        if (d = qa(i, s, a), Qo(n)) {
                             const t = Object.keys(n)[0],
                                 i = n[t];
                             f = u[t].getPixelForValue(i) + g - e
                         } else f = "center" === n ? (c.bottom + c.top) / 2 + g - e : oh(t, n, e);
                         h = a - s
                     } else {
                         if (Qo(n)) {
                             const t = Object.keys(n)[0],
                                 i = n[t];
                             d = u[t].getPixelForValue(i) - m + e
                         } else d = "center" === n ? (c.left + c.right) / 2 - m + e : oh(t, n, e);
-                        f = Ka(i, o, r), p = "left" === n ? -_a : _a
+                        f = qa(i, o, r), p = "left" === n ? -_a : _a
                     }
                     return {
                         titleX: d,
                         titleY: f,
                         maxWidth: h,
                         rotation: p
                     }
@@ -20596,15 +20675,15 @@
                 for (const r of t) {
                     const t = r.plugin;
                     if (!1 === ea(t[n], [e, i, r.options], t) && i.cancelable) return !1
                 }
                 return !0
             }
             invalidate() {
-                qo(this._cache) || (this._oldCache = this._cache, this._cache = void 0)
+                Ko(this._cache) || (this._oldCache = this._cache, this._cache = void 0)
             }
             _descriptors(t) {
                 if (this._cache) return this._cache;
                 const e = this._cache = this._createDescriptors(t);
                 return this._notifyStateChanges(t), e
             }
             _createDescriptors(t, e) {
@@ -20863,15 +20942,15 @@
                             isScriptable: n,
                             isIndexable: i
                         } = Yl(t);
                         for (const r of e) {
                             const e = n(r),
                                 s = i(r),
                                 o = (s || e) && t[r];
-                            if (e && (pa(o) || Ph(o)) || s && Ko(o)) return !0
+                            if (e && (pa(o) || Ph(o)) || s && qo(o)) return !0
                         }
                         return !1
                     }(s, e)) {
                     r.$shared = !1;
                     a = Hl(s, n = pa(n) ? n() : n, this.createResolver(t, n, o))
                 }
                 for (const l of e) r[l] = a[l];
@@ -20982,15 +21061,15 @@
                         aspectRatio: t,
                         maintainAspectRatio: e
                     },
                     width: n,
                     height: i,
                     _aspectRatio: r
                 } = this;
-                return qo(t) ? e && r ? r : i ? n / i : null : t
+                return Ko(t) ? e && r ? r : i ? n / i : null : t
             }
             get data() {
                 return this.config.data
             }
             set data(t) {
                 this.config.data = t
             }
@@ -21527,15 +21606,15 @@
         function Xh(t, e, n, i) {
             return {
                 x: n + t * Math.cos(e),
                 y: i + t * Math.sin(e)
             }
         }
 
-        function qh(t, e, n, i, r, s) {
+        function Kh(t, e, n, i, r, s) {
             const {
                 x: o,
                 y: a,
                 startAngle: l,
                 pixelMargin: c,
                 innerRadius: u
             } = e, h = Math.max(e.outerRadius + i + n - c, 0), d = u > 0 ? u + i + n + c : 0;
@@ -21591,15 +21670,15 @@
                 const i = Math.cos(k) * h + o,
                     r = Math.sin(k) * h + a;
                 t.lineTo(i, r)
             }
             t.closePath()
         }
 
-        function Kh(t, e, n, i, r) {
+        function qh(t, e, n, i, r) {
             const {
                 fullCircles: s,
                 startAngle: o,
                 circumference: a,
                 options: l
             } = e, {
                 borderWidth: c,
@@ -21607,30 +21686,30 @@
                 borderDash: h,
                 borderDashOffset: d
             } = l, f = "inner" === l.borderAlign;
             if (!c) return;
             t.setLineDash(h || []), t.lineDashOffset = d, f ? (t.lineWidth = 2 * c, t.lineJoin = u || "round") : (t.lineWidth = c, t.lineJoin = u || "bevel");
             let p = e.endAngle;
             if (s) {
-                qh(t, e, n, i, p, r);
+                Kh(t, e, n, i, p, r);
                 for (let e = 0; e < s; ++e) t.stroke();
                 isNaN(a) || (p = o + (a % ya || ya))
             }
             f && function(t, e, n) {
                 const {
                     startAngle: i,
                     pixelMargin: r,
                     x: s,
                     y: o,
                     outerRadius: a,
                     innerRadius: l
                 } = e;
                 let c = r / a;
                 t.beginPath(), t.arc(s, o, a, i - c, n + c), l > r ? (c = r / l, t.arc(s, o, l, n + c, i - c, !0)) : t.arc(s, o, r, n + _a, i - _a), t.closePath(), t.clip()
-            }(t, e, p), s || (qh(t, e, n, i, p, r), t.stroke())
+            }(t, e, p), s || (Kh(t, e, n, i, p, r), t.stroke())
         }
         ho(Hh, "defaults", ml), ho(Hh, "instances", Uh), ho(Hh, "overrides", hl), ho(Hh, "registry", mh), ho(Hh, "version", "4.4.2"), ho(Hh, "getChart", Vh);
         class Qh extends ih {
             constructor(t) {
                 super(), ho(this, "circumference", void 0), ho(this, "endAngle", void 0), ho(this, "fullCircles", void 0), ho(this, "innerRadius", void 0), ho(this, "outerRadius", void 0), ho(this, "pixelMargin", void 0), ho(this, "startAngle", void 0), this.options = void 0, this.circumference = void 0, this.startAngle = void 0, this.endAngle = void 0, this.innerRadius = void 0, this.outerRadius = void 0, this.pixelMargin = 0, this.fullCircles = 0, t && Object.assign(this, t)
             }
             inRange(t, e, n) {
@@ -21689,20 +21768,20 @@
                         const {
                             fullCircles: s,
                             startAngle: o,
                             circumference: a
                         } = e;
                         let l = e.endAngle;
                         if (s) {
-                            qh(t, e, n, i, l, r);
+                            Kh(t, e, n, i, l, r);
                             for (let e = 0; e < s; ++e) t.fill();
                             isNaN(a) || (l = o + (a % ya || ya))
                         }
-                        qh(t, e, n, i, l, r), t.fill()
-                    }(t, this, a, r, s), Kh(t, this, a, r, s), t.restore()
+                        Kh(t, e, n, i, l, r), t.fill()
+                    }(t, this, a, r, s), qh(t, this, a, r, s), t.restore()
             }
         }
 
         function Gh(t, e) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : e;
             t.lineCap = Jo(n.borderCapStyle, e.borderCapStyle), t.setLineDash(Jo(n.borderDash, e.borderDash)), t.lineDashOffset = Jo(n.borderDashOffset, e.borderDashOffset), t.lineJoin = Jo(n.borderJoinStyle, e.borderJoinStyle), t.lineWidth = Jo(n.borderWidth, e.borderWidth), t.strokeStyle = Jo(n.borderColor, e.borderColor)
         }
@@ -22287,15 +22366,15 @@
                         return l && (r = Ba(Va(e, s.axis, o).lo, 0, n - 1)), i = c ? Ba(Va(e, s.axis, a).hi + 1, r, n) - r : n - r, {
                             start: r,
                             count: i
                         }
                     }(a, l);
                     if (h <= (n.threshold || 4 * i)) return void Sd(e);
                     let d;
-                    switch (qo(s) && (e._data = l, delete e.data, Object.defineProperty(e, "data", {
+                    switch (Ko(s) && (e._data = l, delete e.data, Object.defineProperty(e, "data", {
                             configurable: !0,
                             enumerable: !0,
                             get: function() {
                                 return this._decimated
                             },
                             set: function(t) {
                                 this._data = t
@@ -22340,15 +22419,15 @@
                                     v = t[y].x - b;
                                 for (r = e; r < e + n; ++r) {
                                     s = t[r], o = (s.x - b) / v * i, a = s.y;
                                     const e = 0 | o;
                                     if (e === l) a < d ? (d = a, c = r) : a > f && (f = a, u = r), p = (g * p + s.x) / ++g;
                                     else {
                                         const n = r - 1;
-                                        if (!qo(c) && !qo(u)) {
+                                        if (!Ko(c) && !Ko(u)) {
                                             const e = Math.min(c, u),
                                                 i = Math.max(c, u);
                                             e !== h && e !== n && m.push({
                                                 ...t[e],
                                                 x: p
                                             }), i !== h && i !== n && m.push({
                                                 ...t[i],
@@ -22394,15 +22473,15 @@
         function Ed(t, e, n, i) {
             return t && e ? i(t[n], e[n]) : t ? t[n] : e ? e[n] : 0
         }
 
         function Dd(t, e) {
             let n = [],
                 i = !1;
-            return Ko(t) ? (i = !0, n = t) : n = function(t, e) {
+            return qo(t) ? (i = !0, n = t) : n = function(t, e) {
                 const {
                     x: n = null,
                     y: i = null
                 } = t || {}, r = e.points, s = [];
                 return e.segments.forEach((t => {
                     let {
                         start: e,
@@ -22952,20 +23031,20 @@
                             },
                             rtl: r
                         }
                     } = this,
                     s = Mc(r, this.left, this.width);
                 if (this.isHorizontal()) {
                     let r = 0,
-                        o = Ka(n, this.left + i, this.right - this.lineWidths[r]);
-                    for (const a of e) r !== a.row && (r = a.row, o = Ka(n, this.left + i, this.right - this.lineWidths[r])), a.top += this.top + t + i, a.left = s.leftForLtr(s.x(o), a.width), o += a.width + i
+                        o = qa(n, this.left + i, this.right - this.lineWidths[r]);
+                    for (const a of e) r !== a.row && (r = a.row, o = qa(n, this.left + i, this.right - this.lineWidths[r])), a.top += this.top + t + i, a.left = s.leftForLtr(s.x(o), a.width), o += a.width + i
                 } else {
                     let r = 0,
-                        o = Ka(n, this.top + t + i, this.bottom - this.columnSizes[r].height);
-                    for (const a of e) a.col !== r && (r = a.col, o = Ka(n, this.top + t + i, this.bottom - this.columnSizes[r].height)), a.top = o, a.left += this.left + i, a.left = s.leftForLtr(s.x(a.left), a.width), o += a.height + i
+                        o = qa(n, this.top + t + i, this.bottom - this.columnSizes[r].height);
+                    for (const a of e) a.col !== r && (r = a.col, o = qa(n, this.top + t + i, this.bottom - this.columnSizes[r].height)), a.top = o, a.left += this.left + i, a.left = s.leftForLtr(s.x(a.left), a.width), o += a.height + i
                 }
             }
             isHorizontal() {
                 return "top" === this.options.position || "bottom" === this.options.position
             }
             draw() {
                 if (this.options.display) {
@@ -22989,31 +23068,31 @@
                 this.drawTitle(), i.textAlign = a.textAlign("left"), i.textBaseline = "middle", i.lineWidth = .5, i.font = l.string;
                 const {
                     boxWidth: f,
                     boxHeight: p,
                     itemHeight: g
                 } = Wd(s, u), m = this.isHorizontal(), y = this._computeTitleHeight();
                 d = m ? {
-                    x: Ka(r, this.left + c, this.right - n[0]),
+                    x: qa(r, this.left + c, this.right - n[0]),
                     y: this.top + c + y,
                     line: 0
                 } : {
                     x: this.left + c,
-                    y: Ka(r, this.top + y + c, this.bottom - e[0].height),
+                    y: qa(r, this.top + y + c, this.bottom - e[0].height),
                     line: 0
                 }, Ic(this.ctx, t.textDirection);
                 const b = g + c;
                 this.legendItems.forEach(((v, x) => {
                     i.strokeStyle = v.fontColor, i.fillStyle = v.fontColor;
                     const _ = i.measureText(v.text).width,
                         w = a.textAlign(v.textAlign || (v.textAlign = s.textAlign)),
                         S = f + h + _;
                     let T = d.x,
                         k = d.y;
-                    a.setWidth(this.width), m ? x > 0 && T + S + c > this.right && (k = d.y += b, d.line++, T = d.x = Ka(r, this.left + c, this.right - n[d.line])) : x > 0 && k + b > this.bottom && (T = d.x = T + e[d.line].width + c, d.line++, k = d.y = Ka(r, this.top + y + c, this.bottom - e[d.line].height));
+                    a.setWidth(this.width), m ? x > 0 && T + S + c > this.right && (k = d.y += b, d.line++, T = d.x = qa(r, this.left + c, this.right - n[d.line])) : x > 0 && k + b > this.bottom && (T = d.x = T + e[d.line].width + c, d.line++, k = d.y = qa(r, this.top + y + c, this.bottom - e[d.line].height));
                     if (function(t, e, n) {
                             if (isNaN(f) || f <= 0 || isNaN(p) || p < 0) return;
                             i.save();
                             const r = Jo(n.lineWidth, 1);
                             if (i.fillStyle = Jo(n.fillStyle, o), i.lineCap = Jo(n.lineCap, "butt"), i.lineDashOffset = Jo(n.lineDashOffset, 0), i.lineJoin = Jo(n.lineJoin, "miter"), i.lineWidth = r, i.strokeStyle = Jo(n.strokeStyle, o), i.setLineDash(Jo(n.lineDash, [])), s.usePointStyle) {
                                 const o = {
                                         radius: p * Math.SQRT2 / 2,
@@ -23057,21 +23136,21 @@
                 const r = Mc(t.rtl, this.left, this.width),
                     s = this.ctx,
                     o = e.position,
                     a = n.size / 2,
                     l = i.top + a;
                 let c, u = this.left,
                     h = this.width;
-                if (this.isHorizontal()) h = Math.max(...this.lineWidths), c = this.top + l, u = Ka(t.align, u, this.right - h);
+                if (this.isHorizontal()) h = Math.max(...this.lineWidths), c = this.top + l, u = qa(t.align, u, this.right - h);
                 else {
                     const e = this.columnSizes.reduce(((t, e) => Math.max(t, e.height)), 0);
-                    c = l + Ka(t.align, this.top, this.bottom - e - t.labels.padding - this._computeTitleHeight())
+                    c = l + qa(t.align, this.top, this.bottom - e - t.labels.padding - this._computeTitleHeight())
                 }
-                const d = Ka(o, u, u + h);
-                s.textAlign = r.textAlign(qa(o)), s.textBaseline = "middle", s.strokeStyle = e.color, s.fillStyle = e.color, s.font = n.string, Ol(s, e.text, d, c, n)
+                const d = qa(o, u, u + h);
+                s.textAlign = r.textAlign(Ka(o)), s.textBaseline = "middle", s.strokeStyle = e.color, s.fillStyle = e.color, s.font = n.string, Ol(s, e.text, d, c, n)
             }
             _computeTitleHeight() {
                 const t = this.options.title,
                     e = Ul(t.font),
                     n = Rl(t.padding);
                 return t.display ? e.lineHeight + n.height : 0
             }
@@ -23198,15 +23277,15 @@
             constructor(t) {
                 super(), this.chart = t.chart, this.options = t.options, this.ctx = t.ctx, this._padding = void 0, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.width = void 0, this.height = void 0, this.position = void 0, this.weight = void 0, this.fullSize = void 0
             }
             update(t, e) {
                 const n = this.options;
                 if (this.left = 0, this.top = 0, !n.display) return void(this.width = this.height = this.right = this.bottom = 0);
                 this.width = this.right = t, this.height = this.bottom = e;
-                const i = Ko(n.text) ? n.text.length : 1;
+                const i = qo(n.text) ? n.text.length : 1;
                 this._padding = Rl(n.padding);
                 const r = i * Ul(n.font).lineHeight + this._padding.height;
                 this.isHorizontal() ? this.height = r : this.width = r
             }
             isHorizontal() {
                 const t = this.options.position;
                 return "top" === t || "bottom" === t
@@ -23216,15 +23295,15 @@
                     top: e,
                     left: n,
                     bottom: i,
                     right: r,
                     options: s
                 } = this, o = s.align;
                 let a, l, c, u = 0;
-                return this.isHorizontal() ? (l = Ka(o, n, r), c = e + t, a = r - n) : ("left" === s.position ? (l = n + t, c = Ka(o, i, e), u = -.5 * ma) : (l = r - t, c = Ka(o, e, i), u = .5 * ma), a = i - e), {
+                return this.isHorizontal() ? (l = qa(o, n, r), c = e + t, a = r - n) : ("left" === s.position ? (l = n + t, c = qa(o, i, e), u = -.5 * ma) : (l = r - t, c = qa(o, e, i), u = .5 * ma), a = i - e), {
                     titleX: l,
                     titleY: c,
                     maxWidth: a,
                     rotation: u
                 }
             }
             draw() {
@@ -23239,21 +23318,21 @@
                         maxWidth: o,
                         rotation: a
                     } = this._drawArgs(i);
                 Ol(t, e.text, 0, 0, n, {
                     color: e.color,
                     maxWidth: o,
                     rotation: a,
-                    textAlign: qa(e.align),
+                    textAlign: Ka(e.align),
                     textBaseline: "middle",
                     translation: [r, s]
                 })
             }
         }
-        var qd = {
+        var Kd = {
             id: "title",
             _element: Xd,
             start(t, e, n) {
                 ! function(t, e) {
                     const n = new Xd({
                         ctx: t.ctx,
                         options: e,
@@ -23286,30 +23365,30 @@
                 color: "color"
             },
             descriptors: {
                 _scriptable: !0,
                 _indexable: !1
             }
         };
-        const Kd = new WeakMap;
+        const qd = new WeakMap;
         var Qd = {
             id: "subtitle",
             start(t, e, n) {
                 const i = new Xd({
                     ctx: t.ctx,
                     options: n,
                     chart: t
                 });
-                Ru.configure(t, i, n), Ru.addBox(t, i), Kd.set(t, i)
+                Ru.configure(t, i, n), Ru.addBox(t, i), qd.set(t, i)
             },
             stop(t) {
-                Ru.removeBox(t, Kd.get(t)), Kd.delete(t)
+                Ru.removeBox(t, qd.get(t)), qd.delete(t)
             },
             beforeUpdate(t, e, n) {
-                const i = Kd.get(t);
+                const i = qd.get(t);
                 Ru.configure(t, i, n), i.options = n
             },
             defaults: {
                 align: "center",
                 display: !1,
                 font: {
                     weight: "normal"
@@ -23366,15 +23445,15 @@
                     x: s,
                     y: o
                 }
             }
         };
 
         function Zd(t, e) {
-            return e && (Ko(e) ? Array.prototype.push.apply(t, e) : t.push(e)), t
+            return e && (qo(e) ? Array.prototype.push.apply(t, e) : t.push(e)), t
         }
 
         function Jd(t) {
             return ("string" === typeof t || t instanceof String) && t.indexOf("\n") > -1 ? t.split("\n") : t
         }
 
         function tf(t, e) {
@@ -23536,15 +23615,15 @@
             beforeBody: $o,
             beforeLabel: $o,
             label(t) {
                 if (this && this.options && "dataset" === this.options.mode) return t.label + ": " + t.formattedValue || t.formattedValue;
                 let e = t.dataset.label || "";
                 e && (e += ": ");
                 const n = t.formattedValue;
-                return qo(n) || (e += n), e
+                return Ko(n) || (e += n), e
             },
             labelColor(t) {
                 const e = t.chart.getDatasetMeta(t.datasetIndex).controller.getStyle(t.dataIndex);
                 return {
                     borderColor: e.borderColor,
                     backgroundColor: e.backgroundColor,
                     borderWidth: e.borderWidth,
@@ -24009,15 +24088,15 @@
             ff = Object.freeze({
                 __proto__: null,
                 Colors: wd,
                 Decimation: kd,
                 Filler: jd,
                 Legend: $d,
                 SubTitle: Qd,
-                Title: qd,
+                Title: Kd,
                 Tooltip: df
             });
 
         function pf(t, e, n, i) {
             const r = t.indexOf(e);
             if (-1 === r) return ((t, e, n, i) => ("string" === typeof e ? (n = t.push(e) - 1, i.unshift({
                 index: n,
@@ -24044,15 +24123,15 @@
                         }
                         of e) t[n] === i && t.splice(n, 1);
                     this._addedLabels = []
                 }
                 super.init(t)
             }
             parse(t, e) {
-                if (qo(t)) return null;
+                if (Ko(t)) return null;
                 const n = this.getLabels();
                 return ((t, e) => null === t ? null : Ba(Math.round(t), 0, e))(e = isFinite(e) && n[e] === t ? e : pf(n, t, Jo(e, t), this._addedLabels), n.length - 1)
             }
             determineDataLimits() {
                 const {
                     minDefined: t,
                     maxDefined: e
@@ -24111,30 +24190,30 @@
                 } = t,
                 d = r || 1,
                 f = c - 1,
                 {
                     min: p,
                     max: g
                 } = e,
-                m = !qo(s),
-                y = !qo(o),
-                b = !qo(l),
+                m = !Ko(s),
+                y = !Ko(o),
+                b = !Ko(l),
                 v = (g - p) / (u + 1);
             let x, _, w, S, T = Ia((g - p) / f / d) * d;
             if (T < 1e-14 && !m && !y) return [{
                 value: p
             }, {
                 value: g
             }];
-            S = Math.ceil(g / T) - Math.floor(p / T), S > f && (T = Ia(S * T / f / d) * d), qo(a) || (x = Math.pow(10, a), T = Math.ceil(T * x) / x), "ticks" === i ? (_ = Math.floor(p / T) * T, w = Math.ceil(g / T) * T) : (_ = p, w = g), m && y && r && function(t, e) {
+            S = Math.ceil(g / T) - Math.floor(p / T), S > f && (T = Ia(S * T / f / d) * d), Ko(a) || (x = Math.pow(10, a), T = Math.ceil(T * x) / x), "ticks" === i ? (_ = Math.floor(p / T) * T, w = Math.ceil(g / T) * T) : (_ = p, w = g), m && y && r && function(t, e) {
                 const n = Math.round(t);
                 return n - e <= t && n + e >= t
             }((o - s) / r, T / 1e3) ? (S = Math.round(Math.min((o - s) / T, c)), T = (o - s) / S, _ = s, w = o) : b ? (_ = m ? s : _, w = y ? o : w, S = l - 1, T = (w - _) / S) : (S = (w - _) / T, S = Ma(S, Math.round(S), T / 1e3) ? Math.round(S) : Math.ceil(S));
             const k = Math.max(Aa(T), Aa(_));
-            x = Math.pow(10, qo(a) ? k : a), _ = Math.round(_ * x) / x, w = Math.round(w * x) / x;
+            x = Math.pow(10, Ko(a) ? k : a), _ = Math.round(_ * x) / x, w = Math.round(w * x) / x;
             let M = 0;
             for (m && (h && _ !== s ? (n.push({
                     value: s
                 }), _ < s && M++, Ma(Math.round((_ + M * T) * x) / x, s, bf(s, v, t)) && M++) : _ < s && M++); M < S; ++M) {
                 const t = Math.round((_ + M * T) * x) / x;
                 if (y && t > o) break;
                 n.push({
@@ -24164,15 +24243,15 @@
             }
         });
         class vf extends fh {
             constructor(t) {
                 super(t), this.start = void 0, this.end = void 0, this._startValue = void 0, this._endValue = void 0, this._valueRange = 0
             }
             parse(t, e) {
-                return qo(t) || ("number" === typeof t || t instanceof Number) && !isFinite(+t) ? null : +t
+                return Ko(t) || ("number" === typeof t || t instanceof Number) && !isFinite(+t) ? null : +t
             }
             handleTickRangeOptions() {
                 const {
                     beginAtZero: t
                 } = this.options, {
                     minDefined: e,
                     maxDefined: n
@@ -24400,15 +24479,15 @@
                 o = t.options.pointLabels,
                 a = o.centerPointLabels ? ma / s : 0;
             for (let h = 0; h < s; h++) {
                 const s = o.setContext(t.getPointLabelContext(h));
                 r[h] = s.padding;
                 const d = t.getPointPosition(h, t.drawingArea + r[h], a),
                     f = Ul(s.font),
-                    p = (l = t.ctx, c = f, u = Ko(u = t._pointLabels[h]) ? u : [u], {
+                    p = (l = t.ctx, c = f, u = qo(u = t._pointLabels[h]) ? u : [u], {
                         w: bl(l, c.string, u),
                         h: u.length * c.lineHeight
                     });
                 i[h] = p;
                 const g = za(t.getIndexAngle(h) + a),
                     m = Math.round(Ca(g));
                 Of(n, e, g, Ef(m, d.x, p.w, 0, 180), Ef(m, d.y, p.h, 90, 270))
@@ -24507,15 +24586,15 @@
                 left: i,
                 top: r,
                 right: s,
                 bottom: o
             } = n, {
                 backdropColor: a
             } = e;
-            if (!qo(a)) {
+            if (!Ko(a)) {
                 const n = Bl(e.borderRadius),
                     l = Rl(e.backdropPadding);
                 t.fillStyle = a;
                 const c = i - l.left,
                     u = r - l.top,
                     h = s - i + l.width,
                     d = o - r + l.height;
@@ -24581,20 +24660,20 @@
             setCenterPoint(t, e, n, i) {
                 this.xCenter += Math.floor((t - e) / 2), this.yCenter += Math.floor((n - i) / 2), this.drawingArea -= Math.min(this.drawingArea / 2, Math.max(t, e, n, i))
             }
             getIndexAngle(t) {
                 return za(t * (ya / (this._pointLabels.length || 1)) + Oa(this.options.startAngle || 0))
             }
             getDistanceFromCenterForValue(t) {
-                if (qo(t)) return NaN;
+                if (Ko(t)) return NaN;
                 const e = this.drawingArea / (this.max - this.min);
                 return this.options.reverse ? (this.max - t) * e : (t - this.min) * e
             }
             getValueForDistanceFromCenter(t) {
-                if (qo(t)) return NaN;
+                if (Ko(t)) return NaN;
                 const e = t / (this.drawingArea / (this.max - this.min));
                 return this.options.reverse ? this.max - e : this.min + e
             }
             getPointLabelContext(t) {
                 const e = this._pointLabels || [];
                 if (t >= 0 && t < e.length) {
                     const n = e[t];
@@ -24823,15 +24902,15 @@
             Nf = Object.keys(zf);
 
         function Bf(t, e) {
             return t - e
         }
 
         function Rf(t, e) {
-            if (qo(e)) return null;
+            if (Ko(e)) return null;
             const n = t._adapter,
                 {
                     parser: i,
                     round: r,
                     isoWeekday: s
                 } = t._parseOpts;
             let o = e;
@@ -25173,16 +25252,16 @@
             LinearScale: xf,
             LogarithmicScale: Mf,
             RadialLinearScale: Lf,
             TimeScale: Wf,
             TimeSeriesScale: Yf
         })];
         var Xf = i(895),
-            qf = i.n(Xf);
-        const Kf = t => t && t.enabled && t.modifierKey,
+            Kf = i.n(Xf);
+        const qf = t => t && t.enabled && t.modifierKey,
             Qf = (t, e) => t && e[t + "Key"],
             Gf = (t, e) => t && !e[t + "Key"];
 
         function Zf(t, e, n) {
             return void 0 === t || ("string" === typeof t ? -1 !== t.indexOf(e) : "function" === typeof t && -1 !== t({
                 chart: n
             }).indexOf(e))
@@ -25589,15 +25668,15 @@
 
         function Dp(t, e) {
             const n = np(t),
                 {
                     pan: i,
                     zoom: r = {}
                 } = n.options;
-            if (0 !== e.button || Qf(Kf(i), e) || Gf(Kf(r.drag), e)) return ea(r.onZoomRejected, [{
+            if (0 !== e.button || Qf(qf(i), e) || Gf(qf(r.drag), e)) return ea(r.onZoomRejected, [{
                 chart: t,
                 event: e
             }]);
             !1 !== Ep(t, e, r) && (n.dragStart = e, kp(t, t.canvas, "mousemove", Mp), kp(t, window.document, "keydown", Ip))
         }
 
         function Op(t, e, n, i) {
@@ -25657,15 +25736,15 @@
                     onZoomComplete: n
                 },
                 options: {
                     zoom: i
                 }
             } = np(t);
             if (! function(t, e, n) {
-                    if (Gf(Kf(n.wheel), e)) ea(n.onZoomRejected, [{
+                    if (Gf(qf(n.wheel), e)) ea(n.onZoomRejected, [{
                         chart: t,
                         event: e
                     }]);
                     else if (!1 !== Ep(t, e, n) && (e.cancelable && e.preventDefault(), void 0 !== e.deltaY)) return !0
                 }(t, e, i)) return;
             const r = e.target.getBoundingClientRect(),
                 s = 1 + (e.deltaY >= 0 ? -i.wheel.speed : i.wheel.speed);
@@ -25694,15 +25773,15 @@
             return function(n, i) {
                 const {
                     pan: r,
                     zoom: s = {}
                 } = e.options;
                 if (!r || !r.enabled) return !1;
                 const o = i && i.srcEvent;
-                return !o || (!(!e.panning && "mouse" === i.pointerType && (Gf(Kf(r), o) || Qf(Kf(s.drag), o))) || (ea(r.onPanRejected, [{
+                return !o || (!(!e.panning && "mouse" === i.pointerType && (Gf(qf(r), o) || Qf(qf(s.drag), o))) || (ea(r.onPanRejected, [{
                     chart: t,
                     event: i
                 }]), !1))
             }
         }
 
         function Lp(t, e, n) {
@@ -25746,22 +25825,22 @@
         function Bp(t, e) {
             const n = np(t),
                 i = t.canvas,
                 {
                     pan: r,
                     zoom: s
                 } = e,
-                o = new(qf().Manager)(i);
-            s && s.pinch.enabled && (o.add(new(qf().Pinch)), o.on("pinchstart", (() => function(t, e) {
+                o = new(Kf().Manager)(i);
+            s && s.pinch.enabled && (o.add(new(Kf().Pinch)), o.on("pinchstart", (() => function(t, e) {
                 e.options.zoom.pinch.enabled && (e.scale = 1)
             }(0, n))), o.on("pinch", (e => Lp(t, n, e))), o.on("pinchend", (e => function(t, e, n) {
                 e.scale && (Lp(t, e, n), e.scale = null, ea(e.options.zoom.onZoomComplete, [{
                     chart: t
                 }]))
-            }(t, n, e)))), r && r.enabled && (o.add(new(qf().Pan)({
+            }(t, n, e)))), r && r.enabled && (o.add(new(Kf().Pan)({
                 threshold: r.threshold,
                 enable: Fp(t, n)
             })), o.on("panstart", (e => function(t, e, n) {
                 const {
                     enabled: i,
                     onPanStart: r,
                     onPanRejected: s
@@ -25830,15 +25909,15 @@
                     pinch: {
                         enabled: !1
                     },
                     mode: "xy"
                 }
             },
             start: function(t, e, n) {
-                np(t).options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), qf() && Bp(t, n), t.pan = (e, n, i) => wp(t, e, n, i), t.zoom = (e, n) => bp(t, e, n), t.zoomRect = (e, n, i) => vp(t, e, n, i), t.zoomScale = (e, n, i) => function(t, e, n) {
+                np(t).options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), Kf() && Bp(t, n), t.pan = (e, n, i) => wp(t, e, n, i), t.zoom = (e, n) => bp(t, e, n), t.zoomRect = (e, n, i) => vp(t, e, n, i), t.zoomScale = (e, n, i) => function(t, e, n) {
                     let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
                     pp(t, np(t)), sp(t.scales[e], n, void 0, !0), t.update(i)
                 }(t, e, n, i), t.resetZoom = e => function(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "default";
                     const n = np(t),
                         i = pp(t, n);
                     na(t.scales, (function(t) {
@@ -25887,15 +25966,15 @@
             },
             afterDraw(t, e, n) {
                 Rp(t, "afterDraw", n)
             },
             stop: function(t) {
                 ! function(t) {
                     Tp(t, "mousedown"), Tp(t, "mousemove"), Tp(t, "mouseup"), Tp(t, "wheel"), Tp(t, "click"), Tp(t, "keydown")
-                }(t), qf() && function(t) {
+                }(t), Kf() && function(t) {
                         const e = Np.get(t);
                         e && (e.remove("pinchstart"), e.remove("pinch"), e.remove("pinchend"), e.remove("panstart"), e.remove("pan"), e.remove("panend"), e.destroy(), Np.delete(t))
                     }(t),
                     function(t) {
                         ep.delete(t)
                     }(t)
             },
@@ -25980,24 +26059,24 @@
             }), [o]), (0, f.useEffect)((() => (m(), () => y())), []), f.createElement("canvas", Object.assign({
                 ref: p,
                 role: "img",
                 height: n,
                 width: i
             }, d), u)
         }
-        const qp = (0, f.forwardRef)(Xp);
+        const Kp = (0, f.forwardRef)(Xp);
 
-        function Kp(t, e) {
-            return Hh.register(e), (0, f.forwardRef)(((e, n) => f.createElement(qp, Object.assign({}, e, {
+        function qp(t, e) {
+            return Hh.register(e), (0, f.forwardRef)(((e, n) => f.createElement(Kp, Object.assign({}, e, {
                 ref: n,
                 type: t
             }))))
         }
-        const Qp = Kp("line", hu),
-            Gp = Kp("scatter", gu);
+        const Qp = qp("line", hu),
+            Gp = qp("scatter", gu);
 
         function Zp(t, e) {
             return {
                 labels: Object.keys(t[Object.keys(t)[0]].data),
                 datasets: Object.entries(t).map(((t, n) => {
                     let [i, r] = t;
                     return {
@@ -26011,23 +26090,24 @@
                         borderColor: r.color,
                         pointRadius: r.point_radius,
                         borderDash: r.border_dash
                     }
                 }))
             }
         }
+        var Jp = i(373);
 
-        function Jp(t, e) {
+        function tg(t, e) {
             return {
                 responsive: !0,
                 indexAxis: "x",
                 animation: {
                     duration: 0
                 },
-                onHover: tg(t),
+                onHover: eg(t),
                 plugins: {
                     zoom: {
                         zoom: {
                             wheel: {
                                 enabled: !0
                             },
                             mode: "xy"
@@ -26042,43 +26122,43 @@
                             },
                             y: {
                                 min: "original",
                                 max: "original"
                             }
                         }
                     },
-                    title: eg(t),
-                    legend: ng(t),
-                    tooltip: rg(t, e)
+                    title: ng(t),
+                    legend: ig(t),
+                    tooltip: og(t, e)
                 },
-                scales: ig(t, e)
+                scales: sg(t, e)
             }
         }
 
-        function tg(t) {
+        function eg(t) {
             return (e, n) => {
                 let i = "default";
                 if (n.length > 0) {
                     i = function(t, e) {
                         if (e.fixed_lines.includes(t)) return "default";
                         return "crosshair"
                     }(e.chart.data.datasets[n[0].datasetIndex].label, t)
                 }
                 e.native.target.style.cursor = i
             }
         }
 
-        function eg(t) {
+        function ng(t) {
             return {
                 display: Boolean(t.title),
                 text: t.title
             }
         }
 
-        function ng(t) {
+        function ig(t) {
             return {
                 display: t.legend,
                 position: t.legend_position,
                 align: t.legend_align,
                 labels: {
                     boxWidth: 16,
                     boxHeight: 8,
@@ -26092,31 +26172,45 @@
                 },
                 onHover: (t, e, n) => {
                     t.native.target.style.cursor = e ? "pointer" : "default"
                 }
             }
         }
 
-        function ig(t, e) {
+        function rg(t, e, n) {
+            return "linear" === n.x_type ? (0, Jp.Ay)(t) : this.getLabelForValue(t)
+        }
+
+        function sg(t, e) {
             const n = {
                 display: !0,
                 type: t.x_type,
+                ticks: {
+                    callback: function(e, n) {
+                        return rg.call(this, e, n, t)
+                    }
+                },
                 title: {
                     display: Boolean(t.x_label),
                     text: t.x_label
                 },
                 grid: {
                     display: t.x_grid,
                     color: e.fadedText05
                 }
             };
             t.x_labels && (n.min = t.x_labels[0], n.max = t.x_labels[t.x_labels.length - 1]);
             const i = {
                 display: !0,
                 type: t.y_type,
+                ticks: {
+                    callback: function(e, n) {
+                        return rg.call(this, e, n, t)
+                    }
+                },
                 title: {
                     display: Boolean(t.y_label),
                     text: t.y_label
                 },
                 grid: {
                     display: t.y_grid,
                     color: e.fadedText05
@@ -26124,15 +26218,15 @@
             };
             return t.y_labels && (i.labels = t.y_labels, i.min = t.y_labels[0], i.max = t.y_labels[t.y_labels.length - 1]), {
                 x: n,
                 y: i
             }
         }
 
-        function rg(t, e) {
+        function og(t, e) {
             return {
                 filter: function(t) {
                     return 0 !== t.dataset.pointRadius
                 },
                 callbacks: {
                     title: function(e) {
                         if (0 === e.length) return "";
@@ -26143,17 +26237,17 @@
                         const e = t.parsed.x.toFixed(2),
                             n = t.parsed.y.toFixed(2);
                         return "".concat(e, ", ").concat(n)
                     }
                 }
             }
         }
-        var sg = i(579);
+        var ag = i(579);
         Hh.register(...$f, Up);
-        const og = class extends ao {
+        const lg = class extends ao {
             constructor(t) {
                 super(t), this.downHandler = t => {
                     const e = $p(this.chartRef.current, t);
                     if (e.length > 0) {
                         const t = this.chartRef.current.data.datasets[e[0].datasetIndex].label;
                         if (this.props.args.options.fixed_lines && this.props.args.options.fixed_lines.includes(t)) return;
                         this.setState({
@@ -26181,40 +26275,40 @@
                             activePoint: null
                         }), this.togglePan(!0), ro.setComponentValue(this.state.originalData)
                     }
                 }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.state = {
                     activePoint: null,
                     originalData: t.args.data,
                     chartData: Zp(t.args.data, t.args.options.colors),
-                    options: Jp(t.args.options, t.theme)
+                    options: tg(t.args.options, t.theme)
                 }
             }
             componentDidUpdate(t) {
                 ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                     originalData: this.props.args.data,
                     chartData: Zp(this.props.args.data, this.props.args.options),
-                    options: Jp(this.props.args.options, this.props.theme)
+                    options: tg(this.props.args.options, this.props.theme)
                 })
             }
             togglePan(t) {
                 this.chartRef.current.options.plugins.zoom.pan.enabled = t, this.chartRef.current.update("none")
             }
             render() {
-                return (0, sg.jsx)(Qp, {
+                return (0, ag.jsx)(Qp, {
                     ref: this.chartRef,
                     data: this.state.chartData,
                     options: this.state.options,
                     onPointerDown: this.downHandler,
                     onPointerUp: this.upHandler,
                     onPointerMove: this.moveHandler
                 })
             }
         };
 
-        function ag(t, e) {
+        function cg(t, e) {
             return {
                 labels: e && e.x_labels ? e.x_labels : [],
                 datasets: Object.entries(t).map(((t, n) => {
                     let [i, r] = t;
                     const s = r.x.map(((t, e) => ({
                         x: t,
                         y: r.y[e]
@@ -26231,15 +26325,15 @@
                         pointRadius: r.point_radius,
                         borderDash: r.border_dash
                     }
                 }))
             }
         }
         Hh.register(...$f, Up);
-        const lg = class extends ao {
+        const ug = class extends ao {
                 constructor(t) {
                     super(t), this.downHandler = t => {
                         const e = $p(this.chartRef.current, t);
                         if (e.length > 0) {
                             const t = this.chartRef.current.data.datasets[e[0].datasetIndex].label;
                             if (this.props.args.options.fixed_lines && this.props.args.options.fixed_lines.includes(t)) return;
                             this.setState({
@@ -26278,69 +26372,69 @@
                             this.state.originalData[i].x[n] = r, this.state.originalData[i].y[n] = s, ro.setComponentValue(this.state.originalData), this.setState({
                                 activePoint: null
                             }), this.togglePan(!0)
                         }
                     }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.state = {
                         activePoint: null,
                         originalData: t.args.data,
-                        chartData: ag(t.args.data, t.args.options.colors),
-                        options: Jp(t.args.options, t.theme)
+                        chartData: cg(t.args.data, t.args.options.colors),
+                        options: tg(t.args.options, t.theme)
                     }
                 }
                 componentDidUpdate(t) {
                     ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                         originalData: this.props.args.data,
-                        chartData: ag(this.props.args.data, this.props.args.options),
-                        options: Jp(this.props.args.options, this.props.theme)
+                        chartData: cg(this.props.args.data, this.props.args.options),
+                        options: tg(this.props.args.options, this.props.theme)
                     })
                 }
                 togglePan(t) {
                     this.chartRef.current.options.plugins.zoom.pan.enabled = t, this.chartRef.current.update("none")
                 }
                 render() {
-                    return (0, sg.jsx)(Gp, {
+                    return (0, ag.jsx)(Gp, {
                         ref: this.chartRef,
                         data: this.state.chartData,
                         options: this.state.options,
                         onPointerDown: this.downHandler,
                         onPointerUp: this.upHandler,
                         onPointerMove: this.moveHandler
                     })
                 }
             },
             {
-                abs: cg,
-                cos: ug,
-                sin: hg,
-                acos: dg,
-                atan2: fg,
-                sqrt: pg,
-                pow: gg
+                abs: hg,
+                cos: dg,
+                sin: fg,
+                acos: pg,
+                atan2: gg,
+                sqrt: mg,
+                pow: yg
             } = Math;
 
-        function mg(t) {
-            return t < 0 ? -gg(-t, 1 / 3) : gg(t, 1 / 3)
+        function bg(t) {
+            return t < 0 ? -yg(-t, 1 / 3) : yg(t, 1 / 3)
         }
-        const yg = Math.PI,
-            bg = 2 * yg,
-            vg = yg / 2,
-            xg = Number.MAX_SAFE_INTEGER || 9007199254740991,
-            _g = Number.MIN_SAFE_INTEGER || -9007199254740991,
-            wg = {
+        const vg = Math.PI,
+            xg = 2 * vg,
+            _g = vg / 2,
+            wg = Number.MAX_SAFE_INTEGER || 9007199254740991,
+            Sg = Number.MIN_SAFE_INTEGER || -9007199254740991,
+            Tg = {
                 x: 0,
                 y: 0,
                 z: 0
             },
-            Sg = {
+            kg = {
                 Tvalues: [-.06405689286260563, .06405689286260563, -.1911188674736163, .1911188674736163, -.3150426796961634, .3150426796961634, -.4337935076260451, .4337935076260451, -.5454214713888396, .5454214713888396, -.6480936519369755, .6480936519369755, -.7401241915785544, .7401241915785544, -.820001985973903, .820001985973903, -.8864155270044011, .8864155270044011, -.9382745520027328, .9382745520027328, -.9747285559713095, .9747285559713095, -.9951872199970213, .9951872199970213],
                 Cvalues: [.12793819534675216, .12793819534675216, .1258374563468283, .1258374563468283, .12167047292780339, .12167047292780339, .1155056680537256, .1155056680537256, .10744427011596563, .10744427011596563, .09761865210411388, .09761865210411388, .08619016153195327, .08619016153195327, .0733464814110803, .0733464814110803, .05929858491543678, .05929858491543678, .04427743881741981, .04427743881741981, .028531388628933663, .028531388628933663, .0123412297999872, .0123412297999872],
                 arcfn: function(t, e) {
                     const n = e(t);
                     let i = n.x * n.x + n.y * n.y;
-                    return "undefined" !== typeof n.z && (i += n.z * n.z), pg(i)
+                    return "undefined" !== typeof n.z && (i += n.z * n.z), mg(i)
                 },
                 compute: function(t, e, n) {
                     if (0 === t) return e[0].t = 0, e[0];
                     const i = e.length - 1;
                     if (1 === t) return e[i].t = 1, e[i];
                     const r = 1 - t;
                     let s = e;
@@ -26353,15 +26447,15 @@
                         };
                         return n && (e.z = r * s[0].z + t * s[1].z), e
                     }
                     if (i < 4) {
                         let e, o, a, l = r * r,
                             c = t * t,
                             u = 0;
-                        2 === i ? (s = [s[0], s[1], s[2], wg], e = l, o = r * t * 2, a = c) : 3 === i && (e = l * r, o = l * t * 3, a = r * c * 3, u = t * c);
+                        2 === i ? (s = [s[0], s[1], s[2], Tg], e = l, o = r * t * 2, a = c) : 3 === i && (e = l * r, o = l * t * 3, a = r * c * 3, u = t * c);
                         const h = {
                             x: e * s[0].x + o * s[1].x + a * s[2].x + u * s[3].x,
                             y: e * s[0].y + o * s[1].y + a * s[2].y + u * s[3].y,
                             t: t
                         };
                         return n && (h.z = e * s[0].z + o * s[1].z + a * s[2].z + u * s[3].z), h
                     }
@@ -26409,23 +26503,23 @@
                             y: s * (i[r + 1].y - i[r].y)
                         }, e && (n.z = s * (i[r + 1].z - i[r].z)), t.push(n);
                         n.push(t), i = t
                     }
                     return n
                 },
                 between: function(t, e, n) {
-                    return e <= t && t <= n || Sg.approximately(t, e) || Sg.approximately(t, n)
+                    return e <= t && t <= n || kg.approximately(t, e) || kg.approximately(t, n)
                 },
                 approximately: function(t, e, n) {
-                    return cg(t - e) <= (n || 1e-6)
+                    return hg(t - e) <= (n || 1e-6)
                 },
                 length: function(t) {
-                    const e = Sg.Tvalues.length;
+                    const e = kg.Tvalues.length;
                     let n = 0;
-                    for (let i, r = 0; r < e; r++) i = .5 * Sg.Tvalues[r] + .5, n += Sg.Cvalues[r] * Sg.arcfn(i, t);
+                    for (let i, r = 0; r < e; r++) i = .5 * kg.Tvalues[r] + .5, n += kg.Cvalues[r] * kg.arcfn(i, t);
                     return .5 * n
                 },
                 map: function(t, e, n, i, r) {
                     return i + (r - i) * ((t - e) / (n - e))
                 },
                 lerp: function(t, e, n) {
                     const i = {
@@ -26435,58 +26529,58 @@
                     return void 0 !== e.z && void 0 !== n.z && (i.z = e.z + t * (n.z - e.z)), i
                 },
                 pointToString: function(t) {
                     let e = t.x + "/" + t.y;
                     return "undefined" !== typeof t.z && (e += "/" + t.z), e
                 },
                 pointsToString: function(t) {
-                    return "[" + t.map(Sg.pointToString).join(", ") + "]"
+                    return "[" + t.map(kg.pointToString).join(", ") + "]"
                 },
                 copy: function(t) {
                     return JSON.parse(JSON.stringify(t))
                 },
                 angle: function(t, e, n) {
                     const i = e.x - t.x,
                         r = e.y - t.y,
                         s = n.x - t.x,
                         o = n.y - t.y;
-                    return fg(i * o - r * s, i * s + r * o)
+                    return gg(i * o - r * s, i * s + r * o)
                 },
                 round: function(t, e) {
                     const n = "" + t,
                         i = n.indexOf(".");
                     return parseFloat(n.substring(0, i + 1 + e))
                 },
                 dist: function(t, e) {
                     const n = t.x - e.x,
                         i = t.y - e.y;
-                    return pg(n * n + i * i)
+                    return mg(n * n + i * i)
                 },
                 closest: function(t, e) {
-                    let n, i, r = gg(2, 63);
+                    let n, i, r = yg(2, 63);
                     return t.forEach((function(t, s) {
-                        i = Sg.dist(e, t), i < r && (r = i, n = s)
+                        i = kg.dist(e, t), i < r && (r = i, n = s)
                     })), {
                         mdist: r,
                         mpos: n
                     }
                 },
                 abcratio: function(t, e) {
                     if (2 !== e && 3 !== e) return !1;
                     if ("undefined" === typeof t) t = .5;
                     else if (0 === t || 1 === t) return t;
-                    const n = gg(t, e) + gg(1 - t, e);
-                    return cg((n - 1) / n)
+                    const n = yg(t, e) + yg(1 - t, e);
+                    return hg((n - 1) / n)
                 },
                 projectionratio: function(t, e) {
                     if (2 !== e && 3 !== e) return !1;
                     if ("undefined" === typeof t) t = .5;
                     else if (0 === t || 1 === t) return t;
-                    const n = gg(1 - t, e);
-                    return n / (gg(t, e) + n)
+                    const n = yg(1 - t, e);
+                    return n / (yg(t, e) + n)
                 },
                 lli8: function(t, e, n, i, r, s, o, a) {
                     const l = (t - n) * (s - a) - (e - i) * (r - o);
                     return 0 != l && {
                         x: ((t * i - e * n) * (r - o) - (t - n) * (r * a - s * o)) / l,
                         y: ((t * i - e * n) * (s - a) - (e - i) * (r * a - s * o)) / l
                     }
@@ -26496,27 +26590,27 @@
                         s = t.y,
                         o = e.x,
                         a = e.y,
                         l = n.x,
                         c = n.y,
                         u = i.x,
                         h = i.y;
-                    return Sg.lli8(r, s, o, a, l, c, u, h)
+                    return kg.lli8(r, s, o, a, l, c, u, h)
                 },
                 lli: function(t, e) {
-                    return Sg.lli4(t, t.c, e, e.c)
+                    return kg.lli4(t, t.c, e, e.c)
                 },
                 makeline: function(t, e) {
-                    return new Pg(t.x, t.y, (t.x + e.x) / 2, (t.y + e.y) / 2, e.x, e.y)
+                    return new Lg(t.x, t.y, (t.x + e.x) / 2, (t.y + e.y) / 2, e.x, e.y)
                 },
                 findbbox: function(t) {
-                    let e = xg,
-                        n = xg,
-                        i = _g,
-                        r = _g;
+                    let e = wg,
+                        n = wg,
+                        i = Sg,
+                        r = Sg;
                     return t.forEach((function(t) {
                         const s = t.bbox();
                         e > s.x.min && (e = s.x.min), n > s.y.min && (n = s.y.min), i < s.x.max && (i = s.x.max), r < s.y.max && (r = s.y.max)
                     })), {
                         x: {
                             min: e,
                             mid: (e + i) / 2,
@@ -26528,66 +26622,66 @@
                             mid: (n + r) / 2,
                             max: r,
                             size: r - n
                         }
                     }
                 },
                 shapeintersections: function(t, e, n, i, r) {
-                    if (!Sg.bboxoverlap(e, i)) return [];
+                    if (!kg.bboxoverlap(e, i)) return [];
                     const s = [],
                         o = [t.startcap, t.forward, t.back, t.endcap],
                         a = [n.startcap, n.forward, n.back, n.endcap];
                     return o.forEach((function(e) {
                         e.virtual || a.forEach((function(i) {
                             if (i.virtual) return;
                             const o = e.intersects(i, r);
                             o.length > 0 && (o.c1 = e, o.c2 = i, o.s1 = t, o.s2 = n, s.push(o))
                         }))
                     })), s
                 },
                 makeshape: function(t, e, n) {
                     const i = e.points.length,
                         r = t.points.length,
-                        s = Sg.makeline(e.points[i - 1], t.points[0]),
-                        o = Sg.makeline(t.points[r - 1], e.points[0]),
+                        s = kg.makeline(e.points[i - 1], t.points[0]),
+                        o = kg.makeline(t.points[r - 1], e.points[0]),
                         a = {
                             startcap: s,
                             forward: t,
                             back: e,
                             endcap: o,
-                            bbox: Sg.findbbox([s, t, e, o]),
+                            bbox: kg.findbbox([s, t, e, o]),
                             intersections: function(t) {
-                                return Sg.shapeintersections(a, a.bbox, t, t.bbox, n)
+                                return kg.shapeintersections(a, a.bbox, t, t.bbox, n)
                             }
                         };
                     return a
                 },
                 getminmax: function(t, e, n) {
                     if (!n) return {
                         min: 0,
                         max: 0
                     };
-                    let i, r, s = xg,
-                        o = _g; - 1 === n.indexOf(0) && (n = [0].concat(n)), -1 === n.indexOf(1) && n.push(1);
+                    let i, r, s = wg,
+                        o = Sg; - 1 === n.indexOf(0) && (n = [0].concat(n)), -1 === n.indexOf(1) && n.push(1);
                     for (let a = 0, l = n.length; a < l; a++) i = n[a], r = t.get(i), r[e] < s && (s = r[e]), r[e] > o && (o = r[e]);
                     return {
                         min: s,
                         mid: (s + o) / 2,
                         max: o,
                         size: o - s
                     }
                 },
                 align: function(t, e) {
                     const n = e.p1.x,
                         i = e.p1.y,
-                        r = -fg(e.p2.y - i, e.p2.x - n);
+                        r = -gg(e.p2.y - i, e.p2.x - n);
                     return t.map((function(t) {
                         return {
-                            x: (t.x - n) * ug(r) - (t.y - i) * hg(r),
-                            y: (t.x - n) * hg(r) + (t.y - i) * ug(r)
+                            x: (t.x - n) * dg(r) - (t.y - i) * fg(r),
+                            y: (t.x - n) * fg(r) + (t.y - i) * dg(r)
                         }
                     }))
                 },
                 roots: function(t, e) {
                     e = e || {
                         p1: {
                             x: 0,
@@ -26595,72 +26689,72 @@
                         },
                         p2: {
                             x: 1,
                             y: 0
                         }
                     };
                     const n = t.length - 1,
-                        i = Sg.align(t, e),
+                        i = kg.align(t, e),
                         r = function(t) {
                             return 0 <= t && t <= 1
                         };
                     if (2 === n) {
                         const t = i[0].y,
                             e = i[1].y,
                             n = i[2].y,
                             s = t - 2 * e + n;
                         if (0 !== s) {
-                            const i = -pg(e * e - t * n),
+                            const i = -mg(e * e - t * n),
                                 o = -t + e;
                             return [-(i + o) / s, -(-i + o) / s].filter(r)
                         }
                         return e !== n && 0 === s ? [(2 * e - n) / (2 * e - 2 * n)].filter(r) : []
                     }
                     const s = i[0].y,
                         o = i[1].y,
                         a = i[2].y;
                     let l = 3 * o - s - 3 * a + i[3].y,
                         c = 3 * s - 6 * o + 3 * a,
                         u = -3 * s + 3 * o,
                         h = s;
-                    if (Sg.approximately(l, 0)) {
-                        if (Sg.approximately(c, 0)) return Sg.approximately(u, 0) ? [] : [-h / u].filter(r);
-                        const t = pg(u * u - 4 * c * h),
+                    if (kg.approximately(l, 0)) {
+                        if (kg.approximately(c, 0)) return kg.approximately(u, 0) ? [] : [-h / u].filter(r);
+                        const t = mg(u * u - 4 * c * h),
                             e = 2 * c;
                         return [(t - u) / e, (-u - t) / e].filter(r)
                     }
                     c /= l, u /= l, h /= l;
                     const d = (3 * u - c * c) / 3,
                         f = d / 3,
                         p = (2 * c * c * c - 9 * c * u + 27 * h) / 27,
                         g = p / 2,
                         m = g * g + f * f * f;
                     let y, b, v, x, _;
                     if (m < 0) {
                         const t = -d / 3,
-                            e = pg(t * t * t),
+                            e = mg(t * t * t),
                             n = -p / (2 * e),
-                            i = dg(n < -1 ? -1 : n > 1 ? 1 : n),
-                            s = 2 * mg(e);
-                        return v = s * ug(i / 3) - c / 3, x = s * ug((i + bg) / 3) - c / 3, _ = s * ug((i + 2 * bg) / 3) - c / 3, [v, x, _].filter(r)
+                            i = pg(n < -1 ? -1 : n > 1 ? 1 : n),
+                            s = 2 * bg(e);
+                        return v = s * dg(i / 3) - c / 3, x = s * dg((i + xg) / 3) - c / 3, _ = s * dg((i + 2 * xg) / 3) - c / 3, [v, x, _].filter(r)
                     }
-                    if (0 === m) return y = g < 0 ? mg(-g) : -mg(g), v = 2 * y - c / 3, x = -y - c / 3, [v, x].filter(r);
+                    if (0 === m) return y = g < 0 ? bg(-g) : -bg(g), v = 2 * y - c / 3, x = -y - c / 3, [v, x].filter(r);
                     {
-                        const t = pg(m);
-                        return y = mg(-g + t), b = mg(g + t), [y - b - c / 3].filter(r)
+                        const t = mg(m);
+                        return y = bg(-g + t), b = bg(g + t), [y - b - c / 3].filter(r)
                     }
                 },
                 droots: function(t) {
                     if (3 === t.length) {
                         const e = t[0],
                             n = t[1],
                             i = t[2],
                             r = e - 2 * n + i;
                         if (0 !== r) {
-                            const t = -pg(n * n - e * i),
+                            const t = -mg(n * n - e * i),
                                 s = -e + n;
                             return [-(t + s) / r, -(-t + s) / r]
                         }
                         return n !== i && 0 === r ? [(2 * n - i) / (2 * (n - i))] : []
                     }
                     if (2 === t.length) {
                         const e = t[0],
@@ -26668,66 +26762,66 @@
                         return e !== n ? [e / (e - n)] : []
                     }
                     return []
                 },
                 curvature: function(t, e, n, i, r) {
                     let s, o, a, l, c = 0,
                         u = 0;
-                    const h = Sg.compute(t, e),
-                        d = Sg.compute(t, n),
+                    const h = kg.compute(t, e),
+                        d = kg.compute(t, n),
                         f = h.x * h.x + h.y * h.y;
-                    if (i ? (s = pg(gg(h.y * d.z - d.y * h.z, 2) + gg(h.z * d.x - d.z * h.x, 2) + gg(h.x * d.y - d.x * h.y, 2)), o = gg(f + h.z * h.z, 1.5)) : (s = h.x * d.y - h.y * d.x, o = gg(f, 1.5)), 0 === s || 0 === o) return {
+                    if (i ? (s = mg(yg(h.y * d.z - d.y * h.z, 2) + yg(h.z * d.x - d.z * h.x, 2) + yg(h.x * d.y - d.x * h.y, 2)), o = yg(f + h.z * h.z, 1.5)) : (s = h.x * d.y - h.y * d.x, o = yg(f, 1.5)), 0 === s || 0 === o) return {
                         k: 0,
                         r: 0
                     };
                     if (c = s / o, u = o / s, !r) {
-                        const r = Sg.curvature(t - .001, e, n, i, !0).k,
-                            s = Sg.curvature(t + .001, e, n, i, !0).k;
-                        l = (s - c + (c - r)) / 2, a = (cg(s - c) + cg(c - r)) / 2
+                        const r = kg.curvature(t - .001, e, n, i, !0).k,
+                            s = kg.curvature(t + .001, e, n, i, !0).k;
+                        l = (s - c + (c - r)) / 2, a = (hg(s - c) + hg(c - r)) / 2
                     }
                     return {
                         k: c,
                         r: u,
                         dk: l,
                         adk: a
                     }
                 },
                 inflections: function(t) {
                     if (t.length < 4) return [];
-                    const e = Sg.align(t, {
+                    const e = kg.align(t, {
                             p1: t[0],
                             p2: t.slice(-1)[0]
                         }),
                         n = e[2].x * e[1].y,
                         i = e[3].x * e[1].y,
                         r = e[1].x * e[2].y,
                         s = 18 * (-3 * n + 2 * i + 3 * r - e[3].x * e[2].y),
                         o = 18 * (3 * n - i - 3 * r),
                         a = 18 * (r - n);
-                    if (Sg.approximately(s, 0)) {
-                        if (!Sg.approximately(o, 0)) {
+                    if (kg.approximately(s, 0)) {
+                        if (!kg.approximately(o, 0)) {
                             let t = -a / o;
                             if (0 <= t && t <= 1) return [t]
                         }
                         return []
                     }
                     const l = 2 * s;
-                    if (Sg.approximately(l, 0)) return [];
+                    if (kg.approximately(l, 0)) return [];
                     const c = o * o - 4 * s * a;
                     if (c < 0) return [];
                     const u = Math.sqrt(c);
                     return [(u - o) / l, -(o + u) / l].filter((function(t) {
                         return 0 <= t && t <= 1
                     }))
                 },
                 bboxoverlap: function(t, e) {
                     const n = ["x", "y"],
                         i = n.length;
                     for (let r, s, o, a, l = 0; l < i; l++)
-                        if (r = n[l], s = t[r].mid, o = e[r].mid, a = (t[r].size + e[r].size) / 2, cg(s - o) >= a) return !1;
+                        if (r = n[l], s = t[r].mid, o = e[r].mid, a = (t[r].size + e[r].size) / 2, hg(s - o) >= a) return !1;
                     return !0
                 },
                 expandbox: function(t, e) {
                     e.x.min < t.x.min && (t.x.min = e.x.min), e.y.min < t.y.min && (t.y.min = e.y.min), e.z && e.z.min < t.z.min && (t.z.min = e.z.min), e.x.max > t.x.max && (t.x.max = e.x.max), e.y.max > t.y.max && (t.y.max = e.y.max), e.z && e.z.max > t.z.max && (t.z.max = e.z.max), t.x.mid = (t.x.min + t.x.max) / 2, t.y.mid = (t.y.min + t.y.max) / 2, t.z && (t.z.mid = (t.z.min + t.z.max) / 2), t.x.size = t.x.max - t.x.min, t.y.size = t.y.max - t.y.min, t.z && (t.z.size = t.z.max - t.z.min)
                 },
                 pairiteration: function(t, e, n) {
                     const i = t.bbox(),
@@ -26747,61 +26841,61 @@
                             left: a.right,
                             right: l.right
                         }, {
                             left: a.right,
                             right: l.left
                         }];
                     c = c.filter((function(t) {
-                        return Sg.bboxoverlap(t.left.bbox(), t.right.bbox())
+                        return kg.bboxoverlap(t.left.bbox(), t.right.bbox())
                     }));
                     let u = [];
                     return 0 === c.length || (c.forEach((function(t) {
-                        u = u.concat(Sg.pairiteration(t.left, t.right, o))
+                        u = u.concat(kg.pairiteration(t.left, t.right, o))
                     })), u = u.filter((function(t, e) {
                         return u.indexOf(t) === e
                     }))), u
                 },
                 getccenter: function(t, e, n) {
                     const i = e.x - t.x,
                         r = e.y - t.y,
                         s = n.x - e.x,
                         o = n.y - e.y,
-                        a = i * ug(vg) - r * hg(vg),
-                        l = i * hg(vg) + r * ug(vg),
-                        c = s * ug(vg) - o * hg(vg),
-                        u = s * hg(vg) + o * ug(vg),
+                        a = i * dg(_g) - r * fg(_g),
+                        l = i * fg(_g) + r * dg(_g),
+                        c = s * dg(_g) - o * fg(_g),
+                        u = s * fg(_g) + o * dg(_g),
                         h = (t.x + e.x) / 2,
                         d = (t.y + e.y) / 2,
                         f = (e.x + n.x) / 2,
                         p = (e.y + n.y) / 2,
                         g = h + a,
                         m = d + l,
                         y = f + c,
                         b = p + u,
-                        v = Sg.lli8(h, d, g, m, f, p, y, b),
-                        x = Sg.dist(v, t);
-                    let _, w = fg(t.y - v.y, t.x - v.x),
-                        S = fg(e.y - v.y, e.x - v.x),
-                        T = fg(n.y - v.y, n.x - v.x);
-                    return w < T ? ((w > S || S > T) && (w += bg), w > T && (_ = T, T = w, w = _)) : T < S && S < w ? (_ = T, T = w, w = _) : T += bg, v.s = w, v.e = T, v.r = x, v
+                        v = kg.lli8(h, d, g, m, f, p, y, b),
+                        x = kg.dist(v, t);
+                    let _, w = gg(t.y - v.y, t.x - v.x),
+                        S = gg(e.y - v.y, e.x - v.x),
+                        T = gg(n.y - v.y, n.x - v.x);
+                    return w < T ? ((w > S || S > T) && (w += xg), w > T && (_ = T, T = w, w = _)) : T < S && S < w ? (_ = T, T = w, w = _) : T += xg, v.s = w, v.e = T, v.r = x, v
                 },
                 numberSort: function(t, e) {
                     return t - e
                 }
             };
-        class Tg {
+        class Mg {
             constructor(t) {
                 this.curves = [], this._3d = !1, t && (this.curves = t, this._3d = this.curves[0]._3d)
             }
             valueOf() {
                 return this.toString()
             }
             toString() {
                 return "[" + this.curves.map((function(t) {
-                    return Sg.pointsToString(t.points)
+                    return kg.pointsToString(t.points)
                 })).join(", ") + "]"
             }
             addCurve(t) {
                 this.curves.push(t), this._3d = this._3d || t._3d
             }
             length() {
                 return this.curves.map((function(t) {
@@ -26811,34 +26905,34 @@
                 }))
             }
             curve(t) {
                 return this.curves[t]
             }
             bbox() {
                 const t = this.curves;
-                for (var e = t[0].bbox(), n = 1; n < t.length; n++) Sg.expandbox(e, t[n].bbox());
+                for (var e = t[0].bbox(), n = 1; n < t.length; n++) kg.expandbox(e, t[n].bbox());
                 return e
             }
             offset(t) {
                 const e = [];
                 return this.curves.forEach((function(n) {
                     e.push(...n.offset(t))
-                })), new Tg(e)
+                })), new Mg(e)
             }
         }
         const {
-            abs: kg,
-            min: Mg,
-            max: Ig,
-            cos: Eg,
-            sin: Dg,
-            acos: Og,
-            sqrt: Cg
-        } = Math, Ag = Math.PI;
-        class Pg {
+            abs: Ig,
+            min: Eg,
+            max: Dg,
+            cos: Og,
+            sin: Cg,
+            acos: Ag,
+            sqrt: Pg
+        } = Math, Fg = Math.PI;
+        class Lg {
             constructor(t) {
                 let e = t && t.forEach ? t : Array.from(arguments).slice(),
                     n = !1;
                 if ("object" === typeof e[0]) {
                     n = e.length;
                     const t = [];
                     e.forEach((function(e) {
@@ -26863,33 +26957,33 @@
                         y: e[d + 1]
                     };
                     s && (a.z = e[d + 2]), o.push(a)
                 }
                 const l = this.order = o.length - 1,
                     c = this.dims = ["x", "y"];
                 s && c.push("z"), this.dimlen = c.length;
-                const u = Sg.align(o, {
+                const u = kg.align(o, {
                         p1: o[0],
                         p2: o[l]
                     }),
-                    h = Sg.dist(o[0], o[l]);
-                this._linear = u.reduce(((t, e) => t + kg(e.y)), 0) < h / 50, this._lut = [], this._t1 = 0, this._t2 = 1, this.update()
+                    h = kg.dist(o[0], o[l]);
+                this._linear = u.reduce(((t, e) => t + Ig(e.y)), 0) < h / 50, this._lut = [], this._t1 = 0, this._t2 = 1, this.update()
             }
             static quadraticFromPoints(t, e, n, i) {
-                if ("undefined" === typeof i && (i = .5), 0 === i) return new Pg(e, e, n);
-                if (1 === i) return new Pg(t, e, e);
-                const r = Pg.getABC(2, t, e, n, i);
-                return new Pg(t, r.A, n)
+                if ("undefined" === typeof i && (i = .5), 0 === i) return new Lg(e, e, n);
+                if (1 === i) return new Lg(t, e, e);
+                const r = Lg.getABC(2, t, e, n, i);
+                return new Lg(t, r.A, n)
             }
             static cubicFromPoints(t, e, n, i, r) {
                 "undefined" === typeof i && (i = .5);
-                const s = Pg.getABC(3, t, e, n, i);
-                "undefined" === typeof r && (r = Sg.dist(e, s.C));
+                const s = Lg.getABC(3, t, e, n, i);
+                "undefined" === typeof r && (r = kg.dist(e, s.C));
                 const o = r * (1 - i) / i,
-                    a = Sg.dist(t, n),
+                    a = kg.dist(t, n),
                     l = (n.x - t.x) / a,
                     c = (n.y - t.y) / a,
                     u = r * l,
                     h = r * c,
                     d = o * l,
                     f = o * c,
                     p = e.x - u,
@@ -26905,30 +26999,30 @@
                         x: t.x + (v - t.x) / i,
                         y: t.y + (x - t.y) / i
                     },
                     T = {
                         x: n.x + (_ - n.x) / (1 - i),
                         y: n.y + (w - n.y) / (1 - i)
                     };
-                return new Pg(t, S, T, n)
+                return new Lg(t, S, T, n)
             }
             static getUtils() {
-                return Sg
+                return kg
             }
             getUtils() {
-                return Pg.getUtils()
+                return Lg.getUtils()
             }
             static get PolyBezier() {
-                return Tg
+                return Mg
             }
             valueOf() {
                 return this.toString()
             }
             toString() {
-                return Sg.pointsToString(this.points)
+                return kg.pointsToString(this.points)
             }
             toSVG() {
                 if (this._3d) return !1;
                 const t = this.points,
                     e = ["M", t[0].x, t[0].y, 2 === this.order ? "Q" : "C"];
                 for (let n = 1, i = t.length; n < i; n++) e.push(t[n].x), e.push(t[n].y);
                 return e.join(" ")
@@ -26943,37 +27037,37 @@
             }
             coordDigest() {
                 return this.points.map((function(t, e) {
                     return "" + e + t.x + t.y + (t.z ? t.z : 0)
                 })).join("")
             }
             update() {
-                this._lut = [], this.dpoints = Sg.derive(this.points, this._3d), this.computedirection()
+                this._lut = [], this.dpoints = kg.derive(this.points, this._3d), this.computedirection()
             }
             computedirection() {
                 const t = this.points,
-                    e = Sg.angle(t[0], t[this.order], t[1]);
+                    e = kg.angle(t[0], t[this.order], t[1]);
                 this.clockwise = e > 0
             }
             length() {
-                return Sg.length(this.derivative.bind(this))
+                return kg.length(this.derivative.bind(this))
             }
             static getABC() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 2,
                     e = arguments.length > 1 ? arguments[1] : void 0,
                     n = arguments.length > 2 ? arguments[2] : void 0,
                     i = arguments.length > 3 ? arguments[3] : void 0,
                     r = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : .5;
-                const s = Sg.projectionratio(r, t),
+                const s = kg.projectionratio(r, t),
                     o = 1 - s,
                     a = {
                         x: s * e.x + o * i.x,
                         y: s * e.y + o * i.y
                     },
-                    l = Sg.abcratio(r, t);
+                    l = kg.abcratio(r, t);
                 return {
                     A: {
                         x: n.x + (n.x - a.x) / l,
                         y: n.y + (n.y - a.y) / l
                     },
                     B: n,
                     C: a,
@@ -26981,106 +27075,106 @@
                     E: i
                 }
             }
             getABC(t, e) {
                 e = e || this.get(t);
                 let n = this.points[0],
                     i = this.points[this.order];
-                return Pg.getABC(this.order, n, e, i, t)
+                return Lg.getABC(this.order, n, e, i, t)
             }
             getLUT(t) {
                 if (this.verify(), t = t || 100, this._lut.length === t + 1) return this._lut;
                 this._lut = [], t++, this._lut = [];
                 for (let e, n, i = 0; i < t; i++) n = i / (t - 1), e = this.compute(n), e.t = n, this._lut.push(e);
                 return this._lut
             }
             on(e, n) {
                 n = n || 5;
                 const i = this.getLUT(),
                     r = [];
-                for (let t, s = 0, o = 0; s < i.length; s++) t = i[s], Sg.dist(t, e) < n && (r.push(t), o += s / i.length);
+                for (let t, s = 0, o = 0; s < i.length; s++) t = i[s], kg.dist(t, e) < n && (r.push(t), o += s / i.length);
                 return !!r.length && (t /= r.length)
             }
             project(t) {
                 const e = this.getLUT(),
                     n = e.length - 1,
-                    i = Sg.closest(e, t),
+                    i = kg.closest(e, t),
                     r = i.mpos,
                     s = (r - 1) / n,
                     o = (r + 1) / n,
                     a = .1 / n;
                 let l, c = i.mdist,
                     u = s,
                     h = u;
                 c += 1;
-                for (let d; u < o + a; u += a) l = this.compute(u), d = Sg.dist(t, l), d < c && (c = d, h = u);
+                for (let d; u < o + a; u += a) l = this.compute(u), d = kg.dist(t, l), d < c && (c = d, h = u);
                 return h = h < 0 ? 0 : h > 1 ? 1 : h, l = this.compute(h), l.t = h, l.d = c, l
             }
             get(t) {
                 return this.compute(t)
             }
             point(t) {
                 return this.points[t]
             }
             compute(t) {
-                return this.ratios ? Sg.computeWithRatios(t, this.points, this.ratios, this._3d) : Sg.compute(t, this.points, this._3d, this.ratios)
+                return this.ratios ? kg.computeWithRatios(t, this.points, this.ratios, this._3d) : kg.compute(t, this.points, this._3d, this.ratios)
             }
             raise() {
                 const t = this.points,
                     e = [t[0]],
                     n = t.length;
                 for (let i, r, s = 1; s < n; s++) i = t[s], r = t[s - 1], e[s] = {
                     x: (n - s) / n * i.x + s / n * r.x,
                     y: (n - s) / n * i.y + s / n * r.y
                 };
-                return e[n] = t[n - 1], new Pg(e)
+                return e[n] = t[n - 1], new Lg(e)
             }
             derivative(t) {
-                return Sg.compute(t, this.dpoints[0], this._3d)
+                return kg.compute(t, this.dpoints[0], this._3d)
             }
             dderivative(t) {
-                return Sg.compute(t, this.dpoints[1], this._3d)
+                return kg.compute(t, this.dpoints[1], this._3d)
             }
             align() {
                 let t = this.points;
-                return new Pg(Sg.align(t, {
+                return new Lg(kg.align(t, {
                     p1: t[0],
                     p2: t[t.length - 1]
                 }))
             }
             curvature(t) {
-                return Sg.curvature(t, this.dpoints[0], this.dpoints[1], this._3d)
+                return kg.curvature(t, this.dpoints[0], this.dpoints[1], this._3d)
             }
             inflections() {
-                return Sg.inflections(this.points)
+                return kg.inflections(this.points)
             }
             normal(t) {
                 return this._3d ? this.__normal3(t) : this.__normal2(t)
             }
             __normal2(t) {
                 const e = this.derivative(t),
-                    n = Cg(e.x * e.x + e.y * e.y);
+                    n = Pg(e.x * e.x + e.y * e.y);
                 return {
                     t: t,
                     x: -e.y / n,
                     y: e.x / n
                 }
             }
             __normal3(t) {
                 const e = this.derivative(t),
                     n = this.derivative(t + .01),
-                    i = Cg(e.x * e.x + e.y * e.y + e.z * e.z),
-                    r = Cg(n.x * n.x + n.y * n.y + n.z * n.z);
+                    i = Pg(e.x * e.x + e.y * e.y + e.z * e.z),
+                    r = Pg(n.x * n.x + n.y * n.y + n.z * n.z);
                 e.x /= i, e.y /= i, e.z /= i, n.x /= r, n.y /= r, n.z /= r;
                 const s = {
                         x: n.y * e.z - n.z * e.y,
                         y: n.z * e.x - n.x * e.z,
                         z: n.x * e.y - n.y * e.x
                     },
-                    o = Cg(s.x * s.x + s.y * s.y + s.z * s.z);
+                    o = Pg(s.x * s.x + s.y * s.y + s.z * s.z);
                 s.x /= o, s.y /= o, s.z /= o;
                 const a = [s.x * s.x, s.x * s.y - s.z, s.x * s.z + s.y, s.x * s.y + s.z, s.y * s.y, s.y * s.z - s.x, s.x * s.z - s.y, s.y * s.z + s.x, s.z * s.z];
                 return {
                     t: t,
                     x: a[0] * e.x + a[1] * e.y + a[2] * e.z,
                     y: a[3] * e.x + a[4] * e.y + a[5] * e.z,
                     z: a[6] * e.x + a[7] * e.y + a[8] * e.z
@@ -27089,56 +27183,56 @@
             hull(t) {
                 let e = this.points,
                     n = [],
                     i = [],
                     r = 0;
                 for (i[r++] = e[0], i[r++] = e[1], i[r++] = e[2], 3 === this.order && (i[r++] = e[3]); e.length > 1;) {
                     n = [];
-                    for (let s, o = 0, a = e.length - 1; o < a; o++) s = Sg.lerp(t, e[o], e[o + 1]), i[r++] = s, n.push(s);
+                    for (let s, o = 0, a = e.length - 1; o < a; o++) s = kg.lerp(t, e[o], e[o + 1]), i[r++] = s, n.push(s);
                     e = n
                 }
                 return i
             }
             split(t, e) {
                 if (0 === t && e) return this.split(e).left;
                 if (1 === e) return this.split(t).right;
                 const n = this.hull(t),
                     i = {
-                        left: 2 === this.order ? new Pg([n[0], n[3], n[5]]) : new Pg([n[0], n[4], n[7], n[9]]),
-                        right: 2 === this.order ? new Pg([n[5], n[4], n[2]]) : new Pg([n[9], n[8], n[6], n[3]]),
+                        left: 2 === this.order ? new Lg([n[0], n[3], n[5]]) : new Lg([n[0], n[4], n[7], n[9]]),
+                        right: 2 === this.order ? new Lg([n[5], n[4], n[2]]) : new Lg([n[9], n[8], n[6], n[3]]),
                         span: n
                     };
-                return i.left._t1 = Sg.map(0, 0, 1, this._t1, this._t2), i.left._t2 = Sg.map(t, 0, 1, this._t1, this._t2), i.right._t1 = Sg.map(t, 0, 1, this._t1, this._t2), i.right._t2 = Sg.map(1, 0, 1, this._t1, this._t2), e ? (e = Sg.map(e, t, 1, 0, 1), i.right.split(e).left) : i
+                return i.left._t1 = kg.map(0, 0, 1, this._t1, this._t2), i.left._t2 = kg.map(t, 0, 1, this._t1, this._t2), i.right._t1 = kg.map(t, 0, 1, this._t1, this._t2), i.right._t2 = kg.map(1, 0, 1, this._t1, this._t2), e ? (e = kg.map(e, t, 1, 0, 1), i.right.split(e).left) : i
             }
             extrema() {
                 const t = {};
                 let e = [];
                 return this.dims.forEach(function(n) {
                     let i = function(t) {
                             return t[n]
                         },
                         r = this.dpoints[0].map(i);
-                    t[n] = Sg.droots(r), 3 === this.order && (r = this.dpoints[1].map(i), t[n] = t[n].concat(Sg.droots(r))), t[n] = t[n].filter((function(t) {
+                    t[n] = kg.droots(r), 3 === this.order && (r = this.dpoints[1].map(i), t[n] = t[n].concat(kg.droots(r))), t[n] = t[n].filter((function(t) {
                         return t >= 0 && t <= 1
-                    })), e = e.concat(t[n].sort(Sg.numberSort))
-                }.bind(this)), t.values = e.sort(Sg.numberSort).filter((function(t, n) {
+                    })), e = e.concat(t[n].sort(kg.numberSort))
+                }.bind(this)), t.values = e.sort(kg.numberSort).filter((function(t, n) {
                     return e.indexOf(t) === n
                 })), t
             }
             bbox() {
                 const t = this.extrema(),
                     e = {};
                 return this.dims.forEach(function(n) {
-                    e[n] = Sg.getminmax(this, n, t[n])
+                    e[n] = kg.getminmax(this, n, t[n])
                 }.bind(this)), e
             }
             overlaps(t) {
                 const e = this.bbox(),
                     n = t.bbox();
-                return Sg.bboxoverlap(e, n)
+                return kg.bboxoverlap(e, n)
             }
             offset(t, e) {
                 if ("undefined" !== typeof e) {
                     const n = this.get(t),
                         i = this.normal(t),
                         r = {
                             c: n,
@@ -27153,54 +27247,54 @@
                         n = this.points.map((function(n) {
                             const i = {
                                 x: n.x + t * e.x,
                                 y: n.y + t * e.y
                             };
                             return n.z && e.z && (i.z = n.z + t * e.z), i
                         }));
-                    return [new Pg(n)]
+                    return [new Lg(n)]
                 }
                 return this.reduce().map((function(e) {
                     return e._linear ? e.offset(t)[0] : e.scale(t)
                 }))
             }
             simple() {
                 if (3 === this.order) {
-                    const t = Sg.angle(this.points[0], this.points[3], this.points[1]),
-                        e = Sg.angle(this.points[0], this.points[3], this.points[2]);
+                    const t = kg.angle(this.points[0], this.points[3], this.points[1]),
+                        e = kg.angle(this.points[0], this.points[3], this.points[2]);
                     if (t > 0 && e < 0 || t < 0 && e > 0) return !1
                 }
                 const t = this.normal(0),
                     e = this.normal(1);
                 let n = t.x * e.x + t.y * e.y;
-                return this._3d && (n += t.z * e.z), kg(Og(n)) < Ag / 3
+                return this._3d && (n += t.z * e.z), Ig(Ag(n)) < Fg / 3
             }
             reduce() {
                 let t, e, n = 0,
                     i = 0,
                     r = .01,
                     s = [],
                     o = [],
                     a = this.extrema().values;
                 for (-1 === a.indexOf(0) && (a = [0].concat(a)), -1 === a.indexOf(1) && a.push(1), n = a[0], t = 1; t < a.length; t++) i = a[t], e = this.split(n, i), e._t1 = n, e._t2 = i, s.push(e), n = i;
                 return s.forEach((function(t) {
                     for (n = 0, i = 0; i <= 1;)
                         for (i = n + r; i <= 1.01; i += r)
                             if (e = t.split(n, i), !e.simple()) {
-                                if (i -= r, kg(n - i) < r) return [];
-                                e = t.split(n, i), e._t1 = Sg.map(n, 0, 1, t._t1, t._t2), e._t2 = Sg.map(i, 0, 1, t._t1, t._t2), o.push(e), n = i;
+                                if (i -= r, Ig(n - i) < r) return [];
+                                e = t.split(n, i), e._t1 = kg.map(n, 0, 1, t._t1, t._t2), e._t2 = kg.map(i, 0, 1, t._t1, t._t2), o.push(e), n = i;
                                 break
-                            } n < 1 && (e = t.split(n, 1), e._t1 = Sg.map(n, 0, 1, t._t1, t._t2), e._t2 = t._t2, o.push(e))
+                            } n < 1 && (e = t.split(n, 1), e._t1 = kg.map(n, 0, 1, t._t1, t._t2), e._t2 = t._t2, o.push(e))
                 })), o
             }
             translate(t, e, n) {
                 n = "number" === typeof n ? n : e;
                 const i = this.order;
                 let r = this.points.map(((t, r) => (1 - r / i) * e + r / i * n));
-                return new Pg(this.points.map(((e, n) => ({
+                return new Lg(this.points.map(((e, n) => ({
                     x: e.x + t.x * r[n],
                     y: e.y + t.y * r[n]
                 }))))
             }
             scale(t) {
                 const e = this.order;
                 let n = !1;
@@ -27208,44 +27302,44 @@
                 const i = this.clockwise,
                     r = this.points;
                 if (this._linear) return this.translate(this.normal(0), n ? n(0) : t, n ? n(1) : t);
                 const s = n ? n(0) : t,
                     o = n ? n(1) : t,
                     a = [this.offset(0, 10), this.offset(1, 10)],
                     l = [],
-                    c = Sg.lli4(a[0], a[0].c, a[1], a[1].c);
+                    c = kg.lli4(a[0], a[0].c, a[1], a[1].c);
                 if (!c) throw new Error("cannot scale this curve. Try reducing it first.");
                 return [0, 1].forEach((function(t) {
-                    const n = l[t * e] = Sg.copy(r[t * e]);
+                    const n = l[t * e] = kg.copy(r[t * e]);
                     n.x += (t ? o : s) * a[t].n.x, n.y += (t ? o : s) * a[t].n.y
                 })), n ? ([0, 1].forEach((function(s) {
                     if (2 !== e || !s) {
                         var o = r[s + 1],
                             a = {
                                 x: o.x - c.x,
                                 y: o.y - c.y
                             },
                             u = n ? n((s + 1) / e) : t;
                         n && !i && (u = -u);
-                        var h = Cg(a.x * a.x + a.y * a.y);
+                        var h = Pg(a.x * a.x + a.y * a.y);
                         a.x /= h, a.y /= h, l[s + 1] = {
                             x: o.x + u * a.x,
                             y: o.y + u * a.y
                         }
                     }
-                })), new Pg(l)) : ([0, 1].forEach((t => {
+                })), new Lg(l)) : ([0, 1].forEach((t => {
                     if (2 === e && t) return;
                     const n = l[t * e],
                         i = this.derivative(t),
                         s = {
                             x: n.x + i.x,
                             y: n.y + i.y
                         };
-                    l[t + 1] = Sg.lli4(n, s, c, r[t + 1])
-                })), new Pg(l))
+                    l[t + 1] = kg.lli4(n, s, c, r[t + 1])
+                })), new Lg(l))
             }
             outline(t, e, n, i) {
                 if (e = void 0 === e ? t : e, this._linear) {
                     const r = this.normal(0),
                         s = this.points[0],
                         o = this.points[this.points.length - 1];
                     let a, l, c;
@@ -27267,71 +27361,71 @@
                         x: o.x - r.x * i,
                         y: o.y - r.y * i
                     }, l = {
                         x: (a.x + c.x) / 2,
                         y: (a.y + c.y) / 2
                     };
                     const h = [c, l, a],
-                        d = Sg.makeline(h[2], u[0]),
-                        f = Sg.makeline(u[2], h[0]),
-                        p = [d, new Pg(u), f, new Pg(h)];
-                    return new Tg(p)
+                        d = kg.makeline(h[2], u[0]),
+                        f = kg.makeline(u[2], h[0]),
+                        p = [d, new Lg(u), f, new Lg(h)];
+                    return new Mg(p)
                 }
                 const r = this.reduce(),
                     s = r.length,
                     o = [];
                 let a, l = [],
                     c = 0,
                     u = this.length();
                 const h = "undefined" !== typeof n && "undefined" !== typeof i;
 
                 function d(t, e, n, i, r) {
                     return function(s) {
                         const o = i / n,
                             a = (i + r) / n,
                             l = e - t;
-                        return Sg.map(s, 0, 1, t + o * l, t + a * l)
+                        return kg.map(s, 0, 1, t + o * l, t + a * l)
                     }
                 }
                 r.forEach((function(r) {
                     const s = r.length();
                     h ? (o.push(r.scale(d(t, n, u, c, s))), l.push(r.scale(d(-e, -i, u, c, s)))) : (o.push(r.scale(t)), l.push(r.scale(-e))), c += s
                 })), l = l.map((function(t) {
                     return a = t.points, a[3] ? t.points = [a[3], a[2], a[1], a[0]] : t.points = [a[2], a[1], a[0]], t
                 })).reverse();
                 const f = o[0].points[0],
                     p = o[s - 1].points[o[s - 1].points.length - 1],
                     g = l[s - 1].points[l[s - 1].points.length - 1],
                     m = l[0].points[0],
-                    y = Sg.makeline(g, f),
-                    b = Sg.makeline(p, m),
+                    y = kg.makeline(g, f),
+                    b = kg.makeline(p, m),
                     v = [y].concat(o).concat([b]).concat(l);
-                return new Tg(v)
+                return new Mg(v)
             }
             outlineshapes(t, e, n) {
                 e = e || t;
                 const i = this.outline(t, e).curves,
                     r = [];
                 for (let s = 1, o = i.length; s < o / 2; s++) {
-                    const t = Sg.makeshape(i[s], i[o - s], n);
+                    const t = kg.makeshape(i[s], i[o - s], n);
                     t.startcap.virtual = s > 1, t.endcap.virtual = s < o / 2 - 1, r.push(t)
                 }
                 return r
             }
             intersects(t, e) {
-                return t ? t.p1 && t.p2 ? this.lineIntersects(t) : (t instanceof Pg && (t = t.reduce()), this.curveintersects(this.reduce(), t, e)) : this.selfintersects(e)
+                return t ? t.p1 && t.p2 ? this.lineIntersects(t) : (t instanceof Lg && (t = t.reduce()), this.curveintersects(this.reduce(), t, e)) : this.selfintersects(e)
             }
             lineIntersects(t) {
-                const e = Mg(t.p1.x, t.p2.x),
-                    n = Mg(t.p1.y, t.p2.y),
-                    i = Ig(t.p1.x, t.p2.x),
-                    r = Ig(t.p1.y, t.p2.y);
-                return Sg.roots(this.points, t).filter((t => {
+                const e = Eg(t.p1.x, t.p2.x),
+                    n = Eg(t.p1.y, t.p2.y),
+                    i = Dg(t.p1.x, t.p2.x),
+                    r = Dg(t.p1.y, t.p2.y);
+                return kg.roots(this.points, t).filter((t => {
                     var s = this.get(t);
-                    return Sg.between(s.x, e, i) && Sg.between(s.y, n, r)
+                    return kg.between(s.x, e, i) && kg.between(s.y, n, r)
                 }))
             }
             selfintersects(t) {
                 const e = this.reduce(),
                     n = e.length - 2,
                     i = [];
                 for (let r, s, o, a = 0; a < n; a++) s = e.slice(a, a + 1), o = e.slice(a + 2), r = this.curveintersects(s, o, t), i.push(...r);
@@ -27345,53 +27439,53 @@
                             left: t,
                             right: e
                         })
                     }))
                 }));
                 let r = [];
                 return i.forEach((function(t) {
-                    const e = Sg.pairiteration(t.left, t.right, n);
+                    const e = kg.pairiteration(t.left, t.right, n);
                     e.length > 0 && (r = r.concat(e))
                 })), r
             }
             arcs(t) {
                 return t = t || .5, this._iterate(t, [])
             }
             _error(t, e, n, i) {
                 const r = (i - n) / 4,
                     s = this.get(n + r),
                     o = this.get(i - r),
-                    a = Sg.dist(t, e),
-                    l = Sg.dist(t, s),
-                    c = Sg.dist(t, o);
-                return kg(l - a) + kg(c - a)
+                    a = kg.dist(t, e),
+                    l = kg.dist(t, s),
+                    c = kg.dist(t, o);
+                return Ig(l - a) + Ig(c - a)
             }
             _iterate(t, e) {
                 let n, i = 0,
                     r = 1;
                 do {
                     n = 0, r = 1;
                     let s, o, a, l, c, u = this.get(i),
                         h = !1,
                         d = !1,
                         f = r,
                         p = 1,
                         g = 0;
                     do {
-                        if (d = h, l = a, f = (i + r) / 2, g++, s = this.get(f), o = this.get(r), a = Sg.getccenter(u, s, o), a.interval = {
+                        if (d = h, l = a, f = (i + r) / 2, g++, s = this.get(f), o = this.get(r), a = kg.getccenter(u, s, o), a.interval = {
                                 start: i,
                                 end: r
                             }, h = this._error(a, u, i, r) <= t, c = d && !h, c || (p = r), h) {
                             if (r >= 1) {
                                 if (a.interval.end = p = 1, l = a, r > 1) {
                                     let t = {
-                                        x: a.x + a.r * Eg(a.e),
-                                        y: a.y + a.r * Dg(a.e)
+                                        x: a.x + a.r * Og(a.e),
+                                        y: a.y + a.r * Cg(a.e)
                                     };
-                                    a.e += Sg.angle({
+                                    a.e += kg.angle({
                                         x: a.x,
                                         y: a.y
                                     }, t, this.get(1))
                                 }
                                 break
                             }
                             r += (r - i) / 2
@@ -27399,15 +27493,15 @@
                     } while (!c && n++ < 100);
                     if (n >= 100) break;
                     l = l || a, e.push(l), i = p
                 } while (r < 1);
                 return e
             }
         }
-        const Fg = {
+        const zg = {
                 aliceblue: [240, 248, 255],
                 antiquewhite: [250, 235, 215],
                 aqua: [0, 255, 255],
                 aquamarine: [127, 255, 212],
                 azure: [240, 255, 255],
                 beige: [245, 245, 220],
                 bisque: [255, 228, 196],
@@ -27549,40 +27643,40 @@
                 violet: [238, 130, 238],
                 wheat: [245, 222, 179],
                 white: [255, 255, 255],
                 whitesmoke: [245, 245, 245],
                 yellow: [255, 255, 0],
                 yellowgreen: [154, 205, 50]
             },
-            Lg = function(t) {
+            Ng = function(t) {
                 var e, n, i = [],
                     r = 1;
                 if ("number" === typeof t) return {
                     space: "rgb",
                     values: [t >>> 16, (65280 & t) >>> 8, 255 & t],
                     alpha: 1
                 };
                 if ("number" === typeof t) return {
                     space: "rgb",
                     values: [t >>> 16, (65280 & t) >>> 8, 255 & t],
                     alpha: 1
                 };
-                if (t = String(t).toLowerCase(), Fg[t]) i = Fg[t].slice(), n = "rgb";
+                if (t = String(t).toLowerCase(), zg[t]) i = zg[t].slice(), n = "rgb";
                 else if ("transparent" === t) r = 0, n = "rgb", i = [0, 0, 0];
                 else if ("#" === t[0]) {
                     var s = t.slice(1),
                         o = s.length;
                     r = 1, o <= 4 ? (i = [parseInt(s[0] + s[0], 16), parseInt(s[1] + s[1], 16), parseInt(s[2] + s[2], 16)], 4 === o && (r = parseInt(s[3] + s[3], 16) / 255)) : (i = [parseInt(s[0] + s[1], 16), parseInt(s[2] + s[3], 16), parseInt(s[4] + s[5], 16)], 8 === o && (r = parseInt(s[6] + s[7], 16) / 255)), i[0] || (i[0] = 0), i[1] || (i[1] = 0), i[2] || (i[2] = 0), n = "rgb"
                 } else if (e = /^((?:rgba?|hs[lvb]a?|hwba?|cmyk?|xy[zy]|gray|lab|lchu?v?|[ly]uv|lms|oklch|oklab|color))\s*\(([^\)]*)\)/.exec(t)) {
                     var a = e[1],
                         l = "cmyk" === (n = a.replace(/a$/, "")) ? 4 : "gray" === n ? 1 : 3;
                     i = e[2].trim().split(/\s*[,\/]\s*|\s+/), "color" === n && (n = i.shift()), r = (i = i.map((function(t, e) {
                         if ("%" === t[t.length - 1]) return t = parseFloat(t) / 100, 3 === e ? t : "rgb" === n ? 255 * t : "h" === n[0] ? 100 * t : "l" !== n[0] || e ? "lab" === n ? 125 * t : "lch" === n ? e < 2 ? 150 * t : 360 * t : "o" !== n[0] || e ? "oklab" === n ? .4 * t : "oklch" === n ? e < 2 ? .4 * t : 360 * t : t : t : 100 * t;
                         if ("h" === n[e] || 2 === e && "h" === n[n.length - 1]) {
-                            if (void 0 !== zg[t]) return zg[t];
+                            if (void 0 !== Bg[t]) return Bg[t];
                             if (t.endsWith("deg")) return parseFloat(t);
                             if (t.endsWith("turn")) return 360 * parseFloat(t);
                             if (t.endsWith("grad")) return 360 * parseFloat(t) / 400;
                             if (t.endsWith("rad")) return 180 * parseFloat(t) / Math.PI
                         }
                         return "none" === t ? 0 : parseFloat(t)
                     }))).length > l ? i.pop() : 1
@@ -27594,30 +27688,30 @@
                 }
                 return {
                     space: n,
                     values: i,
                     alpha: r
                 }
             };
-        var zg = {
+        var Bg = {
             red: 0,
             orange: 60,
             yellow: 120,
             green: 180,
             blue: 240,
             purple: 300
         };
-        const Ng = {
+        const Rg = {
                 name: "rgb",
                 min: [0, 0, 0],
                 max: [255, 255, 255],
                 channel: ["red", "green", "blue"],
                 alias: ["RGB"]
             },
-            Bg = {
+            Ug = {
                 name: "hsl",
                 min: [0, 0, 0],
                 max: [360, 100, 100],
                 channel: ["hue", "saturation", "lightness"],
                 alias: ["HSL"],
                 rgb: function(t) {
                     var e, n, i, r, s, o = t[0] / 360,
@@ -27626,36 +27720,36 @@
                         c = 0;
                     if (0 === a) return [s = 255 * l, s, s];
                     for (e = 2 * l - (n = l < .5 ? l * (1 + a) : l + a - l * a), r = [0, 0, 0]; c < 3;)(i = o + 1 / 3 * -(c - 1)) < 0 ? i++ : i > 1 && i--, s = 6 * i < 1 ? e + 6 * (n - e) * i : 2 * i < 1 ? n : 3 * i < 2 ? e + (n - e) * (2 / 3 - i) * 6 : e, r[c++] = 255 * s;
                     return r
                 }
             };
 
-        function Rg(t) {
+        function Vg(t) {
             var e;
             Array.isArray(t) && t.raw && (t = String.raw(...arguments)), t instanceof Number && (t = +t);
-            var n = Lg(t);
+            var n = Ng(t);
             if (!n.space) return [];
-            const i = "h" === n.space[0] ? Bg.min : Ng.min,
-                r = "h" === n.space[0] ? Bg.max : Ng.max;
-            return (e = Array(3))[0] = Math.min(Math.max(n.values[0], i[0]), r[0]), e[1] = Math.min(Math.max(n.values[1], i[1]), r[1]), e[2] = Math.min(Math.max(n.values[2], i[2]), r[2]), "h" === n.space[0] && (e = Bg.rgb(e)), e.push(Math.min(Math.max(n.alpha, 0), 1)), e
+            const i = "h" === n.space[0] ? Ug.min : Rg.min,
+                r = "h" === n.space[0] ? Ug.max : Rg.max;
+            return (e = Array(3))[0] = Math.min(Math.max(n.values[0], i[0]), r[0]), e[1] = Math.min(Math.max(n.values[1], i[1]), r[1]), e[2] = Math.min(Math.max(n.values[2], i[2]), r[2]), "h" === n.space[0] && (e = Ug.rgb(e)), e.push(Math.min(Math.max(n.alpha, 0), 1)), e
         }
 
-        function Ug(t, e) {
+        function jg(t, e) {
             return {
                 datasets: Object.entries(t).filter((t => {
                     let [n] = t;
                     return !e.fixed_lines.includes(n)
                 })).map(((t, n) => {
                     let [i, r] = t;
                     const s = r.x.map(((t, e) => ({
                             x: t,
                             y: r.y[e]
                         }))),
-                        o = Rg(r.color),
+                        o = Vg(r.color),
                         a = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
                         l = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.5)");
                     return {
                         data: s,
                         isControlPoint: !0,
                         label: i,
                         fill: !1,
@@ -27668,56 +27762,56 @@
                         backgroundColor: l,
                         borderColor: a
                     }
                 }))
             }
         }
 
-        function Vg(t, e) {
+        function Wg(t, e) {
             return {
                 datasets: Object.entries(t).filter((t => {
                     let [n] = t;
                     return !e.fixed_lines.includes(n)
                 })).map(((t, e) => {
                     let [n, i] = t;
                     const r = i.x.map(((t, e) => ({
                             x: t,
                             y: i.y[e]
                         }))),
                         s = [];
                     for (let a = 0; a < r.length - 2; a += 2) {
                         const t = r.slice(a, a + 3),
-                            e = new Pg(t).getLUT(10);
+                            e = new Lg(t).getLUT(10);
                         s.push(...e)
                     }
-                    const o = Rg(i.color);
+                    const o = Vg(i.color);
                     return {
                         label: n + " (bezier)",
                         data: s,
                         isControlPoint: !1,
                         showLine: !0,
                         tension: .3,
                         pointRadius: 0,
                         backgroundColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
                         borderColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.4)"),
                         borderDash: i.border_dash
                     }
                 }))
             }
         }
-        Ng.hsl = function(t) {
+        Rg.hsl = function(t) {
             var e, n, i = t[0] / 255,
                 r = t[1] / 255,
                 s = t[2] / 255,
                 o = Math.min(i, r, s),
                 a = Math.max(i, r, s),
                 l = a - o;
             return a === o ? e = 0 : i === a ? e = (r - s) / l : r === a ? e = 2 + (s - i) / l : s === a && (e = 4 + (i - r) / l), (e = Math.min(60 * e, 360)) < 0 && (e += 360), n = (o + a) / 2, [e, 100 * (a === o ? 0 : n <= .5 ? l / (a + o) : l / (2 - a - o)), 100 * n]
         }, Hh.register(...$f, Up);
-        const jg = class extends ao {
+        const Hg = class extends ao {
             constructor(t) {
                 var e, n;
                 super(t), this.downHandler = t => {
                     const e = $p(this.chartRef.current, t);
                     if (e.length > 0) {
                         this.chartRef.current.data.datasets[e[0].datasetIndex].isControlPoint && (this.setState({
                             activePoint: e[0]
@@ -27739,15 +27833,15 @@
                         const e = this.chartRef.current,
                             n = this.state.activePoint,
                             i = yc(t, e),
                             r = e.chartArea,
                             s = this.calculateNewYValue(i, r, e.scales.y),
                             o = this.calculateNewXValue(i, r, e.scales.x);
                         this.updateControlPointPosition(e, n, o, s), this.updateOriginalData(e, n);
-                        const a = Vg(this.state.originalData, this.props.args.options);
+                        const a = Wg(this.state.originalData, this.props.args.options);
                         this.setState({
                             bezierData: a
                         }), e.update("none")
                     }
                 }, this.upHandler = t => {
                     this.state.activePoint && (this.sendBezierData(), this.setState({
                         activePoint: null
@@ -27758,15 +27852,15 @@
                         return n.fixed_lines.includes(e)
                     })).map(((t, e) => {
                         let [n, i] = t;
                         const r = i.x.map(((t, e) => ({
                                 x: t,
                                 y: i.y[e]
                             }))),
-                            s = Rg(i.color);
+                            s = Vg(i.color);
                         return {
                             data: r,
                             isControlPoint: !1,
                             label: n,
                             fill: !1,
                             tension: .3,
                             spanGaps: !1,
@@ -27776,25 +27870,25 @@
                             pointRadius: i.point_radius,
                             borderDash: i.border_dash
                         }
                     }))
                 }), this.state = {
                     activePoint: null,
                     originalData: t.args.data,
-                    controlData: Ug(this.props.args.data, this.props.args.options),
-                    bezierData: Vg(this.props.args.data, this.props.args.options),
-                    options: Jp(t.args.options, t.theme)
+                    controlData: jg(this.props.args.data, this.props.args.options),
+                    bezierData: Wg(this.props.args.data, this.props.args.options),
+                    options: tg(t.args.options, t.theme)
                 }
             }
             componentDidUpdate(t) {
                 ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                     originalData: this.props.args.data,
-                    controlData: Ug(this.props.args.data, this.props.args.options),
-                    bezierData: Vg(this.props.args.data, this.props.args.options),
-                    options: Jp(this.props.args.options, this.props.theme)
+                    controlData: jg(this.props.args.data, this.props.args.options),
+                    bezierData: Wg(this.props.args.data, this.props.args.options),
+                    options: tg(this.props.args.options, this.props.theme)
                 })
             }
             sendBezierData() {
                 const t = this.convertBezierData(this.state.bezierData.datasets);
                 ro.setComponentValue(t)
             }
             togglePan(t) {
@@ -27812,38 +27906,38 @@
                             x: i,
                             y: r
                         } = t; - 1 === e[n].x.findIndex(((t, s) => t === i && e[n].y[s] === r)) && (e[n].x.push(i), e[n].y.push(r))
                     }))
                 })), e
             }
             render() {
-                return (0, sg.jsx)(Gp, {
+                return (0, ag.jsx)(Gp, {
                     ref: this.chartRef,
                     data: {
                         datasets: [...this.state.controlData.datasets, ...this.state.bezierData.datasets, ...this.fixedData.datasets]
                     },
                     options: this.state.options,
                     onPointerDown: this.downHandler,
                     onPointerUp: this.upHandler,
                     onPointerMove: this.moveHandler
                 })
             }
         };
 
-        function Wg(t, e) {
+        function Yg(t, e) {
             const n = Object.entries(t).filter((t => {
                 let [n] = t;
                 return !e.fixed_lines.includes(n)
             })).map(((t, n) => {
                 let [i, r] = t;
                 const s = r.x.map(((t, e) => ({
                         x: t,
                         y: r.y[e]
                     }))),
-                    o = Rg(r.color),
+                    o = Vg(r.color),
                     a = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 1)"),
                     l = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.8)");
                 return {
                     data: s,
                     isControlPoint: !0,
                     label: i,
                     spanGaps: e.fill_gaps,
@@ -27861,32 +27955,32 @@
                 }
             }));
             return {
                 datasets: n
             }
         }
 
-        function Hg(t, e) {
+        function $g(t, e) {
             return {
                 datasets: Object.entries(t).filter((t => {
                     let [n] = t;
                     return !e.fixed_lines.includes(n)
                 })).map(((t, e) => {
                     let [n, i] = t;
                     const r = i.x.map(((t, e) => ({
                             x: t,
                             y: i.y[e]
                         }))),
                         s = [];
                     for (let a = 0; a < r.length - 3; a += 3) {
                         const t = r.slice(a, a + 4),
-                            e = new Pg(t).getLUT(10);
+                            e = new Lg(t).getLUT(10);
                         s.push(...e)
                     }
-                    const o = Rg(i.color);
+                    const o = Vg(i.color);
                     return {
                         label: n + " (bezier)",
                         data: s,
                         isControlPoint: !1,
                         showLine: !0,
                         tension: .3,
                         backgroundColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
@@ -27894,18 +27988,18 @@
                         pointRadius: 0,
                         borderDash: i.border_dash
                     }
                 }))
             }
         }
         Hh.register(...$f, Up);
-        const Yg = {
-                line_chart: og,
-                scatter_chart: lg,
-                bezier_chart: jg,
+        const Xg = {
+                line_chart: lg,
+                scatter_chart: ug,
+                bezier_chart: Hg,
                 cubic_bezier_chart: class extends ao {
                     constructor(t) {
                         var e, n;
                         super(t), this.downHandler = t => {
                             const e = $p(this.chartRef.current, t);
                             if (e.length > 0) {
                                 this.chartRef.current.data.datasets[e[0].datasetIndex].isControlPoint && (this.setState({
@@ -27927,15 +28021,15 @@
                                 e.data.datasets[a].data[l].x = o, e.data.datasets[a].data[l].y = s;
                                 const h = e.data.datasets[a].label,
                                     d = e.data.datasets[a].data[l].x,
                                     f = e.data.datasets[a].data[l].y;
                                 this.state.originalData[h].x[l] = d, this.state.originalData[h].y[l] = f;
                                 const p = e.data.datasets[a].data.length;
                                 0 === l ? (e.data.datasets[a].data[l + 1].x += u, e.data.datasets[a].data[l + 1].y += c, this.state.originalData[h].x[l + 1] += u, this.state.originalData[h].y[l + 1] += c) : l === p - 1 ? (e.data.datasets[a].data[l - 1].x += u, e.data.datasets[a].data[l - 1].y += c, this.state.originalData[h].x[l - 1] += u, this.state.originalData[h].y[l - 1] += c) : l % 3 === 0 && 0 !== l && l !== p - 1 ? (e.data.datasets[a].data[l - 1].x += u, e.data.datasets[a].data[l - 1].y += c, e.data.datasets[a].data[l + 1].x += u, e.data.datasets[a].data[l + 1].y += c, this.state.originalData[h].x[l - 1] += u, this.state.originalData[h].y[l - 1] += c, this.state.originalData[h].x[l + 1] += u, this.state.originalData[h].y[l + 1] += c) : (l + 1) % 3 === 0 && l + 1 !== p - 1 ? (e.data.datasets[a].data[l + 2].x -= u, e.data.datasets[a].data[l + 2].y -= c, this.state.originalData[h].x[l + 2] -= u, this.state.originalData[h].y[l + 2] -= c) : (l - 1) % 3 === 0 && l - 1 !== 0 && (e.data.datasets[a].data[l - 2].x -= u, e.data.datasets[a].data[l - 2].y -= c, this.state.originalData[h].x[l - 2] -= u, this.state.originalData[h].y[l - 2] -= c);
-                                const g = Hg(this.state.originalData, this.props.args.options);
+                                const g = $g(this.state.originalData, this.props.args.options);
                                 this.setState({
                                     bezierData: g
                                 }), e.update("none")
                             }
                         }, this.upHandler = t => {
                             this.state.activePoint && (this.sendBezierData(), this.setState({
                                 activePoint: null
@@ -27946,15 +28040,15 @@
                                 return n.fixed_lines.includes(e)
                             })).map(((t, e) => {
                                 let [i, r] = t;
                                 const s = r.x.map(((t, e) => ({
                                         x: t,
                                         y: r.y[e]
                                     }))),
-                                    o = Rg(r.color);
+                                    o = Vg(r.color);
                                 return {
                                     data: s,
                                     isControlPoint: !1,
                                     label: i,
                                     fill: !1,
                                     tension: .3,
                                     showLine: !0,
@@ -27964,25 +28058,25 @@
                                     pointRadius: r.point_radius,
                                     borderDash: r.border_dash
                                 }
                             }))
                         }), this.state = {
                             activePoint: null,
                             originalData: t.args.data,
-                            controlData: Wg(this.props.args.data, this.props.args.options),
-                            bezierData: Hg(this.props.args.data, this.props.args.options),
-                            options: Jp(t.args.options, t.theme)
+                            controlData: Yg(this.props.args.data, this.props.args.options),
+                            bezierData: $g(this.props.args.data, this.props.args.options),
+                            options: tg(t.args.options, t.theme)
                         }
                     }
                     componentDidUpdate(t) {
                         ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                             originalData: this.props.args.data,
-                            controlData: Wg(this.props.args.data, this.props.args.options),
-                            bezierData: Hg(this.props.args.data, this.props.args.options),
-                            options: Jp(this.props.args.options, this.props.theme)
+                            controlData: Yg(this.props.args.data, this.props.args.options),
+                            bezierData: $g(this.props.args.data, this.props.args.options),
+                            options: tg(this.props.args.options, this.props.theme)
                         })
                     }
                     sendBezierData() {
                         const t = this.convertBezierData(this.state.bezierData.datasets);
                         ro.setComponentValue(t)
                     }
                     togglePan(t) {
@@ -28000,28 +28094,28 @@
                                     x: i,
                                     y: r
                                 } = t; - 1 === e[n].x.findIndex(((t, s) => t === i && e[n].y[s] === r)) && (e[n].x.push(i), e[n].y.push(r))
                             }))
                         })), e
                     }
                     render() {
-                        return (0, sg.jsx)(Gp, {
+                        return (0, ag.jsx)(Gp, {
                             ref: this.chartRef,
                             data: {
                                 datasets: [...this.state.controlData.datasets, ...this.state.bezierData.datasets, ...this.fixedData.datasets]
                             },
                             options: this.state.options,
                             onPointerDown: this.downHandler,
                             onPointerUp: this.upHandler,
                             onPointerMove: this.moveHandler
                         })
                     }
                 }
             },
-            $g = function(t) {
+            Kg = function(t) {
                 var e = function(e) {
                     function n(t) {
                         var n = e.call(this, t) || this;
                         return n.componentDidMount = function() {
                             ro.events.addEventListener(ro.RENDER_EVENT, n.onRenderEvent), ro.setComponentReady()
                         }, n.componentDidUpdate = function() {
                             null != n.state.componentError && ro.setFrameHeight()
@@ -28049,22 +28143,22 @@
                         }
                     }, n
                 }(f.PureComponent);
                 return d()(e, t)
             }((t => {
                 const e = t.args.id,
                     n = t.args.kw,
-                    i = Yg[e];
+                    i = Xg[e];
                 if (void 0 === i) throw new Error("Component with id ".concat(e, " is not defined in componentsMap."));
-                return (0, sg.jsx)(i, {
+                return (0, ag.jsx)(i, {
                     args: {
                         ...n
                     },
                     theme: t.theme
                 })
             }));
-        lo.render((0, sg.jsx)(f.StrictMode, {
-            children: (0, sg.jsx)($g, {})
+        lo.render((0, ag.jsx)(f.StrictMode, {
+            children: (0, ag.jsx)(Kg, {})
         }), document.getElementById("root"))
     })()
 })();
-//# sourceMappingURL=main.c3c91322.js.map
+//# sourceMappingURL=main.41dd267d.js.map
```

### Comparing `draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/main.c3c91322.js.LICENSE.txt` & `draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/frontend/build/static/js/main.c3c91322.js.map` & `draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8536813472305321%*

 * *Differences: {"'file'": "'static/js/main.41dd267d.js'",*

 * * "'mappings'": "';2BAAA,OAKA,SAAUA,EAAQC,EAAUC,EAAYC,GACtC,aAEF,IA+FIC,EA/FAC,EAAkB,CAAC,GAAI,SAAU,MAAO,KAAM,KAAM,KACpDC,EAAeL,EAASM,cAAc,OAEtCC,EAAgB,WAEhBC,EAAQC,KAAKD,MACbE,EAAMD,KAAKC,IACXC,EAAMC,KAAKD,IASf,SAASE,EAAkBC,EAAIC,EAASC,GACpC,OAAOC,WAAWC,EAAOJ,EAAIE,GAAUD,EAC3C,CAWA,SAASI,EAAeC,EAAKN,EAAIE,GAC7B,QAAIK,MAAMC,QAAQF,KACdG,EAAKH,EAAKJ,EAAQF,GAAKE,IAChB,EAGf,CAQA,SAASO,EAAKC,EAAKC,EAAUT,GACzB,IAAIU,EAEJ,GAAKF,EAIL,GAAIA,EAAIG,QACJH,EAAIG,QAAQF,EAAUT,QACn […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.c3c91322.js",
+    "file": "static/js/main.41dd267d.js",
     "names": [
         "window",
         "document",
         "exportName",
         "undefined",
         "assign",
         "VENDOR_PREFIXES",
@@ -478,27 +478,67 @@
         "targetComponent",
         "sourceComponent",
         "blacklist",
         "inheritedComponent",
         "targetStatics",
         "sourceStatics",
         "descriptor",
+        "options_1",
+        "utils_1",
+        "DIGIT_GROUPING_BASE",
+        "divider",
+        "denominator",
+        "result",
+        "millify",
+        "_a",
+        "_b",
+        "opts",
+        "defaultOptions",
+        "units",
+        "parseValue",
+        "String",
+        "unitIndex",
+        "toString",
+        "rounded",
+        "roundTo",
+        "precision",
+        "unit",
+        "suffix",
+        "lowercase",
+        "space",
+        "formatted",
+        "toLocaleString",
+        "locales",
+        "getLocales",
+        "minimumFractionDigits",
+        "getFractionDigits",
+        "parseFloat",
+        "isNaN",
+        "Number",
+        "MAX_SAFE_INTEGER",
+        "MIN_SAFE_INTEGER",
+        "RangeError",
+        "isFinite",
+        "isInteger",
+        "toFixed",
+        "num",
+        "decimalPart",
+        "from",
+        "languages",
         "propIsEnumerable",
         "propertyIsEnumerable",
         "test1",
-        "String",
         "test2",
         "fromCharCode",
         "map",
         "n",
         "test3",
         "letter",
         "err",
         "shouldUseNative",
-        "from",
         "symbols",
         "to",
         "toObject",
         "s",
         "aa",
         "r",
         "u",
@@ -569,15 +609,14 @@
         "Ua",
         "Va",
         "xlinkHref",
         "Wa",
         "__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED",
         "Xa",
         "Sa",
-        "isNaN",
         "Ta",
         "Ra",
         "removeAttribute",
         "setAttribute",
         "setAttributeNS",
         "ReactCurrentDispatcher",
         "current",
@@ -658,15 +697,14 @@
         "Nb",
         "Ob",
         "Pb",
         "Qb",
         "namespaceURI",
         "innerHTML",
         "valueOf",
-        "toString",
         "firstChild",
         "removeChild",
         "appendChild",
         "MSApp",
         "execUnsafeLocalFunction",
         "Rb",
         "lastChild",
@@ -1588,15 +1626,14 @@
         "isValidElementType",
         "typeOf",
         "__self",
         "__source",
         "jsx",
         "setState",
         "forceUpdate",
-        "result",
         "keyPrefix",
         "func",
         "escape",
         "IsSomeRendererActing",
         "only",
         "PureComponent",
         "cloneElement",
@@ -1731,15 +1768,14 @@
         "yOffset",
         "xLen",
         "yLen",
         "j",
         "collapseContiguousByteRanges",
         "reduce",
         "sliced",
-        "Number",
         "POSITIVE_INFINITY",
         "subarray",
         "toArrayBufferView",
         "ArrayBufferViewCtor",
         "bytes",
         "toInt32Array",
         "Int32Array",
@@ -1783,15 +1819,14 @@
         "base32",
         "Uint16Array",
         "checks",
         "reverse",
         "toJSON",
         "BN",
         "new",
-        "num",
         "isSigned",
         "Int8Array",
         "Int16Array",
         "unsigned",
         "decimal",
         "proto",
         "DataType",
@@ -1832,35 +1867,31 @@
         "Dictionary",
         "isDenseUnion",
         "Dense",
         "isSparseUnion",
         "Sparse",
         "NONE",
         "toStringTag",
-        "_a",
         "ArrayType",
-        "_b",
         "Int_",
         "bitWidth",
         "super",
         "_c",
         "Int32",
-        "precision",
         "HALF",
         "SINGLE",
         "Float32Array",
         "DOUBLE",
         "Float64Array",
         "_d",
         "_e",
         "_f",
         "_g",
         "_h",
         "Date_",
-        "unit",
         "_j",
         "Time_",
         "_k",
         "Timestamp_",
         "timezone",
         "_l",
         "Interval_",
@@ -2331,15 +2362,14 @@
         "distributeVectorsIntoRecordBatches",
         "vecs",
         "cols",
         "batches",
         "numBatches",
         "batchLength",
         "numColumns",
-        "isFinite",
         "distributeChildren",
         "uniformlyDistributeChunksAcrossRecordBatches",
         "unshift",
         "unwrap",
         "batch",
         "empty",
         "nameToIndex",
@@ -2427,15 +2457,14 @@
         "vtable_in_use",
         "isNested",
         "object_start",
         "vtables",
         "vector_num_elems",
         "force_defaults",
         "string_maps",
-        "space",
         "forceDefaults",
         "dataBuffer",
         "asUint8Array",
         "additional_bytes",
         "align_size",
         "old_buf_size",
         "growByteBuffer",
@@ -3029,15 +3058,14 @@
         "_readFooter",
         "_readDictionaryBatch",
         "rest",
         "VectorAssembler",
         "_bufferRegions",
         "assemble",
         "assembler",
-        "RangeError",
         "addBuffer",
         "_null",
         "assembleFlatVector",
         "assembleFlatListVector",
         "firstOffset",
         "lastOffset",
         "assembleListVector",
@@ -3377,15 +3405,14 @@
         "isNullOrUndef",
         "isNumberFinite",
         "finiteOrDefault",
         "valueOrDefault",
         "toDimension",
         "dimension",
         "endsWith",
-        "parseFloat",
         "loopable",
         "_elementsEqual",
         "a0",
         "a1",
         "ilen",
         "v0",
         "v1",
@@ -3543,15 +3570,14 @@
         "chart",
         "notation",
         "delta",
         "maxTick",
         "calculateDelta",
         "logDelta",
         "numDecimal",
-        "minimumFractionDigits",
         "maximumFractionDigits",
         "logarithmic",
         "remain",
         "significand",
         "Ticks",
         "overrides",
         "descriptors",
@@ -3695,15 +3721,14 @@
         "bezierCurveTo",
         "cp1x",
         "cp2x",
         "cp1y",
         "cp2y",
         "decorateText",
         "line",
-        "opts",
         "strikethrough",
         "underline",
         "metrics",
         "actualBoundingBoxLeft",
         "actualBoundingBoxRight",
         "actualBoundingBoxAscent",
         "actualBoundingBoxDescent",
@@ -3846,15 +3871,14 @@
         "parseMaxStyle",
         "styleValue",
         "parentProperty",
         "valueInPixels",
         "getComputedStyle",
         "positions",
         "getPositionedStyle",
-        "suffix",
         "useOffsetPos",
         "shadowRoot",
         "getRelativePosition",
         "borderBox",
         "boxSizing",
         "paddings",
         "borders",
@@ -4180,15 +4204,14 @@
         "_cache",
         "$bar",
         "visibleMetas",
         "getAllScaleValues",
         "curr",
         "updateMinAndPrev",
         "getPixelForTick",
-        "parseValue",
         "startValue",
         "endValue",
         "barStart",
         "barEnd",
         "_custom",
         "parseFloatBar",
         "parseArrayOrPrimitive",
@@ -5339,15 +5362,14 @@
         "rmin",
         "rmax",
         "countDefined",
         "minSpacing",
         "niceMin",
         "niceMax",
         "numSpaces",
-        "rounded",
         "almostWhole",
         "decimalPlaces",
         "relativeLabelSize",
         "LinearScaleBase",
         "_endValue",
         "handleTickRangeOptions",
         "setMin",
@@ -5437,15 +5459,14 @@
         "adapter",
         "_adapter",
         "parser",
         "isoWeekday",
         "_parseOpts",
         "determineUnitForAutoTicks",
         "minUnit",
-        "MAX_SAFE_INTEGER",
         "addTick",
         "timestamps",
         "ticksFromTimestamps",
         "majorUnit",
         "setMajorTicks",
         "TimeScale",
         "_unit",
@@ -5677,27 +5698,27 @@
         "createScalesOptions",
         "chartElement",
         "cursorStyle",
         "fixed_lines",
         "determineCursorStyle",
         "legend_position",
         "legend_align",
-        "xScaleOptions",
+        "formatTickValue",
         "x_type",
+        "xScaleOptions",
         "x_label",
         "x_grid",
         "fadedText05",
         "x_labels",
         "yScaleOptions",
         "y_type",
         "y_label",
         "y_grid",
         "y_labels",
         "Xvalue",
-        "toFixed",
         "Yvalue",
         "zoomPlugin",
         "downHandler",
         "datasetLabel",
         "activePoint",
         "togglePan",
         "moveHandler",
@@ -5724,15 +5745,14 @@
         "xValue",
         "acos",
         "crt",
         "tau",
         "quart",
         "nMax",
         "nMin",
-        "MIN_SAFE_INTEGER",
         "utils",
         "Tvalues",
         "Cvalues",
         "arcfn",
         "derivativeFn",
         "_3d",
         "mt",
@@ -6134,14 +6154,17 @@
         "componentsMap",
         "ReactDOM"
     ],
     "sourceRoot": "",
     "sources": [
         "../node_modules/hammerjs/hammer.js",
         "../node_modules/hoist-non-react-statics/dist/hoist-non-react-statics.cjs.js",
+        "../node_modules/millify/dist/millify.js",
+        "../node_modules/millify/dist/options.js",
+        "../node_modules/millify/dist/utils.js",
         "../node_modules/object-assign/index.js",
         "../node_modules/react-dom/cjs/react-dom.production.min.js",
         "../node_modules/react-dom/index.js",
         "../node_modules/react-is/cjs/react-is.production.min.js",
         "../node_modules/react-is/index.js",
         "../node_modules/react/cjs/react-jsx-runtime.production.min.js",
         "../node_modules/react/cjs/react.production.min.js",
@@ -6346,14 +6369,17 @@
         "CubicBezierChart/CubicBezierChart.jsx",
         "components.jsx",
         "index.jsx"
     ],
     "sourcesContent": [
         "/*! Hammer.JS - v2.0.7 - 2016-04-22\n * http://hammerjs.github.io/\n *\n * Copyright (c) 2016 Jorik Tangelder;\n * Licensed under the MIT license */\n(function(window, document, exportName, undefined) {\n  'use strict';\n\nvar VENDOR_PREFIXES = ['', 'webkit', 'Moz', 'MS', 'ms', 'o'];\nvar TEST_ELEMENT = document.createElement('div');\n\nvar TYPE_FUNCTION = 'function';\n\nvar round = Math.round;\nvar abs = Math.abs;\nvar now = Date.now;\n\n/**\n * set a timeout with a given scope\n * @param {Function} fn\n * @param {Number} timeout\n * @param {Object} context\n * @returns {number}\n */\nfunction setTimeoutContext(fn, timeout, context) {\n    return setTimeout(bindFn(fn, context), timeout);\n}\n\n/**\n * if the argument is an array, we want to execute the fn on each entry\n * if it aint an array we don't want to do a thing.\n * this is used by all the methods that accept a single and array argument.\n * @param {*|Array} arg\n * @param {String} fn\n * @param {Object} [context]\n * @returns {Boolean}\n */\nfunction invokeArrayArg(arg, fn, context) {\n    if (Array.isArray(arg)) {\n        each(arg, context[fn], context);\n        return true;\n    }\n    return false;\n}\n\n/**\n * walk objects and arrays\n * @param {Object} obj\n * @param {Function} iterator\n * @param {Object} context\n */\nfunction each(obj, iterator, context) {\n    var i;\n\n    if (!obj) {\n        return;\n    }\n\n    if (obj.forEach) {\n        obj.forEach(iterator, context);\n    } else if (obj.length !== undefined) {\n        i = 0;\n        while (i < obj.length) {\n            iterator.call(context, obj[i], i, obj);\n            i++;\n        }\n    } else {\n        for (i in obj) {\n            obj.hasOwnProperty(i) && iterator.call(context, obj[i], i, obj);\n        }\n    }\n}\n\n/**\n * wrap a method with a deprecation warning and stack trace\n * @param {Function} method\n * @param {String} name\n * @param {String} message\n * @returns {Function} A new function wrapping the supplied method.\n */\nfunction deprecate(method, name, message) {\n    var deprecationMessage = 'DEPRECATED METHOD: ' + name + '\\n' + message + ' AT \\n';\n    return function() {\n        var e = new Error('get-stack-trace');\n        var stack = e && e.stack ? e.stack.replace(/^[^\\(]+?[\\n$]/gm, '')\n            .replace(/^\\s+at\\s+/gm, '')\n            .replace(/^Object.<anonymous>\\s*\\(/gm, '{anonymous}()@') : 'Unknown Stack Trace';\n\n        var log = window.console && (window.console.warn || window.console.log);\n        if (log) {\n            log.call(window.console, deprecationMessage, stack);\n        }\n        return method.apply(this, arguments);\n    };\n}\n\n/**\n * extend object.\n * means that properties in dest will be overwritten by the ones in src.\n * @param {Object} target\n * @param {...Object} objects_to_assign\n * @returns {Object} target\n */\nvar assign;\nif (typeof Object.assign !== 'function') {\n    assign = function assign(target) {\n        if (target === undefined || target === null) {\n            throw new TypeError('Cannot convert undefined or null to object');\n        }\n\n        var output = Object(target);\n        for (var index = 1; index < arguments.length; index++) {\n            var source = arguments[index];\n            if (source !== undefined && source !== null) {\n                for (var nextKey in source) {\n                    if (source.hasOwnProperty(nextKey)) {\n                        output[nextKey] = source[nextKey];\n                    }\n                }\n            }\n        }\n        return output;\n    };\n} else {\n    assign = Object.assign;\n}\n\n/**\n * extend object.\n * means that properties in dest will be overwritten by the ones in src.\n * @param {Object} dest\n * @param {Object} src\n * @param {Boolean} [merge=false]\n * @returns {Object} dest\n */\nvar extend = deprecate(function extend(dest, src, merge) {\n    var keys = Object.keys(src);\n    var i = 0;\n    while (i < keys.length) {\n        if (!merge || (merge && dest[keys[i]] === undefined)) {\n            dest[keys[i]] = src[keys[i]];\n        }\n        i++;\n    }\n    return dest;\n}, 'extend', 'Use `assign`.');\n\n/**\n * merge the values from src in the dest.\n * means that properties that exist in dest will not be overwritten by src\n * @param {Object} dest\n * @param {Object} src\n * @returns {Object} dest\n */\nvar merge = deprecate(function merge(dest, src) {\n    return extend(dest, src, true);\n}, 'merge', 'Use `assign`.');\n\n/**\n * simple class inheritance\n * @param {Function} child\n * @param {Function} base\n * @param {Object} [properties]\n */\nfunction inherit(child, base, properties) {\n    var baseP = base.prototype,\n        childP;\n\n    childP = child.prototype = Object.create(baseP);\n    childP.constructor = child;\n    childP._super = baseP;\n\n    if (properties) {\n        assign(childP, properties);\n    }\n}\n\n/**\n * simple function bind\n * @param {Function} fn\n * @param {Object} context\n * @returns {Function}\n */\nfunction bindFn(fn, context) {\n    return function boundFn() {\n        return fn.apply(context, arguments);\n    };\n}\n\n/**\n * let a boolean value also be a function that must return a boolean\n * this first item in args will be used as the context\n * @param {Boolean|Function} val\n * @param {Array} [args]\n * @returns {Boolean}\n */\nfunction boolOrFn(val, args) {\n    if (typeof val == TYPE_FUNCTION) {\n        return val.apply(args ? args[0] || undefined : undefined, args);\n    }\n    return val;\n}\n\n/**\n * use the val2 when val1 is undefined\n * @param {*} val1\n * @param {*} val2\n * @returns {*}\n */\nfunction ifUndefined(val1, val2) {\n    return (val1 === undefined) ? val2 : val1;\n}\n\n/**\n * addEventListener with multiple events at once\n * @param {EventTarget} target\n * @param {String} types\n * @param {Function} handler\n */\nfunction addEventListeners(target, types, handler) {\n    each(splitStr(types), function(type) {\n        target.addEventListener(type, handler, false);\n    });\n}\n\n/**\n * removeEventListener with multiple events at once\n * @param {EventTarget} target\n * @param {String} types\n * @param {Function} handler\n */\nfunction removeEventListeners(target, types, handler) {\n    each(splitStr(types), function(type) {\n        target.removeEventListener(type, handler, false);\n    });\n}\n\n/**\n * find if a node is in the given parent\n * @method hasParent\n * @param {HTMLElement} node\n * @param {HTMLElement} parent\n * @return {Boolean} found\n */\nfunction hasParent(node, parent) {\n    while (node) {\n        if (node == parent) {\n            return true;\n        }\n        node = node.parentNode;\n    }\n    return false;\n}\n\n/**\n * small indexOf wrapper\n * @param {String} str\n * @param {String} find\n * @returns {Boolean} found\n */\nfunction inStr(str, find) {\n    return str.indexOf(find) > -1;\n}\n\n/**\n * split string on whitespace\n * @param {String} str\n * @returns {Array} words\n */\nfunction splitStr(str) {\n    return str.trim().split(/\\s+/g);\n}\n\n/**\n * find if a array contains the object using indexOf or a simple polyFill\n * @param {Array} src\n * @param {String} find\n * @param {String} [findByKey]\n * @return {Boolean|Number} false when not found, or the index\n */\nfunction inArray(src, find, findByKey) {\n    if (src.indexOf && !findByKey) {\n        return src.indexOf(find);\n    } else {\n        var i = 0;\n        while (i < src.length) {\n            if ((findByKey && src[i][findByKey] == find) || (!findByKey && src[i] === find)) {\n                return i;\n            }\n            i++;\n        }\n        return -1;\n    }\n}\n\n/**\n * convert array-like objects to real arrays\n * @param {Object} obj\n * @returns {Array}\n */\nfunction toArray(obj) {\n    return Array.prototype.slice.call(obj, 0);\n}\n\n/**\n * unique array with objects based on a key (like 'id') or just by the array's value\n * @param {Array} src [{id:1},{id:2},{id:1}]\n * @param {String} [key]\n * @param {Boolean} [sort=False]\n * @returns {Array} [{id:1},{id:2}]\n */\nfunction uniqueArray(src, key, sort) {\n    var results = [];\n    var values = [];\n    var i = 0;\n\n    while (i < src.length) {\n        var val = key ? src[i][key] : src[i];\n        if (inArray(values, val) < 0) {\n            results.push(src[i]);\n        }\n        values[i] = val;\n        i++;\n    }\n\n    if (sort) {\n        if (!key) {\n            results = results.sort();\n        } else {\n            results = results.sort(function sortUniqueArray(a, b) {\n                return a[key] > b[key];\n            });\n        }\n    }\n\n    return results;\n}\n\n/**\n * get the prefixed property\n * @param {Object} obj\n * @param {String} property\n * @returns {String|Undefined} prefixed\n */\nfunction prefixed(obj, property) {\n    var prefix, prop;\n    var camelProp = property[0].toUpperCase() + property.slice(1);\n\n    var i = 0;\n    while (i < VENDOR_PREFIXES.length) {\n        prefix = VENDOR_PREFIXES[i];\n        prop = (prefix) ? prefix + camelProp : property;\n\n        if (prop in obj) {\n            return prop;\n        }\n        i++;\n    }\n    return undefined;\n}\n\n/**\n * get a unique id\n * @returns {number} uniqueId\n */\nvar _uniqueId = 1;\nfunction uniqueId() {\n    return _uniqueId++;\n}\n\n/**\n * get the window object of an element\n * @param {HTMLElement} element\n * @returns {DocumentView|Window}\n */\nfunction getWindowForElement(element) {\n    var doc = element.ownerDocument || element;\n    return (doc.defaultView || doc.parentWindow || window);\n}\n\nvar MOBILE_REGEX = /mobile|tablet|ip(ad|hone|od)|android/i;\n\nvar SUPPORT_TOUCH = ('ontouchstart' in window);\nvar SUPPORT_POINTER_EVENTS = prefixed(window, 'PointerEvent') !== undefined;\nvar SUPPORT_ONLY_TOUCH = SUPPORT_TOUCH && MOBILE_REGEX.test(navigator.userAgent);\n\nvar INPUT_TYPE_TOUCH = 'touch';\nvar INPUT_TYPE_PEN = 'pen';\nvar INPUT_TYPE_MOUSE = 'mouse';\nvar INPUT_TYPE_KINECT = 'kinect';\n\nvar COMPUTE_INTERVAL = 25;\n\nvar INPUT_START = 1;\nvar INPUT_MOVE = 2;\nvar INPUT_END = 4;\nvar INPUT_CANCEL = 8;\n\nvar DIRECTION_NONE = 1;\nvar DIRECTION_LEFT = 2;\nvar DIRECTION_RIGHT = 4;\nvar DIRECTION_UP = 8;\nvar DIRECTION_DOWN = 16;\n\nvar DIRECTION_HORIZONTAL = DIRECTION_LEFT | DIRECTION_RIGHT;\nvar DIRECTION_VERTICAL = DIRECTION_UP | DIRECTION_DOWN;\nvar DIRECTION_ALL = DIRECTION_HORIZONTAL | DIRECTION_VERTICAL;\n\nvar PROPS_XY = ['x', 'y'];\nvar PROPS_CLIENT_XY = ['clientX', 'clientY'];\n\n/**\n * create new input type manager\n * @param {Manager} manager\n * @param {Function} callback\n * @returns {Input}\n * @constructor\n */\nfunction Input(manager, callback) {\n    var self = this;\n    this.manager = manager;\n    this.callback = callback;\n    this.element = manager.element;\n    this.target = manager.options.inputTarget;\n\n    // smaller wrapper around the handler, for the scope and the enabled state of the manager,\n    // so when disabled the input events are completely bypassed.\n    this.domHandler = function(ev) {\n        if (boolOrFn(manager.options.enable, [manager])) {\n            self.handler(ev);\n        }\n    };\n\n    this.init();\n\n}\n\nInput.prototype = {\n    /**\n     * should handle the inputEvent data and trigger the callback\n     * @virtual\n     */\n    handler: function() { },\n\n    /**\n     * bind the events\n     */\n    init: function() {\n        this.evEl && addEventListeners(this.element, this.evEl, this.domHandler);\n        this.evTarget && addEventListeners(this.target, this.evTarget, this.domHandler);\n        this.evWin && addEventListeners(getWindowForElement(this.element), this.evWin, this.domHandler);\n    },\n\n    /**\n     * unbind the events\n     */\n    destroy: function() {\n        this.evEl && removeEventListeners(this.element, this.evEl, this.domHandler);\n        this.evTarget && removeEventListeners(this.target, this.evTarget, this.domHandler);\n        this.evWin && removeEventListeners(getWindowForElement(this.element), this.evWin, this.domHandler);\n    }\n};\n\n/**\n * create new input type manager\n * called by the Manager constructor\n * @param {Hammer} manager\n * @returns {Input}\n */\nfunction createInputInstance(manager) {\n    var Type;\n    var inputClass = manager.options.inputClass;\n\n    if (inputClass) {\n        Type = inputClass;\n    } else if (SUPPORT_POINTER_EVENTS) {\n        Type = PointerEventInput;\n    } else if (SUPPORT_ONLY_TOUCH) {\n        Type = TouchInput;\n    } else if (!SUPPORT_TOUCH) {\n        Type = MouseInput;\n    } else {\n        Type = TouchMouseInput;\n    }\n    return new (Type)(manager, inputHandler);\n}\n\n/**\n * handle input events\n * @param {Manager} manager\n * @param {String} eventType\n * @param {Object} input\n */\nfunction inputHandler(manager, eventType, input) {\n    var pointersLen = input.pointers.length;\n    var changedPointersLen = input.changedPointers.length;\n    var isFirst = (eventType & INPUT_START && (pointersLen - changedPointersLen === 0));\n    var isFinal = (eventType & (INPUT_END | INPUT_CANCEL) && (pointersLen - changedPointersLen === 0));\n\n    input.isFirst = !!isFirst;\n    input.isFinal = !!isFinal;\n\n    if (isFirst) {\n        manager.session = {};\n    }\n\n    // source event is the normalized value of the domEvents\n    // like 'touchstart, mouseup, pointerdown'\n    input.eventType = eventType;\n\n    // compute scale, rotation etc\n    computeInputData(manager, input);\n\n    // emit secret event\n    manager.emit('hammer.input', input);\n\n    manager.recognize(input);\n    manager.session.prevInput = input;\n}\n\n/**\n * extend the data with some usable properties like scale, rotate, velocity etc\n * @param {Object} manager\n * @param {Object} input\n */\nfunction computeInputData(manager, input) {\n    var session = manager.session;\n    var pointers = input.pointers;\n    var pointersLength = pointers.length;\n\n    // store the first input to calculate the distance and direction\n    if (!session.firstInput) {\n        session.firstInput = simpleCloneInputData(input);\n    }\n\n    // to compute scale and rotation we need to store the multiple touches\n    if (pointersLength > 1 && !session.firstMultiple) {\n        session.firstMultiple = simpleCloneInputData(input);\n    } else if (pointersLength === 1) {\n        session.firstMultiple = false;\n    }\n\n    var firstInput = session.firstInput;\n    var firstMultiple = session.firstMultiple;\n    var offsetCenter = firstMultiple ? firstMultiple.center : firstInput.center;\n\n    var center = input.center = getCenter(pointers);\n    input.timeStamp = now();\n    input.deltaTime = input.timeStamp - firstInput.timeStamp;\n\n    input.angle = getAngle(offsetCenter, center);\n    input.distance = getDistance(offsetCenter, center);\n\n    computeDeltaXY(session, input);\n    input.offsetDirection = getDirection(input.deltaX, input.deltaY);\n\n    var overallVelocity = getVelocity(input.deltaTime, input.deltaX, input.deltaY);\n    input.overallVelocityX = overallVelocity.x;\n    input.overallVelocityY = overallVelocity.y;\n    input.overallVelocity = (abs(overallVelocity.x) > abs(overallVelocity.y)) ? overallVelocity.x : overallVelocity.y;\n\n    input.scale = firstMultiple ? getScale(firstMultiple.pointers, pointers) : 1;\n    input.rotation = firstMultiple ? getRotation(firstMultiple.pointers, pointers) : 0;\n\n    input.maxPointers = !session.prevInput ? input.pointers.length : ((input.pointers.length >\n        session.prevInput.maxPointers) ? input.pointers.length : session.prevInput.maxPointers);\n\n    computeIntervalInputData(session, input);\n\n    // find the correct target\n    var target = manager.element;\n    if (hasParent(input.srcEvent.target, target)) {\n        target = input.srcEvent.target;\n    }\n    input.target = target;\n}\n\nfunction computeDeltaXY(session, input) {\n    var center = input.center;\n    var offset = session.offsetDelta || {};\n    var prevDelta = session.prevDelta || {};\n    var prevInput = session.prevInput || {};\n\n    if (input.eventType === INPUT_START || prevInput.eventType === INPUT_END) {\n        prevDelta = session.prevDelta = {\n            x: prevInput.deltaX || 0,\n            y: prevInput.deltaY || 0\n        };\n\n        offset = session.offsetDelta = {\n            x: center.x,\n            y: center.y\n        };\n    }\n\n    input.deltaX = prevDelta.x + (center.x - offset.x);\n    input.deltaY = prevDelta.y + (center.y - offset.y);\n}\n\n/**\n * velocity is calculated every x ms\n * @param {Object} session\n * @param {Object} input\n */\nfunction computeIntervalInputData(session, input) {\n    var last = session.lastInterval || input,\n        deltaTime = input.timeStamp - last.timeStamp,\n        velocity, velocityX, velocityY, direction;\n\n    if (input.eventType != INPUT_CANCEL && (deltaTime > COMPUTE_INTERVAL || last.velocity === undefined)) {\n        var deltaX = input.deltaX - last.deltaX;\n        var deltaY = input.deltaY - last.deltaY;\n\n        var v = getVelocity(deltaTime, deltaX, deltaY);\n        velocityX = v.x;\n        velocityY = v.y;\n        velocity = (abs(v.x) > abs(v.y)) ? v.x : v.y;\n        direction = getDirection(deltaX, deltaY);\n\n        session.lastInterval = input;\n    } else {\n        // use latest velocity info if it doesn't overtake a minimum period\n        velocity = last.velocity;\n        velocityX = last.velocityX;\n        velocityY = last.velocityY;\n        direction = last.direction;\n    }\n\n    input.velocity = velocity;\n    input.velocityX = velocityX;\n    input.velocityY = velocityY;\n    input.direction = direction;\n}\n\n/**\n * create a simple clone from the input used for storage of firstInput and firstMultiple\n * @param {Object} input\n * @returns {Object} clonedInputData\n */\nfunction simpleCloneInputData(input) {\n    // make a simple copy of the pointers because we will get a reference if we don't\n    // we only need clientXY for the calculations\n    var pointers = [];\n    var i = 0;\n    while (i < input.pointers.length) {\n        pointers[i] = {\n            clientX: round(input.pointers[i].clientX),\n            clientY: round(input.pointers[i].clientY)\n        };\n        i++;\n    }\n\n    return {\n        timeStamp: now(),\n        pointers: pointers,\n        center: getCenter(pointers),\n        deltaX: input.deltaX,\n        deltaY: input.deltaY\n    };\n}\n\n/**\n * get the center of all the pointers\n * @param {Array} pointers\n * @return {Object} center contains `x` and `y` properties\n */\nfunction getCenter(pointers) {\n    var pointersLength = pointers.length;\n\n    // no need to loop when only one touch\n    if (pointersLength === 1) {\n        return {\n            x: round(pointers[0].clientX),\n            y: round(pointers[0].clientY)\n        };\n    }\n\n    var x = 0, y = 0, i = 0;\n    while (i < pointersLength) {\n        x += pointers[i].clientX;\n        y += pointers[i].clientY;\n        i++;\n    }\n\n    return {\n        x: round(x / pointersLength),\n        y: round(y / pointersLength)\n    };\n}\n\n/**\n * calculate the velocity between two points. unit is in px per ms.\n * @param {Number} deltaTime\n * @param {Number} x\n * @param {Number} y\n * @return {Object} velocity `x` and `y`\n */\nfunction getVelocity(deltaTime, x, y) {\n    return {\n        x: x / deltaTime || 0,\n        y: y / deltaTime || 0\n    };\n}\n\n/**\n * get the direction between two points\n * @param {Number} x\n * @param {Number} y\n * @return {Number} direction\n */\nfunction getDirection(x, y) {\n    if (x === y) {\n        return DIRECTION_NONE;\n    }\n\n    if (abs(x) >= abs(y)) {\n        return x < 0 ? DIRECTION_LEFT : DIRECTION_RIGHT;\n    }\n    return y < 0 ? DIRECTION_UP : DIRECTION_DOWN;\n}\n\n/**\n * calculate the absolute distance between two points\n * @param {Object} p1 {x, y}\n * @param {Object} p2 {x, y}\n * @param {Array} [props] containing x and y keys\n * @return {Number} distance\n */\nfunction getDistance(p1, p2, props) {\n    if (!props) {\n        props = PROPS_XY;\n    }\n    var x = p2[props[0]] - p1[props[0]],\n        y = p2[props[1]] - p1[props[1]];\n\n    return Math.sqrt((x * x) + (y * y));\n}\n\n/**\n * calculate the angle between two coordinates\n * @param {Object} p1\n * @param {Object} p2\n * @param {Array} [props] containing x and y keys\n * @return {Number} angle\n */\nfunction getAngle(p1, p2, props) {\n    if (!props) {\n        props = PROPS_XY;\n    }\n    var x = p2[props[0]] - p1[props[0]],\n        y = p2[props[1]] - p1[props[1]];\n    return Math.atan2(y, x) * 180 / Math.PI;\n}\n\n/**\n * calculate the rotation degrees between two pointersets\n * @param {Array} start array of pointers\n * @param {Array} end array of pointers\n * @return {Number} rotation\n */\nfunction getRotation(start, end) {\n    return getAngle(end[1], end[0], PROPS_CLIENT_XY) + getAngle(start[1], start[0], PROPS_CLIENT_XY);\n}\n\n/**\n * calculate the scale factor between two pointersets\n * no scale is 1, and goes down to 0 when pinched together, and bigger when pinched out\n * @param {Array} start array of pointers\n * @param {Array} end array of pointers\n * @return {Number} scale\n */\nfunction getScale(start, end) {\n    return getDistance(end[0], end[1], PROPS_CLIENT_XY) / getDistance(start[0], start[1], PROPS_CLIENT_XY);\n}\n\nvar MOUSE_INPUT_MAP = {\n    mousedown: INPUT_START,\n    mousemove: INPUT_MOVE,\n    mouseup: INPUT_END\n};\n\nvar MOUSE_ELEMENT_EVENTS = 'mousedown';\nvar MOUSE_WINDOW_EVENTS = 'mousemove mouseup';\n\n/**\n * Mouse events input\n * @constructor\n * @extends Input\n */\nfunction MouseInput() {\n    this.evEl = MOUSE_ELEMENT_EVENTS;\n    this.evWin = MOUSE_WINDOW_EVENTS;\n\n    this.pressed = false; // mousedown state\n\n    Input.apply(this, arguments);\n}\n\ninherit(MouseInput, Input, {\n    /**\n     * handle mouse events\n     * @param {Object} ev\n     */\n    handler: function MEhandler(ev) {\n        var eventType = MOUSE_INPUT_MAP[ev.type];\n\n        // on start we want to have the left mouse button down\n        if (eventType & INPUT_START && ev.button === 0) {\n            this.pressed = true;\n        }\n\n        if (eventType & INPUT_MOVE && ev.which !== 1) {\n            eventType = INPUT_END;\n        }\n\n        // mouse must be down\n        if (!this.pressed) {\n            return;\n        }\n\n        if (eventType & INPUT_END) {\n            this.pressed = false;\n        }\n\n        this.callback(this.manager, eventType, {\n            pointers: [ev],\n            changedPointers: [ev],\n            pointerType: INPUT_TYPE_MOUSE,\n            srcEvent: ev\n        });\n    }\n});\n\nvar POINTER_INPUT_MAP = {\n    pointerdown: INPUT_START,\n    pointermove: INPUT_MOVE,\n    pointerup: INPUT_END,\n    pointercancel: INPUT_CANCEL,\n    pointerout: INPUT_CANCEL\n};\n\n// in IE10 the pointer types is defined as an enum\nvar IE10_POINTER_TYPE_ENUM = {\n    2: INPUT_TYPE_TOUCH,\n    3: INPUT_TYPE_PEN,\n    4: INPUT_TYPE_MOUSE,\n    5: INPUT_TYPE_KINECT // see https://twitter.com/jacobrossi/status/480596438489890816\n};\n\nvar POINTER_ELEMENT_EVENTS = 'pointerdown';\nvar POINTER_WINDOW_EVENTS = 'pointermove pointerup pointercancel';\n\n// IE10 has prefixed support, and case-sensitive\nif (window.MSPointerEvent && !window.PointerEvent) {\n    POINTER_ELEMENT_EVENTS = 'MSPointerDown';\n    POINTER_WINDOW_EVENTS = 'MSPointerMove MSPointerUp MSPointerCancel';\n}\n\n/**\n * Pointer events input\n * @constructor\n * @extends Input\n */\nfunction PointerEventInput() {\n    this.evEl = POINTER_ELEMENT_EVENTS;\n    this.evWin = POINTER_WINDOW_EVENTS;\n\n    Input.apply(this, arguments);\n\n    this.store = (this.manager.session.pointerEvents = []);\n}\n\ninherit(PointerEventInput, Input, {\n    /**\n     * handle mouse events\n     * @param {Object} ev\n     */\n    handler: function PEhandler(ev) {\n        var store = this.store;\n        var removePointer = false;\n\n        var eventTypeNormalized = ev.type.toLowerCase().replace('ms', '');\n        var eventType = POINTER_INPUT_MAP[eventTypeNormalized];\n        var pointerType = IE10_POINTER_TYPE_ENUM[ev.pointerType] || ev.pointerType;\n\n        var isTouch = (pointerType == INPUT_TYPE_TOUCH);\n\n        // get index of the event in the store\n        var storeIndex = inArray(store, ev.pointerId, 'pointerId');\n\n        // start and mouse must be down\n        if (eventType & INPUT_START && (ev.button === 0 || isTouch)) {\n            if (storeIndex < 0) {\n                store.push(ev);\n                storeIndex = store.length - 1;\n            }\n        } else if (eventType & (INPUT_END | INPUT_CANCEL)) {\n            removePointer = true;\n        }\n\n        // it not found, so the pointer hasn't been down (so it's probably a hover)\n        if (storeIndex < 0) {\n            return;\n        }\n\n        // update the event in the store\n        store[storeIndex] = ev;\n\n        this.callback(this.manager, eventType, {\n            pointers: store,\n            changedPointers: [ev],\n            pointerType: pointerType,\n            srcEvent: ev\n        });\n\n        if (removePointer) {\n            // remove from the store\n            store.splice(storeIndex, 1);\n        }\n    }\n});\n\nvar SINGLE_TOUCH_INPUT_MAP = {\n    touchstart: INPUT_START,\n    touchmove: INPUT_MOVE,\n    touchend: INPUT_END,\n    touchcancel: INPUT_CANCEL\n};\n\nvar SINGLE_TOUCH_TARGET_EVENTS = 'touchstart';\nvar SINGLE_TOUCH_WINDOW_EVENTS = 'touchstart touchmove touchend touchcancel';\n\n/**\n * Touch events input\n * @constructor\n * @extends Input\n */\nfunction SingleTouchInput() {\n    this.evTarget = SINGLE_TOUCH_TARGET_EVENTS;\n    this.evWin = SINGLE_TOUCH_WINDOW_EVENTS;\n    this.started = false;\n\n    Input.apply(this, arguments);\n}\n\ninherit(SingleTouchInput, Input, {\n    handler: function TEhandler(ev) {\n        var type = SINGLE_TOUCH_INPUT_MAP[ev.type];\n\n        // should we handle the touch events?\n        if (type === INPUT_START) {\n            this.started = true;\n        }\n\n        if (!this.started) {\n            return;\n        }\n\n        var touches = normalizeSingleTouches.call(this, ev, type);\n\n        // when done, reset the started state\n        if (type & (INPUT_END | INPUT_CANCEL) && touches[0].length - touches[1].length === 0) {\n            this.started = false;\n        }\n\n        this.callback(this.manager, type, {\n            pointers: touches[0],\n            changedPointers: touches[1],\n            pointerType: INPUT_TYPE_TOUCH,\n            srcEvent: ev\n        });\n    }\n});\n\n/**\n * @this {TouchInput}\n * @param {Object} ev\n * @param {Number} type flag\n * @returns {undefined|Array} [all, changed]\n */\nfunction normalizeSingleTouches(ev, type) {\n    var all = toArray(ev.touches);\n    var changed = toArray(ev.changedTouches);\n\n    if (type & (INPUT_END | INPUT_CANCEL)) {\n        all = uniqueArray(all.concat(changed), 'identifier', true);\n    }\n\n    return [all, changed];\n}\n\nvar TOUCH_INPUT_MAP = {\n    touchstart: INPUT_START,\n    touchmove: INPUT_MOVE,\n    touchend: INPUT_END,\n    touchcancel: INPUT_CANCEL\n};\n\nvar TOUCH_TARGET_EVENTS = 'touchstart touchmove touchend touchcancel';\n\n/**\n * Multi-user touch events input\n * @constructor\n * @extends Input\n */\nfunction TouchInput() {\n    this.evTarget = TOUCH_TARGET_EVENTS;\n    this.targetIds = {};\n\n    Input.apply(this, arguments);\n}\n\ninherit(TouchInput, Input, {\n    handler: function MTEhandler(ev) {\n        var type = TOUCH_INPUT_MAP[ev.type];\n        var touches = getTouches.call(this, ev, type);\n        if (!touches) {\n            return;\n        }\n\n        this.callback(this.manager, type, {\n            pointers: touches[0],\n            changedPointers: touches[1],\n            pointerType: INPUT_TYPE_TOUCH,\n            srcEvent: ev\n        });\n    }\n});\n\n/**\n * @this {TouchInput}\n * @param {Object} ev\n * @param {Number} type flag\n * @returns {undefined|Array} [all, changed]\n */\nfunction getTouches(ev, type) {\n    var allTouches = toArray(ev.touches);\n    var targetIds = this.targetIds;\n\n    // when there is only one touch, the process can be simplified\n    if (type & (INPUT_START | INPUT_MOVE) && allTouches.length === 1) {\n        targetIds[allTouches[0].identifier] = true;\n        return [allTouches, allTouches];\n    }\n\n    var i,\n        targetTouches,\n        changedTouches = toArray(ev.changedTouches),\n        changedTargetTouches = [],\n        target = this.target;\n\n    // get target touches from touches\n    targetTouches = allTouches.filter(function(touch) {\n        return hasParent(touch.target, target);\n    });\n\n    // collect touches\n    if (type === INPUT_START) {\n        i = 0;\n        while (i < targetTouches.length) {\n            targetIds[targetTouches[i].identifier] = true;\n            i++;\n        }\n    }\n\n    // filter changed touches to only contain touches that exist in the collected target ids\n    i = 0;\n    while (i < changedTouches.length) {\n        if (targetIds[changedTouches[i].identifier]) {\n            changedTargetTouches.push(changedTouches[i]);\n        }\n\n        // cleanup removed touches\n        if (type & (INPUT_END | INPUT_CANCEL)) {\n            delete targetIds[changedTouches[i].identifier];\n        }\n        i++;\n    }\n\n    if (!changedTargetTouches.length) {\n        return;\n    }\n\n    return [\n        // merge targetTouches with changedTargetTouches so it contains ALL touches, including 'end' and 'cancel'\n        uniqueArray(targetTouches.concat(changedTargetTouches), 'identifier', true),\n        changedTargetTouches\n    ];\n}\n\n/**\n * Combined touch and mouse input\n *\n * Touch has a higher priority then mouse, and while touching no mouse events are allowed.\n * This because touch devices also emit mouse events while doing a touch.\n *\n * @constructor\n * @extends Input\n */\n\nvar DEDUP_TIMEOUT = 2500;\nvar DEDUP_DISTANCE = 25;\n\nfunction TouchMouseInput() {\n    Input.apply(this, arguments);\n\n    var handler = bindFn(this.handler, this);\n    this.touch = new TouchInput(this.manager, handler);\n    this.mouse = new MouseInput(this.manager, handler);\n\n    this.primaryTouch = null;\n    this.lastTouches = [];\n}\n\ninherit(TouchMouseInput, Input, {\n    /**\n     * handle mouse and touch events\n     * @param {Hammer} manager\n     * @param {String} inputEvent\n     * @param {Object} inputData\n     */\n    handler: function TMEhandler(manager, inputEvent, inputData) {\n        var isTouch = (inputData.pointerType == INPUT_TYPE_TOUCH),\n            isMouse = (inputData.pointerType == INPUT_TYPE_MOUSE);\n\n        if (isMouse && inputData.sourceCapabilities && inputData.sourceCapabilities.firesTouchEvents) {\n            return;\n        }\n\n        // when we're in a touch event, record touches to  de-dupe synthetic mouse event\n        if (isTouch) {\n            recordTouches.call(this, inputEvent, inputData);\n        } else if (isMouse && isSyntheticEvent.call(this, inputData)) {\n            return;\n        }\n\n        this.callback(manager, inputEvent, inputData);\n    },\n\n    /**\n     * remove the event listeners\n     */\n    destroy: function destroy() {\n        this.touch.destroy();\n        this.mouse.destroy();\n    }\n});\n\nfunction recordTouches(eventType, eventData) {\n    if (eventType & INPUT_START) {\n        this.primaryTouch = eventData.changedPointers[0].identifier;\n        setLastTouch.call(this, eventData);\n    } else if (eventType & (INPUT_END | INPUT_CANCEL)) {\n        setLastTouch.call(this, eventData);\n    }\n}\n\nfunction setLastTouch(eventData) {\n    var touch = eventData.changedPointers[0];\n\n    if (touch.identifier === this.primaryTouch) {\n        var lastTouch = {x: touch.clientX, y: touch.clientY};\n        this.lastTouches.push(lastTouch);\n        var lts = this.lastTouches;\n        var removeLastTouch = function() {\n            var i = lts.indexOf(lastTouch);\n            if (i > -1) {\n                lts.splice(i, 1);\n            }\n        };\n        setTimeout(removeLastTouch, DEDUP_TIMEOUT);\n    }\n}\n\nfunction isSyntheticEvent(eventData) {\n    var x = eventData.srcEvent.clientX, y = eventData.srcEvent.clientY;\n    for (var i = 0; i < this.lastTouches.length; i++) {\n        var t = this.lastTouches[i];\n        var dx = Math.abs(x - t.x), dy = Math.abs(y - t.y);\n        if (dx <= DEDUP_DISTANCE && dy <= DEDUP_DISTANCE) {\n            return true;\n        }\n    }\n    return false;\n}\n\nvar PREFIXED_TOUCH_ACTION = prefixed(TEST_ELEMENT.style, 'touchAction');\nvar NATIVE_TOUCH_ACTION = PREFIXED_TOUCH_ACTION !== undefined;\n\n// magical touchAction value\nvar TOUCH_ACTION_COMPUTE = 'compute';\nvar TOUCH_ACTION_AUTO = 'auto';\nvar TOUCH_ACTION_MANIPULATION = 'manipulation'; // not implemented\nvar TOUCH_ACTION_NONE = 'none';\nvar TOUCH_ACTION_PAN_X = 'pan-x';\nvar TOUCH_ACTION_PAN_Y = 'pan-y';\nvar TOUCH_ACTION_MAP = getTouchActionProps();\n\n/**\n * Touch Action\n * sets the touchAction property or uses the js alternative\n * @param {Manager} manager\n * @param {String} value\n * @constructor\n */\nfunction TouchAction(manager, value) {\n    this.manager = manager;\n    this.set(value);\n}\n\nTouchAction.prototype = {\n    /**\n     * set the touchAction value on the element or enable the polyfill\n     * @param {String} value\n     */\n    set: function(value) {\n        // find out the touch-action by the event handlers\n        if (value == TOUCH_ACTION_COMPUTE) {\n            value = this.compute();\n        }\n\n        if (NATIVE_TOUCH_ACTION && this.manager.element.style && TOUCH_ACTION_MAP[value]) {\n            this.manager.element.style[PREFIXED_TOUCH_ACTION] = value;\n        }\n        this.actions = value.toLowerCase().trim();\n    },\n\n    /**\n     * just re-set the touchAction value\n     */\n    update: function() {\n        this.set(this.manager.options.touchAction);\n    },\n\n    /**\n     * compute the value for the touchAction property based on the recognizer's settings\n     * @returns {String} value\n     */\n    compute: function() {\n        var actions = [];\n        each(this.manager.recognizers, function(recognizer) {\n            if (boolOrFn(recognizer.options.enable, [recognizer])) {\n                actions = actions.concat(recognizer.getTouchAction());\n            }\n        });\n        return cleanTouchActions(actions.join(' '));\n    },\n\n    /**\n     * this method is called on each input cycle and provides the preventing of the browser behavior\n     * @param {Object} input\n     */\n    preventDefaults: function(input) {\n        var srcEvent = input.srcEvent;\n        var direction = input.offsetDirection;\n\n        // if the touch action did prevented once this session\n        if (this.manager.session.prevented) {\n            srcEvent.preventDefault();\n            return;\n        }\n\n        var actions = this.actions;\n        var hasNone = inStr(actions, TOUCH_ACTION_NONE) && !TOUCH_ACTION_MAP[TOUCH_ACTION_NONE];\n        var hasPanY = inStr(actions, TOUCH_ACTION_PAN_Y) && !TOUCH_ACTION_MAP[TOUCH_ACTION_PAN_Y];\n        var hasPanX = inStr(actions, TOUCH_ACTION_PAN_X) && !TOUCH_ACTION_MAP[TOUCH_ACTION_PAN_X];\n\n        if (hasNone) {\n            //do not prevent defaults if this is a tap gesture\n\n            var isTapPointer = input.pointers.length === 1;\n            var isTapMovement = input.distance < 2;\n            var isTapTouchTime = input.deltaTime < 250;\n\n            if (isTapPointer && isTapMovement && isTapTouchTime) {\n                return;\n            }\n        }\n\n        if (hasPanX && hasPanY) {\n            // `pan-x pan-y` means browser handles all scrolling/panning, do not prevent\n            return;\n        }\n\n        if (hasNone ||\n            (hasPanY && direction & DIRECTION_HORIZONTAL) ||\n            (hasPanX && direction & DIRECTION_VERTICAL)) {\n            return this.preventSrc(srcEvent);\n        }\n    },\n\n    /**\n     * call preventDefault to prevent the browser's default behavior (scrolling in most cases)\n     * @param {Object} srcEvent\n     */\n    preventSrc: function(srcEvent) {\n        this.manager.session.prevented = true;\n        srcEvent.preventDefault();\n    }\n};\n\n/**\n * when the touchActions are collected they are not a valid value, so we need to clean things up. *\n * @param {String} actions\n * @returns {*}\n */\nfunction cleanTouchActions(actions) {\n    // none\n    if (inStr(actions, TOUCH_ACTION_NONE)) {\n        return TOUCH_ACTION_NONE;\n    }\n\n    var hasPanX = inStr(actions, TOUCH_ACTION_PAN_X);\n    var hasPanY = inStr(actions, TOUCH_ACTION_PAN_Y);\n\n    // if both pan-x and pan-y are set (different recognizers\n    // for different directions, e.g. horizontal pan but vertical swipe?)\n    // we need none (as otherwise with pan-x pan-y combined none of these\n    // recognizers will work, since the browser would handle all panning\n    if (hasPanX && hasPanY) {\n        return TOUCH_ACTION_NONE;\n    }\n\n    // pan-x OR pan-y\n    if (hasPanX || hasPanY) {\n        return hasPanX ? TOUCH_ACTION_PAN_X : TOUCH_ACTION_PAN_Y;\n    }\n\n    // manipulation\n    if (inStr(actions, TOUCH_ACTION_MANIPULATION)) {\n        return TOUCH_ACTION_MANIPULATION;\n    }\n\n    return TOUCH_ACTION_AUTO;\n}\n\nfunction getTouchActionProps() {\n    if (!NATIVE_TOUCH_ACTION) {\n        return false;\n    }\n    var touchMap = {};\n    var cssSupports = window.CSS && window.CSS.supports;\n    ['auto', 'manipulation', 'pan-y', 'pan-x', 'pan-x pan-y', 'none'].forEach(function(val) {\n\n        // If css.supports is not supported but there is native touch-action assume it supports\n        // all values. This is the case for IE 10 and 11.\n        touchMap[val] = cssSupports ? window.CSS.supports('touch-action', val) : true;\n    });\n    return touchMap;\n}\n\n/**\n * Recognizer flow explained; *\n * All recognizers have the initial state of POSSIBLE when a input session starts.\n * The definition of a input session is from the first input until the last input, with all it's movement in it. *\n * Example session for mouse-input: mousedown -> mousemove -> mouseup\n *\n * On each recognizing cycle (see Manager.recognize) the .recognize() method is executed\n * which determines with state it should be.\n *\n * If the recognizer has the state FAILED, CANCELLED or RECOGNIZED (equals ENDED), it is reset to\n * POSSIBLE to give it another change on the next cycle.\n *\n *               Possible\n *                  |\n *            +-----+---------------+\n *            |                     |\n *      +-----+-----+               |\n *      |           |               |\n *   Failed      Cancelled          |\n *                          +-------+------+\n *                          |              |\n *                      Recognized       Began\n *                                         |\n *                                      Changed\n *                                         |\n *                                  Ended/Recognized\n */\nvar STATE_POSSIBLE = 1;\nvar STATE_BEGAN = 2;\nvar STATE_CHANGED = 4;\nvar STATE_ENDED = 8;\nvar STATE_RECOGNIZED = STATE_ENDED;\nvar STATE_CANCELLED = 16;\nvar STATE_FAILED = 32;\n\n/**\n * Recognizer\n * Every recognizer needs to extend from this class.\n * @constructor\n * @param {Object} options\n */\nfunction Recognizer(options) {\n    this.options = assign({}, this.defaults, options || {});\n\n    this.id = uniqueId();\n\n    this.manager = null;\n\n    // default is enable true\n    this.options.enable = ifUndefined(this.options.enable, true);\n\n    this.state = STATE_POSSIBLE;\n\n    this.simultaneous = {};\n    this.requireFail = [];\n}\n\nRecognizer.prototype = {\n    /**\n     * @virtual\n     * @type {Object}\n     */\n    defaults: {},\n\n    /**\n     * set options\n     * @param {Object} options\n     * @return {Recognizer}\n     */\n    set: function(options) {\n        assign(this.options, options);\n\n        // also update the touchAction, in case something changed about the directions/enabled state\n        this.manager && this.manager.touchAction.update();\n        return this;\n    },\n\n    /**\n     * recognize simultaneous with an other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    recognizeWith: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'recognizeWith', this)) {\n            return this;\n        }\n\n        var simultaneous = this.simultaneous;\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        if (!simultaneous[otherRecognizer.id]) {\n            simultaneous[otherRecognizer.id] = otherRecognizer;\n            otherRecognizer.recognizeWith(this);\n        }\n        return this;\n    },\n\n    /**\n     * drop the simultaneous link. it doesnt remove the link on the other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    dropRecognizeWith: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'dropRecognizeWith', this)) {\n            return this;\n        }\n\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        delete this.simultaneous[otherRecognizer.id];\n        return this;\n    },\n\n    /**\n     * recognizer can only run when an other is failing\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    requireFailure: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'requireFailure', this)) {\n            return this;\n        }\n\n        var requireFail = this.requireFail;\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        if (inArray(requireFail, otherRecognizer) === -1) {\n            requireFail.push(otherRecognizer);\n            otherRecognizer.requireFailure(this);\n        }\n        return this;\n    },\n\n    /**\n     * drop the requireFailure link. it does not remove the link on the other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    dropRequireFailure: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'dropRequireFailure', this)) {\n            return this;\n        }\n\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        var index = inArray(this.requireFail, otherRecognizer);\n        if (index > -1) {\n            this.requireFail.splice(index, 1);\n        }\n        return this;\n    },\n\n    /**\n     * has require failures boolean\n     * @returns {boolean}\n     */\n    hasRequireFailures: function() {\n        return this.requireFail.length > 0;\n    },\n\n    /**\n     * if the recognizer can recognize simultaneous with an other recognizer\n     * @param {Recognizer} otherRecognizer\n     * @returns {Boolean}\n     */\n    canRecognizeWith: function(otherRecognizer) {\n        return !!this.simultaneous[otherRecognizer.id];\n    },\n\n    /**\n     * You should use `tryEmit` instead of `emit` directly to check\n     * that all the needed recognizers has failed before emitting.\n     * @param {Object} input\n     */\n    emit: function(input) {\n        var self = this;\n        var state = this.state;\n\n        function emit(event) {\n            self.manager.emit(event, input);\n        }\n\n        // 'panstart' and 'panmove'\n        if (state < STATE_ENDED) {\n            emit(self.options.event + stateStr(state));\n        }\n\n        emit(self.options.event); // simple 'eventName' events\n\n        if (input.additionalEvent) { // additional event(panleft, panright, pinchin, pinchout...)\n            emit(input.additionalEvent);\n        }\n\n        // panend and pancancel\n        if (state >= STATE_ENDED) {\n            emit(self.options.event + stateStr(state));\n        }\n    },\n\n    /**\n     * Check that all the require failure recognizers has failed,\n     * if true, it emits a gesture event,\n     * otherwise, setup the state to FAILED.\n     * @param {Object} input\n     */\n    tryEmit: function(input) {\n        if (this.canEmit()) {\n            return this.emit(input);\n        }\n        // it's failing anyway\n        this.state = STATE_FAILED;\n    },\n\n    /**\n     * can we emit?\n     * @returns {boolean}\n     */\n    canEmit: function() {\n        var i = 0;\n        while (i < this.requireFail.length) {\n            if (!(this.requireFail[i].state & (STATE_FAILED | STATE_POSSIBLE))) {\n                return false;\n            }\n            i++;\n        }\n        return true;\n    },\n\n    /**\n     * update the recognizer\n     * @param {Object} inputData\n     */\n    recognize: function(inputData) {\n        // make a new copy of the inputData\n        // so we can change the inputData without messing up the other recognizers\n        var inputDataClone = assign({}, inputData);\n\n        // is is enabled and allow recognizing?\n        if (!boolOrFn(this.options.enable, [this, inputDataClone])) {\n            this.reset();\n            this.state = STATE_FAILED;\n            return;\n        }\n\n        // reset when we've reached the end\n        if (this.state & (STATE_RECOGNIZED | STATE_CANCELLED | STATE_FAILED)) {\n            this.state = STATE_POSSIBLE;\n        }\n\n        this.state = this.process(inputDataClone);\n\n        // the recognizer has recognized a gesture\n        // so trigger an event\n        if (this.state & (STATE_BEGAN | STATE_CHANGED | STATE_ENDED | STATE_CANCELLED)) {\n            this.tryEmit(inputDataClone);\n        }\n    },\n\n    /**\n     * return the state of the recognizer\n     * the actual recognizing happens in this method\n     * @virtual\n     * @param {Object} inputData\n     * @returns {Const} STATE\n     */\n    process: function(inputData) { }, // jshint ignore:line\n\n    /**\n     * return the preferred touch-action\n     * @virtual\n     * @returns {Array}\n     */\n    getTouchAction: function() { },\n\n    /**\n     * called when the gesture isn't allowed to recognize\n     * like when another is being recognized or it is disabled\n     * @virtual\n     */\n    reset: function() { }\n};\n\n/**\n * get a usable string, used as event postfix\n * @param {Const} state\n * @returns {String} state\n */\nfunction stateStr(state) {\n    if (state & STATE_CANCELLED) {\n        return 'cancel';\n    } else if (state & STATE_ENDED) {\n        return 'end';\n    } else if (state & STATE_CHANGED) {\n        return 'move';\n    } else if (state & STATE_BEGAN) {\n        return 'start';\n    }\n    return '';\n}\n\n/**\n * direction cons to string\n * @param {Const} direction\n * @returns {String}\n */\nfunction directionStr(direction) {\n    if (direction == DIRECTION_DOWN) {\n        return 'down';\n    } else if (direction == DIRECTION_UP) {\n        return 'up';\n    } else if (direction == DIRECTION_LEFT) {\n        return 'left';\n    } else if (direction == DIRECTION_RIGHT) {\n        return 'right';\n    }\n    return '';\n}\n\n/**\n * get a recognizer by name if it is bound to a manager\n * @param {Recognizer|String} otherRecognizer\n * @param {Recognizer} recognizer\n * @returns {Recognizer}\n */\nfunction getRecognizerByNameIfManager(otherRecognizer, recognizer) {\n    var manager = recognizer.manager;\n    if (manager) {\n        return manager.get(otherRecognizer);\n    }\n    return otherRecognizer;\n}\n\n/**\n * This recognizer is just used as a base for the simple attribute recognizers.\n * @constructor\n * @extends Recognizer\n */\nfunction AttrRecognizer() {\n    Recognizer.apply(this, arguments);\n}\n\ninherit(AttrRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof AttrRecognizer\n     */\n    defaults: {\n        /**\n         * @type {Number}\n         * @default 1\n         */\n        pointers: 1\n    },\n\n    /**\n     * Used to check if it the recognizer receives valid input, like input.distance > 10.\n     * @memberof AttrRecognizer\n     * @param {Object} input\n     * @returns {Boolean} recognized\n     */\n    attrTest: function(input) {\n        var optionPointers = this.options.pointers;\n        return optionPointers === 0 || input.pointers.length === optionPointers;\n    },\n\n    /**\n     * Process the input and return the state for the recognizer\n     * @memberof AttrRecognizer\n     * @param {Object} input\n     * @returns {*} State\n     */\n    process: function(input) {\n        var state = this.state;\n        var eventType = input.eventType;\n\n        var isRecognized = state & (STATE_BEGAN | STATE_CHANGED);\n        var isValid = this.attrTest(input);\n\n        // on cancel input and we've recognized before, return STATE_CANCELLED\n        if (isRecognized && (eventType & INPUT_CANCEL || !isValid)) {\n            return state | STATE_CANCELLED;\n        } else if (isRecognized || isValid) {\n            if (eventType & INPUT_END) {\n                return state | STATE_ENDED;\n            } else if (!(state & STATE_BEGAN)) {\n                return STATE_BEGAN;\n            }\n            return state | STATE_CHANGED;\n        }\n        return STATE_FAILED;\n    }\n});\n\n/**\n * Pan\n * Recognized when the pointer is down and moved in the allowed direction.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction PanRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n\n    this.pX = null;\n    this.pY = null;\n}\n\ninherit(PanRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof PanRecognizer\n     */\n    defaults: {\n        event: 'pan',\n        threshold: 10,\n        pointers: 1,\n        direction: DIRECTION_ALL\n    },\n\n    getTouchAction: function() {\n        var direction = this.options.direction;\n        var actions = [];\n        if (direction & DIRECTION_HORIZONTAL) {\n            actions.push(TOUCH_ACTION_PAN_Y);\n        }\n        if (direction & DIRECTION_VERTICAL) {\n            actions.push(TOUCH_ACTION_PAN_X);\n        }\n        return actions;\n    },\n\n    directionTest: function(input) {\n        var options = this.options;\n        var hasMoved = true;\n        var distance = input.distance;\n        var direction = input.direction;\n        var x = input.deltaX;\n        var y = input.deltaY;\n\n        // lock to axis?\n        if (!(direction & options.direction)) {\n            if (options.direction & DIRECTION_HORIZONTAL) {\n                direction = (x === 0) ? DIRECTION_NONE : (x < 0) ? DIRECTION_LEFT : DIRECTION_RIGHT;\n                hasMoved = x != this.pX;\n                distance = Math.abs(input.deltaX);\n            } else {\n                direction = (y === 0) ? DIRECTION_NONE : (y < 0) ? DIRECTION_UP : DIRECTION_DOWN;\n                hasMoved = y != this.pY;\n                distance = Math.abs(input.deltaY);\n            }\n        }\n        input.direction = direction;\n        return hasMoved && distance > options.threshold && direction & options.direction;\n    },\n\n    attrTest: function(input) {\n        return AttrRecognizer.prototype.attrTest.call(this, input) &&\n            (this.state & STATE_BEGAN || (!(this.state & STATE_BEGAN) && this.directionTest(input)));\n    },\n\n    emit: function(input) {\n\n        this.pX = input.deltaX;\n        this.pY = input.deltaY;\n\n        var direction = directionStr(input.direction);\n\n        if (direction) {\n            input.additionalEvent = this.options.event + direction;\n        }\n        this._super.emit.call(this, input);\n    }\n});\n\n/**\n * Pinch\n * Recognized when two or more pointers are moving toward (zoom-in) or away from each other (zoom-out).\n * @constructor\n * @extends AttrRecognizer\n */\nfunction PinchRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(PinchRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof PinchRecognizer\n     */\n    defaults: {\n        event: 'pinch',\n        threshold: 0,\n        pointers: 2\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_NONE];\n    },\n\n    attrTest: function(input) {\n        return this._super.attrTest.call(this, input) &&\n            (Math.abs(input.scale - 1) > this.options.threshold || this.state & STATE_BEGAN);\n    },\n\n    emit: function(input) {\n        if (input.scale !== 1) {\n            var inOut = input.scale < 1 ? 'in' : 'out';\n            input.additionalEvent = this.options.event + inOut;\n        }\n        this._super.emit.call(this, input);\n    }\n});\n\n/**\n * Press\n * Recognized when the pointer is down for x ms without any movement.\n * @constructor\n * @extends Recognizer\n */\nfunction PressRecognizer() {\n    Recognizer.apply(this, arguments);\n\n    this._timer = null;\n    this._input = null;\n}\n\ninherit(PressRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof PressRecognizer\n     */\n    defaults: {\n        event: 'press',\n        pointers: 1,\n        time: 251, // minimal time of the pointer to be pressed\n        threshold: 9 // a minimal movement is ok, but keep it low\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_AUTO];\n    },\n\n    process: function(input) {\n        var options = this.options;\n        var validPointers = input.pointers.length === options.pointers;\n        var validMovement = input.distance < options.threshold;\n        var validTime = input.deltaTime > options.time;\n\n        this._input = input;\n\n        // we only allow little movement\n        // and we've reached an end event, so a tap is possible\n        if (!validMovement || !validPointers || (input.eventType & (INPUT_END | INPUT_CANCEL) && !validTime)) {\n            this.reset();\n        } else if (input.eventType & INPUT_START) {\n            this.reset();\n            this._timer = setTimeoutContext(function() {\n                this.state = STATE_RECOGNIZED;\n                this.tryEmit();\n            }, options.time, this);\n        } else if (input.eventType & INPUT_END) {\n            return STATE_RECOGNIZED;\n        }\n        return STATE_FAILED;\n    },\n\n    reset: function() {\n        clearTimeout(this._timer);\n    },\n\n    emit: function(input) {\n        if (this.state !== STATE_RECOGNIZED) {\n            return;\n        }\n\n        if (input && (input.eventType & INPUT_END)) {\n            this.manager.emit(this.options.event + 'up', input);\n        } else {\n            this._input.timeStamp = now();\n            this.manager.emit(this.options.event, this._input);\n        }\n    }\n});\n\n/**\n * Rotate\n * Recognized when two or more pointer are moving in a circular motion.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction RotateRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(RotateRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof RotateRecognizer\n     */\n    defaults: {\n        event: 'rotate',\n        threshold: 0,\n        pointers: 2\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_NONE];\n    },\n\n    attrTest: function(input) {\n        return this._super.attrTest.call(this, input) &&\n            (Math.abs(input.rotation) > this.options.threshold || this.state & STATE_BEGAN);\n    }\n});\n\n/**\n * Swipe\n * Recognized when the pointer is moving fast (velocity), with enough distance in the allowed direction.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction SwipeRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(SwipeRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof SwipeRecognizer\n     */\n    defaults: {\n        event: 'swipe',\n        threshold: 10,\n        velocity: 0.3,\n        direction: DIRECTION_HORIZONTAL | DIRECTION_VERTICAL,\n        pointers: 1\n    },\n\n    getTouchAction: function() {\n        return PanRecognizer.prototype.getTouchAction.call(this);\n    },\n\n    attrTest: function(input) {\n        var direction = this.options.direction;\n        var velocity;\n\n        if (direction & (DIRECTION_HORIZONTAL | DIRECTION_VERTICAL)) {\n            velocity = input.overallVelocity;\n        } else if (direction & DIRECTION_HORIZONTAL) {\n            velocity = input.overallVelocityX;\n        } else if (direction & DIRECTION_VERTICAL) {\n            velocity = input.overallVelocityY;\n        }\n\n        return this._super.attrTest.call(this, input) &&\n            direction & input.offsetDirection &&\n            input.distance > this.options.threshold &&\n            input.maxPointers == this.options.pointers &&\n            abs(velocity) > this.options.velocity && input.eventType & INPUT_END;\n    },\n\n    emit: function(input) {\n        var direction = directionStr(input.offsetDirection);\n        if (direction) {\n            this.manager.emit(this.options.event + direction, input);\n        }\n\n        this.manager.emit(this.options.event, input);\n    }\n});\n\n/**\n * A tap is ecognized when the pointer is doing a small tap/click. Multiple taps are recognized if they occur\n * between the given interval and position. The delay option can be used to recognize multi-taps without firing\n * a single tap.\n *\n * The eventData from the emitted event contains the property `tapCount`, which contains the amount of\n * multi-taps being recognized.\n * @constructor\n * @extends Recognizer\n */\nfunction TapRecognizer() {\n    Recognizer.apply(this, arguments);\n\n    // previous time and center,\n    // used for tap counting\n    this.pTime = false;\n    this.pCenter = false;\n\n    this._timer = null;\n    this._input = null;\n    this.count = 0;\n}\n\ninherit(TapRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof PinchRecognizer\n     */\n    defaults: {\n        event: 'tap',\n        pointers: 1,\n        taps: 1,\n        interval: 300, // max time between the multi-tap taps\n        time: 250, // max time of the pointer to be down (like finger on the screen)\n        threshold: 9, // a minimal movement is ok, but keep it low\n        posThreshold: 10 // a multi-tap can be a bit off the initial position\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_MANIPULATION];\n    },\n\n    process: function(input) {\n        var options = this.options;\n\n        var validPointers = input.pointers.length === options.pointers;\n        var validMovement = input.distance < options.threshold;\n        var validTouchTime = input.deltaTime < options.time;\n\n        this.reset();\n\n        if ((input.eventType & INPUT_START) && (this.count === 0)) {\n            return this.failTimeout();\n        }\n\n        // we only allow little movement\n        // and we've reached an end event, so a tap is possible\n        if (validMovement && validTouchTime && validPointers) {\n            if (input.eventType != INPUT_END) {\n                return this.failTimeout();\n            }\n\n            var validInterval = this.pTime ? (input.timeStamp - this.pTime < options.interval) : true;\n            var validMultiTap = !this.pCenter || getDistance(this.pCenter, input.center) < options.posThreshold;\n\n            this.pTime = input.timeStamp;\n            this.pCenter = input.center;\n\n            if (!validMultiTap || !validInterval) {\n                this.count = 1;\n            } else {\n                this.count += 1;\n            }\n\n            this._input = input;\n\n            // if tap count matches we have recognized it,\n            // else it has began recognizing...\n            var tapCount = this.count % options.taps;\n            if (tapCount === 0) {\n                // no failing requirements, immediately trigger the tap event\n                // or wait as long as the multitap interval to trigger\n                if (!this.hasRequireFailures()) {\n                    return STATE_RECOGNIZED;\n                } else {\n                    this._timer = setTimeoutContext(function() {\n                        this.state = STATE_RECOGNIZED;\n                        this.tryEmit();\n                    }, options.interval, this);\n                    return STATE_BEGAN;\n                }\n            }\n        }\n        return STATE_FAILED;\n    },\n\n    failTimeout: function() {\n        this._timer = setTimeoutContext(function() {\n            this.state = STATE_FAILED;\n        }, this.options.interval, this);\n        return STATE_FAILED;\n    },\n\n    reset: function() {\n        clearTimeout(this._timer);\n    },\n\n    emit: function() {\n        if (this.state == STATE_RECOGNIZED) {\n            this._input.tapCount = this.count;\n            this.manager.emit(this.options.event, this._input);\n        }\n    }\n});\n\n/**\n * Simple way to create a manager with a default set of recognizers.\n * @param {HTMLElement} element\n * @param {Object} [options]\n * @constructor\n */\nfunction Hammer(element, options) {\n    options = options || {};\n    options.recognizers = ifUndefined(options.recognizers, Hammer.defaults.preset);\n    return new Manager(element, options);\n}\n\n/**\n * @const {string}\n */\nHammer.VERSION = '2.0.7';\n\n/**\n * default settings\n * @namespace\n */\nHammer.defaults = {\n    /**\n     * set if DOM events are being triggered.\n     * But this is slower and unused by simple implementations, so disabled by default.\n     * @type {Boolean}\n     * @default false\n     */\n    domEvents: false,\n\n    /**\n     * The value for the touchAction property/fallback.\n     * When set to `compute` it will magically set the correct value based on the added recognizers.\n     * @type {String}\n     * @default compute\n     */\n    touchAction: TOUCH_ACTION_COMPUTE,\n\n    /**\n     * @type {Boolean}\n     * @default true\n     */\n    enable: true,\n\n    /**\n     * EXPERIMENTAL FEATURE -- can be removed/changed\n     * Change the parent input target element.\n     * If Null, then it is being set the to main element.\n     * @type {Null|EventTarget}\n     * @default null\n     */\n    inputTarget: null,\n\n    /**\n     * force an input class\n     * @type {Null|Function}\n     * @default null\n     */\n    inputClass: null,\n\n    /**\n     * Default recognizer setup when calling `Hammer()`\n     * When creating a new Manager these will be skipped.\n     * @type {Array}\n     */\n    preset: [\n        // RecognizerClass, options, [recognizeWith, ...], [requireFailure, ...]\n        [RotateRecognizer, {enable: false}],\n        [PinchRecognizer, {enable: false}, ['rotate']],\n        [SwipeRecognizer, {direction: DIRECTION_HORIZONTAL}],\n        [PanRecognizer, {direction: DIRECTION_HORIZONTAL}, ['swipe']],\n        [TapRecognizer],\n        [TapRecognizer, {event: 'doubletap', taps: 2}, ['tap']],\n        [PressRecognizer]\n    ],\n\n    /**\n     * Some CSS properties can be used to improve the working of Hammer.\n     * Add them to this method and they will be set when creating a new Manager.\n     * @namespace\n     */\n    cssProps: {\n        /**\n         * Disables text selection to improve the dragging gesture. Mainly for desktop browsers.\n         * @type {String}\n         * @default 'none'\n         */\n        userSelect: 'none',\n\n        /**\n         * Disable the Windows Phone grippers when pressing an element.\n         * @type {String}\n         * @default 'none'\n         */\n        touchSelect: 'none',\n\n        /**\n         * Disables the default callout shown when you touch and hold a touch target.\n         * On iOS, when you touch and hold a touch target such as a link, Safari displays\n         * a callout containing information about the link. This property allows you to disable that callout.\n         * @type {String}\n         * @default 'none'\n         */\n        touchCallout: 'none',\n\n        /**\n         * Specifies whether zooming is enabled. Used by IE10>\n         * @type {String}\n         * @default 'none'\n         */\n        contentZooming: 'none',\n\n        /**\n         * Specifies that an entire element should be draggable instead of its contents. Mainly for desktop browsers.\n         * @type {String}\n         * @default 'none'\n         */\n        userDrag: 'none',\n\n        /**\n         * Overrides the highlight color shown when the user taps a link or a JavaScript\n         * clickable element in iOS. This property obeys the alpha value, if specified.\n         * @type {String}\n         * @default 'rgba(0,0,0,0)'\n         */\n        tapHighlightColor: 'rgba(0,0,0,0)'\n    }\n};\n\nvar STOP = 1;\nvar FORCED_STOP = 2;\n\n/**\n * Manager\n * @param {HTMLElement} element\n * @param {Object} [options]\n * @constructor\n */\nfunction Manager(element, options) {\n    this.options = assign({}, Hammer.defaults, options || {});\n\n    this.options.inputTarget = this.options.inputTarget || element;\n\n    this.handlers = {};\n    this.session = {};\n    this.recognizers = [];\n    this.oldCssProps = {};\n\n    this.element = element;\n    this.input = createInputInstance(this);\n    this.touchAction = new TouchAction(this, this.options.touchAction);\n\n    toggleCssProps(this, true);\n\n    each(this.options.recognizers, function(item) {\n        var recognizer = this.add(new (item[0])(item[1]));\n        item[2] && recognizer.recognizeWith(item[2]);\n        item[3] && recognizer.requireFailure(item[3]);\n    }, this);\n}\n\nManager.prototype = {\n    /**\n     * set options\n     * @param {Object} options\n     * @returns {Manager}\n     */\n    set: function(options) {\n        assign(this.options, options);\n\n        // Options that need a little more setup\n        if (options.touchAction) {\n            this.touchAction.update();\n        }\n        if (options.inputTarget) {\n            // Clean up existing event listeners and reinitialize\n            this.input.destroy();\n            this.input.target = options.inputTarget;\n            this.input.init();\n        }\n        return this;\n    },\n\n    /**\n     * stop recognizing for this session.\n     * This session will be discarded, when a new [input]start event is fired.\n     * When forced, the recognizer cycle is stopped immediately.\n     * @param {Boolean} [force]\n     */\n    stop: function(force) {\n        this.session.stopped = force ? FORCED_STOP : STOP;\n    },\n\n    /**\n     * run the recognizers!\n     * called by the inputHandler function on every movement of the pointers (touches)\n     * it walks through all the recognizers and tries to detect the gesture that is being made\n     * @param {Object} inputData\n     */\n    recognize: function(inputData) {\n        var session = this.session;\n        if (session.stopped) {\n            return;\n        }\n\n        // run the touch-action polyfill\n        this.touchAction.preventDefaults(inputData);\n\n        var recognizer;\n        var recognizers = this.recognizers;\n\n        // this holds the recognizer that is being recognized.\n        // so the recognizer's state needs to be BEGAN, CHANGED, ENDED or RECOGNIZED\n        // if no recognizer is detecting a thing, it is set to `null`\n        var curRecognizer = session.curRecognizer;\n\n        // reset when the last recognizer is recognized\n        // or when we're in a new session\n        if (!curRecognizer || (curRecognizer && curRecognizer.state & STATE_RECOGNIZED)) {\n            curRecognizer = session.curRecognizer = null;\n        }\n\n        var i = 0;\n        while (i < recognizers.length) {\n            recognizer = recognizers[i];\n\n            // find out if we are allowed try to recognize the input for this one.\n            // 1.   allow if the session is NOT forced stopped (see the .stop() method)\n            // 2.   allow if we still haven't recognized a gesture in this session, or the this recognizer is the one\n            //      that is being recognized.\n            // 3.   allow if the recognizer is allowed to run simultaneous with the current recognized recognizer.\n            //      this can be setup with the `recognizeWith()` method on the recognizer.\n            if (session.stopped !== FORCED_STOP && ( // 1\n                    !curRecognizer || recognizer == curRecognizer || // 2\n                    recognizer.canRecognizeWith(curRecognizer))) { // 3\n                recognizer.recognize(inputData);\n            } else {\n                recognizer.reset();\n            }\n\n            // if the recognizer has been recognizing the input as a valid gesture, we want to store this one as the\n            // current active recognizer. but only if we don't already have an active recognizer\n            if (!curRecognizer && recognizer.state & (STATE_BEGAN | STATE_CHANGED | STATE_ENDED)) {\n                curRecognizer = session.curRecognizer = recognizer;\n            }\n            i++;\n        }\n    },\n\n    /**\n     * get a recognizer by its event name.\n     * @param {Recognizer|String} recognizer\n     * @returns {Recognizer|Null}\n     */\n    get: function(recognizer) {\n        if (recognizer instanceof Recognizer) {\n            return recognizer;\n        }\n\n        var recognizers = this.recognizers;\n        for (var i = 0; i < recognizers.length; i++) {\n            if (recognizers[i].options.event == recognizer) {\n                return recognizers[i];\n            }\n        }\n        return null;\n    },\n\n    /**\n     * add a recognizer to the manager\n     * existing recognizers with the same event name will be removed\n     * @param {Recognizer} recognizer\n     * @returns {Recognizer|Manager}\n     */\n    add: function(recognizer) {\n        if (invokeArrayArg(recognizer, 'add', this)) {\n            return this;\n        }\n\n        // remove existing\n        var existing = this.get(recognizer.options.event);\n        if (existing) {\n            this.remove(existing);\n        }\n\n        this.recognizers.push(recognizer);\n        recognizer.manager = this;\n\n        this.touchAction.update();\n        return recognizer;\n    },\n\n    /**\n     * remove a recognizer by name or instance\n     * @param {Recognizer|String} recognizer\n     * @returns {Manager}\n     */\n    remove: function(recognizer) {\n        if (invokeArrayArg(recognizer, 'remove', this)) {\n            return this;\n        }\n\n        recognizer = this.get(recognizer);\n\n        // let's make sure this recognizer exists\n        if (recognizer) {\n            var recognizers = this.recognizers;\n            var index = inArray(recognizers, recognizer);\n\n            if (index !== -1) {\n                recognizers.splice(index, 1);\n                this.touchAction.update();\n            }\n        }\n\n        return this;\n    },\n\n    /**\n     * bind event\n     * @param {String} events\n     * @param {Function} handler\n     * @returns {EventEmitter} this\n     */\n    on: function(events, handler) {\n        if (events === undefined) {\n            return;\n        }\n        if (handler === undefined) {\n            return;\n        }\n\n        var handlers = this.handlers;\n        each(splitStr(events), function(event) {\n            handlers[event] = handlers[event] || [];\n            handlers[event].push(handler);\n        });\n        return this;\n    },\n\n    /**\n     * unbind event, leave emit blank to remove all handlers\n     * @param {String} events\n     * @param {Function} [handler]\n     * @returns {EventEmitter} this\n     */\n    off: function(events, handler) {\n        if (events === undefined) {\n            return;\n        }\n\n        var handlers = this.handlers;\n        each(splitStr(events), function(event) {\n            if (!handler) {\n                delete handlers[event];\n            } else {\n                handlers[event] && handlers[event].splice(inArray(handlers[event], handler), 1);\n            }\n        });\n        return this;\n    },\n\n    /**\n     * emit event to the listeners\n     * @param {String} event\n     * @param {Object} data\n     */\n    emit: function(event, data) {\n        // we also want to trigger dom events\n        if (this.options.domEvents) {\n            triggerDomEvent(event, data);\n        }\n\n        // no handlers, so skip it all\n        var handlers = this.handlers[event] && this.handlers[event].slice();\n        if (!handlers || !handlers.length) {\n            return;\n        }\n\n        data.type = event;\n        data.preventDefault = function() {\n            data.srcEvent.preventDefault();\n        };\n\n        var i = 0;\n        while (i < handlers.length) {\n            handlers[i](data);\n            i++;\n        }\n    },\n\n    /**\n     * destroy the manager and unbinds all events\n     * it doesn't unbind dom events, that is the user own responsibility\n     */\n    destroy: function() {\n        this.element && toggleCssProps(this, false);\n\n        this.handlers = {};\n        this.session = {};\n        this.input.destroy();\n        this.element = null;\n    }\n};\n\n/**\n * add/remove the css properties as defined in manager.options.cssProps\n * @param {Manager} manager\n * @param {Boolean} add\n */\nfunction toggleCssProps(manager, add) {\n    var element = manager.element;\n    if (!element.style) {\n        return;\n    }\n    var prop;\n    each(manager.options.cssProps, function(value, name) {\n        prop = prefixed(element.style, name);\n        if (add) {\n            manager.oldCssProps[prop] = element.style[prop];\n            element.style[prop] = value;\n        } else {\n            element.style[prop] = manager.oldCssProps[prop] || '';\n        }\n    });\n    if (!add) {\n        manager.oldCssProps = {};\n    }\n}\n\n/**\n * trigger dom event\n * @param {String} event\n * @param {Object} data\n */\nfunction triggerDomEvent(event, data) {\n    var gestureEvent = document.createEvent('Event');\n    gestureEvent.initEvent(event, true, true);\n    gestureEvent.gesture = data;\n    data.target.dispatchEvent(gestureEvent);\n}\n\nassign(Hammer, {\n    INPUT_START: INPUT_START,\n    INPUT_MOVE: INPUT_MOVE,\n    INPUT_END: INPUT_END,\n    INPUT_CANCEL: INPUT_CANCEL,\n\n    STATE_POSSIBLE: STATE_POSSIBLE,\n    STATE_BEGAN: STATE_BEGAN,\n    STATE_CHANGED: STATE_CHANGED,\n    STATE_ENDED: STATE_ENDED,\n    STATE_RECOGNIZED: STATE_RECOGNIZED,\n    STATE_CANCELLED: STATE_CANCELLED,\n    STATE_FAILED: STATE_FAILED,\n\n    DIRECTION_NONE: DIRECTION_NONE,\n    DIRECTION_LEFT: DIRECTION_LEFT,\n    DIRECTION_RIGHT: DIRECTION_RIGHT,\n    DIRECTION_UP: DIRECTION_UP,\n    DIRECTION_DOWN: DIRECTION_DOWN,\n    DIRECTION_HORIZONTAL: DIRECTION_HORIZONTAL,\n    DIRECTION_VERTICAL: DIRECTION_VERTICAL,\n    DIRECTION_ALL: DIRECTION_ALL,\n\n    Manager: Manager,\n    Input: Input,\n    TouchAction: TouchAction,\n\n    TouchInput: TouchInput,\n    MouseInput: MouseInput,\n    PointerEventInput: PointerEventInput,\n    TouchMouseInput: TouchMouseInput,\n    SingleTouchInput: SingleTouchInput,\n\n    Recognizer: Recognizer,\n    AttrRecognizer: AttrRecognizer,\n    Tap: TapRecognizer,\n    Pan: PanRecognizer,\n    Swipe: SwipeRecognizer,\n    Pinch: PinchRecognizer,\n    Rotate: RotateRecognizer,\n    Press: PressRecognizer,\n\n    on: addEventListeners,\n    off: removeEventListeners,\n    each: each,\n    merge: merge,\n    extend: extend,\n    assign: assign,\n    inherit: inherit,\n    bindFn: bindFn,\n    prefixed: prefixed\n});\n\n// this prevents errors when Hammer is loaded in the presence of an AMD\n//  style loader but by script tag, not by the loader.\nvar freeGlobal = (typeof window !== 'undefined' ? window : (typeof self !== 'undefined' ? self : {})); // jshint ignore:line\nfreeGlobal.Hammer = Hammer;\n\nif (typeof define === 'function' && define.amd) {\n    define(function() {\n        return Hammer;\n    });\n} else if (typeof module != 'undefined' && module.exports) {\n    module.exports = Hammer;\n} else {\n    window[exportName] = Hammer;\n}\n\n})(window, document, 'Hammer');\n",
         "'use strict';\n\nvar reactIs = require('react-is');\n\n/**\n * Copyright 2015, Yahoo! Inc.\n * Copyrights licensed under the New BSD License. See the accompanying LICENSE file for terms.\n */\nvar REACT_STATICS = {\n  childContextTypes: true,\n  contextType: true,\n  contextTypes: true,\n  defaultProps: true,\n  displayName: true,\n  getDefaultProps: true,\n  getDerivedStateFromError: true,\n  getDerivedStateFromProps: true,\n  mixins: true,\n  propTypes: true,\n  type: true\n};\nvar KNOWN_STATICS = {\n  name: true,\n  length: true,\n  prototype: true,\n  caller: true,\n  callee: true,\n  arguments: true,\n  arity: true\n};\nvar FORWARD_REF_STATICS = {\n  '$$typeof': true,\n  render: true,\n  defaultProps: true,\n  displayName: true,\n  propTypes: true\n};\nvar MEMO_STATICS = {\n  '$$typeof': true,\n  compare: true,\n  defaultProps: true,\n  displayName: true,\n  propTypes: true,\n  type: true\n};\nvar TYPE_STATICS = {};\nTYPE_STATICS[reactIs.ForwardRef] = FORWARD_REF_STATICS;\nTYPE_STATICS[reactIs.Memo] = MEMO_STATICS;\n\nfunction getStatics(component) {\n  // React v16.11 and below\n  if (reactIs.isMemo(component)) {\n    return MEMO_STATICS;\n  } // React v16.12 and above\n\n\n  return TYPE_STATICS[component['$$typeof']] || REACT_STATICS;\n}\n\nvar defineProperty = Object.defineProperty;\nvar getOwnPropertyNames = Object.getOwnPropertyNames;\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar getOwnPropertyDescriptor = Object.getOwnPropertyDescriptor;\nvar getPrototypeOf = Object.getPrototypeOf;\nvar objectPrototype = Object.prototype;\nfunction hoistNonReactStatics(targetComponent, sourceComponent, blacklist) {\n  if (typeof sourceComponent !== 'string') {\n    // don't hoist over string (html) components\n    if (objectPrototype) {\n      var inheritedComponent = getPrototypeOf(sourceComponent);\n\n      if (inheritedComponent && inheritedComponent !== objectPrototype) {\n        hoistNonReactStatics(targetComponent, inheritedComponent, blacklist);\n      }\n    }\n\n    var keys = getOwnPropertyNames(sourceComponent);\n\n    if (getOwnPropertySymbols) {\n      keys = keys.concat(getOwnPropertySymbols(sourceComponent));\n    }\n\n    var targetStatics = getStatics(targetComponent);\n    var sourceStatics = getStatics(sourceComponent);\n\n    for (var i = 0; i < keys.length; ++i) {\n      var key = keys[i];\n\n      if (!KNOWN_STATICS[key] && !(blacklist && blacklist[key]) && !(sourceStatics && sourceStatics[key]) && !(targetStatics && targetStatics[key])) {\n        var descriptor = getOwnPropertyDescriptor(sourceComponent, key);\n\n        try {\n          // Avoid failures from read-only properties\n          defineProperty(targetComponent, key, descriptor);\n        } catch (e) {}\n      }\n    }\n  }\n\n  return targetComponent;\n}\n\nmodule.exports = hoistNonReactStatics;\n",
+        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.millify = void 0;\nconst options_1 = require(\"./options\");\nconst utils_1 = require(\"./utils\");\n// Most commonly used digit grouping base.\nconst DIGIT_GROUPING_BASE = 1000;\n/**\n * Generator that divides a number until a decimal value is found.\n *\n * The denominator is defined by the numerical digit grouping base,\n * or interval. The most commonly-used digit group interval is 1000.\n *\n * e.g. 1,000,000 is grouped in multiples of 1000.\n */\nfunction* divider(value) {\n    // Create a mutable copy of the base.\n    let denominator = DIGIT_GROUPING_BASE;\n    while (true) {\n        const result = value / denominator;\n        if (result < 1) {\n            // End of operation. We can't divide the value any further.\n            return;\n        }\n        yield result;\n        // The denominator is increased every iteration by multiplying\n        // the base by itself, until a decimal value remains.\n        denominator *= DIGIT_GROUPING_BASE;\n    }\n}\n/**\n * millify converts long numbers to human-readable strings.\n */\nfunction millify(value, options) {\n    var _a, _b;\n    // Override default options with options supplied by user.\n    const opts = options\n        ? { ...options_1.defaultOptions, ...options }\n        : options_1.defaultOptions;\n    if (!Array.isArray(opts.units) || !opts.units.length) {\n        throw new Error(\"Option `units` must be a non-empty array\");\n    }\n    // If the input value is invalid, then return the value in string form.\n    // Originally this threw an error, but was changed to return a graceful fallback.\n    let val;\n    try {\n        val = utils_1.parseValue(value);\n    }\n    catch (e) {\n        if (e instanceof Error) {\n            console.warn(`WARN: ${e.message} (millify)`);\n        }\n        // Invalid values will be converted to string as per `String()`.\n        return String(value);\n    }\n    // Add a minus sign (-) prefix if it's a negative number.\n    const prefix = val < 0 ? \"-\" : \"\";\n    // Work only with positive values for simplicity's sake.\n    val = Math.abs(val);\n    // Keep dividing the input value by the digit grouping base\n    // until the decimal and the unit index is deciphered.\n    let unitIndex = 0;\n    for (const result of divider(val)) {\n        val = result;\n        unitIndex += 1;\n    }\n    // Return the original number if the number is too large to have\n    // a corresponding unit. Returning anything else is ambiguous.\n    const unitIndexOutOfRange = unitIndex >= opts.units.length;\n    if (unitIndexOutOfRange) {\n        // At this point we don't know what to do with the input value,\n        // so we return it as is, without localizing the string.\n        return value.toString();\n    }\n    // Round decimal up to desired precision.\n    let rounded = utils_1.roundTo(val, opts.precision);\n    // Fixes an edge case bug that outputs certain numbers as 1000K instead of 1M.\n    // The rounded value needs another iteration in the divider cycle.\n    for (const result of divider(rounded)) {\n        rounded = result;\n        unitIndex += 1;\n    }\n    // Calculate the unit suffix and make it lowercase (if needed).\n    const unit = (_a = opts.units[unitIndex]) !== null && _a !== void 0 ? _a : \"\";\n    const suffix = opts.lowercase ? unit.toLowerCase() : unit;\n    // Add a space between number and abbreviation.\n    const space = opts.space ? \" \" : \"\";\n    // Format the number according to the desired locale.\n    const formatted = rounded.toLocaleString((_b = opts.locales) !== null && _b !== void 0 ? _b : utils_1.getLocales(), {\n        // toLocaleString needs the explicit fraction digits.\n        minimumFractionDigits: utils_1.getFractionDigits(rounded),\n    });\n    return `${prefix}${formatted}${space}${suffix}`;\n}\nexports.millify = millify;\nexports.default = millify;\n",
+        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.defaultOptions = void 0;\n/**\n * Default options for Millify.\n */\nexports.defaultOptions = {\n    lowercase: false,\n    precision: 1,\n    space: false,\n    units: [\n        \"\",\n        \"K\",\n        \"M\",\n        \"B\",\n        \"T\",\n        \"P\",\n        \"E\", // Quintillion\n    ],\n};\n",
+        "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.getLocales = exports.getFractionDigits = exports.roundTo = exports.parseValue = void 0;\n/**\n * parseValue ensures the value is a number and within accepted range.\n */\nfunction parseValue(value) {\n    const val = parseFloat(value === null || value === void 0 ? void 0 : value.toString());\n    if (isNaN(val)) {\n        throw new Error(`Input value is not a number`);\n    }\n    if (val > Number.MAX_SAFE_INTEGER || val < Number.MIN_SAFE_INTEGER) {\n        throw new RangeError(\"Input value is outside of safe integer range\");\n    }\n    return val;\n}\nexports.parseValue = parseValue;\n/**\n * Rounds a number [value] up to a specified [precision].\n */\nfunction roundTo(value, precision) {\n    if (!Number.isFinite(value)) {\n        throw new Error(\"Input value is not a finite number\");\n    }\n    if (!Number.isInteger(precision) || precision < 0) {\n        throw new Error(\"Precision is not a positive integer\");\n    }\n    if (Number.isInteger(value)) {\n        return value;\n    }\n    return parseFloat(value.toFixed(precision));\n}\nexports.roundTo = roundTo;\n/**\n * Returns the number of digits after the decimal.\n */\nfunction getFractionDigits(num) {\n    var _a;\n    if (Number.isInteger(num)) {\n        return 0;\n    }\n    const decimalPart = num.toString().split(\".\")[1];\n    return (_a = decimalPart === null || decimalPart === void 0 ? void 0 : decimalPart.length) !== null && _a !== void 0 ? _a : 0;\n}\nexports.getFractionDigits = getFractionDigits;\n/**\n * Returns the default browser locales.\n */\nfunction getLocales() {\n    var _a;\n    if (typeof navigator === \"undefined\") {\n        return [];\n    }\n    return Array.from((_a = navigator.languages) !== null && _a !== void 0 ? _a : []);\n}\nexports.getLocales = getLocales;\n",
         "/*\nobject-assign\n(c) Sindre Sorhus\n@license MIT\n*/\n\n'use strict';\n/* eslint-disable no-unused-vars */\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar hasOwnProperty = Object.prototype.hasOwnProperty;\nvar propIsEnumerable = Object.prototype.propertyIsEnumerable;\n\nfunction toObject(val) {\n\tif (val === null || val === undefined) {\n\t\tthrow new TypeError('Object.assign cannot be called with null or undefined');\n\t}\n\n\treturn Object(val);\n}\n\nfunction shouldUseNative() {\n\ttry {\n\t\tif (!Object.assign) {\n\t\t\treturn false;\n\t\t}\n\n\t\t// Detect buggy property enumeration order in older V8 versions.\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=4118\n\t\tvar test1 = new String('abc');  // eslint-disable-line no-new-wrappers\n\t\ttest1[5] = 'de';\n\t\tif (Object.getOwnPropertyNames(test1)[0] === '5') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test2 = {};\n\t\tfor (var i = 0; i < 10; i++) {\n\t\t\ttest2['_' + String.fromCharCode(i)] = i;\n\t\t}\n\t\tvar order2 = Object.getOwnPropertyNames(test2).map(function (n) {\n\t\t\treturn test2[n];\n\t\t});\n\t\tif (order2.join('') !== '0123456789') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test3 = {};\n\t\t'abcdefghijklmnopqrst'.split('').forEach(function (letter) {\n\t\t\ttest3[letter] = letter;\n\t\t});\n\t\tif (Object.keys(Object.assign({}, test3)).join('') !==\n\t\t\t\t'abcdefghijklmnopqrst') {\n\t\t\treturn false;\n\t\t}\n\n\t\treturn true;\n\t} catch (err) {\n\t\t// We don't expect any of the above to throw, but better to be safe.\n\t\treturn false;\n\t}\n}\n\nmodule.exports = shouldUseNative() ? Object.assign : function (target, source) {\n\tvar from;\n\tvar to = toObject(target);\n\tvar symbols;\n\n\tfor (var s = 1; s < arguments.length; s++) {\n\t\tfrom = Object(arguments[s]);\n\n\t\tfor (var key in from) {\n\t\t\tif (hasOwnProperty.call(from, key)) {\n\t\t\t\tto[key] = from[key];\n\t\t\t}\n\t\t}\n\n\t\tif (getOwnPropertySymbols) {\n\t\t\tsymbols = getOwnPropertySymbols(from);\n\t\t\tfor (var i = 0; i < symbols.length; i++) {\n\t\t\t\tif (propIsEnumerable.call(from, symbols[i])) {\n\t\t\t\t\tto[symbols[i]] = from[symbols[i]];\n\t\t\t\t}\n\t\t\t}\n\t\t}\n\t}\n\n\treturn to;\n};\n",
         "/** @license React v16.14.0\n * react-dom.production.min.js\n *\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n\n/*\n Modernizr 3.0.0pre (Custom Build) | MIT\n*/\n'use strict';var aa=require(\"react\"),n=require(\"object-assign\"),r=require(\"scheduler\");function u(a){for(var b=\"https://reactjs.org/docs/error-decoder.html?invariant=\"+a,c=1;c<arguments.length;c++)b+=\"&args[]=\"+encodeURIComponent(arguments[c]);return\"Minified React error #\"+a+\"; visit \"+b+\" for the full message or use the non-minified dev environment for full errors and additional helpful warnings.\"}if(!aa)throw Error(u(227));\nfunction ba(a,b,c,d,e,f,g,h,k){var l=Array.prototype.slice.call(arguments,3);try{b.apply(c,l)}catch(m){this.onError(m)}}var da=!1,ea=null,fa=!1,ha=null,ia={onError:function(a){da=!0;ea=a}};function ja(a,b,c,d,e,f,g,h,k){da=!1;ea=null;ba.apply(ia,arguments)}function ka(a,b,c,d,e,f,g,h,k){ja.apply(this,arguments);if(da){if(da){var l=ea;da=!1;ea=null}else throw Error(u(198));fa||(fa=!0,ha=l)}}var la=null,ma=null,na=null;\nfunction oa(a,b,c){var d=a.type||\"unknown-event\";a.currentTarget=na(c);ka(d,b,void 0,a);a.currentTarget=null}var pa=null,qa={};\nfunction ra(){if(pa)for(var a in qa){var b=qa[a],c=pa.indexOf(a);if(!(-1<c))throw Error(u(96,a));if(!sa[c]){if(!b.extractEvents)throw Error(u(97,a));sa[c]=b;c=b.eventTypes;for(var d in c){var e=void 0;var f=c[d],g=b,h=d;if(ta.hasOwnProperty(h))throw Error(u(99,h));ta[h]=f;var k=f.phasedRegistrationNames;if(k){for(e in k)k.hasOwnProperty(e)&&ua(k[e],g,h);e=!0}else f.registrationName?(ua(f.registrationName,g,h),e=!0):e=!1;if(!e)throw Error(u(98,d,a));}}}}\nfunction ua(a,b,c){if(va[a])throw Error(u(100,a));va[a]=b;wa[a]=b.eventTypes[c].dependencies}var sa=[],ta={},va={},wa={};function xa(a){var b=!1,c;for(c in a)if(a.hasOwnProperty(c)){var d=a[c];if(!qa.hasOwnProperty(c)||qa[c]!==d){if(qa[c])throw Error(u(102,c));qa[c]=d;b=!0}}b&&ra()}var ya=!(\"undefined\"===typeof window||\"undefined\"===typeof window.document||\"undefined\"===typeof window.document.createElement),za=null,Aa=null,Ba=null;\nfunction Ca(a){if(a=ma(a)){if(\"function\"!==typeof za)throw Error(u(280));var b=a.stateNode;b&&(b=la(b),za(a.stateNode,a.type,b))}}function Da(a){Aa?Ba?Ba.push(a):Ba=[a]:Aa=a}function Ea(){if(Aa){var a=Aa,b=Ba;Ba=Aa=null;Ca(a);if(b)for(a=0;a<b.length;a++)Ca(b[a])}}function Fa(a,b){return a(b)}function Ga(a,b,c,d,e){return a(b,c,d,e)}function Ha(){}var Ia=Fa,Ja=!1,Ka=!1;function La(){if(null!==Aa||null!==Ba)Ha(),Ea()}\nfunction Ma(a,b,c){if(Ka)return a(b,c);Ka=!0;try{return Ia(a,b,c)}finally{Ka=!1,La()}}var Na=/^[:A-Z_a-z\\u00C0-\\u00D6\\u00D8-\\u00F6\\u00F8-\\u02FF\\u0370-\\u037D\\u037F-\\u1FFF\\u200C-\\u200D\\u2070-\\u218F\\u2C00-\\u2FEF\\u3001-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFFD][:A-Z_a-z\\u00C0-\\u00D6\\u00D8-\\u00F6\\u00F8-\\u02FF\\u0370-\\u037D\\u037F-\\u1FFF\\u200C-\\u200D\\u2070-\\u218F\\u2C00-\\u2FEF\\u3001-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFFD\\-.0-9\\u00B7\\u0300-\\u036F\\u203F-\\u2040]*$/,Oa=Object.prototype.hasOwnProperty,Pa={},Qa={};\nfunction Ra(a){if(Oa.call(Qa,a))return!0;if(Oa.call(Pa,a))return!1;if(Na.test(a))return Qa[a]=!0;Pa[a]=!0;return!1}function Sa(a,b,c,d){if(null!==c&&0===c.type)return!1;switch(typeof b){case \"function\":case \"symbol\":return!0;case \"boolean\":if(d)return!1;if(null!==c)return!c.acceptsBooleans;a=a.toLowerCase().slice(0,5);return\"data-\"!==a&&\"aria-\"!==a;default:return!1}}\nfunction Ta(a,b,c,d){if(null===b||\"undefined\"===typeof b||Sa(a,b,c,d))return!0;if(d)return!1;if(null!==c)switch(c.type){case 3:return!b;case 4:return!1===b;case 5:return isNaN(b);case 6:return isNaN(b)||1>b}return!1}function v(a,b,c,d,e,f){this.acceptsBooleans=2===b||3===b||4===b;this.attributeName=d;this.attributeNamespace=e;this.mustUseProperty=c;this.propertyName=a;this.type=b;this.sanitizeURL=f}var C={};\n\"children dangerouslySetInnerHTML defaultValue defaultChecked innerHTML suppressContentEditableWarning suppressHydrationWarning style\".split(\" \").forEach(function(a){C[a]=new v(a,0,!1,a,null,!1)});[[\"acceptCharset\",\"accept-charset\"],[\"className\",\"class\"],[\"htmlFor\",\"for\"],[\"httpEquiv\",\"http-equiv\"]].forEach(function(a){var b=a[0];C[b]=new v(b,1,!1,a[1],null,!1)});[\"contentEditable\",\"draggable\",\"spellCheck\",\"value\"].forEach(function(a){C[a]=new v(a,2,!1,a.toLowerCase(),null,!1)});\n[\"autoReverse\",\"externalResourcesRequired\",\"focusable\",\"preserveAlpha\"].forEach(function(a){C[a]=new v(a,2,!1,a,null,!1)});\"allowFullScreen async autoFocus autoPlay controls default defer disabled disablePictureInPicture formNoValidate hidden loop noModule noValidate open playsInline readOnly required reversed scoped seamless itemScope\".split(\" \").forEach(function(a){C[a]=new v(a,3,!1,a.toLowerCase(),null,!1)});\n[\"checked\",\"multiple\",\"muted\",\"selected\"].forEach(function(a){C[a]=new v(a,3,!0,a,null,!1)});[\"capture\",\"download\"].forEach(function(a){C[a]=new v(a,4,!1,a,null,!1)});[\"cols\",\"rows\",\"size\",\"span\"].forEach(function(a){C[a]=new v(a,6,!1,a,null,!1)});[\"rowSpan\",\"start\"].forEach(function(a){C[a]=new v(a,5,!1,a.toLowerCase(),null,!1)});var Ua=/[\\-:]([a-z])/g;function Va(a){return a[1].toUpperCase()}\n\"accent-height alignment-baseline arabic-form baseline-shift cap-height clip-path clip-rule color-interpolation color-interpolation-filters color-profile color-rendering dominant-baseline enable-background fill-opacity fill-rule flood-color flood-opacity font-family font-size font-size-adjust font-stretch font-style font-variant font-weight glyph-name glyph-orientation-horizontal glyph-orientation-vertical horiz-adv-x horiz-origin-x image-rendering letter-spacing lighting-color marker-end marker-mid marker-start overline-position overline-thickness paint-order panose-1 pointer-events rendering-intent shape-rendering stop-color stop-opacity strikethrough-position strikethrough-thickness stroke-dasharray stroke-dashoffset stroke-linecap stroke-linejoin stroke-miterlimit stroke-opacity stroke-width text-anchor text-decoration text-rendering underline-position underline-thickness unicode-bidi unicode-range units-per-em v-alphabetic v-hanging v-ideographic v-mathematical vector-effect vert-adv-y vert-origin-x vert-origin-y word-spacing writing-mode xmlns:xlink x-height\".split(\" \").forEach(function(a){var b=a.replace(Ua,\nVa);C[b]=new v(b,1,!1,a,null,!1)});\"xlink:actuate xlink:arcrole xlink:role xlink:show xlink:title xlink:type\".split(\" \").forEach(function(a){var b=a.replace(Ua,Va);C[b]=new v(b,1,!1,a,\"http://www.w3.org/1999/xlink\",!1)});[\"xml:base\",\"xml:lang\",\"xml:space\"].forEach(function(a){var b=a.replace(Ua,Va);C[b]=new v(b,1,!1,a,\"http://www.w3.org/XML/1998/namespace\",!1)});[\"tabIndex\",\"crossOrigin\"].forEach(function(a){C[a]=new v(a,1,!1,a.toLowerCase(),null,!1)});\nC.xlinkHref=new v(\"xlinkHref\",1,!1,\"xlink:href\",\"http://www.w3.org/1999/xlink\",!0);[\"src\",\"href\",\"action\",\"formAction\"].forEach(function(a){C[a]=new v(a,1,!1,a.toLowerCase(),null,!0)});var Wa=aa.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED;Wa.hasOwnProperty(\"ReactCurrentDispatcher\")||(Wa.ReactCurrentDispatcher={current:null});Wa.hasOwnProperty(\"ReactCurrentBatchConfig\")||(Wa.ReactCurrentBatchConfig={suspense:null});\nfunction Xa(a,b,c,d){var e=C.hasOwnProperty(b)?C[b]:null;var f=null!==e?0===e.type:d?!1:!(2<b.length)||\"o\"!==b[0]&&\"O\"!==b[0]||\"n\"!==b[1]&&\"N\"!==b[1]?!1:!0;f||(Ta(b,c,e,d)&&(c=null),d||null===e?Ra(b)&&(null===c?a.removeAttribute(b):a.setAttribute(b,\"\"+c)):e.mustUseProperty?a[e.propertyName]=null===c?3===e.type?!1:\"\":c:(b=e.attributeName,d=e.attributeNamespace,null===c?a.removeAttribute(b):(e=e.type,c=3===e||4===e&&!0===c?\"\":\"\"+c,d?a.setAttributeNS(d,b,c):a.setAttribute(b,c))))}\nvar Ya=/^(.*)[\\\\\\/]/,E=\"function\"===typeof Symbol&&Symbol.for,Za=E?Symbol.for(\"react.element\"):60103,$a=E?Symbol.for(\"react.portal\"):60106,ab=E?Symbol.for(\"react.fragment\"):60107,bb=E?Symbol.for(\"react.strict_mode\"):60108,cb=E?Symbol.for(\"react.profiler\"):60114,db=E?Symbol.for(\"react.provider\"):60109,eb=E?Symbol.for(\"react.context\"):60110,fb=E?Symbol.for(\"react.concurrent_mode\"):60111,gb=E?Symbol.for(\"react.forward_ref\"):60112,hb=E?Symbol.for(\"react.suspense\"):60113,ib=E?Symbol.for(\"react.suspense_list\"):\n60120,jb=E?Symbol.for(\"react.memo\"):60115,kb=E?Symbol.for(\"react.lazy\"):60116,lb=E?Symbol.for(\"react.block\"):60121,mb=\"function\"===typeof Symbol&&Symbol.iterator;function nb(a){if(null===a||\"object\"!==typeof a)return null;a=mb&&a[mb]||a[\"@@iterator\"];return\"function\"===typeof a?a:null}function ob(a){if(-1===a._status){a._status=0;var b=a._ctor;b=b();a._result=b;b.then(function(b){0===a._status&&(b=b.default,a._status=1,a._result=b)},function(b){0===a._status&&(a._status=2,a._result=b)})}}\nfunction pb(a){if(null==a)return null;if(\"function\"===typeof a)return a.displayName||a.name||null;if(\"string\"===typeof a)return a;switch(a){case ab:return\"Fragment\";case $a:return\"Portal\";case cb:return\"Profiler\";case bb:return\"StrictMode\";case hb:return\"Suspense\";case ib:return\"SuspenseList\"}if(\"object\"===typeof a)switch(a.$$typeof){case eb:return\"Context.Consumer\";case db:return\"Context.Provider\";case gb:var b=a.render;b=b.displayName||b.name||\"\";return a.displayName||(\"\"!==b?\"ForwardRef(\"+b+\")\":\n\"ForwardRef\");case jb:return pb(a.type);case lb:return pb(a.render);case kb:if(a=1===a._status?a._result:null)return pb(a)}return null}function qb(a){var b=\"\";do{a:switch(a.tag){case 3:case 4:case 6:case 7:case 10:case 9:var c=\"\";break a;default:var d=a._debugOwner,e=a._debugSource,f=pb(a.type);c=null;d&&(c=pb(d.type));d=f;f=\"\";e?f=\" (at \"+e.fileName.replace(Ya,\"\")+\":\"+e.lineNumber+\")\":c&&(f=\" (created by \"+c+\")\");c=\"\\n    in \"+(d||\"Unknown\")+f}b+=c;a=a.return}while(a);return b}\nfunction rb(a){switch(typeof a){case \"boolean\":case \"number\":case \"object\":case \"string\":case \"undefined\":return a;default:return\"\"}}function sb(a){var b=a.type;return(a=a.nodeName)&&\"input\"===a.toLowerCase()&&(\"checkbox\"===b||\"radio\"===b)}\nfunction tb(a){var b=sb(a)?\"checked\":\"value\",c=Object.getOwnPropertyDescriptor(a.constructor.prototype,b),d=\"\"+a[b];if(!a.hasOwnProperty(b)&&\"undefined\"!==typeof c&&\"function\"===typeof c.get&&\"function\"===typeof c.set){var e=c.get,f=c.set;Object.defineProperty(a,b,{configurable:!0,get:function(){return e.call(this)},set:function(a){d=\"\"+a;f.call(this,a)}});Object.defineProperty(a,b,{enumerable:c.enumerable});return{getValue:function(){return d},setValue:function(a){d=\"\"+a},stopTracking:function(){a._valueTracker=\nnull;delete a[b]}}}}function xb(a){a._valueTracker||(a._valueTracker=tb(a))}function yb(a){if(!a)return!1;var b=a._valueTracker;if(!b)return!0;var c=b.getValue();var d=\"\";a&&(d=sb(a)?a.checked?\"true\":\"false\":a.value);a=d;return a!==c?(b.setValue(a),!0):!1}function zb(a,b){var c=b.checked;return n({},b,{defaultChecked:void 0,defaultValue:void 0,value:void 0,checked:null!=c?c:a._wrapperState.initialChecked})}\nfunction Ab(a,b){var c=null==b.defaultValue?\"\":b.defaultValue,d=null!=b.checked?b.checked:b.defaultChecked;c=rb(null!=b.value?b.value:c);a._wrapperState={initialChecked:d,initialValue:c,controlled:\"checkbox\"===b.type||\"radio\"===b.type?null!=b.checked:null!=b.value}}function Bb(a,b){b=b.checked;null!=b&&Xa(a,\"checked\",b,!1)}\nfunction Cb(a,b){Bb(a,b);var c=rb(b.value),d=b.type;if(null!=c)if(\"number\"===d){if(0===c&&\"\"===a.value||a.value!=c)a.value=\"\"+c}else a.value!==\"\"+c&&(a.value=\"\"+c);else if(\"submit\"===d||\"reset\"===d){a.removeAttribute(\"value\");return}b.hasOwnProperty(\"value\")?Db(a,b.type,c):b.hasOwnProperty(\"defaultValue\")&&Db(a,b.type,rb(b.defaultValue));null==b.checked&&null!=b.defaultChecked&&(a.defaultChecked=!!b.defaultChecked)}\nfunction Eb(a,b,c){if(b.hasOwnProperty(\"value\")||b.hasOwnProperty(\"defaultValue\")){var d=b.type;if(!(\"submit\"!==d&&\"reset\"!==d||void 0!==b.value&&null!==b.value))return;b=\"\"+a._wrapperState.initialValue;c||b===a.value||(a.value=b);a.defaultValue=b}c=a.name;\"\"!==c&&(a.name=\"\");a.defaultChecked=!!a._wrapperState.initialChecked;\"\"!==c&&(a.name=c)}\nfunction Db(a,b,c){if(\"number\"!==b||a.ownerDocument.activeElement!==a)null==c?a.defaultValue=\"\"+a._wrapperState.initialValue:a.defaultValue!==\"\"+c&&(a.defaultValue=\"\"+c)}function Fb(a){var b=\"\";aa.Children.forEach(a,function(a){null!=a&&(b+=a)});return b}function Gb(a,b){a=n({children:void 0},b);if(b=Fb(b.children))a.children=b;return a}\nfunction Hb(a,b,c,d){a=a.options;if(b){b={};for(var e=0;e<c.length;e++)b[\"$\"+c[e]]=!0;for(c=0;c<a.length;c++)e=b.hasOwnProperty(\"$\"+a[c].value),a[c].selected!==e&&(a[c].selected=e),e&&d&&(a[c].defaultSelected=!0)}else{c=\"\"+rb(c);b=null;for(e=0;e<a.length;e++){if(a[e].value===c){a[e].selected=!0;d&&(a[e].defaultSelected=!0);return}null!==b||a[e].disabled||(b=a[e])}null!==b&&(b.selected=!0)}}\nfunction Ib(a,b){if(null!=b.dangerouslySetInnerHTML)throw Error(u(91));return n({},b,{value:void 0,defaultValue:void 0,children:\"\"+a._wrapperState.initialValue})}function Jb(a,b){var c=b.value;if(null==c){c=b.children;b=b.defaultValue;if(null!=c){if(null!=b)throw Error(u(92));if(Array.isArray(c)){if(!(1>=c.length))throw Error(u(93));c=c[0]}b=c}null==b&&(b=\"\");c=b}a._wrapperState={initialValue:rb(c)}}\nfunction Kb(a,b){var c=rb(b.value),d=rb(b.defaultValue);null!=c&&(c=\"\"+c,c!==a.value&&(a.value=c),null==b.defaultValue&&a.defaultValue!==c&&(a.defaultValue=c));null!=d&&(a.defaultValue=\"\"+d)}function Lb(a){var b=a.textContent;b===a._wrapperState.initialValue&&\"\"!==b&&null!==b&&(a.value=b)}var Mb={html:\"http://www.w3.org/1999/xhtml\",mathml:\"http://www.w3.org/1998/Math/MathML\",svg:\"http://www.w3.org/2000/svg\"};\nfunction Nb(a){switch(a){case \"svg\":return\"http://www.w3.org/2000/svg\";case \"math\":return\"http://www.w3.org/1998/Math/MathML\";default:return\"http://www.w3.org/1999/xhtml\"}}function Ob(a,b){return null==a||\"http://www.w3.org/1999/xhtml\"===a?Nb(b):\"http://www.w3.org/2000/svg\"===a&&\"foreignObject\"===b?\"http://www.w3.org/1999/xhtml\":a}\nvar Pb,Qb=function(a){return\"undefined\"!==typeof MSApp&&MSApp.execUnsafeLocalFunction?function(b,c,d,e){MSApp.execUnsafeLocalFunction(function(){return a(b,c,d,e)})}:a}(function(a,b){if(a.namespaceURI!==Mb.svg||\"innerHTML\"in a)a.innerHTML=b;else{Pb=Pb||document.createElement(\"div\");Pb.innerHTML=\"<svg>\"+b.valueOf().toString()+\"</svg>\";for(b=Pb.firstChild;a.firstChild;)a.removeChild(a.firstChild);for(;b.firstChild;)a.appendChild(b.firstChild)}});\nfunction Rb(a,b){if(b){var c=a.firstChild;if(c&&c===a.lastChild&&3===c.nodeType){c.nodeValue=b;return}}a.textContent=b}function Sb(a,b){var c={};c[a.toLowerCase()]=b.toLowerCase();c[\"Webkit\"+a]=\"webkit\"+b;c[\"Moz\"+a]=\"moz\"+b;return c}var Tb={animationend:Sb(\"Animation\",\"AnimationEnd\"),animationiteration:Sb(\"Animation\",\"AnimationIteration\"),animationstart:Sb(\"Animation\",\"AnimationStart\"),transitionend:Sb(\"Transition\",\"TransitionEnd\")},Ub={},Vb={};\nya&&(Vb=document.createElement(\"div\").style,\"AnimationEvent\"in window||(delete Tb.animationend.animation,delete Tb.animationiteration.animation,delete Tb.animationstart.animation),\"TransitionEvent\"in window||delete Tb.transitionend.transition);function Wb(a){if(Ub[a])return Ub[a];if(!Tb[a])return a;var b=Tb[a],c;for(c in b)if(b.hasOwnProperty(c)&&c in Vb)return Ub[a]=b[c];return a}\nvar Xb=Wb(\"animationend\"),Yb=Wb(\"animationiteration\"),Zb=Wb(\"animationstart\"),$b=Wb(\"transitionend\"),ac=\"abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange seeked seeking stalled suspend timeupdate volumechange waiting\".split(\" \"),bc=new (\"function\"===typeof WeakMap?WeakMap:Map);function cc(a){var b=bc.get(a);void 0===b&&(b=new Map,bc.set(a,b));return b}\nfunction dc(a){var b=a,c=a;if(a.alternate)for(;b.return;)b=b.return;else{a=b;do b=a,0!==(b.effectTag&1026)&&(c=b.return),a=b.return;while(a)}return 3===b.tag?c:null}function ec(a){if(13===a.tag){var b=a.memoizedState;null===b&&(a=a.alternate,null!==a&&(b=a.memoizedState));if(null!==b)return b.dehydrated}return null}function fc(a){if(dc(a)!==a)throw Error(u(188));}\nfunction gc(a){var b=a.alternate;if(!b){b=dc(a);if(null===b)throw Error(u(188));return b!==a?null:a}for(var c=a,d=b;;){var e=c.return;if(null===e)break;var f=e.alternate;if(null===f){d=e.return;if(null!==d){c=d;continue}break}if(e.child===f.child){for(f=e.child;f;){if(f===c)return fc(e),a;if(f===d)return fc(e),b;f=f.sibling}throw Error(u(188));}if(c.return!==d.return)c=e,d=f;else{for(var g=!1,h=e.child;h;){if(h===c){g=!0;c=e;d=f;break}if(h===d){g=!0;d=e;c=f;break}h=h.sibling}if(!g){for(h=f.child;h;){if(h===\nc){g=!0;c=f;d=e;break}if(h===d){g=!0;d=f;c=e;break}h=h.sibling}if(!g)throw Error(u(189));}}if(c.alternate!==d)throw Error(u(190));}if(3!==c.tag)throw Error(u(188));return c.stateNode.current===c?a:b}function hc(a){a=gc(a);if(!a)return null;for(var b=a;;){if(5===b.tag||6===b.tag)return b;if(b.child)b.child.return=b,b=b.child;else{if(b===a)break;for(;!b.sibling;){if(!b.return||b.return===a)return null;b=b.return}b.sibling.return=b.return;b=b.sibling}}return null}\nfunction ic(a,b){if(null==b)throw Error(u(30));if(null==a)return b;if(Array.isArray(a)){if(Array.isArray(b))return a.push.apply(a,b),a;a.push(b);return a}return Array.isArray(b)?[a].concat(b):[a,b]}function jc(a,b,c){Array.isArray(a)?a.forEach(b,c):a&&b.call(c,a)}var kc=null;\nfunction lc(a){if(a){var b=a._dispatchListeners,c=a._dispatchInstances;if(Array.isArray(b))for(var d=0;d<b.length&&!a.isPropagationStopped();d++)oa(a,b[d],c[d]);else b&&oa(a,b,c);a._dispatchListeners=null;a._dispatchInstances=null;a.isPersistent()||a.constructor.release(a)}}function mc(a){null!==a&&(kc=ic(kc,a));a=kc;kc=null;if(a){jc(a,lc);if(kc)throw Error(u(95));if(fa)throw a=ha,fa=!1,ha=null,a;}}\nfunction nc(a){a=a.target||a.srcElement||window;a.correspondingUseElement&&(a=a.correspondingUseElement);return 3===a.nodeType?a.parentNode:a}function oc(a){if(!ya)return!1;a=\"on\"+a;var b=a in document;b||(b=document.createElement(\"div\"),b.setAttribute(a,\"return;\"),b=\"function\"===typeof b[a]);return b}var pc=[];function qc(a){a.topLevelType=null;a.nativeEvent=null;a.targetInst=null;a.ancestors.length=0;10>pc.length&&pc.push(a)}\nfunction rc(a,b,c,d){if(pc.length){var e=pc.pop();e.topLevelType=a;e.eventSystemFlags=d;e.nativeEvent=b;e.targetInst=c;return e}return{topLevelType:a,eventSystemFlags:d,nativeEvent:b,targetInst:c,ancestors:[]}}\nfunction sc(a){var b=a.targetInst,c=b;do{if(!c){a.ancestors.push(c);break}var d=c;if(3===d.tag)d=d.stateNode.containerInfo;else{for(;d.return;)d=d.return;d=3!==d.tag?null:d.stateNode.containerInfo}if(!d)break;b=c.tag;5!==b&&6!==b||a.ancestors.push(c);c=tc(d)}while(c);for(c=0;c<a.ancestors.length;c++){b=a.ancestors[c];var e=nc(a.nativeEvent);d=a.topLevelType;var f=a.nativeEvent,g=a.eventSystemFlags;0===c&&(g|=64);for(var h=null,k=0;k<sa.length;k++){var l=sa[k];l&&(l=l.extractEvents(d,b,f,e,g))&&(h=\nic(h,l))}mc(h)}}function uc(a,b,c){if(!c.has(a)){switch(a){case \"scroll\":vc(b,\"scroll\",!0);break;case \"focus\":case \"blur\":vc(b,\"focus\",!0);vc(b,\"blur\",!0);c.set(\"blur\",null);c.set(\"focus\",null);break;case \"cancel\":case \"close\":oc(a)&&vc(b,a,!0);break;case \"invalid\":case \"submit\":case \"reset\":break;default:-1===ac.indexOf(a)&&F(a,b)}c.set(a,null)}}\nvar wc,xc,yc,zc=!1,Ac=[],Bc=null,Cc=null,Dc=null,Ec=new Map,Fc=new Map,Gc=[],Hc=\"mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput close cancel copy cut paste click change contextmenu reset submit\".split(\" \"),Ic=\"focus blur dragenter dragleave mouseover mouseout pointerover pointerout gotpointercapture lostpointercapture\".split(\" \");\nfunction Jc(a,b){var c=cc(b);Hc.forEach(function(a){uc(a,b,c)});Ic.forEach(function(a){uc(a,b,c)})}function Kc(a,b,c,d,e){return{blockedOn:a,topLevelType:b,eventSystemFlags:c|32,nativeEvent:e,container:d}}\nfunction Lc(a,b){switch(a){case \"focus\":case \"blur\":Bc=null;break;case \"dragenter\":case \"dragleave\":Cc=null;break;case \"mouseover\":case \"mouseout\":Dc=null;break;case \"pointerover\":case \"pointerout\":Ec.delete(b.pointerId);break;case \"gotpointercapture\":case \"lostpointercapture\":Fc.delete(b.pointerId)}}function Mc(a,b,c,d,e,f){if(null===a||a.nativeEvent!==f)return a=Kc(b,c,d,e,f),null!==b&&(b=Nc(b),null!==b&&xc(b)),a;a.eventSystemFlags|=d;return a}\nfunction Oc(a,b,c,d,e){switch(b){case \"focus\":return Bc=Mc(Bc,a,b,c,d,e),!0;case \"dragenter\":return Cc=Mc(Cc,a,b,c,d,e),!0;case \"mouseover\":return Dc=Mc(Dc,a,b,c,d,e),!0;case \"pointerover\":var f=e.pointerId;Ec.set(f,Mc(Ec.get(f)||null,a,b,c,d,e));return!0;case \"gotpointercapture\":return f=e.pointerId,Fc.set(f,Mc(Fc.get(f)||null,a,b,c,d,e)),!0}return!1}\nfunction Pc(a){var b=tc(a.target);if(null!==b){var c=dc(b);if(null!==c)if(b=c.tag,13===b){if(b=ec(c),null!==b){a.blockedOn=b;r.unstable_runWithPriority(a.priority,function(){yc(c)});return}}else if(3===b&&c.stateNode.hydrate){a.blockedOn=3===c.tag?c.stateNode.containerInfo:null;return}}a.blockedOn=null}function Qc(a){if(null!==a.blockedOn)return!1;var b=Rc(a.topLevelType,a.eventSystemFlags,a.container,a.nativeEvent);if(null!==b){var c=Nc(b);null!==c&&xc(c);a.blockedOn=b;return!1}return!0}\nfunction Sc(a,b,c){Qc(a)&&c.delete(b)}function Tc(){for(zc=!1;0<Ac.length;){var a=Ac[0];if(null!==a.blockedOn){a=Nc(a.blockedOn);null!==a&&wc(a);break}var b=Rc(a.topLevelType,a.eventSystemFlags,a.container,a.nativeEvent);null!==b?a.blockedOn=b:Ac.shift()}null!==Bc&&Qc(Bc)&&(Bc=null);null!==Cc&&Qc(Cc)&&(Cc=null);null!==Dc&&Qc(Dc)&&(Dc=null);Ec.forEach(Sc);Fc.forEach(Sc)}function Uc(a,b){a.blockedOn===b&&(a.blockedOn=null,zc||(zc=!0,r.unstable_scheduleCallback(r.unstable_NormalPriority,Tc)))}\nfunction Vc(a){function b(b){return Uc(b,a)}if(0<Ac.length){Uc(Ac[0],a);for(var c=1;c<Ac.length;c++){var d=Ac[c];d.blockedOn===a&&(d.blockedOn=null)}}null!==Bc&&Uc(Bc,a);null!==Cc&&Uc(Cc,a);null!==Dc&&Uc(Dc,a);Ec.forEach(b);Fc.forEach(b);for(c=0;c<Gc.length;c++)d=Gc[c],d.blockedOn===a&&(d.blockedOn=null);for(;0<Gc.length&&(c=Gc[0],null===c.blockedOn);)Pc(c),null===c.blockedOn&&Gc.shift()}\nvar Wc={},Yc=new Map,Zc=new Map,$c=[\"abort\",\"abort\",Xb,\"animationEnd\",Yb,\"animationIteration\",Zb,\"animationStart\",\"canplay\",\"canPlay\",\"canplaythrough\",\"canPlayThrough\",\"durationchange\",\"durationChange\",\"emptied\",\"emptied\",\"encrypted\",\"encrypted\",\"ended\",\"ended\",\"error\",\"error\",\"gotpointercapture\",\"gotPointerCapture\",\"load\",\"load\",\"loadeddata\",\"loadedData\",\"loadedmetadata\",\"loadedMetadata\",\"loadstart\",\"loadStart\",\"lostpointercapture\",\"lostPointerCapture\",\"playing\",\"playing\",\"progress\",\"progress\",\"seeking\",\n\"seeking\",\"stalled\",\"stalled\",\"suspend\",\"suspend\",\"timeupdate\",\"timeUpdate\",$b,\"transitionEnd\",\"waiting\",\"waiting\"];function ad(a,b){for(var c=0;c<a.length;c+=2){var d=a[c],e=a[c+1],f=\"on\"+(e[0].toUpperCase()+e.slice(1));f={phasedRegistrationNames:{bubbled:f,captured:f+\"Capture\"},dependencies:[d],eventPriority:b};Zc.set(d,b);Yc.set(d,f);Wc[e]=f}}\nad(\"blur blur cancel cancel click click close close contextmenu contextMenu copy copy cut cut auxclick auxClick dblclick doubleClick dragend dragEnd dragstart dragStart drop drop focus focus input input invalid invalid keydown keyDown keypress keyPress keyup keyUp mousedown mouseDown mouseup mouseUp paste paste pause pause play play pointercancel pointerCancel pointerdown pointerDown pointerup pointerUp ratechange rateChange reset reset seeked seeked submit submit touchcancel touchCancel touchend touchEnd touchstart touchStart volumechange volumeChange\".split(\" \"),0);\nad(\"drag drag dragenter dragEnter dragexit dragExit dragleave dragLeave dragover dragOver mousemove mouseMove mouseout mouseOut mouseover mouseOver pointermove pointerMove pointerout pointerOut pointerover pointerOver scroll scroll toggle toggle touchmove touchMove wheel wheel\".split(\" \"),1);ad($c,2);for(var bd=\"change selectionchange textInput compositionstart compositionend compositionupdate\".split(\" \"),cd=0;cd<bd.length;cd++)Zc.set(bd[cd],0);\nvar dd=r.unstable_UserBlockingPriority,ed=r.unstable_runWithPriority,fd=!0;function F(a,b){vc(b,a,!1)}function vc(a,b,c){var d=Zc.get(b);switch(void 0===d?2:d){case 0:d=gd.bind(null,b,1,a);break;case 1:d=hd.bind(null,b,1,a);break;default:d=id.bind(null,b,1,a)}c?a.addEventListener(b,d,!0):a.addEventListener(b,d,!1)}function gd(a,b,c,d){Ja||Ha();var e=id,f=Ja;Ja=!0;try{Ga(e,a,b,c,d)}finally{(Ja=f)||La()}}function hd(a,b,c,d){ed(dd,id.bind(null,a,b,c,d))}\nfunction id(a,b,c,d){if(fd)if(0<Ac.length&&-1<Hc.indexOf(a))a=Kc(null,a,b,c,d),Ac.push(a);else{var e=Rc(a,b,c,d);if(null===e)Lc(a,d);else if(-1<Hc.indexOf(a))a=Kc(e,a,b,c,d),Ac.push(a);else if(!Oc(e,a,b,c,d)){Lc(a,d);a=rc(a,d,null,b);try{Ma(sc,a)}finally{qc(a)}}}}\nfunction Rc(a,b,c,d){c=nc(d);c=tc(c);if(null!==c){var e=dc(c);if(null===e)c=null;else{var f=e.tag;if(13===f){c=ec(e);if(null!==c)return c;c=null}else if(3===f){if(e.stateNode.hydrate)return 3===e.tag?e.stateNode.containerInfo:null;c=null}else e!==c&&(c=null)}}a=rc(a,d,c,b);try{Ma(sc,a)}finally{qc(a)}return null}\nvar jd={animationIterationCount:!0,borderImageOutset:!0,borderImageSlice:!0,borderImageWidth:!0,boxFlex:!0,boxFlexGroup:!0,boxOrdinalGroup:!0,columnCount:!0,columns:!0,flex:!0,flexGrow:!0,flexPositive:!0,flexShrink:!0,flexNegative:!0,flexOrder:!0,gridArea:!0,gridRow:!0,gridRowEnd:!0,gridRowSpan:!0,gridRowStart:!0,gridColumn:!0,gridColumnEnd:!0,gridColumnSpan:!0,gridColumnStart:!0,fontWeight:!0,lineClamp:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,tabSize:!0,widows:!0,zIndex:!0,zoom:!0,fillOpacity:!0,\nfloodOpacity:!0,stopOpacity:!0,strokeDasharray:!0,strokeDashoffset:!0,strokeMiterlimit:!0,strokeOpacity:!0,strokeWidth:!0},kd=[\"Webkit\",\"ms\",\"Moz\",\"O\"];Object.keys(jd).forEach(function(a){kd.forEach(function(b){b=b+a.charAt(0).toUpperCase()+a.substring(1);jd[b]=jd[a]})});function ld(a,b,c){return null==b||\"boolean\"===typeof b||\"\"===b?\"\":c||\"number\"!==typeof b||0===b||jd.hasOwnProperty(a)&&jd[a]?(\"\"+b).trim():b+\"px\"}\nfunction md(a,b){a=a.style;for(var c in b)if(b.hasOwnProperty(c)){var d=0===c.indexOf(\"--\"),e=ld(c,b[c],d);\"float\"===c&&(c=\"cssFloat\");d?a.setProperty(c,e):a[c]=e}}var nd=n({menuitem:!0},{area:!0,base:!0,br:!0,col:!0,embed:!0,hr:!0,img:!0,input:!0,keygen:!0,link:!0,meta:!0,param:!0,source:!0,track:!0,wbr:!0});\nfunction od(a,b){if(b){if(nd[a]&&(null!=b.children||null!=b.dangerouslySetInnerHTML))throw Error(u(137,a,\"\"));if(null!=b.dangerouslySetInnerHTML){if(null!=b.children)throw Error(u(60));if(!(\"object\"===typeof b.dangerouslySetInnerHTML&&\"__html\"in b.dangerouslySetInnerHTML))throw Error(u(61));}if(null!=b.style&&\"object\"!==typeof b.style)throw Error(u(62,\"\"));}}\nfunction pd(a,b){if(-1===a.indexOf(\"-\"))return\"string\"===typeof b.is;switch(a){case \"annotation-xml\":case \"color-profile\":case \"font-face\":case \"font-face-src\":case \"font-face-uri\":case \"font-face-format\":case \"font-face-name\":case \"missing-glyph\":return!1;default:return!0}}var qd=Mb.html;function rd(a,b){a=9===a.nodeType||11===a.nodeType?a:a.ownerDocument;var c=cc(a);b=wa[b];for(var d=0;d<b.length;d++)uc(b[d],a,c)}function sd(){}\nfunction td(a){a=a||(\"undefined\"!==typeof document?document:void 0);if(\"undefined\"===typeof a)return null;try{return a.activeElement||a.body}catch(b){return a.body}}function ud(a){for(;a&&a.firstChild;)a=a.firstChild;return a}function vd(a,b){var c=ud(a);a=0;for(var d;c;){if(3===c.nodeType){d=a+c.textContent.length;if(a<=b&&d>=b)return{node:c,offset:b-a};a=d}a:{for(;c;){if(c.nextSibling){c=c.nextSibling;break a}c=c.parentNode}c=void 0}c=ud(c)}}\nfunction wd(a,b){return a&&b?a===b?!0:a&&3===a.nodeType?!1:b&&3===b.nodeType?wd(a,b.parentNode):\"contains\"in a?a.contains(b):a.compareDocumentPosition?!!(a.compareDocumentPosition(b)&16):!1:!1}function xd(){for(var a=window,b=td();b instanceof a.HTMLIFrameElement;){try{var c=\"string\"===typeof b.contentWindow.location.href}catch(d){c=!1}if(c)a=b.contentWindow;else break;b=td(a.document)}return b}\nfunction yd(a){var b=a&&a.nodeName&&a.nodeName.toLowerCase();return b&&(\"input\"===b&&(\"text\"===a.type||\"search\"===a.type||\"tel\"===a.type||\"url\"===a.type||\"password\"===a.type)||\"textarea\"===b||\"true\"===a.contentEditable)}var zd=\"$\",Ad=\"/$\",Bd=\"$?\",Cd=\"$!\",Dd=null,Ed=null;function Fd(a,b){switch(a){case \"button\":case \"input\":case \"select\":case \"textarea\":return!!b.autoFocus}return!1}\nfunction Gd(a,b){return\"textarea\"===a||\"option\"===a||\"noscript\"===a||\"string\"===typeof b.children||\"number\"===typeof b.children||\"object\"===typeof b.dangerouslySetInnerHTML&&null!==b.dangerouslySetInnerHTML&&null!=b.dangerouslySetInnerHTML.__html}var Hd=\"function\"===typeof setTimeout?setTimeout:void 0,Id=\"function\"===typeof clearTimeout?clearTimeout:void 0;function Jd(a){for(;null!=a;a=a.nextSibling){var b=a.nodeType;if(1===b||3===b)break}return a}\nfunction Kd(a){a=a.previousSibling;for(var b=0;a;){if(8===a.nodeType){var c=a.data;if(c===zd||c===Cd||c===Bd){if(0===b)return a;b--}else c===Ad&&b++}a=a.previousSibling}return null}var Ld=Math.random().toString(36).slice(2),Md=\"__reactInternalInstance$\"+Ld,Nd=\"__reactEventHandlers$\"+Ld,Od=\"__reactContainere$\"+Ld;\nfunction tc(a){var b=a[Md];if(b)return b;for(var c=a.parentNode;c;){if(b=c[Od]||c[Md]){c=b.alternate;if(null!==b.child||null!==c&&null!==c.child)for(a=Kd(a);null!==a;){if(c=a[Md])return c;a=Kd(a)}return b}a=c;c=a.parentNode}return null}function Nc(a){a=a[Md]||a[Od];return!a||5!==a.tag&&6!==a.tag&&13!==a.tag&&3!==a.tag?null:a}function Pd(a){if(5===a.tag||6===a.tag)return a.stateNode;throw Error(u(33));}function Qd(a){return a[Nd]||null}\nfunction Rd(a){do a=a.return;while(a&&5!==a.tag);return a?a:null}\nfunction Sd(a,b){var c=a.stateNode;if(!c)return null;var d=la(c);if(!d)return null;c=d[b];a:switch(b){case \"onClick\":case \"onClickCapture\":case \"onDoubleClick\":case \"onDoubleClickCapture\":case \"onMouseDown\":case \"onMouseDownCapture\":case \"onMouseMove\":case \"onMouseMoveCapture\":case \"onMouseUp\":case \"onMouseUpCapture\":case \"onMouseEnter\":(d=!d.disabled)||(a=a.type,d=!(\"button\"===a||\"input\"===a||\"select\"===a||\"textarea\"===a));a=!d;break a;default:a=!1}if(a)return null;if(c&&\"function\"!==typeof c)throw Error(u(231,\nb,typeof c));return c}function Td(a,b,c){if(b=Sd(a,c.dispatchConfig.phasedRegistrationNames[b]))c._dispatchListeners=ic(c._dispatchListeners,b),c._dispatchInstances=ic(c._dispatchInstances,a)}function Ud(a){if(a&&a.dispatchConfig.phasedRegistrationNames){for(var b=a._targetInst,c=[];b;)c.push(b),b=Rd(b);for(b=c.length;0<b--;)Td(c[b],\"captured\",a);for(b=0;b<c.length;b++)Td(c[b],\"bubbled\",a)}}\nfunction Vd(a,b,c){a&&c&&c.dispatchConfig.registrationName&&(b=Sd(a,c.dispatchConfig.registrationName))&&(c._dispatchListeners=ic(c._dispatchListeners,b),c._dispatchInstances=ic(c._dispatchInstances,a))}function Wd(a){a&&a.dispatchConfig.registrationName&&Vd(a._targetInst,null,a)}function Xd(a){jc(a,Ud)}var Yd=null,Zd=null,$d=null;\nfunction ae(){if($d)return $d;var a,b=Zd,c=b.length,d,e=\"value\"in Yd?Yd.value:Yd.textContent,f=e.length;for(a=0;a<c&&b[a]===e[a];a++);var g=c-a;for(d=1;d<=g&&b[c-d]===e[f-d];d++);return $d=e.slice(a,1<d?1-d:void 0)}function be(){return!0}function ce(){return!1}\nfunction G(a,b,c,d){this.dispatchConfig=a;this._targetInst=b;this.nativeEvent=c;a=this.constructor.Interface;for(var e in a)a.hasOwnProperty(e)&&((b=a[e])?this[e]=b(c):\"target\"===e?this.target=d:this[e]=c[e]);this.isDefaultPrevented=(null!=c.defaultPrevented?c.defaultPrevented:!1===c.returnValue)?be:ce;this.isPropagationStopped=ce;return this}\nn(G.prototype,{preventDefault:function(){this.defaultPrevented=!0;var a=this.nativeEvent;a&&(a.preventDefault?a.preventDefault():\"unknown\"!==typeof a.returnValue&&(a.returnValue=!1),this.isDefaultPrevented=be)},stopPropagation:function(){var a=this.nativeEvent;a&&(a.stopPropagation?a.stopPropagation():\"unknown\"!==typeof a.cancelBubble&&(a.cancelBubble=!0),this.isPropagationStopped=be)},persist:function(){this.isPersistent=be},isPersistent:ce,destructor:function(){var a=this.constructor.Interface,\nb;for(b in a)this[b]=null;this.nativeEvent=this._targetInst=this.dispatchConfig=null;this.isPropagationStopped=this.isDefaultPrevented=ce;this._dispatchInstances=this._dispatchListeners=null}});G.Interface={type:null,target:null,currentTarget:function(){return null},eventPhase:null,bubbles:null,cancelable:null,timeStamp:function(a){return a.timeStamp||Date.now()},defaultPrevented:null,isTrusted:null};\nG.extend=function(a){function b(){}function c(){return d.apply(this,arguments)}var d=this;b.prototype=d.prototype;var e=new b;n(e,c.prototype);c.prototype=e;c.prototype.constructor=c;c.Interface=n({},d.Interface,a);c.extend=d.extend;de(c);return c};de(G);function ee(a,b,c,d){if(this.eventPool.length){var e=this.eventPool.pop();this.call(e,a,b,c,d);return e}return new this(a,b,c,d)}\nfunction fe(a){if(!(a instanceof this))throw Error(u(279));a.destructor();10>this.eventPool.length&&this.eventPool.push(a)}function de(a){a.eventPool=[];a.getPooled=ee;a.release=fe}var ge=G.extend({data:null}),he=G.extend({data:null}),ie=[9,13,27,32],je=ya&&\"CompositionEvent\"in window,ke=null;ya&&\"documentMode\"in document&&(ke=document.documentMode);\nvar le=ya&&\"TextEvent\"in window&&!ke,me=ya&&(!je||ke&&8<ke&&11>=ke),ne=String.fromCharCode(32),oe={beforeInput:{phasedRegistrationNames:{bubbled:\"onBeforeInput\",captured:\"onBeforeInputCapture\"},dependencies:[\"compositionend\",\"keypress\",\"textInput\",\"paste\"]},compositionEnd:{phasedRegistrationNames:{bubbled:\"onCompositionEnd\",captured:\"onCompositionEndCapture\"},dependencies:\"blur compositionend keydown keypress keyup mousedown\".split(\" \")},compositionStart:{phasedRegistrationNames:{bubbled:\"onCompositionStart\",\ncaptured:\"onCompositionStartCapture\"},dependencies:\"blur compositionstart keydown keypress keyup mousedown\".split(\" \")},compositionUpdate:{phasedRegistrationNames:{bubbled:\"onCompositionUpdate\",captured:\"onCompositionUpdateCapture\"},dependencies:\"blur compositionupdate keydown keypress keyup mousedown\".split(\" \")}},pe=!1;\nfunction qe(a,b){switch(a){case \"keyup\":return-1!==ie.indexOf(b.keyCode);case \"keydown\":return 229!==b.keyCode;case \"keypress\":case \"mousedown\":case \"blur\":return!0;default:return!1}}function re(a){a=a.detail;return\"object\"===typeof a&&\"data\"in a?a.data:null}var se=!1;function te(a,b){switch(a){case \"compositionend\":return re(b);case \"keypress\":if(32!==b.which)return null;pe=!0;return ne;case \"textInput\":return a=b.data,a===ne&&pe?null:a;default:return null}}\nfunction ue(a,b){if(se)return\"compositionend\"===a||!je&&qe(a,b)?(a=ae(),$d=Zd=Yd=null,se=!1,a):null;switch(a){case \"paste\":return null;case \"keypress\":if(!(b.ctrlKey||b.altKey||b.metaKey)||b.ctrlKey&&b.altKey){if(b.char&&1<b.char.length)return b.char;if(b.which)return String.fromCharCode(b.which)}return null;case \"compositionend\":return me&&\"ko\"!==b.locale?null:b.data;default:return null}}\nvar ve={eventTypes:oe,extractEvents:function(a,b,c,d){var e;if(je)b:{switch(a){case \"compositionstart\":var f=oe.compositionStart;break b;case \"compositionend\":f=oe.compositionEnd;break b;case \"compositionupdate\":f=oe.compositionUpdate;break b}f=void 0}else se?qe(a,c)&&(f=oe.compositionEnd):\"keydown\"===a&&229===c.keyCode&&(f=oe.compositionStart);f?(me&&\"ko\"!==c.locale&&(se||f!==oe.compositionStart?f===oe.compositionEnd&&se&&(e=ae()):(Yd=d,Zd=\"value\"in Yd?Yd.value:Yd.textContent,se=!0)),f=ge.getPooled(f,\nb,c,d),e?f.data=e:(e=re(c),null!==e&&(f.data=e)),Xd(f),e=f):e=null;(a=le?te(a,c):ue(a,c))?(b=he.getPooled(oe.beforeInput,b,c,d),b.data=a,Xd(b)):b=null;return null===e?b:null===b?e:[e,b]}},we={color:!0,date:!0,datetime:!0,\"datetime-local\":!0,email:!0,month:!0,number:!0,password:!0,range:!0,search:!0,tel:!0,text:!0,time:!0,url:!0,week:!0};function xe(a){var b=a&&a.nodeName&&a.nodeName.toLowerCase();return\"input\"===b?!!we[a.type]:\"textarea\"===b?!0:!1}\nvar ye={change:{phasedRegistrationNames:{bubbled:\"onChange\",captured:\"onChangeCapture\"},dependencies:\"blur change click focus input keydown keyup selectionchange\".split(\" \")}};function ze(a,b,c){a=G.getPooled(ye.change,a,b,c);a.type=\"change\";Da(c);Xd(a);return a}var Ae=null,Be=null;function Ce(a){mc(a)}function De(a){var b=Pd(a);if(yb(b))return a}function Ee(a,b){if(\"change\"===a)return b}var Fe=!1;ya&&(Fe=oc(\"input\")&&(!document.documentMode||9<document.documentMode));\nfunction Ge(){Ae&&(Ae.detachEvent(\"onpropertychange\",He),Be=Ae=null)}function He(a){if(\"value\"===a.propertyName&&De(Be))if(a=ze(Be,a,nc(a)),Ja)mc(a);else{Ja=!0;try{Fa(Ce,a)}finally{Ja=!1,La()}}}function Ie(a,b,c){\"focus\"===a?(Ge(),Ae=b,Be=c,Ae.attachEvent(\"onpropertychange\",He)):\"blur\"===a&&Ge()}function Je(a){if(\"selectionchange\"===a||\"keyup\"===a||\"keydown\"===a)return De(Be)}function Ke(a,b){if(\"click\"===a)return De(b)}function Le(a,b){if(\"input\"===a||\"change\"===a)return De(b)}\nvar Me={eventTypes:ye,_isInputEventSupported:Fe,extractEvents:function(a,b,c,d){var e=b?Pd(b):window,f=e.nodeName&&e.nodeName.toLowerCase();if(\"select\"===f||\"input\"===f&&\"file\"===e.type)var g=Ee;else if(xe(e))if(Fe)g=Le;else{g=Je;var h=Ie}else(f=e.nodeName)&&\"input\"===f.toLowerCase()&&(\"checkbox\"===e.type||\"radio\"===e.type)&&(g=Ke);if(g&&(g=g(a,b)))return ze(g,c,d);h&&h(a,e,b);\"blur\"===a&&(a=e._wrapperState)&&a.controlled&&\"number\"===e.type&&Db(e,\"number\",e.value)}},Ne=G.extend({view:null,detail:null}),\nOe={Alt:\"altKey\",Control:\"ctrlKey\",Meta:\"metaKey\",Shift:\"shiftKey\"};function Pe(a){var b=this.nativeEvent;return b.getModifierState?b.getModifierState(a):(a=Oe[a])?!!b[a]:!1}function Qe(){return Pe}\nvar Re=0,Se=0,Te=!1,Ue=!1,Ve=Ne.extend({screenX:null,screenY:null,clientX:null,clientY:null,pageX:null,pageY:null,ctrlKey:null,shiftKey:null,altKey:null,metaKey:null,getModifierState:Qe,button:null,buttons:null,relatedTarget:function(a){return a.relatedTarget||(a.fromElement===a.srcElement?a.toElement:a.fromElement)},movementX:function(a){if(\"movementX\"in a)return a.movementX;var b=Re;Re=a.screenX;return Te?\"mousemove\"===a.type?a.screenX-b:0:(Te=!0,0)},movementY:function(a){if(\"movementY\"in a)return a.movementY;\nvar b=Se;Se=a.screenY;return Ue?\"mousemove\"===a.type?a.screenY-b:0:(Ue=!0,0)}}),We=Ve.extend({pointerId:null,width:null,height:null,pressure:null,tangentialPressure:null,tiltX:null,tiltY:null,twist:null,pointerType:null,isPrimary:null}),Xe={mouseEnter:{registrationName:\"onMouseEnter\",dependencies:[\"mouseout\",\"mouseover\"]},mouseLeave:{registrationName:\"onMouseLeave\",dependencies:[\"mouseout\",\"mouseover\"]},pointerEnter:{registrationName:\"onPointerEnter\",dependencies:[\"pointerout\",\"pointerover\"]},pointerLeave:{registrationName:\"onPointerLeave\",\ndependencies:[\"pointerout\",\"pointerover\"]}},Ye={eventTypes:Xe,extractEvents:function(a,b,c,d,e){var f=\"mouseover\"===a||\"pointerover\"===a,g=\"mouseout\"===a||\"pointerout\"===a;if(f&&0===(e&32)&&(c.relatedTarget||c.fromElement)||!g&&!f)return null;f=d.window===d?d:(f=d.ownerDocument)?f.defaultView||f.parentWindow:window;if(g){if(g=b,b=(b=c.relatedTarget||c.toElement)?tc(b):null,null!==b){var h=dc(b);if(b!==h||5!==b.tag&&6!==b.tag)b=null}}else g=null;if(g===b)return null;if(\"mouseout\"===a||\"mouseover\"===\na){var k=Ve;var l=Xe.mouseLeave;var m=Xe.mouseEnter;var p=\"mouse\"}else if(\"pointerout\"===a||\"pointerover\"===a)k=We,l=Xe.pointerLeave,m=Xe.pointerEnter,p=\"pointer\";a=null==g?f:Pd(g);f=null==b?f:Pd(b);l=k.getPooled(l,g,c,d);l.type=p+\"leave\";l.target=a;l.relatedTarget=f;c=k.getPooled(m,b,c,d);c.type=p+\"enter\";c.target=f;c.relatedTarget=a;d=g;p=b;if(d&&p)a:{k=d;m=p;g=0;for(a=k;a;a=Rd(a))g++;a=0;for(b=m;b;b=Rd(b))a++;for(;0<g-a;)k=Rd(k),g--;for(;0<a-g;)m=Rd(m),a--;for(;g--;){if(k===m||k===m.alternate)break a;\nk=Rd(k);m=Rd(m)}k=null}else k=null;m=k;for(k=[];d&&d!==m;){g=d.alternate;if(null!==g&&g===m)break;k.push(d);d=Rd(d)}for(d=[];p&&p!==m;){g=p.alternate;if(null!==g&&g===m)break;d.push(p);p=Rd(p)}for(p=0;p<k.length;p++)Vd(k[p],\"bubbled\",l);for(p=d.length;0<p--;)Vd(d[p],\"captured\",c);return 0===(e&64)?[l]:[l,c]}};function Ze(a,b){return a===b&&(0!==a||1/a===1/b)||a!==a&&b!==b}var $e=\"function\"===typeof Object.is?Object.is:Ze,af=Object.prototype.hasOwnProperty;\nfunction bf(a,b){if($e(a,b))return!0;if(\"object\"!==typeof a||null===a||\"object\"!==typeof b||null===b)return!1;var c=Object.keys(a),d=Object.keys(b);if(c.length!==d.length)return!1;for(d=0;d<c.length;d++)if(!af.call(b,c[d])||!$e(a[c[d]],b[c[d]]))return!1;return!0}\nvar cf=ya&&\"documentMode\"in document&&11>=document.documentMode,df={select:{phasedRegistrationNames:{bubbled:\"onSelect\",captured:\"onSelectCapture\"},dependencies:\"blur contextmenu dragend focus keydown keyup mousedown mouseup selectionchange\".split(\" \")}},ef=null,ff=null,gf=null,hf=!1;\nfunction jf(a,b){var c=b.window===b?b.document:9===b.nodeType?b:b.ownerDocument;if(hf||null==ef||ef!==td(c))return null;c=ef;\"selectionStart\"in c&&yd(c)?c={start:c.selectionStart,end:c.selectionEnd}:(c=(c.ownerDocument&&c.ownerDocument.defaultView||window).getSelection(),c={anchorNode:c.anchorNode,anchorOffset:c.anchorOffset,focusNode:c.focusNode,focusOffset:c.focusOffset});return gf&&bf(gf,c)?null:(gf=c,a=G.getPooled(df.select,ff,a,b),a.type=\"select\",a.target=ef,Xd(a),a)}\nvar kf={eventTypes:df,extractEvents:function(a,b,c,d,e,f){e=f||(d.window===d?d.document:9===d.nodeType?d:d.ownerDocument);if(!(f=!e)){a:{e=cc(e);f=wa.onSelect;for(var g=0;g<f.length;g++)if(!e.has(f[g])){e=!1;break a}e=!0}f=!e}if(f)return null;e=b?Pd(b):window;switch(a){case \"focus\":if(xe(e)||\"true\"===e.contentEditable)ef=e,ff=b,gf=null;break;case \"blur\":gf=ff=ef=null;break;case \"mousedown\":hf=!0;break;case \"contextmenu\":case \"mouseup\":case \"dragend\":return hf=!1,jf(c,d);case \"selectionchange\":if(cf)break;\ncase \"keydown\":case \"keyup\":return jf(c,d)}return null}},lf=G.extend({animationName:null,elapsedTime:null,pseudoElement:null}),mf=G.extend({clipboardData:function(a){return\"clipboardData\"in a?a.clipboardData:window.clipboardData}}),nf=Ne.extend({relatedTarget:null});function of(a){var b=a.keyCode;\"charCode\"in a?(a=a.charCode,0===a&&13===b&&(a=13)):a=b;10===a&&(a=13);return 32<=a||13===a?a:0}\nvar pf={Esc:\"Escape\",Spacebar:\" \",Left:\"ArrowLeft\",Up:\"ArrowUp\",Right:\"ArrowRight\",Down:\"ArrowDown\",Del:\"Delete\",Win:\"OS\",Menu:\"ContextMenu\",Apps:\"ContextMenu\",Scroll:\"ScrollLock\",MozPrintableKey:\"Unidentified\"},qf={8:\"Backspace\",9:\"Tab\",12:\"Clear\",13:\"Enter\",16:\"Shift\",17:\"Control\",18:\"Alt\",19:\"Pause\",20:\"CapsLock\",27:\"Escape\",32:\" \",33:\"PageUp\",34:\"PageDown\",35:\"End\",36:\"Home\",37:\"ArrowLeft\",38:\"ArrowUp\",39:\"ArrowRight\",40:\"ArrowDown\",45:\"Insert\",46:\"Delete\",112:\"F1\",113:\"F2\",114:\"F3\",115:\"F4\",\n116:\"F5\",117:\"F6\",118:\"F7\",119:\"F8\",120:\"F9\",121:\"F10\",122:\"F11\",123:\"F12\",144:\"NumLock\",145:\"ScrollLock\",224:\"Meta\"},rf=Ne.extend({key:function(a){if(a.key){var b=pf[a.key]||a.key;if(\"Unidentified\"!==b)return b}return\"keypress\"===a.type?(a=of(a),13===a?\"Enter\":String.fromCharCode(a)):\"keydown\"===a.type||\"keyup\"===a.type?qf[a.keyCode]||\"Unidentified\":\"\"},location:null,ctrlKey:null,shiftKey:null,altKey:null,metaKey:null,repeat:null,locale:null,getModifierState:Qe,charCode:function(a){return\"keypress\"===\na.type?of(a):0},keyCode:function(a){return\"keydown\"===a.type||\"keyup\"===a.type?a.keyCode:0},which:function(a){return\"keypress\"===a.type?of(a):\"keydown\"===a.type||\"keyup\"===a.type?a.keyCode:0}}),sf=Ve.extend({dataTransfer:null}),tf=Ne.extend({touches:null,targetTouches:null,changedTouches:null,altKey:null,metaKey:null,ctrlKey:null,shiftKey:null,getModifierState:Qe}),uf=G.extend({propertyName:null,elapsedTime:null,pseudoElement:null}),vf=Ve.extend({deltaX:function(a){return\"deltaX\"in a?a.deltaX:\"wheelDeltaX\"in\na?-a.wheelDeltaX:0},deltaY:function(a){return\"deltaY\"in a?a.deltaY:\"wheelDeltaY\"in a?-a.wheelDeltaY:\"wheelDelta\"in a?-a.wheelDelta:0},deltaZ:null,deltaMode:null}),wf={eventTypes:Wc,extractEvents:function(a,b,c,d){var e=Yc.get(a);if(!e)return null;switch(a){case \"keypress\":if(0===of(c))return null;case \"keydown\":case \"keyup\":a=rf;break;case \"blur\":case \"focus\":a=nf;break;case \"click\":if(2===c.button)return null;case \"auxclick\":case \"dblclick\":case \"mousedown\":case \"mousemove\":case \"mouseup\":case \"mouseout\":case \"mouseover\":case \"contextmenu\":a=\nVe;break;case \"drag\":case \"dragend\":case \"dragenter\":case \"dragexit\":case \"dragleave\":case \"dragover\":case \"dragstart\":case \"drop\":a=sf;break;case \"touchcancel\":case \"touchend\":case \"touchmove\":case \"touchstart\":a=tf;break;case Xb:case Yb:case Zb:a=lf;break;case $b:a=uf;break;case \"scroll\":a=Ne;break;case \"wheel\":a=vf;break;case \"copy\":case \"cut\":case \"paste\":a=mf;break;case \"gotpointercapture\":case \"lostpointercapture\":case \"pointercancel\":case \"pointerdown\":case \"pointermove\":case \"pointerout\":case \"pointerover\":case \"pointerup\":a=\nWe;break;default:a=G}b=a.getPooled(e,b,c,d);Xd(b);return b}};if(pa)throw Error(u(101));pa=Array.prototype.slice.call(\"ResponderEventPlugin SimpleEventPlugin EnterLeaveEventPlugin ChangeEventPlugin SelectEventPlugin BeforeInputEventPlugin\".split(\" \"));ra();var xf=Nc;la=Qd;ma=xf;na=Pd;xa({SimpleEventPlugin:wf,EnterLeaveEventPlugin:Ye,ChangeEventPlugin:Me,SelectEventPlugin:kf,BeforeInputEventPlugin:ve});var yf=[],zf=-1;function H(a){0>zf||(a.current=yf[zf],yf[zf]=null,zf--)}\nfunction I(a,b){zf++;yf[zf]=a.current;a.current=b}var Af={},J={current:Af},K={current:!1},Bf=Af;function Cf(a,b){var c=a.type.contextTypes;if(!c)return Af;var d=a.stateNode;if(d&&d.__reactInternalMemoizedUnmaskedChildContext===b)return d.__reactInternalMemoizedMaskedChildContext;var e={},f;for(f in c)e[f]=b[f];d&&(a=a.stateNode,a.__reactInternalMemoizedUnmaskedChildContext=b,a.__reactInternalMemoizedMaskedChildContext=e);return e}function L(a){a=a.childContextTypes;return null!==a&&void 0!==a}\nfunction Df(){H(K);H(J)}function Ef(a,b,c){if(J.current!==Af)throw Error(u(168));I(J,b);I(K,c)}function Ff(a,b,c){var d=a.stateNode;a=b.childContextTypes;if(\"function\"!==typeof d.getChildContext)return c;d=d.getChildContext();for(var e in d)if(!(e in a))throw Error(u(108,pb(b)||\"Unknown\",e));return n({},c,{},d)}function Gf(a){a=(a=a.stateNode)&&a.__reactInternalMemoizedMergedChildContext||Af;Bf=J.current;I(J,a);I(K,K.current);return!0}\nfunction Hf(a,b,c){var d=a.stateNode;if(!d)throw Error(u(169));c?(a=Ff(a,b,Bf),d.__reactInternalMemoizedMergedChildContext=a,H(K),H(J),I(J,a)):H(K);I(K,c)}\nvar If=r.unstable_runWithPriority,Jf=r.unstable_scheduleCallback,Kf=r.unstable_cancelCallback,Lf=r.unstable_requestPaint,Mf=r.unstable_now,Nf=r.unstable_getCurrentPriorityLevel,Of=r.unstable_ImmediatePriority,Pf=r.unstable_UserBlockingPriority,Qf=r.unstable_NormalPriority,Rf=r.unstable_LowPriority,Sf=r.unstable_IdlePriority,Tf={},Uf=r.unstable_shouldYield,Vf=void 0!==Lf?Lf:function(){},Wf=null,Xf=null,Yf=!1,Zf=Mf(),$f=1E4>Zf?Mf:function(){return Mf()-Zf};\nfunction ag(){switch(Nf()){case Of:return 99;case Pf:return 98;case Qf:return 97;case Rf:return 96;case Sf:return 95;default:throw Error(u(332));}}function bg(a){switch(a){case 99:return Of;case 98:return Pf;case 97:return Qf;case 96:return Rf;case 95:return Sf;default:throw Error(u(332));}}function cg(a,b){a=bg(a);return If(a,b)}function dg(a,b,c){a=bg(a);return Jf(a,b,c)}function eg(a){null===Wf?(Wf=[a],Xf=Jf(Of,fg)):Wf.push(a);return Tf}function gg(){if(null!==Xf){var a=Xf;Xf=null;Kf(a)}fg()}\nfunction fg(){if(!Yf&&null!==Wf){Yf=!0;var a=0;try{var b=Wf;cg(99,function(){for(;a<b.length;a++){var c=b[a];do c=c(!0);while(null!==c)}});Wf=null}catch(c){throw null!==Wf&&(Wf=Wf.slice(a+1)),Jf(Of,gg),c;}finally{Yf=!1}}}function hg(a,b,c){c/=10;return 1073741821-(((1073741821-a+b/10)/c|0)+1)*c}function ig(a,b){if(a&&a.defaultProps){b=n({},b);a=a.defaultProps;for(var c in a)void 0===b[c]&&(b[c]=a[c])}return b}var jg={current:null},kg=null,lg=null,mg=null;function ng(){mg=lg=kg=null}\nfunction og(a){var b=jg.current;H(jg);a.type._context._currentValue=b}function pg(a,b){for(;null!==a;){var c=a.alternate;if(a.childExpirationTime<b)a.childExpirationTime=b,null!==c&&c.childExpirationTime<b&&(c.childExpirationTime=b);else if(null!==c&&c.childExpirationTime<b)c.childExpirationTime=b;else break;a=a.return}}function qg(a,b){kg=a;mg=lg=null;a=a.dependencies;null!==a&&null!==a.firstContext&&(a.expirationTime>=b&&(rg=!0),a.firstContext=null)}\nfunction sg(a,b){if(mg!==a&&!1!==b&&0!==b){if(\"number\"!==typeof b||1073741823===b)mg=a,b=1073741823;b={context:a,observedBits:b,next:null};if(null===lg){if(null===kg)throw Error(u(308));lg=b;kg.dependencies={expirationTime:0,firstContext:b,responders:null}}else lg=lg.next=b}return a._currentValue}var tg=!1;function ug(a){a.updateQueue={baseState:a.memoizedState,baseQueue:null,shared:{pending:null},effects:null}}\nfunction vg(a,b){a=a.updateQueue;b.updateQueue===a&&(b.updateQueue={baseState:a.baseState,baseQueue:a.baseQueue,shared:a.shared,effects:a.effects})}function wg(a,b){a={expirationTime:a,suspenseConfig:b,tag:0,payload:null,callback:null,next:null};return a.next=a}function xg(a,b){a=a.updateQueue;if(null!==a){a=a.shared;var c=a.pending;null===c?b.next=b:(b.next=c.next,c.next=b);a.pending=b}}\nfunction yg(a,b){var c=a.alternate;null!==c&&vg(c,a);a=a.updateQueue;c=a.baseQueue;null===c?(a.baseQueue=b.next=b,b.next=b):(b.next=c.next,c.next=b)}\nfunction zg(a,b,c,d){var e=a.updateQueue;tg=!1;var f=e.baseQueue,g=e.shared.pending;if(null!==g){if(null!==f){var h=f.next;f.next=g.next;g.next=h}f=g;e.shared.pending=null;h=a.alternate;null!==h&&(h=h.updateQueue,null!==h&&(h.baseQueue=g))}if(null!==f){h=f.next;var k=e.baseState,l=0,m=null,p=null,x=null;if(null!==h){var z=h;do{g=z.expirationTime;if(g<d){var ca={expirationTime:z.expirationTime,suspenseConfig:z.suspenseConfig,tag:z.tag,payload:z.payload,callback:z.callback,next:null};null===x?(p=x=\nca,m=k):x=x.next=ca;g>l&&(l=g)}else{null!==x&&(x=x.next={expirationTime:1073741823,suspenseConfig:z.suspenseConfig,tag:z.tag,payload:z.payload,callback:z.callback,next:null});Ag(g,z.suspenseConfig);a:{var D=a,t=z;g=b;ca=c;switch(t.tag){case 1:D=t.payload;if(\"function\"===typeof D){k=D.call(ca,k,g);break a}k=D;break a;case 3:D.effectTag=D.effectTag&-4097|64;case 0:D=t.payload;g=\"function\"===typeof D?D.call(ca,k,g):D;if(null===g||void 0===g)break a;k=n({},k,g);break a;case 2:tg=!0}}null!==z.callback&&\n(a.effectTag|=32,g=e.effects,null===g?e.effects=[z]:g.push(z))}z=z.next;if(null===z||z===h)if(g=e.shared.pending,null===g)break;else z=f.next=g.next,g.next=h,e.baseQueue=f=g,e.shared.pending=null}while(1)}null===x?m=k:x.next=p;e.baseState=m;e.baseQueue=x;Bg(l);a.expirationTime=l;a.memoizedState=k}}\nfunction Cg(a,b,c){a=b.effects;b.effects=null;if(null!==a)for(b=0;b<a.length;b++){var d=a[b],e=d.callback;if(null!==e){d.callback=null;d=e;e=c;if(\"function\"!==typeof d)throw Error(u(191,d));d.call(e)}}}var Dg=Wa.ReactCurrentBatchConfig,Eg=(new aa.Component).refs;function Fg(a,b,c,d){b=a.memoizedState;c=c(d,b);c=null===c||void 0===c?b:n({},b,c);a.memoizedState=c;0===a.expirationTime&&(a.updateQueue.baseState=c)}\nvar Jg={isMounted:function(a){return(a=a._reactInternalFiber)?dc(a)===a:!1},enqueueSetState:function(a,b,c){a=a._reactInternalFiber;var d=Gg(),e=Dg.suspense;d=Hg(d,a,e);e=wg(d,e);e.payload=b;void 0!==c&&null!==c&&(e.callback=c);xg(a,e);Ig(a,d)},enqueueReplaceState:function(a,b,c){a=a._reactInternalFiber;var d=Gg(),e=Dg.suspense;d=Hg(d,a,e);e=wg(d,e);e.tag=1;e.payload=b;void 0!==c&&null!==c&&(e.callback=c);xg(a,e);Ig(a,d)},enqueueForceUpdate:function(a,b){a=a._reactInternalFiber;var c=Gg(),d=Dg.suspense;\nc=Hg(c,a,d);d=wg(c,d);d.tag=2;void 0!==b&&null!==b&&(d.callback=b);xg(a,d);Ig(a,c)}};function Kg(a,b,c,d,e,f,g){a=a.stateNode;return\"function\"===typeof a.shouldComponentUpdate?a.shouldComponentUpdate(d,f,g):b.prototype&&b.prototype.isPureReactComponent?!bf(c,d)||!bf(e,f):!0}\nfunction Lg(a,b,c){var d=!1,e=Af;var f=b.contextType;\"object\"===typeof f&&null!==f?f=sg(f):(e=L(b)?Bf:J.current,d=b.contextTypes,f=(d=null!==d&&void 0!==d)?Cf(a,e):Af);b=new b(c,f);a.memoizedState=null!==b.state&&void 0!==b.state?b.state:null;b.updater=Jg;a.stateNode=b;b._reactInternalFiber=a;d&&(a=a.stateNode,a.__reactInternalMemoizedUnmaskedChildContext=e,a.__reactInternalMemoizedMaskedChildContext=f);return b}\nfunction Mg(a,b,c,d){a=b.state;\"function\"===typeof b.componentWillReceiveProps&&b.componentWillReceiveProps(c,d);\"function\"===typeof b.UNSAFE_componentWillReceiveProps&&b.UNSAFE_componentWillReceiveProps(c,d);b.state!==a&&Jg.enqueueReplaceState(b,b.state,null)}\nfunction Ng(a,b,c,d){var e=a.stateNode;e.props=c;e.state=a.memoizedState;e.refs=Eg;ug(a);var f=b.contextType;\"object\"===typeof f&&null!==f?e.context=sg(f):(f=L(b)?Bf:J.current,e.context=Cf(a,f));zg(a,c,e,d);e.state=a.memoizedState;f=b.getDerivedStateFromProps;\"function\"===typeof f&&(Fg(a,b,f,c),e.state=a.memoizedState);\"function\"===typeof b.getDerivedStateFromProps||\"function\"===typeof e.getSnapshotBeforeUpdate||\"function\"!==typeof e.UNSAFE_componentWillMount&&\"function\"!==typeof e.componentWillMount||\n(b=e.state,\"function\"===typeof e.componentWillMount&&e.componentWillMount(),\"function\"===typeof e.UNSAFE_componentWillMount&&e.UNSAFE_componentWillMount(),b!==e.state&&Jg.enqueueReplaceState(e,e.state,null),zg(a,c,e,d),e.state=a.memoizedState);\"function\"===typeof e.componentDidMount&&(a.effectTag|=4)}var Og=Array.isArray;\nfunction Pg(a,b,c){a=c.ref;if(null!==a&&\"function\"!==typeof a&&\"object\"!==typeof a){if(c._owner){c=c._owner;if(c){if(1!==c.tag)throw Error(u(309));var d=c.stateNode}if(!d)throw Error(u(147,a));var e=\"\"+a;if(null!==b&&null!==b.ref&&\"function\"===typeof b.ref&&b.ref._stringRef===e)return b.ref;b=function(a){var b=d.refs;b===Eg&&(b=d.refs={});null===a?delete b[e]:b[e]=a};b._stringRef=e;return b}if(\"string\"!==typeof a)throw Error(u(284));if(!c._owner)throw Error(u(290,a));}return a}\nfunction Qg(a,b){if(\"textarea\"!==a.type)throw Error(u(31,\"[object Object]\"===Object.prototype.toString.call(b)?\"object with keys {\"+Object.keys(b).join(\", \")+\"}\":b,\"\"));}\nfunction Rg(a){function b(b,c){if(a){var d=b.lastEffect;null!==d?(d.nextEffect=c,b.lastEffect=c):b.firstEffect=b.lastEffect=c;c.nextEffect=null;c.effectTag=8}}function c(c,d){if(!a)return null;for(;null!==d;)b(c,d),d=d.sibling;return null}function d(a,b){for(a=new Map;null!==b;)null!==b.key?a.set(b.key,b):a.set(b.index,b),b=b.sibling;return a}function e(a,b){a=Sg(a,b);a.index=0;a.sibling=null;return a}function f(b,c,d){b.index=d;if(!a)return c;d=b.alternate;if(null!==d)return d=d.index,d<c?(b.effectTag=\n2,c):d;b.effectTag=2;return c}function g(b){a&&null===b.alternate&&(b.effectTag=2);return b}function h(a,b,c,d){if(null===b||6!==b.tag)return b=Tg(c,a.mode,d),b.return=a,b;b=e(b,c);b.return=a;return b}function k(a,b,c,d){if(null!==b&&b.elementType===c.type)return d=e(b,c.props),d.ref=Pg(a,b,c),d.return=a,d;d=Ug(c.type,c.key,c.props,null,a.mode,d);d.ref=Pg(a,b,c);d.return=a;return d}function l(a,b,c,d){if(null===b||4!==b.tag||b.stateNode.containerInfo!==c.containerInfo||b.stateNode.implementation!==\nc.implementation)return b=Vg(c,a.mode,d),b.return=a,b;b=e(b,c.children||[]);b.return=a;return b}function m(a,b,c,d,f){if(null===b||7!==b.tag)return b=Wg(c,a.mode,d,f),b.return=a,b;b=e(b,c);b.return=a;return b}function p(a,b,c){if(\"string\"===typeof b||\"number\"===typeof b)return b=Tg(\"\"+b,a.mode,c),b.return=a,b;if(\"object\"===typeof b&&null!==b){switch(b.$$typeof){case Za:return c=Ug(b.type,b.key,b.props,null,a.mode,c),c.ref=Pg(a,null,b),c.return=a,c;case $a:return b=Vg(b,a.mode,c),b.return=a,b}if(Og(b)||\nnb(b))return b=Wg(b,a.mode,c,null),b.return=a,b;Qg(a,b)}return null}function x(a,b,c,d){var e=null!==b?b.key:null;if(\"string\"===typeof c||\"number\"===typeof c)return null!==e?null:h(a,b,\"\"+c,d);if(\"object\"===typeof c&&null!==c){switch(c.$$typeof){case Za:return c.key===e?c.type===ab?m(a,b,c.props.children,d,e):k(a,b,c,d):null;case $a:return c.key===e?l(a,b,c,d):null}if(Og(c)||nb(c))return null!==e?null:m(a,b,c,d,null);Qg(a,c)}return null}function z(a,b,c,d,e){if(\"string\"===typeof d||\"number\"===typeof d)return a=\na.get(c)||null,h(b,a,\"\"+d,e);if(\"object\"===typeof d&&null!==d){switch(d.$$typeof){case Za:return a=a.get(null===d.key?c:d.key)||null,d.type===ab?m(b,a,d.props.children,e,d.key):k(b,a,d,e);case $a:return a=a.get(null===d.key?c:d.key)||null,l(b,a,d,e)}if(Og(d)||nb(d))return a=a.get(c)||null,m(b,a,d,e,null);Qg(b,d)}return null}function ca(e,g,h,k){for(var l=null,t=null,m=g,y=g=0,A=null;null!==m&&y<h.length;y++){m.index>y?(A=m,m=null):A=m.sibling;var q=x(e,m,h[y],k);if(null===q){null===m&&(m=A);break}a&&\nm&&null===q.alternate&&b(e,m);g=f(q,g,y);null===t?l=q:t.sibling=q;t=q;m=A}if(y===h.length)return c(e,m),l;if(null===m){for(;y<h.length;y++)m=p(e,h[y],k),null!==m&&(g=f(m,g,y),null===t?l=m:t.sibling=m,t=m);return l}for(m=d(e,m);y<h.length;y++)A=z(m,e,y,h[y],k),null!==A&&(a&&null!==A.alternate&&m.delete(null===A.key?y:A.key),g=f(A,g,y),null===t?l=A:t.sibling=A,t=A);a&&m.forEach(function(a){return b(e,a)});return l}function D(e,g,h,l){var k=nb(h);if(\"function\"!==typeof k)throw Error(u(150));h=k.call(h);\nif(null==h)throw Error(u(151));for(var m=k=null,t=g,y=g=0,A=null,q=h.next();null!==t&&!q.done;y++,q=h.next()){t.index>y?(A=t,t=null):A=t.sibling;var D=x(e,t,q.value,l);if(null===D){null===t&&(t=A);break}a&&t&&null===D.alternate&&b(e,t);g=f(D,g,y);null===m?k=D:m.sibling=D;m=D;t=A}if(q.done)return c(e,t),k;if(null===t){for(;!q.done;y++,q=h.next())q=p(e,q.value,l),null!==q&&(g=f(q,g,y),null===m?k=q:m.sibling=q,m=q);return k}for(t=d(e,t);!q.done;y++,q=h.next())q=z(t,e,y,q.value,l),null!==q&&(a&&null!==\nq.alternate&&t.delete(null===q.key?y:q.key),g=f(q,g,y),null===m?k=q:m.sibling=q,m=q);a&&t.forEach(function(a){return b(e,a)});return k}return function(a,d,f,h){var k=\"object\"===typeof f&&null!==f&&f.type===ab&&null===f.key;k&&(f=f.props.children);var l=\"object\"===typeof f&&null!==f;if(l)switch(f.$$typeof){case Za:a:{l=f.key;for(k=d;null!==k;){if(k.key===l){switch(k.tag){case 7:if(f.type===ab){c(a,k.sibling);d=e(k,f.props.children);d.return=a;a=d;break a}break;default:if(k.elementType===f.type){c(a,\nk.sibling);d=e(k,f.props);d.ref=Pg(a,k,f);d.return=a;a=d;break a}}c(a,k);break}else b(a,k);k=k.sibling}f.type===ab?(d=Wg(f.props.children,a.mode,h,f.key),d.return=a,a=d):(h=Ug(f.type,f.key,f.props,null,a.mode,h),h.ref=Pg(a,d,f),h.return=a,a=h)}return g(a);case $a:a:{for(k=f.key;null!==d;){if(d.key===k)if(4===d.tag&&d.stateNode.containerInfo===f.containerInfo&&d.stateNode.implementation===f.implementation){c(a,d.sibling);d=e(d,f.children||[]);d.return=a;a=d;break a}else{c(a,d);break}else b(a,d);d=\nd.sibling}d=Vg(f,a.mode,h);d.return=a;a=d}return g(a)}if(\"string\"===typeof f||\"number\"===typeof f)return f=\"\"+f,null!==d&&6===d.tag?(c(a,d.sibling),d=e(d,f),d.return=a,a=d):(c(a,d),d=Tg(f,a.mode,h),d.return=a,a=d),g(a);if(Og(f))return ca(a,d,f,h);if(nb(f))return D(a,d,f,h);l&&Qg(a,f);if(\"undefined\"===typeof f&&!k)switch(a.tag){case 1:case 0:throw a=a.type,Error(u(152,a.displayName||a.name||\"Component\"));}return c(a,d)}}var Xg=Rg(!0),Yg=Rg(!1),Zg={},$g={current:Zg},ah={current:Zg},bh={current:Zg};\nfunction ch(a){if(a===Zg)throw Error(u(174));return a}function dh(a,b){I(bh,b);I(ah,a);I($g,Zg);a=b.nodeType;switch(a){case 9:case 11:b=(b=b.documentElement)?b.namespaceURI:Ob(null,\"\");break;default:a=8===a?b.parentNode:b,b=a.namespaceURI||null,a=a.tagName,b=Ob(b,a)}H($g);I($g,b)}function eh(){H($g);H(ah);H(bh)}function fh(a){ch(bh.current);var b=ch($g.current);var c=Ob(b,a.type);b!==c&&(I(ah,a),I($g,c))}function gh(a){ah.current===a&&(H($g),H(ah))}var M={current:0};\nfunction hh(a){for(var b=a;null!==b;){if(13===b.tag){var c=b.memoizedState;if(null!==c&&(c=c.dehydrated,null===c||c.data===Bd||c.data===Cd))return b}else if(19===b.tag&&void 0!==b.memoizedProps.revealOrder){if(0!==(b.effectTag&64))return b}else if(null!==b.child){b.child.return=b;b=b.child;continue}if(b===a)break;for(;null===b.sibling;){if(null===b.return||b.return===a)return null;b=b.return}b.sibling.return=b.return;b=b.sibling}return null}function ih(a,b){return{responder:a,props:b}}\nvar jh=Wa.ReactCurrentDispatcher,kh=Wa.ReactCurrentBatchConfig,lh=0,N=null,O=null,P=null,mh=!1;function Q(){throw Error(u(321));}function nh(a,b){if(null===b)return!1;for(var c=0;c<b.length&&c<a.length;c++)if(!$e(a[c],b[c]))return!1;return!0}\nfunction oh(a,b,c,d,e,f){lh=f;N=b;b.memoizedState=null;b.updateQueue=null;b.expirationTime=0;jh.current=null===a||null===a.memoizedState?ph:qh;a=c(d,e);if(b.expirationTime===lh){f=0;do{b.expirationTime=0;if(!(25>f))throw Error(u(301));f+=1;P=O=null;b.updateQueue=null;jh.current=rh;a=c(d,e)}while(b.expirationTime===lh)}jh.current=sh;b=null!==O&&null!==O.next;lh=0;P=O=N=null;mh=!1;if(b)throw Error(u(300));return a}\nfunction th(){var a={memoizedState:null,baseState:null,baseQueue:null,queue:null,next:null};null===P?N.memoizedState=P=a:P=P.next=a;return P}function uh(){if(null===O){var a=N.alternate;a=null!==a?a.memoizedState:null}else a=O.next;var b=null===P?N.memoizedState:P.next;if(null!==b)P=b,O=a;else{if(null===a)throw Error(u(310));O=a;a={memoizedState:O.memoizedState,baseState:O.baseState,baseQueue:O.baseQueue,queue:O.queue,next:null};null===P?N.memoizedState=P=a:P=P.next=a}return P}\nfunction vh(a,b){return\"function\"===typeof b?b(a):b}\nfunction wh(a){var b=uh(),c=b.queue;if(null===c)throw Error(u(311));c.lastRenderedReducer=a;var d=O,e=d.baseQueue,f=c.pending;if(null!==f){if(null!==e){var g=e.next;e.next=f.next;f.next=g}d.baseQueue=e=f;c.pending=null}if(null!==e){e=e.next;d=d.baseState;var h=g=f=null,k=e;do{var l=k.expirationTime;if(l<lh){var m={expirationTime:k.expirationTime,suspenseConfig:k.suspenseConfig,action:k.action,eagerReducer:k.eagerReducer,eagerState:k.eagerState,next:null};null===h?(g=h=m,f=d):h=h.next=m;l>N.expirationTime&&\n(N.expirationTime=l,Bg(l))}else null!==h&&(h=h.next={expirationTime:1073741823,suspenseConfig:k.suspenseConfig,action:k.action,eagerReducer:k.eagerReducer,eagerState:k.eagerState,next:null}),Ag(l,k.suspenseConfig),d=k.eagerReducer===a?k.eagerState:a(d,k.action);k=k.next}while(null!==k&&k!==e);null===h?f=d:h.next=g;$e(d,b.memoizedState)||(rg=!0);b.memoizedState=d;b.baseState=f;b.baseQueue=h;c.lastRenderedState=d}return[b.memoizedState,c.dispatch]}\nfunction xh(a){var b=uh(),c=b.queue;if(null===c)throw Error(u(311));c.lastRenderedReducer=a;var d=c.dispatch,e=c.pending,f=b.memoizedState;if(null!==e){c.pending=null;var g=e=e.next;do f=a(f,g.action),g=g.next;while(g!==e);$e(f,b.memoizedState)||(rg=!0);b.memoizedState=f;null===b.baseQueue&&(b.baseState=f);c.lastRenderedState=f}return[f,d]}\nfunction yh(a){var b=th();\"function\"===typeof a&&(a=a());b.memoizedState=b.baseState=a;a=b.queue={pending:null,dispatch:null,lastRenderedReducer:vh,lastRenderedState:a};a=a.dispatch=zh.bind(null,N,a);return[b.memoizedState,a]}function Ah(a,b,c,d){a={tag:a,create:b,destroy:c,deps:d,next:null};b=N.updateQueue;null===b?(b={lastEffect:null},N.updateQueue=b,b.lastEffect=a.next=a):(c=b.lastEffect,null===c?b.lastEffect=a.next=a:(d=c.next,c.next=a,a.next=d,b.lastEffect=a));return a}\nfunction Bh(){return uh().memoizedState}function Ch(a,b,c,d){var e=th();N.effectTag|=a;e.memoizedState=Ah(1|b,c,void 0,void 0===d?null:d)}function Dh(a,b,c,d){var e=uh();d=void 0===d?null:d;var f=void 0;if(null!==O){var g=O.memoizedState;f=g.destroy;if(null!==d&&nh(d,g.deps)){Ah(b,c,f,d);return}}N.effectTag|=a;e.memoizedState=Ah(1|b,c,f,d)}function Eh(a,b){return Ch(516,4,a,b)}function Fh(a,b){return Dh(516,4,a,b)}function Gh(a,b){return Dh(4,2,a,b)}\nfunction Hh(a,b){if(\"function\"===typeof b)return a=a(),b(a),function(){b(null)};if(null!==b&&void 0!==b)return a=a(),b.current=a,function(){b.current=null}}function Ih(a,b,c){c=null!==c&&void 0!==c?c.concat([a]):null;return Dh(4,2,Hh.bind(null,b,a),c)}function Jh(){}function Kh(a,b){th().memoizedState=[a,void 0===b?null:b];return a}function Lh(a,b){var c=uh();b=void 0===b?null:b;var d=c.memoizedState;if(null!==d&&null!==b&&nh(b,d[1]))return d[0];c.memoizedState=[a,b];return a}\nfunction Mh(a,b){var c=uh();b=void 0===b?null:b;var d=c.memoizedState;if(null!==d&&null!==b&&nh(b,d[1]))return d[0];a=a();c.memoizedState=[a,b];return a}function Nh(a,b,c){var d=ag();cg(98>d?98:d,function(){a(!0)});cg(97<d?97:d,function(){var d=kh.suspense;kh.suspense=void 0===b?null:b;try{a(!1),c()}finally{kh.suspense=d}})}\nfunction zh(a,b,c){var d=Gg(),e=Dg.suspense;d=Hg(d,a,e);e={expirationTime:d,suspenseConfig:e,action:c,eagerReducer:null,eagerState:null,next:null};var f=b.pending;null===f?e.next=e:(e.next=f.next,f.next=e);b.pending=e;f=a.alternate;if(a===N||null!==f&&f===N)mh=!0,e.expirationTime=lh,N.expirationTime=lh;else{if(0===a.expirationTime&&(null===f||0===f.expirationTime)&&(f=b.lastRenderedReducer,null!==f))try{var g=b.lastRenderedState,h=f(g,c);e.eagerReducer=f;e.eagerState=h;if($e(h,g))return}catch(k){}finally{}Ig(a,\nd)}}\nvar sh={readContext:sg,useCallback:Q,useContext:Q,useEffect:Q,useImperativeHandle:Q,useLayoutEffect:Q,useMemo:Q,useReducer:Q,useRef:Q,useState:Q,useDebugValue:Q,useResponder:Q,useDeferredValue:Q,useTransition:Q},ph={readContext:sg,useCallback:Kh,useContext:sg,useEffect:Eh,useImperativeHandle:function(a,b,c){c=null!==c&&void 0!==c?c.concat([a]):null;return Ch(4,2,Hh.bind(null,b,a),c)},useLayoutEffect:function(a,b){return Ch(4,2,a,b)},useMemo:function(a,b){var c=th();b=void 0===b?null:b;a=a();c.memoizedState=[a,\nb];return a},useReducer:function(a,b,c){var d=th();b=void 0!==c?c(b):b;d.memoizedState=d.baseState=b;a=d.queue={pending:null,dispatch:null,lastRenderedReducer:a,lastRenderedState:b};a=a.dispatch=zh.bind(null,N,a);return[d.memoizedState,a]},useRef:function(a){var b=th();a={current:a};return b.memoizedState=a},useState:yh,useDebugValue:Jh,useResponder:ih,useDeferredValue:function(a,b){var c=yh(a),d=c[0],e=c[1];Eh(function(){var c=kh.suspense;kh.suspense=void 0===b?null:b;try{e(a)}finally{kh.suspense=\nc}},[a,b]);return d},useTransition:function(a){var b=yh(!1),c=b[0];b=b[1];return[Kh(Nh.bind(null,b,a),[b,a]),c]}},qh={readContext:sg,useCallback:Lh,useContext:sg,useEffect:Fh,useImperativeHandle:Ih,useLayoutEffect:Gh,useMemo:Mh,useReducer:wh,useRef:Bh,useState:function(){return wh(vh)},useDebugValue:Jh,useResponder:ih,useDeferredValue:function(a,b){var c=wh(vh),d=c[0],e=c[1];Fh(function(){var c=kh.suspense;kh.suspense=void 0===b?null:b;try{e(a)}finally{kh.suspense=c}},[a,b]);return d},useTransition:function(a){var b=\nwh(vh),c=b[0];b=b[1];return[Lh(Nh.bind(null,b,a),[b,a]),c]}},rh={readContext:sg,useCallback:Lh,useContext:sg,useEffect:Fh,useImperativeHandle:Ih,useLayoutEffect:Gh,useMemo:Mh,useReducer:xh,useRef:Bh,useState:function(){return xh(vh)},useDebugValue:Jh,useResponder:ih,useDeferredValue:function(a,b){var c=xh(vh),d=c[0],e=c[1];Fh(function(){var c=kh.suspense;kh.suspense=void 0===b?null:b;try{e(a)}finally{kh.suspense=c}},[a,b]);return d},useTransition:function(a){var b=xh(vh),c=b[0];b=b[1];return[Lh(Nh.bind(null,\nb,a),[b,a]),c]}},Oh=null,Ph=null,Qh=!1;function Rh(a,b){var c=Sh(5,null,null,0);c.elementType=\"DELETED\";c.type=\"DELETED\";c.stateNode=b;c.return=a;c.effectTag=8;null!==a.lastEffect?(a.lastEffect.nextEffect=c,a.lastEffect=c):a.firstEffect=a.lastEffect=c}\nfunction Th(a,b){switch(a.tag){case 5:var c=a.type;b=1!==b.nodeType||c.toLowerCase()!==b.nodeName.toLowerCase()?null:b;return null!==b?(a.stateNode=b,!0):!1;case 6:return b=\"\"===a.pendingProps||3!==b.nodeType?null:b,null!==b?(a.stateNode=b,!0):!1;case 13:return!1;default:return!1}}\nfunction Uh(a){if(Qh){var b=Ph;if(b){var c=b;if(!Th(a,b)){b=Jd(c.nextSibling);if(!b||!Th(a,b)){a.effectTag=a.effectTag&-1025|2;Qh=!1;Oh=a;return}Rh(Oh,c)}Oh=a;Ph=Jd(b.firstChild)}else a.effectTag=a.effectTag&-1025|2,Qh=!1,Oh=a}}function Vh(a){for(a=a.return;null!==a&&5!==a.tag&&3!==a.tag&&13!==a.tag;)a=a.return;Oh=a}\nfunction Wh(a){if(a!==Oh)return!1;if(!Qh)return Vh(a),Qh=!0,!1;var b=a.type;if(5!==a.tag||\"head\"!==b&&\"body\"!==b&&!Gd(b,a.memoizedProps))for(b=Ph;b;)Rh(a,b),b=Jd(b.nextSibling);Vh(a);if(13===a.tag){a=a.memoizedState;a=null!==a?a.dehydrated:null;if(!a)throw Error(u(317));a:{a=a.nextSibling;for(b=0;a;){if(8===a.nodeType){var c=a.data;if(c===Ad){if(0===b){Ph=Jd(a.nextSibling);break a}b--}else c!==zd&&c!==Cd&&c!==Bd||b++}a=a.nextSibling}Ph=null}}else Ph=Oh?Jd(a.stateNode.nextSibling):null;return!0}\nfunction Xh(){Ph=Oh=null;Qh=!1}var Yh=Wa.ReactCurrentOwner,rg=!1;function R(a,b,c,d){b.child=null===a?Yg(b,null,c,d):Xg(b,a.child,c,d)}function Zh(a,b,c,d,e){c=c.render;var f=b.ref;qg(b,e);d=oh(a,b,c,d,f,e);if(null!==a&&!rg)return b.updateQueue=a.updateQueue,b.effectTag&=-517,a.expirationTime<=e&&(a.expirationTime=0),$h(a,b,e);b.effectTag|=1;R(a,b,d,e);return b.child}\nfunction ai(a,b,c,d,e,f){if(null===a){var g=c.type;if(\"function\"===typeof g&&!bi(g)&&void 0===g.defaultProps&&null===c.compare&&void 0===c.defaultProps)return b.tag=15,b.type=g,ci(a,b,g,d,e,f);a=Ug(c.type,null,d,null,b.mode,f);a.ref=b.ref;a.return=b;return b.child=a}g=a.child;if(e<f&&(e=g.memoizedProps,c=c.compare,c=null!==c?c:bf,c(e,d)&&a.ref===b.ref))return $h(a,b,f);b.effectTag|=1;a=Sg(g,d);a.ref=b.ref;a.return=b;return b.child=a}\nfunction ci(a,b,c,d,e,f){return null!==a&&bf(a.memoizedProps,d)&&a.ref===b.ref&&(rg=!1,e<f)?(b.expirationTime=a.expirationTime,$h(a,b,f)):di(a,b,c,d,f)}function ei(a,b){var c=b.ref;if(null===a&&null!==c||null!==a&&a.ref!==c)b.effectTag|=128}function di(a,b,c,d,e){var f=L(c)?Bf:J.current;f=Cf(b,f);qg(b,e);c=oh(a,b,c,d,f,e);if(null!==a&&!rg)return b.updateQueue=a.updateQueue,b.effectTag&=-517,a.expirationTime<=e&&(a.expirationTime=0),$h(a,b,e);b.effectTag|=1;R(a,b,c,e);return b.child}\nfunction fi(a,b,c,d,e){if(L(c)){var f=!0;Gf(b)}else f=!1;qg(b,e);if(null===b.stateNode)null!==a&&(a.alternate=null,b.alternate=null,b.effectTag|=2),Lg(b,c,d),Ng(b,c,d,e),d=!0;else if(null===a){var g=b.stateNode,h=b.memoizedProps;g.props=h;var k=g.context,l=c.contextType;\"object\"===typeof l&&null!==l?l=sg(l):(l=L(c)?Bf:J.current,l=Cf(b,l));var m=c.getDerivedStateFromProps,p=\"function\"===typeof m||\"function\"===typeof g.getSnapshotBeforeUpdate;p||\"function\"!==typeof g.UNSAFE_componentWillReceiveProps&&\n\"function\"!==typeof g.componentWillReceiveProps||(h!==d||k!==l)&&Mg(b,g,d,l);tg=!1;var x=b.memoizedState;g.state=x;zg(b,d,g,e);k=b.memoizedState;h!==d||x!==k||K.current||tg?(\"function\"===typeof m&&(Fg(b,c,m,d),k=b.memoizedState),(h=tg||Kg(b,c,h,d,x,k,l))?(p||\"function\"!==typeof g.UNSAFE_componentWillMount&&\"function\"!==typeof g.componentWillMount||(\"function\"===typeof g.componentWillMount&&g.componentWillMount(),\"function\"===typeof g.UNSAFE_componentWillMount&&g.UNSAFE_componentWillMount()),\"function\"===\ntypeof g.componentDidMount&&(b.effectTag|=4)):(\"function\"===typeof g.componentDidMount&&(b.effectTag|=4),b.memoizedProps=d,b.memoizedState=k),g.props=d,g.state=k,g.context=l,d=h):(\"function\"===typeof g.componentDidMount&&(b.effectTag|=4),d=!1)}else g=b.stateNode,vg(a,b),h=b.memoizedProps,g.props=b.type===b.elementType?h:ig(b.type,h),k=g.context,l=c.contextType,\"object\"===typeof l&&null!==l?l=sg(l):(l=L(c)?Bf:J.current,l=Cf(b,l)),m=c.getDerivedStateFromProps,(p=\"function\"===typeof m||\"function\"===\ntypeof g.getSnapshotBeforeUpdate)||\"function\"!==typeof g.UNSAFE_componentWillReceiveProps&&\"function\"!==typeof g.componentWillReceiveProps||(h!==d||k!==l)&&Mg(b,g,d,l),tg=!1,k=b.memoizedState,g.state=k,zg(b,d,g,e),x=b.memoizedState,h!==d||k!==x||K.current||tg?(\"function\"===typeof m&&(Fg(b,c,m,d),x=b.memoizedState),(m=tg||Kg(b,c,h,d,k,x,l))?(p||\"function\"!==typeof g.UNSAFE_componentWillUpdate&&\"function\"!==typeof g.componentWillUpdate||(\"function\"===typeof g.componentWillUpdate&&g.componentWillUpdate(d,\nx,l),\"function\"===typeof g.UNSAFE_componentWillUpdate&&g.UNSAFE_componentWillUpdate(d,x,l)),\"function\"===typeof g.componentDidUpdate&&(b.effectTag|=4),\"function\"===typeof g.getSnapshotBeforeUpdate&&(b.effectTag|=256)):(\"function\"!==typeof g.componentDidUpdate||h===a.memoizedProps&&k===a.memoizedState||(b.effectTag|=4),\"function\"!==typeof g.getSnapshotBeforeUpdate||h===a.memoizedProps&&k===a.memoizedState||(b.effectTag|=256),b.memoizedProps=d,b.memoizedState=x),g.props=d,g.state=x,g.context=l,d=m):\n(\"function\"!==typeof g.componentDidUpdate||h===a.memoizedProps&&k===a.memoizedState||(b.effectTag|=4),\"function\"!==typeof g.getSnapshotBeforeUpdate||h===a.memoizedProps&&k===a.memoizedState||(b.effectTag|=256),d=!1);return gi(a,b,c,d,f,e)}\nfunction gi(a,b,c,d,e,f){ei(a,b);var g=0!==(b.effectTag&64);if(!d&&!g)return e&&Hf(b,c,!1),$h(a,b,f);d=b.stateNode;Yh.current=b;var h=g&&\"function\"!==typeof c.getDerivedStateFromError?null:d.render();b.effectTag|=1;null!==a&&g?(b.child=Xg(b,a.child,null,f),b.child=Xg(b,null,h,f)):R(a,b,h,f);b.memoizedState=d.state;e&&Hf(b,c,!0);return b.child}function hi(a){var b=a.stateNode;b.pendingContext?Ef(a,b.pendingContext,b.pendingContext!==b.context):b.context&&Ef(a,b.context,!1);dh(a,b.containerInfo)}\nvar ii={dehydrated:null,retryTime:0};\nfunction ji(a,b,c){var d=b.mode,e=b.pendingProps,f=M.current,g=!1,h;(h=0!==(b.effectTag&64))||(h=0!==(f&2)&&(null===a||null!==a.memoizedState));h?(g=!0,b.effectTag&=-65):null!==a&&null===a.memoizedState||void 0===e.fallback||!0===e.unstable_avoidThisFallback||(f|=1);I(M,f&1);if(null===a){void 0!==e.fallback&&Uh(b);if(g){g=e.fallback;e=Wg(null,d,0,null);e.return=b;if(0===(b.mode&2))for(a=null!==b.memoizedState?b.child.child:b.child,e.child=a;null!==a;)a.return=e,a=a.sibling;c=Wg(g,d,c,null);c.return=\nb;e.sibling=c;b.memoizedState=ii;b.child=e;return c}d=e.children;b.memoizedState=null;return b.child=Yg(b,null,d,c)}if(null!==a.memoizedState){a=a.child;d=a.sibling;if(g){e=e.fallback;c=Sg(a,a.pendingProps);c.return=b;if(0===(b.mode&2)&&(g=null!==b.memoizedState?b.child.child:b.child,g!==a.child))for(c.child=g;null!==g;)g.return=c,g=g.sibling;d=Sg(d,e);d.return=b;c.sibling=d;c.childExpirationTime=0;b.memoizedState=ii;b.child=c;return d}c=Xg(b,a.child,e.children,c);b.memoizedState=null;return b.child=\nc}a=a.child;if(g){g=e.fallback;e=Wg(null,d,0,null);e.return=b;e.child=a;null!==a&&(a.return=e);if(0===(b.mode&2))for(a=null!==b.memoizedState?b.child.child:b.child,e.child=a;null!==a;)a.return=e,a=a.sibling;c=Wg(g,d,c,null);c.return=b;e.sibling=c;c.effectTag|=2;e.childExpirationTime=0;b.memoizedState=ii;b.child=e;return c}b.memoizedState=null;return b.child=Xg(b,a,e.children,c)}\nfunction ki(a,b){a.expirationTime<b&&(a.expirationTime=b);var c=a.alternate;null!==c&&c.expirationTime<b&&(c.expirationTime=b);pg(a.return,b)}function li(a,b,c,d,e,f){var g=a.memoizedState;null===g?a.memoizedState={isBackwards:b,rendering:null,renderingStartTime:0,last:d,tail:c,tailExpiration:0,tailMode:e,lastEffect:f}:(g.isBackwards=b,g.rendering=null,g.renderingStartTime=0,g.last=d,g.tail=c,g.tailExpiration=0,g.tailMode=e,g.lastEffect=f)}\nfunction mi(a,b,c){var d=b.pendingProps,e=d.revealOrder,f=d.tail;R(a,b,d.children,c);d=M.current;if(0!==(d&2))d=d&1|2,b.effectTag|=64;else{if(null!==a&&0!==(a.effectTag&64))a:for(a=b.child;null!==a;){if(13===a.tag)null!==a.memoizedState&&ki(a,c);else if(19===a.tag)ki(a,c);else if(null!==a.child){a.child.return=a;a=a.child;continue}if(a===b)break a;for(;null===a.sibling;){if(null===a.return||a.return===b)break a;a=a.return}a.sibling.return=a.return;a=a.sibling}d&=1}I(M,d);if(0===(b.mode&2))b.memoizedState=\nnull;else switch(e){case \"forwards\":c=b.child;for(e=null;null!==c;)a=c.alternate,null!==a&&null===hh(a)&&(e=c),c=c.sibling;c=e;null===c?(e=b.child,b.child=null):(e=c.sibling,c.sibling=null);li(b,!1,e,c,f,b.lastEffect);break;case \"backwards\":c=null;e=b.child;for(b.child=null;null!==e;){a=e.alternate;if(null!==a&&null===hh(a)){b.child=e;break}a=e.sibling;e.sibling=c;c=e;e=a}li(b,!0,c,null,f,b.lastEffect);break;case \"together\":li(b,!1,null,null,void 0,b.lastEffect);break;default:b.memoizedState=null}return b.child}\nfunction $h(a,b,c){null!==a&&(b.dependencies=a.dependencies);var d=b.expirationTime;0!==d&&Bg(d);if(b.childExpirationTime<c)return null;if(null!==a&&b.child!==a.child)throw Error(u(153));if(null!==b.child){a=b.child;c=Sg(a,a.pendingProps);b.child=c;for(c.return=b;null!==a.sibling;)a=a.sibling,c=c.sibling=Sg(a,a.pendingProps),c.return=b;c.sibling=null}return b.child}var ni,oi,pi,qi;\nni=function(a,b){for(var c=b.child;null!==c;){if(5===c.tag||6===c.tag)a.appendChild(c.stateNode);else if(4!==c.tag&&null!==c.child){c.child.return=c;c=c.child;continue}if(c===b)break;for(;null===c.sibling;){if(null===c.return||c.return===b)return;c=c.return}c.sibling.return=c.return;c=c.sibling}};oi=function(){};\npi=function(a,b,c,d,e){var f=a.memoizedProps;if(f!==d){var g=b.stateNode;ch($g.current);a=null;switch(c){case \"input\":f=zb(g,f);d=zb(g,d);a=[];break;case \"option\":f=Gb(g,f);d=Gb(g,d);a=[];break;case \"select\":f=n({},f,{value:void 0});d=n({},d,{value:void 0});a=[];break;case \"textarea\":f=Ib(g,f);d=Ib(g,d);a=[];break;default:\"function\"!==typeof f.onClick&&\"function\"===typeof d.onClick&&(g.onclick=sd)}od(c,d);var h,k;c=null;for(h in f)if(!d.hasOwnProperty(h)&&f.hasOwnProperty(h)&&null!=f[h])if(\"style\"===\nh)for(k in g=f[h],g)g.hasOwnProperty(k)&&(c||(c={}),c[k]=\"\");else\"dangerouslySetInnerHTML\"!==h&&\"children\"!==h&&\"suppressContentEditableWarning\"!==h&&\"suppressHydrationWarning\"!==h&&\"autoFocus\"!==h&&(va.hasOwnProperty(h)?a||(a=[]):(a=a||[]).push(h,null));for(h in d){var l=d[h];g=null!=f?f[h]:void 0;if(d.hasOwnProperty(h)&&l!==g&&(null!=l||null!=g))if(\"style\"===h)if(g){for(k in g)!g.hasOwnProperty(k)||l&&l.hasOwnProperty(k)||(c||(c={}),c[k]=\"\");for(k in l)l.hasOwnProperty(k)&&g[k]!==l[k]&&(c||(c={}),\nc[k]=l[k])}else c||(a||(a=[]),a.push(h,c)),c=l;else\"dangerouslySetInnerHTML\"===h?(l=l?l.__html:void 0,g=g?g.__html:void 0,null!=l&&g!==l&&(a=a||[]).push(h,l)):\"children\"===h?g===l||\"string\"!==typeof l&&\"number\"!==typeof l||(a=a||[]).push(h,\"\"+l):\"suppressContentEditableWarning\"!==h&&\"suppressHydrationWarning\"!==h&&(va.hasOwnProperty(h)?(null!=l&&rd(e,h),a||g===l||(a=[])):(a=a||[]).push(h,l))}c&&(a=a||[]).push(\"style\",c);e=a;if(b.updateQueue=e)b.effectTag|=4}};\nqi=function(a,b,c,d){c!==d&&(b.effectTag|=4)};function ri(a,b){switch(a.tailMode){case \"hidden\":b=a.tail;for(var c=null;null!==b;)null!==b.alternate&&(c=b),b=b.sibling;null===c?a.tail=null:c.sibling=null;break;case \"collapsed\":c=a.tail;for(var d=null;null!==c;)null!==c.alternate&&(d=c),c=c.sibling;null===d?b||null===a.tail?a.tail=null:a.tail.sibling=null:d.sibling=null}}\nfunction si(a,b,c){var d=b.pendingProps;switch(b.tag){case 2:case 16:case 15:case 0:case 11:case 7:case 8:case 12:case 9:case 14:return null;case 1:return L(b.type)&&Df(),null;case 3:return eh(),H(K),H(J),c=b.stateNode,c.pendingContext&&(c.context=c.pendingContext,c.pendingContext=null),null!==a&&null!==a.child||!Wh(b)||(b.effectTag|=4),oi(b),null;case 5:gh(b);c=ch(bh.current);var e=b.type;if(null!==a&&null!=b.stateNode)pi(a,b,e,d,c),a.ref!==b.ref&&(b.effectTag|=128);else{if(!d){if(null===b.stateNode)throw Error(u(166));\nreturn null}a=ch($g.current);if(Wh(b)){d=b.stateNode;e=b.type;var f=b.memoizedProps;d[Md]=b;d[Nd]=f;switch(e){case \"iframe\":case \"object\":case \"embed\":F(\"load\",d);break;case \"video\":case \"audio\":for(a=0;a<ac.length;a++)F(ac[a],d);break;case \"source\":F(\"error\",d);break;case \"img\":case \"image\":case \"link\":F(\"error\",d);F(\"load\",d);break;case \"form\":F(\"reset\",d);F(\"submit\",d);break;case \"details\":F(\"toggle\",d);break;case \"input\":Ab(d,f);F(\"invalid\",d);rd(c,\"onChange\");break;case \"select\":d._wrapperState=\n{wasMultiple:!!f.multiple};F(\"invalid\",d);rd(c,\"onChange\");break;case \"textarea\":Jb(d,f),F(\"invalid\",d),rd(c,\"onChange\")}od(e,f);a=null;for(var g in f)if(f.hasOwnProperty(g)){var h=f[g];\"children\"===g?\"string\"===typeof h?d.textContent!==h&&(a=[\"children\",h]):\"number\"===typeof h&&d.textContent!==\"\"+h&&(a=[\"children\",\"\"+h]):va.hasOwnProperty(g)&&null!=h&&rd(c,g)}switch(e){case \"input\":xb(d);Eb(d,f,!0);break;case \"textarea\":xb(d);Lb(d);break;case \"select\":case \"option\":break;default:\"function\"===typeof f.onClick&&\n(d.onclick=sd)}c=a;b.updateQueue=c;null!==c&&(b.effectTag|=4)}else{g=9===c.nodeType?c:c.ownerDocument;a===qd&&(a=Nb(e));a===qd?\"script\"===e?(a=g.createElement(\"div\"),a.innerHTML=\"<script>\\x3c/script>\",a=a.removeChild(a.firstChild)):\"string\"===typeof d.is?a=g.createElement(e,{is:d.is}):(a=g.createElement(e),\"select\"===e&&(g=a,d.multiple?g.multiple=!0:d.size&&(g.size=d.size))):a=g.createElementNS(a,e);a[Md]=b;a[Nd]=d;ni(a,b,!1,!1);b.stateNode=a;g=pd(e,d);switch(e){case \"iframe\":case \"object\":case \"embed\":F(\"load\",\na);h=d;break;case \"video\":case \"audio\":for(h=0;h<ac.length;h++)F(ac[h],a);h=d;break;case \"source\":F(\"error\",a);h=d;break;case \"img\":case \"image\":case \"link\":F(\"error\",a);F(\"load\",a);h=d;break;case \"form\":F(\"reset\",a);F(\"submit\",a);h=d;break;case \"details\":F(\"toggle\",a);h=d;break;case \"input\":Ab(a,d);h=zb(a,d);F(\"invalid\",a);rd(c,\"onChange\");break;case \"option\":h=Gb(a,d);break;case \"select\":a._wrapperState={wasMultiple:!!d.multiple};h=n({},d,{value:void 0});F(\"invalid\",a);rd(c,\"onChange\");break;case \"textarea\":Jb(a,\nd);h=Ib(a,d);F(\"invalid\",a);rd(c,\"onChange\");break;default:h=d}od(e,h);var k=h;for(f in k)if(k.hasOwnProperty(f)){var l=k[f];\"style\"===f?md(a,l):\"dangerouslySetInnerHTML\"===f?(l=l?l.__html:void 0,null!=l&&Qb(a,l)):\"children\"===f?\"string\"===typeof l?(\"textarea\"!==e||\"\"!==l)&&Rb(a,l):\"number\"===typeof l&&Rb(a,\"\"+l):\"suppressContentEditableWarning\"!==f&&\"suppressHydrationWarning\"!==f&&\"autoFocus\"!==f&&(va.hasOwnProperty(f)?null!=l&&rd(c,f):null!=l&&Xa(a,f,l,g))}switch(e){case \"input\":xb(a);Eb(a,d,!1);\nbreak;case \"textarea\":xb(a);Lb(a);break;case \"option\":null!=d.value&&a.setAttribute(\"value\",\"\"+rb(d.value));break;case \"select\":a.multiple=!!d.multiple;c=d.value;null!=c?Hb(a,!!d.multiple,c,!1):null!=d.defaultValue&&Hb(a,!!d.multiple,d.defaultValue,!0);break;default:\"function\"===typeof h.onClick&&(a.onclick=sd)}Fd(e,d)&&(b.effectTag|=4)}null!==b.ref&&(b.effectTag|=128)}return null;case 6:if(a&&null!=b.stateNode)qi(a,b,a.memoizedProps,d);else{if(\"string\"!==typeof d&&null===b.stateNode)throw Error(u(166));\nc=ch(bh.current);ch($g.current);Wh(b)?(c=b.stateNode,d=b.memoizedProps,c[Md]=b,c.nodeValue!==d&&(b.effectTag|=4)):(c=(9===c.nodeType?c:c.ownerDocument).createTextNode(d),c[Md]=b,b.stateNode=c)}return null;case 13:H(M);d=b.memoizedState;if(0!==(b.effectTag&64))return b.expirationTime=c,b;c=null!==d;d=!1;null===a?void 0!==b.memoizedProps.fallback&&Wh(b):(e=a.memoizedState,d=null!==e,c||null===e||(e=a.child.sibling,null!==e&&(f=b.firstEffect,null!==f?(b.firstEffect=e,e.nextEffect=f):(b.firstEffect=b.lastEffect=\ne,e.nextEffect=null),e.effectTag=8)));if(c&&!d&&0!==(b.mode&2))if(null===a&&!0!==b.memoizedProps.unstable_avoidThisFallback||0!==(M.current&1))S===ti&&(S=ui);else{if(S===ti||S===ui)S=vi;0!==wi&&null!==T&&(xi(T,U),yi(T,wi))}if(c||d)b.effectTag|=4;return null;case 4:return eh(),oi(b),null;case 10:return og(b),null;case 17:return L(b.type)&&Df(),null;case 19:H(M);d=b.memoizedState;if(null===d)return null;e=0!==(b.effectTag&64);f=d.rendering;if(null===f)if(e)ri(d,!1);else{if(S!==ti||null!==a&&0!==(a.effectTag&\n64))for(f=b.child;null!==f;){a=hh(f);if(null!==a){b.effectTag|=64;ri(d,!1);e=a.updateQueue;null!==e&&(b.updateQueue=e,b.effectTag|=4);null===d.lastEffect&&(b.firstEffect=null);b.lastEffect=d.lastEffect;for(d=b.child;null!==d;)e=d,f=c,e.effectTag&=2,e.nextEffect=null,e.firstEffect=null,e.lastEffect=null,a=e.alternate,null===a?(e.childExpirationTime=0,e.expirationTime=f,e.child=null,e.memoizedProps=null,e.memoizedState=null,e.updateQueue=null,e.dependencies=null):(e.childExpirationTime=a.childExpirationTime,\ne.expirationTime=a.expirationTime,e.child=a.child,e.memoizedProps=a.memoizedProps,e.memoizedState=a.memoizedState,e.updateQueue=a.updateQueue,f=a.dependencies,e.dependencies=null===f?null:{expirationTime:f.expirationTime,firstContext:f.firstContext,responders:f.responders}),d=d.sibling;I(M,M.current&1|2);return b.child}f=f.sibling}}else{if(!e)if(a=hh(f),null!==a){if(b.effectTag|=64,e=!0,c=a.updateQueue,null!==c&&(b.updateQueue=c,b.effectTag|=4),ri(d,!0),null===d.tail&&\"hidden\"===d.tailMode&&!f.alternate)return b=\nb.lastEffect=d.lastEffect,null!==b&&(b.nextEffect=null),null}else 2*$f()-d.renderingStartTime>d.tailExpiration&&1<c&&(b.effectTag|=64,e=!0,ri(d,!1),b.expirationTime=b.childExpirationTime=c-1);d.isBackwards?(f.sibling=b.child,b.child=f):(c=d.last,null!==c?c.sibling=f:b.child=f,d.last=f)}return null!==d.tail?(0===d.tailExpiration&&(d.tailExpiration=$f()+500),c=d.tail,d.rendering=c,d.tail=c.sibling,d.lastEffect=b.lastEffect,d.renderingStartTime=$f(),c.sibling=null,b=M.current,I(M,e?b&1|2:b&1),c):null}throw Error(u(156,\nb.tag));}function zi(a){switch(a.tag){case 1:L(a.type)&&Df();var b=a.effectTag;return b&4096?(a.effectTag=b&-4097|64,a):null;case 3:eh();H(K);H(J);b=a.effectTag;if(0!==(b&64))throw Error(u(285));a.effectTag=b&-4097|64;return a;case 5:return gh(a),null;case 13:return H(M),b=a.effectTag,b&4096?(a.effectTag=b&-4097|64,a):null;case 19:return H(M),null;case 4:return eh(),null;case 10:return og(a),null;default:return null}}function Ai(a,b){return{value:a,source:b,stack:qb(b)}}\nvar Bi=\"function\"===typeof WeakSet?WeakSet:Set;function Ci(a,b){var c=b.source,d=b.stack;null===d&&null!==c&&(d=qb(c));null!==c&&pb(c.type);b=b.value;null!==a&&1===a.tag&&pb(a.type);try{console.error(b)}catch(e){setTimeout(function(){throw e;})}}function Di(a,b){try{b.props=a.memoizedProps,b.state=a.memoizedState,b.componentWillUnmount()}catch(c){Ei(a,c)}}function Fi(a){var b=a.ref;if(null!==b)if(\"function\"===typeof b)try{b(null)}catch(c){Ei(a,c)}else b.current=null}\nfunction Gi(a,b){switch(b.tag){case 0:case 11:case 15:case 22:return;case 1:if(b.effectTag&256&&null!==a){var c=a.memoizedProps,d=a.memoizedState;a=b.stateNode;b=a.getSnapshotBeforeUpdate(b.elementType===b.type?c:ig(b.type,c),d);a.__reactInternalSnapshotBeforeUpdate=b}return;case 3:case 5:case 6:case 4:case 17:return}throw Error(u(163));}\nfunction Hi(a,b){b=b.updateQueue;b=null!==b?b.lastEffect:null;if(null!==b){var c=b=b.next;do{if((c.tag&a)===a){var d=c.destroy;c.destroy=void 0;void 0!==d&&d()}c=c.next}while(c!==b)}}function Ii(a,b){b=b.updateQueue;b=null!==b?b.lastEffect:null;if(null!==b){var c=b=b.next;do{if((c.tag&a)===a){var d=c.create;c.destroy=d()}c=c.next}while(c!==b)}}\nfunction Ji(a,b,c){switch(c.tag){case 0:case 11:case 15:case 22:Ii(3,c);return;case 1:a=c.stateNode;if(c.effectTag&4)if(null===b)a.componentDidMount();else{var d=c.elementType===c.type?b.memoizedProps:ig(c.type,b.memoizedProps);a.componentDidUpdate(d,b.memoizedState,a.__reactInternalSnapshotBeforeUpdate)}b=c.updateQueue;null!==b&&Cg(c,b,a);return;case 3:b=c.updateQueue;if(null!==b){a=null;if(null!==c.child)switch(c.child.tag){case 5:a=c.child.stateNode;break;case 1:a=c.child.stateNode}Cg(c,b,a)}return;\ncase 5:a=c.stateNode;null===b&&c.effectTag&4&&Fd(c.type,c.memoizedProps)&&a.focus();return;case 6:return;case 4:return;case 12:return;case 13:null===c.memoizedState&&(c=c.alternate,null!==c&&(c=c.memoizedState,null!==c&&(c=c.dehydrated,null!==c&&Vc(c))));return;case 19:case 17:case 20:case 21:return}throw Error(u(163));}\nfunction Ki(a,b,c){\"function\"===typeof Li&&Li(b);switch(b.tag){case 0:case 11:case 14:case 15:case 22:a=b.updateQueue;if(null!==a&&(a=a.lastEffect,null!==a)){var d=a.next;cg(97<c?97:c,function(){var a=d;do{var c=a.destroy;if(void 0!==c){var g=b;try{c()}catch(h){Ei(g,h)}}a=a.next}while(a!==d)})}break;case 1:Fi(b);c=b.stateNode;\"function\"===typeof c.componentWillUnmount&&Di(b,c);break;case 5:Fi(b);break;case 4:Mi(a,b,c)}}\nfunction Ni(a){var b=a.alternate;a.return=null;a.child=null;a.memoizedState=null;a.updateQueue=null;a.dependencies=null;a.alternate=null;a.firstEffect=null;a.lastEffect=null;a.pendingProps=null;a.memoizedProps=null;a.stateNode=null;null!==b&&Ni(b)}function Oi(a){return 5===a.tag||3===a.tag||4===a.tag}\nfunction Pi(a){a:{for(var b=a.return;null!==b;){if(Oi(b)){var c=b;break a}b=b.return}throw Error(u(160));}b=c.stateNode;switch(c.tag){case 5:var d=!1;break;case 3:b=b.containerInfo;d=!0;break;case 4:b=b.containerInfo;d=!0;break;default:throw Error(u(161));}c.effectTag&16&&(Rb(b,\"\"),c.effectTag&=-17);a:b:for(c=a;;){for(;null===c.sibling;){if(null===c.return||Oi(c.return)){c=null;break a}c=c.return}c.sibling.return=c.return;for(c=c.sibling;5!==c.tag&&6!==c.tag&&18!==c.tag;){if(c.effectTag&2)continue b;\nif(null===c.child||4===c.tag)continue b;else c.child.return=c,c=c.child}if(!(c.effectTag&2)){c=c.stateNode;break a}}d?Qi(a,c,b):Ri(a,c,b)}\nfunction Qi(a,b,c){var d=a.tag,e=5===d||6===d;if(e)a=e?a.stateNode:a.stateNode.instance,b?8===c.nodeType?c.parentNode.insertBefore(a,b):c.insertBefore(a,b):(8===c.nodeType?(b=c.parentNode,b.insertBefore(a,c)):(b=c,b.appendChild(a)),c=c._reactRootContainer,null!==c&&void 0!==c||null!==b.onclick||(b.onclick=sd));else if(4!==d&&(a=a.child,null!==a))for(Qi(a,b,c),a=a.sibling;null!==a;)Qi(a,b,c),a=a.sibling}\nfunction Ri(a,b,c){var d=a.tag,e=5===d||6===d;if(e)a=e?a.stateNode:a.stateNode.instance,b?c.insertBefore(a,b):c.appendChild(a);else if(4!==d&&(a=a.child,null!==a))for(Ri(a,b,c),a=a.sibling;null!==a;)Ri(a,b,c),a=a.sibling}\nfunction Mi(a,b,c){for(var d=b,e=!1,f,g;;){if(!e){e=d.return;a:for(;;){if(null===e)throw Error(u(160));f=e.stateNode;switch(e.tag){case 5:g=!1;break a;case 3:f=f.containerInfo;g=!0;break a;case 4:f=f.containerInfo;g=!0;break a}e=e.return}e=!0}if(5===d.tag||6===d.tag){a:for(var h=a,k=d,l=c,m=k;;)if(Ki(h,m,l),null!==m.child&&4!==m.tag)m.child.return=m,m=m.child;else{if(m===k)break a;for(;null===m.sibling;){if(null===m.return||m.return===k)break a;m=m.return}m.sibling.return=m.return;m=m.sibling}g?(h=\nf,k=d.stateNode,8===h.nodeType?h.parentNode.removeChild(k):h.removeChild(k)):f.removeChild(d.stateNode)}else if(4===d.tag){if(null!==d.child){f=d.stateNode.containerInfo;g=!0;d.child.return=d;d=d.child;continue}}else if(Ki(a,d,c),null!==d.child){d.child.return=d;d=d.child;continue}if(d===b)break;for(;null===d.sibling;){if(null===d.return||d.return===b)return;d=d.return;4===d.tag&&(e=!1)}d.sibling.return=d.return;d=d.sibling}}\nfunction Si(a,b){switch(b.tag){case 0:case 11:case 14:case 15:case 22:Hi(3,b);return;case 1:return;case 5:var c=b.stateNode;if(null!=c){var d=b.memoizedProps,e=null!==a?a.memoizedProps:d;a=b.type;var f=b.updateQueue;b.updateQueue=null;if(null!==f){c[Nd]=d;\"input\"===a&&\"radio\"===d.type&&null!=d.name&&Bb(c,d);pd(a,e);b=pd(a,d);for(e=0;e<f.length;e+=2){var g=f[e],h=f[e+1];\"style\"===g?md(c,h):\"dangerouslySetInnerHTML\"===g?Qb(c,h):\"children\"===g?Rb(c,h):Xa(c,g,h,b)}switch(a){case \"input\":Cb(c,d);break;\ncase \"textarea\":Kb(c,d);break;case \"select\":b=c._wrapperState.wasMultiple,c._wrapperState.wasMultiple=!!d.multiple,a=d.value,null!=a?Hb(c,!!d.multiple,a,!1):b!==!!d.multiple&&(null!=d.defaultValue?Hb(c,!!d.multiple,d.defaultValue,!0):Hb(c,!!d.multiple,d.multiple?[]:\"\",!1))}}}return;case 6:if(null===b.stateNode)throw Error(u(162));b.stateNode.nodeValue=b.memoizedProps;return;case 3:b=b.stateNode;b.hydrate&&(b.hydrate=!1,Vc(b.containerInfo));return;case 12:return;case 13:c=b;null===b.memoizedState?\nd=!1:(d=!0,c=b.child,Ti=$f());if(null!==c)a:for(a=c;;){if(5===a.tag)f=a.stateNode,d?(f=f.style,\"function\"===typeof f.setProperty?f.setProperty(\"display\",\"none\",\"important\"):f.display=\"none\"):(f=a.stateNode,e=a.memoizedProps.style,e=void 0!==e&&null!==e&&e.hasOwnProperty(\"display\")?e.display:null,f.style.display=ld(\"display\",e));else if(6===a.tag)a.stateNode.nodeValue=d?\"\":a.memoizedProps;else if(13===a.tag&&null!==a.memoizedState&&null===a.memoizedState.dehydrated){f=a.child.sibling;f.return=a;a=\nf;continue}else if(null!==a.child){a.child.return=a;a=a.child;continue}if(a===c)break;for(;null===a.sibling;){if(null===a.return||a.return===c)break a;a=a.return}a.sibling.return=a.return;a=a.sibling}Ui(b);return;case 19:Ui(b);return;case 17:return}throw Error(u(163));}function Ui(a){var b=a.updateQueue;if(null!==b){a.updateQueue=null;var c=a.stateNode;null===c&&(c=a.stateNode=new Bi);b.forEach(function(b){var d=Vi.bind(null,a,b);c.has(b)||(c.add(b),b.then(d,d))})}}\nvar Wi=\"function\"===typeof WeakMap?WeakMap:Map;function Xi(a,b,c){c=wg(c,null);c.tag=3;c.payload={element:null};var d=b.value;c.callback=function(){Yi||(Yi=!0,Zi=d);Ci(a,b)};return c}\nfunction $i(a,b,c){c=wg(c,null);c.tag=3;var d=a.type.getDerivedStateFromError;if(\"function\"===typeof d){var e=b.value;c.payload=function(){Ci(a,b);return d(e)}}var f=a.stateNode;null!==f&&\"function\"===typeof f.componentDidCatch&&(c.callback=function(){\"function\"!==typeof d&&(null===aj?aj=new Set([this]):aj.add(this),Ci(a,b));var c=b.stack;this.componentDidCatch(b.value,{componentStack:null!==c?c:\"\"})});return c}\nvar bj=Math.ceil,cj=Wa.ReactCurrentDispatcher,dj=Wa.ReactCurrentOwner,V=0,ej=8,fj=16,gj=32,ti=0,hj=1,ij=2,ui=3,vi=4,jj=5,W=V,T=null,X=null,U=0,S=ti,kj=null,lj=1073741823,mj=1073741823,nj=null,wi=0,oj=!1,Ti=0,pj=500,Y=null,Yi=!1,Zi=null,aj=null,qj=!1,rj=null,sj=90,tj=null,uj=0,vj=null,wj=0;function Gg(){return(W&(fj|gj))!==V?1073741821-($f()/10|0):0!==wj?wj:wj=1073741821-($f()/10|0)}\nfunction Hg(a,b,c){b=b.mode;if(0===(b&2))return 1073741823;var d=ag();if(0===(b&4))return 99===d?1073741823:1073741822;if((W&fj)!==V)return U;if(null!==c)a=hg(a,c.timeoutMs|0||5E3,250);else switch(d){case 99:a=1073741823;break;case 98:a=hg(a,150,100);break;case 97:case 96:a=hg(a,5E3,250);break;case 95:a=2;break;default:throw Error(u(326));}null!==T&&a===U&&--a;return a}\nfunction Ig(a,b){if(50<uj)throw uj=0,vj=null,Error(u(185));a=xj(a,b);if(null!==a){var c=ag();1073741823===b?(W&ej)!==V&&(W&(fj|gj))===V?yj(a):(Z(a),W===V&&gg()):Z(a);(W&4)===V||98!==c&&99!==c||(null===tj?tj=new Map([[a,b]]):(c=tj.get(a),(void 0===c||c>b)&&tj.set(a,b)))}}\nfunction xj(a,b){a.expirationTime<b&&(a.expirationTime=b);var c=a.alternate;null!==c&&c.expirationTime<b&&(c.expirationTime=b);var d=a.return,e=null;if(null===d&&3===a.tag)e=a.stateNode;else for(;null!==d;){c=d.alternate;d.childExpirationTime<b&&(d.childExpirationTime=b);null!==c&&c.childExpirationTime<b&&(c.childExpirationTime=b);if(null===d.return&&3===d.tag){e=d.stateNode;break}d=d.return}null!==e&&(T===e&&(Bg(b),S===vi&&xi(e,U)),yi(e,b));return e}\nfunction zj(a){var b=a.lastExpiredTime;if(0!==b)return b;b=a.firstPendingTime;if(!Aj(a,b))return b;var c=a.lastPingedTime;a=a.nextKnownPendingLevel;a=c>a?c:a;return 2>=a&&b!==a?0:a}\nfunction Z(a){if(0!==a.lastExpiredTime)a.callbackExpirationTime=1073741823,a.callbackPriority=99,a.callbackNode=eg(yj.bind(null,a));else{var b=zj(a),c=a.callbackNode;if(0===b)null!==c&&(a.callbackNode=null,a.callbackExpirationTime=0,a.callbackPriority=90);else{var d=Gg();1073741823===b?d=99:1===b||2===b?d=95:(d=10*(1073741821-b)-10*(1073741821-d),d=0>=d?99:250>=d?98:5250>=d?97:95);if(null!==c){var e=a.callbackPriority;if(a.callbackExpirationTime===b&&e>=d)return;c!==Tf&&Kf(c)}a.callbackExpirationTime=\nb;a.callbackPriority=d;b=1073741823===b?eg(yj.bind(null,a)):dg(d,Bj.bind(null,a),{timeout:10*(1073741821-b)-$f()});a.callbackNode=b}}}\nfunction Bj(a,b){wj=0;if(b)return b=Gg(),Cj(a,b),Z(a),null;var c=zj(a);if(0!==c){b=a.callbackNode;if((W&(fj|gj))!==V)throw Error(u(327));Dj();a===T&&c===U||Ej(a,c);if(null!==X){var d=W;W|=fj;var e=Fj();do try{Gj();break}catch(h){Hj(a,h)}while(1);ng();W=d;cj.current=e;if(S===hj)throw b=kj,Ej(a,c),xi(a,c),Z(a),b;if(null===X)switch(e=a.finishedWork=a.current.alternate,a.finishedExpirationTime=c,d=S,T=null,d){case ti:case hj:throw Error(u(345));case ij:Cj(a,2<c?2:c);break;case ui:xi(a,c);d=a.lastSuspendedTime;\nc===d&&(a.nextKnownPendingLevel=Ij(e));if(1073741823===lj&&(e=Ti+pj-$f(),10<e)){if(oj){var f=a.lastPingedTime;if(0===f||f>=c){a.lastPingedTime=c;Ej(a,c);break}}f=zj(a);if(0!==f&&f!==c)break;if(0!==d&&d!==c){a.lastPingedTime=d;break}a.timeoutHandle=Hd(Jj.bind(null,a),e);break}Jj(a);break;case vi:xi(a,c);d=a.lastSuspendedTime;c===d&&(a.nextKnownPendingLevel=Ij(e));if(oj&&(e=a.lastPingedTime,0===e||e>=c)){a.lastPingedTime=c;Ej(a,c);break}e=zj(a);if(0!==e&&e!==c)break;if(0!==d&&d!==c){a.lastPingedTime=\nd;break}1073741823!==mj?d=10*(1073741821-mj)-$f():1073741823===lj?d=0:(d=10*(1073741821-lj)-5E3,e=$f(),c=10*(1073741821-c)-e,d=e-d,0>d&&(d=0),d=(120>d?120:480>d?480:1080>d?1080:1920>d?1920:3E3>d?3E3:4320>d?4320:1960*bj(d/1960))-d,c<d&&(d=c));if(10<d){a.timeoutHandle=Hd(Jj.bind(null,a),d);break}Jj(a);break;case jj:if(1073741823!==lj&&null!==nj){f=lj;var g=nj;d=g.busyMinDurationMs|0;0>=d?d=0:(e=g.busyDelayMs|0,f=$f()-(10*(1073741821-f)-(g.timeoutMs|0||5E3)),d=f<=e?0:e+d-f);if(10<d){xi(a,c);a.timeoutHandle=\nHd(Jj.bind(null,a),d);break}}Jj(a);break;default:throw Error(u(329));}Z(a);if(a.callbackNode===b)return Bj.bind(null,a)}}return null}\nfunction yj(a){var b=a.lastExpiredTime;b=0!==b?b:1073741823;if((W&(fj|gj))!==V)throw Error(u(327));Dj();a===T&&b===U||Ej(a,b);if(null!==X){var c=W;W|=fj;var d=Fj();do try{Kj();break}catch(e){Hj(a,e)}while(1);ng();W=c;cj.current=d;if(S===hj)throw c=kj,Ej(a,b),xi(a,b),Z(a),c;if(null!==X)throw Error(u(261));a.finishedWork=a.current.alternate;a.finishedExpirationTime=b;T=null;Jj(a);Z(a)}return null}function Lj(){if(null!==tj){var a=tj;tj=null;a.forEach(function(a,c){Cj(c,a);Z(c)});gg()}}\nfunction Mj(a,b){var c=W;W|=1;try{return a(b)}finally{W=c,W===V&&gg()}}function Nj(a,b){var c=W;W&=-2;W|=ej;try{return a(b)}finally{W=c,W===V&&gg()}}\nfunction Ej(a,b){a.finishedWork=null;a.finishedExpirationTime=0;var c=a.timeoutHandle;-1!==c&&(a.timeoutHandle=-1,Id(c));if(null!==X)for(c=X.return;null!==c;){var d=c;switch(d.tag){case 1:d=d.type.childContextTypes;null!==d&&void 0!==d&&Df();break;case 3:eh();H(K);H(J);break;case 5:gh(d);break;case 4:eh();break;case 13:H(M);break;case 19:H(M);break;case 10:og(d)}c=c.return}T=a;X=Sg(a.current,null);U=b;S=ti;kj=null;mj=lj=1073741823;nj=null;wi=0;oj=!1}\nfunction Hj(a,b){do{try{ng();jh.current=sh;if(mh)for(var c=N.memoizedState;null!==c;){var d=c.queue;null!==d&&(d.pending=null);c=c.next}lh=0;P=O=N=null;mh=!1;if(null===X||null===X.return)return S=hj,kj=b,X=null;a:{var e=a,f=X.return,g=X,h=b;b=U;g.effectTag|=2048;g.firstEffect=g.lastEffect=null;if(null!==h&&\"object\"===typeof h&&\"function\"===typeof h.then){var k=h;if(0===(g.mode&2)){var l=g.alternate;l?(g.updateQueue=l.updateQueue,g.memoizedState=l.memoizedState,g.expirationTime=l.expirationTime):(g.updateQueue=\nnull,g.memoizedState=null)}var m=0!==(M.current&1),p=f;do{var x;if(x=13===p.tag){var z=p.memoizedState;if(null!==z)x=null!==z.dehydrated?!0:!1;else{var ca=p.memoizedProps;x=void 0===ca.fallback?!1:!0!==ca.unstable_avoidThisFallback?!0:m?!1:!0}}if(x){var D=p.updateQueue;if(null===D){var t=new Set;t.add(k);p.updateQueue=t}else D.add(k);if(0===(p.mode&2)){p.effectTag|=64;g.effectTag&=-2981;if(1===g.tag)if(null===g.alternate)g.tag=17;else{var y=wg(1073741823,null);y.tag=2;xg(g,y)}g.expirationTime=1073741823;\nbreak a}h=void 0;g=b;var A=e.pingCache;null===A?(A=e.pingCache=new Wi,h=new Set,A.set(k,h)):(h=A.get(k),void 0===h&&(h=new Set,A.set(k,h)));if(!h.has(g)){h.add(g);var q=Oj.bind(null,e,k,g);k.then(q,q)}p.effectTag|=4096;p.expirationTime=b;break a}p=p.return}while(null!==p);h=Error((pb(g.type)||\"A React component\")+\" suspended while rendering, but no fallback UI was specified.\\n\\nAdd a <Suspense fallback=...> component higher in the tree to provide a loading indicator or placeholder to display.\"+qb(g))}S!==\njj&&(S=ij);h=Ai(h,g);p=f;do{switch(p.tag){case 3:k=h;p.effectTag|=4096;p.expirationTime=b;var B=Xi(p,k,b);yg(p,B);break a;case 1:k=h;var w=p.type,ub=p.stateNode;if(0===(p.effectTag&64)&&(\"function\"===typeof w.getDerivedStateFromError||null!==ub&&\"function\"===typeof ub.componentDidCatch&&(null===aj||!aj.has(ub)))){p.effectTag|=4096;p.expirationTime=b;var vb=$i(p,k,b);yg(p,vb);break a}}p=p.return}while(null!==p)}X=Pj(X)}catch(Xc){b=Xc;continue}break}while(1)}\nfunction Fj(){var a=cj.current;cj.current=sh;return null===a?sh:a}function Ag(a,b){a<lj&&2<a&&(lj=a);null!==b&&a<mj&&2<a&&(mj=a,nj=b)}function Bg(a){a>wi&&(wi=a)}function Kj(){for(;null!==X;)X=Qj(X)}function Gj(){for(;null!==X&&!Uf();)X=Qj(X)}function Qj(a){var b=Rj(a.alternate,a,U);a.memoizedProps=a.pendingProps;null===b&&(b=Pj(a));dj.current=null;return b}\nfunction Pj(a){X=a;do{var b=X.alternate;a=X.return;if(0===(X.effectTag&2048)){b=si(b,X,U);if(1===U||1!==X.childExpirationTime){for(var c=0,d=X.child;null!==d;){var e=d.expirationTime,f=d.childExpirationTime;e>c&&(c=e);f>c&&(c=f);d=d.sibling}X.childExpirationTime=c}if(null!==b)return b;null!==a&&0===(a.effectTag&2048)&&(null===a.firstEffect&&(a.firstEffect=X.firstEffect),null!==X.lastEffect&&(null!==a.lastEffect&&(a.lastEffect.nextEffect=X.firstEffect),a.lastEffect=X.lastEffect),1<X.effectTag&&(null!==\na.lastEffect?a.lastEffect.nextEffect=X:a.firstEffect=X,a.lastEffect=X))}else{b=zi(X);if(null!==b)return b.effectTag&=2047,b;null!==a&&(a.firstEffect=a.lastEffect=null,a.effectTag|=2048)}b=X.sibling;if(null!==b)return b;X=a}while(null!==X);S===ti&&(S=jj);return null}function Ij(a){var b=a.expirationTime;a=a.childExpirationTime;return b>a?b:a}function Jj(a){var b=ag();cg(99,Sj.bind(null,a,b));return null}\nfunction Sj(a,b){do Dj();while(null!==rj);if((W&(fj|gj))!==V)throw Error(u(327));var c=a.finishedWork,d=a.finishedExpirationTime;if(null===c)return null;a.finishedWork=null;a.finishedExpirationTime=0;if(c===a.current)throw Error(u(177));a.callbackNode=null;a.callbackExpirationTime=0;a.callbackPriority=90;a.nextKnownPendingLevel=0;var e=Ij(c);a.firstPendingTime=e;d<=a.lastSuspendedTime?a.firstSuspendedTime=a.lastSuspendedTime=a.nextKnownPendingLevel=0:d<=a.firstSuspendedTime&&(a.firstSuspendedTime=\nd-1);d<=a.lastPingedTime&&(a.lastPingedTime=0);d<=a.lastExpiredTime&&(a.lastExpiredTime=0);a===T&&(X=T=null,U=0);1<c.effectTag?null!==c.lastEffect?(c.lastEffect.nextEffect=c,e=c.firstEffect):e=c:e=c.firstEffect;if(null!==e){var f=W;W|=gj;dj.current=null;Dd=fd;var g=xd();if(yd(g)){if(\"selectionStart\"in g)var h={start:g.selectionStart,end:g.selectionEnd};else a:{h=(h=g.ownerDocument)&&h.defaultView||window;var k=h.getSelection&&h.getSelection();if(k&&0!==k.rangeCount){h=k.anchorNode;var l=k.anchorOffset,\nm=k.focusNode;k=k.focusOffset;try{h.nodeType,m.nodeType}catch(wb){h=null;break a}var p=0,x=-1,z=-1,ca=0,D=0,t=g,y=null;b:for(;;){for(var A;;){t!==h||0!==l&&3!==t.nodeType||(x=p+l);t!==m||0!==k&&3!==t.nodeType||(z=p+k);3===t.nodeType&&(p+=t.nodeValue.length);if(null===(A=t.firstChild))break;y=t;t=A}for(;;){if(t===g)break b;y===h&&++ca===l&&(x=p);y===m&&++D===k&&(z=p);if(null!==(A=t.nextSibling))break;t=y;y=t.parentNode}t=A}h=-1===x||-1===z?null:{start:x,end:z}}else h=null}h=h||{start:0,end:0}}else h=\nnull;Ed={activeElementDetached:null,focusedElem:g,selectionRange:h};fd=!1;Y=e;do try{Tj()}catch(wb){if(null===Y)throw Error(u(330));Ei(Y,wb);Y=Y.nextEffect}while(null!==Y);Y=e;do try{for(g=a,h=b;null!==Y;){var q=Y.effectTag;q&16&&Rb(Y.stateNode,\"\");if(q&128){var B=Y.alternate;if(null!==B){var w=B.ref;null!==w&&(\"function\"===typeof w?w(null):w.current=null)}}switch(q&1038){case 2:Pi(Y);Y.effectTag&=-3;break;case 6:Pi(Y);Y.effectTag&=-3;Si(Y.alternate,Y);break;case 1024:Y.effectTag&=-1025;break;case 1028:Y.effectTag&=\n-1025;Si(Y.alternate,Y);break;case 4:Si(Y.alternate,Y);break;case 8:l=Y,Mi(g,l,h),Ni(l)}Y=Y.nextEffect}}catch(wb){if(null===Y)throw Error(u(330));Ei(Y,wb);Y=Y.nextEffect}while(null!==Y);w=Ed;B=xd();q=w.focusedElem;h=w.selectionRange;if(B!==q&&q&&q.ownerDocument&&wd(q.ownerDocument.documentElement,q)){null!==h&&yd(q)&&(B=h.start,w=h.end,void 0===w&&(w=B),\"selectionStart\"in q?(q.selectionStart=B,q.selectionEnd=Math.min(w,q.value.length)):(w=(B=q.ownerDocument||document)&&B.defaultView||window,w.getSelection&&\n(w=w.getSelection(),l=q.textContent.length,g=Math.min(h.start,l),h=void 0===h.end?g:Math.min(h.end,l),!w.extend&&g>h&&(l=h,h=g,g=l),l=vd(q,g),m=vd(q,h),l&&m&&(1!==w.rangeCount||w.anchorNode!==l.node||w.anchorOffset!==l.offset||w.focusNode!==m.node||w.focusOffset!==m.offset)&&(B=B.createRange(),B.setStart(l.node,l.offset),w.removeAllRanges(),g>h?(w.addRange(B),w.extend(m.node,m.offset)):(B.setEnd(m.node,m.offset),w.addRange(B))))));B=[];for(w=q;w=w.parentNode;)1===w.nodeType&&B.push({element:w,left:w.scrollLeft,\ntop:w.scrollTop});\"function\"===typeof q.focus&&q.focus();for(q=0;q<B.length;q++)w=B[q],w.element.scrollLeft=w.left,w.element.scrollTop=w.top}fd=!!Dd;Ed=Dd=null;a.current=c;Y=e;do try{for(q=a;null!==Y;){var ub=Y.effectTag;ub&36&&Ji(q,Y.alternate,Y);if(ub&128){B=void 0;var vb=Y.ref;if(null!==vb){var Xc=Y.stateNode;switch(Y.tag){case 5:B=Xc;break;default:B=Xc}\"function\"===typeof vb?vb(B):vb.current=B}}Y=Y.nextEffect}}catch(wb){if(null===Y)throw Error(u(330));Ei(Y,wb);Y=Y.nextEffect}while(null!==Y);Y=\nnull;Vf();W=f}else a.current=c;if(qj)qj=!1,rj=a,sj=b;else for(Y=e;null!==Y;)b=Y.nextEffect,Y.nextEffect=null,Y=b;b=a.firstPendingTime;0===b&&(aj=null);1073741823===b?a===vj?uj++:(uj=0,vj=a):uj=0;\"function\"===typeof Uj&&Uj(c.stateNode,d);Z(a);if(Yi)throw Yi=!1,a=Zi,Zi=null,a;if((W&ej)!==V)return null;gg();return null}function Tj(){for(;null!==Y;){var a=Y.effectTag;0!==(a&256)&&Gi(Y.alternate,Y);0===(a&512)||qj||(qj=!0,dg(97,function(){Dj();return null}));Y=Y.nextEffect}}\nfunction Dj(){if(90!==sj){var a=97<sj?97:sj;sj=90;return cg(a,Vj)}}function Vj(){if(null===rj)return!1;var a=rj;rj=null;if((W&(fj|gj))!==V)throw Error(u(331));var b=W;W|=gj;for(a=a.current.firstEffect;null!==a;){try{var c=a;if(0!==(c.effectTag&512))switch(c.tag){case 0:case 11:case 15:case 22:Hi(5,c),Ii(5,c)}}catch(d){if(null===a)throw Error(u(330));Ei(a,d)}c=a.nextEffect;a.nextEffect=null;a=c}W=b;gg();return!0}\nfunction Wj(a,b,c){b=Ai(c,b);b=Xi(a,b,1073741823);xg(a,b);a=xj(a,1073741823);null!==a&&Z(a)}function Ei(a,b){if(3===a.tag)Wj(a,a,b);else for(var c=a.return;null!==c;){if(3===c.tag){Wj(c,a,b);break}else if(1===c.tag){var d=c.stateNode;if(\"function\"===typeof c.type.getDerivedStateFromError||\"function\"===typeof d.componentDidCatch&&(null===aj||!aj.has(d))){a=Ai(b,a);a=$i(c,a,1073741823);xg(c,a);c=xj(c,1073741823);null!==c&&Z(c);break}}c=c.return}}\nfunction Oj(a,b,c){var d=a.pingCache;null!==d&&d.delete(b);T===a&&U===c?S===vi||S===ui&&1073741823===lj&&$f()-Ti<pj?Ej(a,U):oj=!0:Aj(a,c)&&(b=a.lastPingedTime,0!==b&&b<c||(a.lastPingedTime=c,Z(a)))}function Vi(a,b){var c=a.stateNode;null!==c&&c.delete(b);b=0;0===b&&(b=Gg(),b=Hg(b,a,null));a=xj(a,b);null!==a&&Z(a)}var Rj;\nRj=function(a,b,c){var d=b.expirationTime;if(null!==a){var e=b.pendingProps;if(a.memoizedProps!==e||K.current)rg=!0;else{if(d<c){rg=!1;switch(b.tag){case 3:hi(b);Xh();break;case 5:fh(b);if(b.mode&4&&1!==c&&e.hidden)return b.expirationTime=b.childExpirationTime=1,null;break;case 1:L(b.type)&&Gf(b);break;case 4:dh(b,b.stateNode.containerInfo);break;case 10:d=b.memoizedProps.value;e=b.type._context;I(jg,e._currentValue);e._currentValue=d;break;case 13:if(null!==b.memoizedState){d=b.child.childExpirationTime;\nif(0!==d&&d>=c)return ji(a,b,c);I(M,M.current&1);b=$h(a,b,c);return null!==b?b.sibling:null}I(M,M.current&1);break;case 19:d=b.childExpirationTime>=c;if(0!==(a.effectTag&64)){if(d)return mi(a,b,c);b.effectTag|=64}e=b.memoizedState;null!==e&&(e.rendering=null,e.tail=null);I(M,M.current);if(!d)return null}return $h(a,b,c)}rg=!1}}else rg=!1;b.expirationTime=0;switch(b.tag){case 2:d=b.type;null!==a&&(a.alternate=null,b.alternate=null,b.effectTag|=2);a=b.pendingProps;e=Cf(b,J.current);qg(b,c);e=oh(null,\nb,d,a,e,c);b.effectTag|=1;if(\"object\"===typeof e&&null!==e&&\"function\"===typeof e.render&&void 0===e.$$typeof){b.tag=1;b.memoizedState=null;b.updateQueue=null;if(L(d)){var f=!0;Gf(b)}else f=!1;b.memoizedState=null!==e.state&&void 0!==e.state?e.state:null;ug(b);var g=d.getDerivedStateFromProps;\"function\"===typeof g&&Fg(b,d,g,a);e.updater=Jg;b.stateNode=e;e._reactInternalFiber=b;Ng(b,d,a,c);b=gi(null,b,d,!0,f,c)}else b.tag=0,R(null,b,e,c),b=b.child;return b;case 16:a:{e=b.elementType;null!==a&&(a.alternate=\nnull,b.alternate=null,b.effectTag|=2);a=b.pendingProps;ob(e);if(1!==e._status)throw e._result;e=e._result;b.type=e;f=b.tag=Xj(e);a=ig(e,a);switch(f){case 0:b=di(null,b,e,a,c);break a;case 1:b=fi(null,b,e,a,c);break a;case 11:b=Zh(null,b,e,a,c);break a;case 14:b=ai(null,b,e,ig(e.type,a),d,c);break a}throw Error(u(306,e,\"\"));}return b;case 0:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ig(d,e),di(a,b,d,e,c);case 1:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ig(d,e),fi(a,b,d,e,c);\ncase 3:hi(b);d=b.updateQueue;if(null===a||null===d)throw Error(u(282));d=b.pendingProps;e=b.memoizedState;e=null!==e?e.element:null;vg(a,b);zg(b,d,null,c);d=b.memoizedState.element;if(d===e)Xh(),b=$h(a,b,c);else{if(e=b.stateNode.hydrate)Ph=Jd(b.stateNode.containerInfo.firstChild),Oh=b,e=Qh=!0;if(e)for(c=Yg(b,null,d,c),b.child=c;c;)c.effectTag=c.effectTag&-3|1024,c=c.sibling;else R(a,b,d,c),Xh();b=b.child}return b;case 5:return fh(b),null===a&&Uh(b),d=b.type,e=b.pendingProps,f=null!==a?a.memoizedProps:\nnull,g=e.children,Gd(d,e)?g=null:null!==f&&Gd(d,f)&&(b.effectTag|=16),ei(a,b),b.mode&4&&1!==c&&e.hidden?(b.expirationTime=b.childExpirationTime=1,b=null):(R(a,b,g,c),b=b.child),b;case 6:return null===a&&Uh(b),null;case 13:return ji(a,b,c);case 4:return dh(b,b.stateNode.containerInfo),d=b.pendingProps,null===a?b.child=Xg(b,null,d,c):R(a,b,d,c),b.child;case 11:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ig(d,e),Zh(a,b,d,e,c);case 7:return R(a,b,b.pendingProps,c),b.child;case 8:return R(a,\nb,b.pendingProps.children,c),b.child;case 12:return R(a,b,b.pendingProps.children,c),b.child;case 10:a:{d=b.type._context;e=b.pendingProps;g=b.memoizedProps;f=e.value;var h=b.type._context;I(jg,h._currentValue);h._currentValue=f;if(null!==g)if(h=g.value,f=$e(h,f)?0:(\"function\"===typeof d._calculateChangedBits?d._calculateChangedBits(h,f):1073741823)|0,0===f){if(g.children===e.children&&!K.current){b=$h(a,b,c);break a}}else for(h=b.child,null!==h&&(h.return=b);null!==h;){var k=h.dependencies;if(null!==\nk){g=h.child;for(var l=k.firstContext;null!==l;){if(l.context===d&&0!==(l.observedBits&f)){1===h.tag&&(l=wg(c,null),l.tag=2,xg(h,l));h.expirationTime<c&&(h.expirationTime=c);l=h.alternate;null!==l&&l.expirationTime<c&&(l.expirationTime=c);pg(h.return,c);k.expirationTime<c&&(k.expirationTime=c);break}l=l.next}}else g=10===h.tag?h.type===b.type?null:h.child:h.child;if(null!==g)g.return=h;else for(g=h;null!==g;){if(g===b){g=null;break}h=g.sibling;if(null!==h){h.return=g.return;g=h;break}g=g.return}h=\ng}R(a,b,e.children,c);b=b.child}return b;case 9:return e=b.type,f=b.pendingProps,d=f.children,qg(b,c),e=sg(e,f.unstable_observedBits),d=d(e),b.effectTag|=1,R(a,b,d,c),b.child;case 14:return e=b.type,f=ig(e,b.pendingProps),f=ig(e.type,f),ai(a,b,e,f,d,c);case 15:return ci(a,b,b.type,b.pendingProps,d,c);case 17:return d=b.type,e=b.pendingProps,e=b.elementType===d?e:ig(d,e),null!==a&&(a.alternate=null,b.alternate=null,b.effectTag|=2),b.tag=1,L(d)?(a=!0,Gf(b)):a=!1,qg(b,c),Lg(b,d,e),Ng(b,d,e,c),gi(null,\nb,d,!0,a,c);case 19:return mi(a,b,c)}throw Error(u(156,b.tag));};var Uj=null,Li=null;function Yj(a){if(\"undefined\"===typeof __REACT_DEVTOOLS_GLOBAL_HOOK__)return!1;var b=__REACT_DEVTOOLS_GLOBAL_HOOK__;if(b.isDisabled||!b.supportsFiber)return!0;try{var c=b.inject(a);Uj=function(a){try{b.onCommitFiberRoot(c,a,void 0,64===(a.current.effectTag&64))}catch(e){}};Li=function(a){try{b.onCommitFiberUnmount(c,a)}catch(e){}}}catch(d){}return!0}\nfunction Zj(a,b,c,d){this.tag=a;this.key=c;this.sibling=this.child=this.return=this.stateNode=this.type=this.elementType=null;this.index=0;this.ref=null;this.pendingProps=b;this.dependencies=this.memoizedState=this.updateQueue=this.memoizedProps=null;this.mode=d;this.effectTag=0;this.lastEffect=this.firstEffect=this.nextEffect=null;this.childExpirationTime=this.expirationTime=0;this.alternate=null}function Sh(a,b,c,d){return new Zj(a,b,c,d)}\nfunction bi(a){a=a.prototype;return!(!a||!a.isReactComponent)}function Xj(a){if(\"function\"===typeof a)return bi(a)?1:0;if(void 0!==a&&null!==a){a=a.$$typeof;if(a===gb)return 11;if(a===jb)return 14}return 2}\nfunction Sg(a,b){var c=a.alternate;null===c?(c=Sh(a.tag,b,a.key,a.mode),c.elementType=a.elementType,c.type=a.type,c.stateNode=a.stateNode,c.alternate=a,a.alternate=c):(c.pendingProps=b,c.effectTag=0,c.nextEffect=null,c.firstEffect=null,c.lastEffect=null);c.childExpirationTime=a.childExpirationTime;c.expirationTime=a.expirationTime;c.child=a.child;c.memoizedProps=a.memoizedProps;c.memoizedState=a.memoizedState;c.updateQueue=a.updateQueue;b=a.dependencies;c.dependencies=null===b?null:{expirationTime:b.expirationTime,\nfirstContext:b.firstContext,responders:b.responders};c.sibling=a.sibling;c.index=a.index;c.ref=a.ref;return c}\nfunction Ug(a,b,c,d,e,f){var g=2;d=a;if(\"function\"===typeof a)bi(a)&&(g=1);else if(\"string\"===typeof a)g=5;else a:switch(a){case ab:return Wg(c.children,e,f,b);case fb:g=8;e|=7;break;case bb:g=8;e|=1;break;case cb:return a=Sh(12,c,b,e|8),a.elementType=cb,a.type=cb,a.expirationTime=f,a;case hb:return a=Sh(13,c,b,e),a.type=hb,a.elementType=hb,a.expirationTime=f,a;case ib:return a=Sh(19,c,b,e),a.elementType=ib,a.expirationTime=f,a;default:if(\"object\"===typeof a&&null!==a)switch(a.$$typeof){case db:g=\n10;break a;case eb:g=9;break a;case gb:g=11;break a;case jb:g=14;break a;case kb:g=16;d=null;break a;case lb:g=22;break a}throw Error(u(130,null==a?a:typeof a,\"\"));}b=Sh(g,c,b,e);b.elementType=a;b.type=d;b.expirationTime=f;return b}function Wg(a,b,c,d){a=Sh(7,a,d,b);a.expirationTime=c;return a}function Tg(a,b,c){a=Sh(6,a,null,b);a.expirationTime=c;return a}\nfunction Vg(a,b,c){b=Sh(4,null!==a.children?a.children:[],a.key,b);b.expirationTime=c;b.stateNode={containerInfo:a.containerInfo,pendingChildren:null,implementation:a.implementation};return b}\nfunction ak(a,b,c){this.tag=b;this.current=null;this.containerInfo=a;this.pingCache=this.pendingChildren=null;this.finishedExpirationTime=0;this.finishedWork=null;this.timeoutHandle=-1;this.pendingContext=this.context=null;this.hydrate=c;this.callbackNode=null;this.callbackPriority=90;this.lastExpiredTime=this.lastPingedTime=this.nextKnownPendingLevel=this.lastSuspendedTime=this.firstSuspendedTime=this.firstPendingTime=0}\nfunction Aj(a,b){var c=a.firstSuspendedTime;a=a.lastSuspendedTime;return 0!==c&&c>=b&&a<=b}function xi(a,b){var c=a.firstSuspendedTime,d=a.lastSuspendedTime;c<b&&(a.firstSuspendedTime=b);if(d>b||0===c)a.lastSuspendedTime=b;b<=a.lastPingedTime&&(a.lastPingedTime=0);b<=a.lastExpiredTime&&(a.lastExpiredTime=0)}\nfunction yi(a,b){b>a.firstPendingTime&&(a.firstPendingTime=b);var c=a.firstSuspendedTime;0!==c&&(b>=c?a.firstSuspendedTime=a.lastSuspendedTime=a.nextKnownPendingLevel=0:b>=a.lastSuspendedTime&&(a.lastSuspendedTime=b+1),b>a.nextKnownPendingLevel&&(a.nextKnownPendingLevel=b))}function Cj(a,b){var c=a.lastExpiredTime;if(0===c||c>b)a.lastExpiredTime=b}\nfunction bk(a,b,c,d){var e=b.current,f=Gg(),g=Dg.suspense;f=Hg(f,e,g);a:if(c){c=c._reactInternalFiber;b:{if(dc(c)!==c||1!==c.tag)throw Error(u(170));var h=c;do{switch(h.tag){case 3:h=h.stateNode.context;break b;case 1:if(L(h.type)){h=h.stateNode.__reactInternalMemoizedMergedChildContext;break b}}h=h.return}while(null!==h);throw Error(u(171));}if(1===c.tag){var k=c.type;if(L(k)){c=Ff(c,k,h);break a}}c=h}else c=Af;null===b.context?b.context=c:b.pendingContext=c;b=wg(f,g);b.payload={element:a};d=void 0===\nd?null:d;null!==d&&(b.callback=d);xg(e,b);Ig(e,f);return f}function ck(a){a=a.current;if(!a.child)return null;switch(a.child.tag){case 5:return a.child.stateNode;default:return a.child.stateNode}}function dk(a,b){a=a.memoizedState;null!==a&&null!==a.dehydrated&&a.retryTime<b&&(a.retryTime=b)}function ek(a,b){dk(a,b);(a=a.alternate)&&dk(a,b)}\nfunction fk(a,b,c){c=null!=c&&!0===c.hydrate;var d=new ak(a,b,c),e=Sh(3,null,null,2===b?7:1===b?3:0);d.current=e;e.stateNode=d;ug(e);a[Od]=d.current;c&&0!==b&&Jc(a,9===a.nodeType?a:a.ownerDocument);this._internalRoot=d}fk.prototype.render=function(a){bk(a,this._internalRoot,null,null)};fk.prototype.unmount=function(){var a=this._internalRoot,b=a.containerInfo;bk(null,a,null,function(){b[Od]=null})};\nfunction gk(a){return!(!a||1!==a.nodeType&&9!==a.nodeType&&11!==a.nodeType&&(8!==a.nodeType||\" react-mount-point-unstable \"!==a.nodeValue))}function hk(a,b){b||(b=a?9===a.nodeType?a.documentElement:a.firstChild:null,b=!(!b||1!==b.nodeType||!b.hasAttribute(\"data-reactroot\")));if(!b)for(var c;c=a.lastChild;)a.removeChild(c);return new fk(a,0,b?{hydrate:!0}:void 0)}\nfunction ik(a,b,c,d,e){var f=c._reactRootContainer;if(f){var g=f._internalRoot;if(\"function\"===typeof e){var h=e;e=function(){var a=ck(g);h.call(a)}}bk(b,g,a,e)}else{f=c._reactRootContainer=hk(c,d);g=f._internalRoot;if(\"function\"===typeof e){var k=e;e=function(){var a=ck(g);k.call(a)}}Nj(function(){bk(b,g,a,e)})}return ck(g)}function jk(a,b,c){var d=3<arguments.length&&void 0!==arguments[3]?arguments[3]:null;return{$$typeof:$a,key:null==d?null:\"\"+d,children:a,containerInfo:b,implementation:c}}\nwc=function(a){if(13===a.tag){var b=hg(Gg(),150,100);Ig(a,b);ek(a,b)}};xc=function(a){13===a.tag&&(Ig(a,3),ek(a,3))};yc=function(a){if(13===a.tag){var b=Gg();b=Hg(b,a,null);Ig(a,b);ek(a,b)}};\nza=function(a,b,c){switch(b){case \"input\":Cb(a,c);b=c.name;if(\"radio\"===c.type&&null!=b){for(c=a;c.parentNode;)c=c.parentNode;c=c.querySelectorAll(\"input[name=\"+JSON.stringify(\"\"+b)+'][type=\"radio\"]');for(b=0;b<c.length;b++){var d=c[b];if(d!==a&&d.form===a.form){var e=Qd(d);if(!e)throw Error(u(90));yb(d);Cb(d,e)}}}break;case \"textarea\":Kb(a,c);break;case \"select\":b=c.value,null!=b&&Hb(a,!!c.multiple,b,!1)}};Fa=Mj;\nGa=function(a,b,c,d,e){var f=W;W|=4;try{return cg(98,a.bind(null,b,c,d,e))}finally{W=f,W===V&&gg()}};Ha=function(){(W&(1|fj|gj))===V&&(Lj(),Dj())};Ia=function(a,b){var c=W;W|=2;try{return a(b)}finally{W=c,W===V&&gg()}};function kk(a,b){var c=2<arguments.length&&void 0!==arguments[2]?arguments[2]:null;if(!gk(b))throw Error(u(200));return jk(a,b,null,c)}var lk={Events:[Nc,Pd,Qd,xa,ta,Xd,function(a){jc(a,Wd)},Da,Ea,id,mc,Dj,{current:!1}]};\n(function(a){var b=a.findFiberByHostInstance;return Yj(n({},a,{overrideHookState:null,overrideProps:null,setSuspenseHandler:null,scheduleUpdate:null,currentDispatcherRef:Wa.ReactCurrentDispatcher,findHostInstanceByFiber:function(a){a=hc(a);return null===a?null:a.stateNode},findFiberByHostInstance:function(a){return b?b(a):null},findHostInstancesForRefresh:null,scheduleRefresh:null,scheduleRoot:null,setRefreshHandler:null,getCurrentFiber:null}))})({findFiberByHostInstance:tc,bundleType:0,version:\"16.14.0\",\nrendererPackageName:\"react-dom\"});exports.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED=lk;exports.createPortal=kk;exports.findDOMNode=function(a){if(null==a)return null;if(1===a.nodeType)return a;var b=a._reactInternalFiber;if(void 0===b){if(\"function\"===typeof a.render)throw Error(u(188));throw Error(u(268,Object.keys(a)));}a=hc(b);a=null===a?null:a.stateNode;return a};\nexports.flushSync=function(a,b){if((W&(fj|gj))!==V)throw Error(u(187));var c=W;W|=1;try{return cg(99,a.bind(null,b))}finally{W=c,gg()}};exports.hydrate=function(a,b,c){if(!gk(b))throw Error(u(200));return ik(null,a,b,!0,c)};exports.render=function(a,b,c){if(!gk(b))throw Error(u(200));return ik(null,a,b,!1,c)};\nexports.unmountComponentAtNode=function(a){if(!gk(a))throw Error(u(40));return a._reactRootContainer?(Nj(function(){ik(null,null,a,!1,function(){a._reactRootContainer=null;a[Od]=null})}),!0):!1};exports.unstable_batchedUpdates=Mj;exports.unstable_createPortal=function(a,b){return kk(a,b,2<arguments.length&&void 0!==arguments[2]?arguments[2]:null)};\nexports.unstable_renderSubtreeIntoContainer=function(a,b,c,d){if(!gk(c))throw Error(u(200));if(null==a||void 0===a._reactInternalFiber)throw Error(u(38));return ik(a,b,c,!1,d)};exports.version=\"16.14.0\";\n",
         "'use strict';\n\nfunction checkDCE() {\n  /* global __REACT_DEVTOOLS_GLOBAL_HOOK__ */\n  if (\n    typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ === 'undefined' ||\n    typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE !== 'function'\n  ) {\n    return;\n  }\n  if (process.env.NODE_ENV !== 'production') {\n    // This branch is unreachable because this function is only called\n    // in production, but the condition is true only in development.\n    // Therefore if the branch is still here, dead code elimination wasn't\n    // properly applied.\n    // Don't change the message. React DevTools relies on it. Also make sure\n    // this message doesn't occur elsewhere in this function, or it will cause\n    // a false positive.\n    throw new Error('^_^');\n  }\n  try {\n    // Verify that the code above has been dead code eliminated (DCE'd).\n    __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(checkDCE);\n  } catch (err) {\n    // DevTools shouldn't crash React, no matter what.\n    // We should still report in case we break this code.\n    console.error(err);\n  }\n}\n\nif (process.env.NODE_ENV === 'production') {\n  // DCE check should happen before ReactDOM bundle executes so that\n  // DevTools can report bad minification during injection.\n  checkDCE();\n  module.exports = require('./cjs/react-dom.production.min.js');\n} else {\n  module.exports = require('./cjs/react-dom.development.js');\n}\n",
         "/** @license React v16.13.1\n * react-is.production.min.js\n *\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n\n'use strict';var b=\"function\"===typeof Symbol&&Symbol.for,c=b?Symbol.for(\"react.element\"):60103,d=b?Symbol.for(\"react.portal\"):60106,e=b?Symbol.for(\"react.fragment\"):60107,f=b?Symbol.for(\"react.strict_mode\"):60108,g=b?Symbol.for(\"react.profiler\"):60114,h=b?Symbol.for(\"react.provider\"):60109,k=b?Symbol.for(\"react.context\"):60110,l=b?Symbol.for(\"react.async_mode\"):60111,m=b?Symbol.for(\"react.concurrent_mode\"):60111,n=b?Symbol.for(\"react.forward_ref\"):60112,p=b?Symbol.for(\"react.suspense\"):60113,q=b?\nSymbol.for(\"react.suspense_list\"):60120,r=b?Symbol.for(\"react.memo\"):60115,t=b?Symbol.for(\"react.lazy\"):60116,v=b?Symbol.for(\"react.block\"):60121,w=b?Symbol.for(\"react.fundamental\"):60117,x=b?Symbol.for(\"react.responder\"):60118,y=b?Symbol.for(\"react.scope\"):60119;\nfunction z(a){if(\"object\"===typeof a&&null!==a){var u=a.$$typeof;switch(u){case c:switch(a=a.type,a){case l:case m:case e:case g:case f:case p:return a;default:switch(a=a&&a.$$typeof,a){case k:case n:case t:case r:case h:return a;default:return u}}case d:return u}}}function A(a){return z(a)===m}exports.AsyncMode=l;exports.ConcurrentMode=m;exports.ContextConsumer=k;exports.ContextProvider=h;exports.Element=c;exports.ForwardRef=n;exports.Fragment=e;exports.Lazy=t;exports.Memo=r;exports.Portal=d;\nexports.Profiler=g;exports.StrictMode=f;exports.Suspense=p;exports.isAsyncMode=function(a){return A(a)||z(a)===l};exports.isConcurrentMode=A;exports.isContextConsumer=function(a){return z(a)===k};exports.isContextProvider=function(a){return z(a)===h};exports.isElement=function(a){return\"object\"===typeof a&&null!==a&&a.$$typeof===c};exports.isForwardRef=function(a){return z(a)===n};exports.isFragment=function(a){return z(a)===e};exports.isLazy=function(a){return z(a)===t};\nexports.isMemo=function(a){return z(a)===r};exports.isPortal=function(a){return z(a)===d};exports.isProfiler=function(a){return z(a)===g};exports.isStrictMode=function(a){return z(a)===f};exports.isSuspense=function(a){return z(a)===p};\nexports.isValidElementType=function(a){return\"string\"===typeof a||\"function\"===typeof a||a===e||a===m||a===g||a===f||a===p||a===q||\"object\"===typeof a&&null!==a&&(a.$$typeof===t||a.$$typeof===r||a.$$typeof===h||a.$$typeof===k||a.$$typeof===n||a.$$typeof===w||a.$$typeof===x||a.$$typeof===y||a.$$typeof===v)};exports.typeOf=z;\n",
         "'use strict';\n\nif (process.env.NODE_ENV === 'production') {\n  module.exports = require('./cjs/react-is.production.min.js');\n} else {\n  module.exports = require('./cjs/react-is.development.js');\n}\n",
         "/** @license React v16.14.0\n * react-jsx-runtime.production.min.js\n *\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n'use strict';var f=require(\"react\"),g=60103;exports.Fragment=60107;if(\"function\"===typeof Symbol&&Symbol.for){var h=Symbol.for;g=h(\"react.element\");exports.Fragment=h(\"react.fragment\")}var m=f.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,n=Object.prototype.hasOwnProperty,p={key:!0,ref:!0,__self:!0,__source:!0};\nfunction q(c,a,k){var b,d={},e=null,l=null;void 0!==k&&(e=\"\"+k);void 0!==a.key&&(e=\"\"+a.key);void 0!==a.ref&&(l=a.ref);for(b in a)n.call(a,b)&&!p.hasOwnProperty(b)&&(d[b]=a[b]);if(c&&c.defaultProps)for(b in a=c.defaultProps,a)void 0===d[b]&&(d[b]=a[b]);return{$$typeof:g,type:c,key:e,ref:l,props:d,_owner:m.current}}exports.jsx=q;exports.jsxs=q;\n",
         "/** @license React v16.14.0\n * react.production.min.js\n *\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n\n'use strict';var l=require(\"object-assign\"),n=\"function\"===typeof Symbol&&Symbol.for,p=n?Symbol.for(\"react.element\"):60103,q=n?Symbol.for(\"react.portal\"):60106,r=n?Symbol.for(\"react.fragment\"):60107,t=n?Symbol.for(\"react.strict_mode\"):60108,u=n?Symbol.for(\"react.profiler\"):60114,v=n?Symbol.for(\"react.provider\"):60109,w=n?Symbol.for(\"react.context\"):60110,x=n?Symbol.for(\"react.forward_ref\"):60112,y=n?Symbol.for(\"react.suspense\"):60113,z=n?Symbol.for(\"react.memo\"):60115,A=n?Symbol.for(\"react.lazy\"):\n60116,B=\"function\"===typeof Symbol&&Symbol.iterator;function C(a){for(var b=\"https://reactjs.org/docs/error-decoder.html?invariant=\"+a,c=1;c<arguments.length;c++)b+=\"&args[]=\"+encodeURIComponent(arguments[c]);return\"Minified React error #\"+a+\"; visit \"+b+\" for the full message or use the non-minified dev environment for full errors and additional helpful warnings.\"}\nvar D={isMounted:function(){return!1},enqueueForceUpdate:function(){},enqueueReplaceState:function(){},enqueueSetState:function(){}},E={};function F(a,b,c){this.props=a;this.context=b;this.refs=E;this.updater=c||D}F.prototype.isReactComponent={};F.prototype.setState=function(a,b){if(\"object\"!==typeof a&&\"function\"!==typeof a&&null!=a)throw Error(C(85));this.updater.enqueueSetState(this,a,b,\"setState\")};F.prototype.forceUpdate=function(a){this.updater.enqueueForceUpdate(this,a,\"forceUpdate\")};\nfunction G(){}G.prototype=F.prototype;function H(a,b,c){this.props=a;this.context=b;this.refs=E;this.updater=c||D}var I=H.prototype=new G;I.constructor=H;l(I,F.prototype);I.isPureReactComponent=!0;var J={current:null},K=Object.prototype.hasOwnProperty,L={key:!0,ref:!0,__self:!0,__source:!0};\nfunction M(a,b,c){var e,d={},g=null,k=null;if(null!=b)for(e in void 0!==b.ref&&(k=b.ref),void 0!==b.key&&(g=\"\"+b.key),b)K.call(b,e)&&!L.hasOwnProperty(e)&&(d[e]=b[e]);var f=arguments.length-2;if(1===f)d.children=c;else if(1<f){for(var h=Array(f),m=0;m<f;m++)h[m]=arguments[m+2];d.children=h}if(a&&a.defaultProps)for(e in f=a.defaultProps,f)void 0===d[e]&&(d[e]=f[e]);return{$$typeof:p,type:a,key:g,ref:k,props:d,_owner:J.current}}\nfunction N(a,b){return{$$typeof:p,type:a.type,key:b,ref:a.ref,props:a.props,_owner:a._owner}}function O(a){return\"object\"===typeof a&&null!==a&&a.$$typeof===p}function escape(a){var b={\"=\":\"=0\",\":\":\"=2\"};return\"$\"+(\"\"+a).replace(/[=:]/g,function(a){return b[a]})}var P=/\\/+/g,Q=[];function R(a,b,c,e){if(Q.length){var d=Q.pop();d.result=a;d.keyPrefix=b;d.func=c;d.context=e;d.count=0;return d}return{result:a,keyPrefix:b,func:c,context:e,count:0}}\nfunction S(a){a.result=null;a.keyPrefix=null;a.func=null;a.context=null;a.count=0;10>Q.length&&Q.push(a)}\nfunction T(a,b,c,e){var d=typeof a;if(\"undefined\"===d||\"boolean\"===d)a=null;var g=!1;if(null===a)g=!0;else switch(d){case \"string\":case \"number\":g=!0;break;case \"object\":switch(a.$$typeof){case p:case q:g=!0}}if(g)return c(e,a,\"\"===b?\".\"+U(a,0):b),1;g=0;b=\"\"===b?\".\":b+\":\";if(Array.isArray(a))for(var k=0;k<a.length;k++){d=a[k];var f=b+U(d,k);g+=T(d,f,c,e)}else if(null===a||\"object\"!==typeof a?f=null:(f=B&&a[B]||a[\"@@iterator\"],f=\"function\"===typeof f?f:null),\"function\"===typeof f)for(a=f.call(a),k=\n0;!(d=a.next()).done;)d=d.value,f=b+U(d,k++),g+=T(d,f,c,e);else if(\"object\"===d)throw c=\"\"+a,Error(C(31,\"[object Object]\"===c?\"object with keys {\"+Object.keys(a).join(\", \")+\"}\":c,\"\"));return g}function V(a,b,c){return null==a?0:T(a,\"\",b,c)}function U(a,b){return\"object\"===typeof a&&null!==a&&null!=a.key?escape(a.key):b.toString(36)}function W(a,b){a.func.call(a.context,b,a.count++)}\nfunction aa(a,b,c){var e=a.result,d=a.keyPrefix;a=a.func.call(a.context,b,a.count++);Array.isArray(a)?X(a,e,c,function(a){return a}):null!=a&&(O(a)&&(a=N(a,d+(!a.key||b&&b.key===a.key?\"\":(\"\"+a.key).replace(P,\"$&/\")+\"/\")+c)),e.push(a))}function X(a,b,c,e,d){var g=\"\";null!=c&&(g=(\"\"+c).replace(P,\"$&/\")+\"/\");b=R(b,g,e,d);V(a,aa,b);S(b)}var Y={current:null};function Z(){var a=Y.current;if(null===a)throw Error(C(321));return a}\nvar ba={ReactCurrentDispatcher:Y,ReactCurrentBatchConfig:{suspense:null},ReactCurrentOwner:J,IsSomeRendererActing:{current:!1},assign:l};exports.Children={map:function(a,b,c){if(null==a)return a;var e=[];X(a,e,null,b,c);return e},forEach:function(a,b,c){if(null==a)return a;b=R(null,null,b,c);V(a,W,b);S(b)},count:function(a){return V(a,function(){return null},null)},toArray:function(a){var b=[];X(a,b,null,function(a){return a});return b},only:function(a){if(!O(a))throw Error(C(143));return a}};\nexports.Component=F;exports.Fragment=r;exports.Profiler=u;exports.PureComponent=H;exports.StrictMode=t;exports.Suspense=y;exports.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED=ba;\nexports.cloneElement=function(a,b,c){if(null===a||void 0===a)throw Error(C(267,a));var e=l({},a.props),d=a.key,g=a.ref,k=a._owner;if(null!=b){void 0!==b.ref&&(g=b.ref,k=J.current);void 0!==b.key&&(d=\"\"+b.key);if(a.type&&a.type.defaultProps)var f=a.type.defaultProps;for(h in b)K.call(b,h)&&!L.hasOwnProperty(h)&&(e[h]=void 0===b[h]&&void 0!==f?f[h]:b[h])}var h=arguments.length-2;if(1===h)e.children=c;else if(1<h){f=Array(h);for(var m=0;m<h;m++)f[m]=arguments[m+2];e.children=f}return{$$typeof:p,type:a.type,\nkey:d,ref:g,props:e,_owner:k}};exports.createContext=function(a,b){void 0===b&&(b=null);a={$$typeof:w,_calculateChangedBits:b,_currentValue:a,_currentValue2:a,_threadCount:0,Provider:null,Consumer:null};a.Provider={$$typeof:v,_context:a};return a.Consumer=a};exports.createElement=M;exports.createFactory=function(a){var b=M.bind(null,a);b.type=a;return b};exports.createRef=function(){return{current:null}};exports.forwardRef=function(a){return{$$typeof:x,render:a}};exports.isValidElement=O;\nexports.lazy=function(a){return{$$typeof:A,_ctor:a,_status:-1,_result:null}};exports.memo=function(a,b){return{$$typeof:z,type:a,compare:void 0===b?null:b}};exports.useCallback=function(a,b){return Z().useCallback(a,b)};exports.useContext=function(a,b){return Z().useContext(a,b)};exports.useDebugValue=function(){};exports.useEffect=function(a,b){return Z().useEffect(a,b)};exports.useImperativeHandle=function(a,b,c){return Z().useImperativeHandle(a,b,c)};\nexports.useLayoutEffect=function(a,b){return Z().useLayoutEffect(a,b)};exports.useMemo=function(a,b){return Z().useMemo(a,b)};exports.useReducer=function(a,b,c){return Z().useReducer(a,b,c)};exports.useRef=function(a){return Z().useRef(a)};exports.useState=function(a){return Z().useState(a)};exports.version=\"16.14.0\";\n",
@@ -6536,15 +6562,15 @@
         "import TimeScale from './scale.time.js';\nimport {_lookupByKey} from '../helpers/helpers.collection.js';\n\n/**\n * Linearly interpolates the given source `val` using the table. If value is out of bounds, values\n * at edges are used for the interpolation.\n * @param {object} table\n * @param {number} val\n * @param {boolean} [reverse] lookup time based on position instead of vice versa\n * @return {object}\n */\nfunction interpolate(table, val, reverse) {\n  let lo = 0;\n  let hi = table.length - 1;\n  let prevSource, nextSource, prevTarget, nextTarget;\n  if (reverse) {\n    if (val >= table[lo].pos && val <= table[hi].pos) {\n      ({lo, hi} = _lookupByKey(table, 'pos', val));\n    }\n    ({pos: prevSource, time: prevTarget} = table[lo]);\n    ({pos: nextSource, time: nextTarget} = table[hi]);\n  } else {\n    if (val >= table[lo].time && val <= table[hi].time) {\n      ({lo, hi} = _lookupByKey(table, 'time', val));\n    }\n    ({time: prevSource, pos: prevTarget} = table[lo]);\n    ({time: nextSource, pos: nextTarget} = table[hi]);\n  }\n\n  const span = nextSource - prevSource;\n  return span ? prevTarget + (nextTarget - prevTarget) * (val - prevSource) / span : prevTarget;\n}\n\nclass TimeSeriesScale extends TimeScale {\n\n  static id = 'timeseries';\n\n  /**\n   * @type {any}\n   */\n  static defaults = TimeScale.defaults;\n\n  /**\n\t * @param {object} props\n\t */\n  constructor(props) {\n    super(props);\n\n    /** @type {object[]} */\n    this._table = [];\n    /** @type {number} */\n    this._minPos = undefined;\n    /** @type {number} */\n    this._tableRange = undefined;\n  }\n\n  /**\n\t * @protected\n\t */\n  initOffsets() {\n    const timestamps = this._getTimestampsForTable();\n    const table = this._table = this.buildLookupTable(timestamps);\n    this._minPos = interpolate(table, this.min);\n    this._tableRange = interpolate(table, this.max) - this._minPos;\n    super.initOffsets(timestamps);\n  }\n\n  /**\n\t * Returns an array of {time, pos} objects used to interpolate a specific `time` or position\n\t * (`pos`) on the scale, by searching entries before and after the requested value. `pos` is\n\t * a decimal between 0 and 1: 0 being the start of the scale (left or top) and 1 the other\n\t * extremity (left + width or top + height). Note that it would be more optimized to directly\n\t * store pre-computed pixels, but the scale dimensions are not guaranteed at the time we need\n\t * to create the lookup table. The table ALWAYS contains at least two items: min and max.\n\t * @param {number[]} timestamps\n\t * @return {object[]}\n\t * @protected\n\t */\n  buildLookupTable(timestamps) {\n    const {min, max} = this;\n    const items = [];\n    const table = [];\n    let i, ilen, prev, curr, next;\n\n    for (i = 0, ilen = timestamps.length; i < ilen; ++i) {\n      curr = timestamps[i];\n      if (curr >= min && curr <= max) {\n        items.push(curr);\n      }\n    }\n\n    if (items.length < 2) {\n      // In case there is less that 2 timestamps between min and max, the scale is defined by min and max\n      return [\n        {time: min, pos: 0},\n        {time: max, pos: 1}\n      ];\n    }\n\n    for (i = 0, ilen = items.length; i < ilen; ++i) {\n      next = items[i + 1];\n      prev = items[i - 1];\n      curr = items[i];\n\n      // only add points that breaks the scale linearity\n      if (Math.round((next + prev) / 2) !== curr) {\n        table.push({time: curr, pos: i / (ilen - 1)});\n      }\n    }\n    return table;\n  }\n\n  /**\n    * Generates all timestamps defined in the data.\n    * Important: this method can return ticks outside the min and max range, it's the\n    * responsibility of the calling code to clamp values if needed.\n    * @protected\n    */\n  _generate() {\n    const min = this.min;\n    const max = this.max;\n    let timestamps = super.getDataTimestamps();\n    if (!timestamps.includes(min) || !timestamps.length) {\n      timestamps.splice(0, 0, min);\n    }\n    if (!timestamps.includes(max) || timestamps.length === 1) {\n      timestamps.push(max);\n    }\n    return timestamps.sort((a, b) => a - b);\n  }\n\n  /**\n\t * Returns all timestamps\n\t * @return {number[]}\n\t * @private\n\t */\n  _getTimestampsForTable() {\n    let timestamps = this._cache.all || [];\n\n    if (timestamps.length) {\n      return timestamps;\n    }\n\n    const data = this.getDataTimestamps();\n    const label = this.getLabelTimestamps();\n    if (data.length && label.length) {\n      // If combining labels and data (data might not contain all labels),\n      // we need to recheck uniqueness and sort\n      timestamps = this.normalize(data.concat(label));\n    } else {\n      timestamps = data.length ? data : label;\n    }\n    timestamps = this._cache.all = timestamps;\n\n    return timestamps;\n  }\n\n  /**\n\t * @param {number} value - Milliseconds since epoch (1 January 1970 00:00:00 UTC)\n\t * @return {number}\n\t */\n  getDecimalForValue(value) {\n    return (interpolate(this._table, value) - this._minPos) / this._tableRange;\n  }\n\n  /**\n\t * @param {number} pixel\n\t * @return {number}\n\t */\n  getValueForPixel(pixel) {\n    const offsets = this._offsets;\n    const decimal = this.getDecimalForPixel(pixel) / offsets.factor - offsets.end;\n    return interpolate(this._table, decimal * this._tableRange + this._minPos, true);\n  }\n}\n\nexport default TimeSeriesScale;\n",
         "export * from './controllers/index.js';\nexport * from './core/index.js';\nexport * from './elements/index.js';\nexport * from './platform/index.js';\nexport * from './plugins/index.js';\nexport * from './scales/index.js';\n\nimport * as controllers from './controllers/index.js';\nimport * as elements from './elements/index.js';\nimport * as plugins from './plugins/index.js';\nimport * as scales from './scales/index.js';\n\nexport {\n  controllers,\n  elements,\n  plugins,\n  scales,\n};\n\nexport const registerables = [\n  controllers,\n  elements,\n  plugins,\n  scales,\n];\n",
         "/*!\n* chartjs-plugin-zoom v2.0.1\n* undefined\n * (c) 2016-2023 chartjs-plugin-zoom Contributors\n * Released under the MIT License\n */\nimport Hammer from 'hammerjs';\nimport { each, valueOrDefault, callback, sign, getRelativePosition } from 'chart.js/helpers';\n\nconst getModifierKey = opts => opts && opts.enabled && opts.modifierKey;\nconst keyPressed = (key, event) => key && event[key + 'Key'];\nconst keyNotPressed = (key, event) => key && !event[key + 'Key'];\n\n/**\n * @param {string|function} mode can be 'x', 'y' or 'xy'\n * @param {string} dir can be 'x' or 'y'\n * @param {import('chart.js').Chart} chart instance of the chart in question\n * @returns {boolean}\n */\nfunction directionEnabled(mode, dir, chart) {\n  if (mode === undefined) {\n    return true;\n  } else if (typeof mode === 'string') {\n    return mode.indexOf(dir) !== -1;\n  } else if (typeof mode === 'function') {\n    return mode({chart}).indexOf(dir) !== -1;\n  }\n\n  return false;\n}\n\nfunction directionsEnabled(mode, chart) {\n  if (typeof mode === 'function') {\n    mode = mode({chart});\n  }\n  if (typeof mode === 'string') {\n    return {x: mode.indexOf('x') !== -1, y: mode.indexOf('y') !== -1};\n  }\n\n  return {x: false, y: false};\n}\n\n/**\n * Debounces calling `fn` for `delay` ms\n * @param {function} fn - Function to call. No arguments are passed.\n * @param {number} delay - Delay in ms. 0 = immediate invocation.\n * @returns {function}\n */\nfunction debounce(fn, delay) {\n  let timeout;\n  return function() {\n    clearTimeout(timeout);\n    timeout = setTimeout(fn, delay);\n    return delay;\n  };\n}\n\n/**\n * Checks which axis is under the mouse cursor.\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale}\n */\nfunction getScaleUnderPoint({x, y}, chart) {\n  const scales = chart.scales;\n  const scaleIds = Object.keys(scales);\n  for (let i = 0; i < scaleIds.length; i++) {\n    const scale = scales[scaleIds[i]];\n    if (y >= scale.top && y <= scale.bottom && x >= scale.left && x <= scale.right) {\n      return scale;\n    }\n  }\n  return null;\n}\n\n/**\n * Evaluate the chart's mode, scaleMode, and overScaleMode properties to\n * determine which axes are eligible for scaling.\n * options.overScaleMode can be a function if user want zoom only one scale of many for example.\n * @param options - Zoom or pan options\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale[]}\n */\nfunction getEnabledScalesByPoint(options, point, chart) {\n  const {mode = 'xy', scaleMode, overScaleMode} = options || {};\n  const scale = getScaleUnderPoint(point, chart);\n\n  const enabled = directionsEnabled(mode, chart);\n  const scaleEnabled = directionsEnabled(scaleMode, chart);\n\n  // Convert deprecated overScaleEnabled to new scaleEnabled.\n  if (overScaleMode) {\n    const overScaleEnabled = directionsEnabled(overScaleMode, chart);\n    for (const axis of ['x', 'y']) {\n      if (overScaleEnabled[axis]) {\n        scaleEnabled[axis] = enabled[axis];\n        enabled[axis] = false;\n      }\n    }\n  }\n\n  if (scale && scaleEnabled[scale.axis]) {\n    return [scale];\n  }\n\n  const enabledScales = [];\n  each(chart.scales, function(scaleItem) {\n    if (enabled[scaleItem.axis]) {\n      enabledScales.push(scaleItem);\n    }\n  });\n  return enabledScales;\n}\n\nconst chartStates = new WeakMap();\n\nfunction getState(chart) {\n  let state = chartStates.get(chart);\n  if (!state) {\n    state = {\n      originalScaleLimits: {},\n      updatedScaleLimits: {},\n      handlers: {},\n      panDelta: {}\n    };\n    chartStates.set(chart, state);\n  }\n  return state;\n}\n\nfunction removeState(chart) {\n  chartStates.delete(chart);\n}\n\nfunction zoomDelta(scale, zoom, center) {\n  const range = scale.max - scale.min;\n  const newRange = range * (zoom - 1);\n\n  const centerPoint = scale.isHorizontal() ? center.x : center.y;\n  // `scale.getValueForPixel()` can return a value less than the `scale.min` or\n  // greater than `scale.max` when `centerPoint` is outside chartArea.\n  const minPercent = Math.max(0, Math.min(1,\n    (scale.getValueForPixel(centerPoint) - scale.min) / range || 0\n  ));\n\n  const maxPercent = 1 - minPercent;\n\n  return {\n    min: newRange * minPercent,\n    max: newRange * maxPercent\n  };\n}\n\nfunction getLimit(state, scale, scaleLimits, prop, fallback) {\n  let limit = scaleLimits[prop];\n  if (limit === 'original') {\n    const original = state.originalScaleLimits[scale.id][prop];\n    limit = valueOrDefault(original.options, original.scale);\n  }\n  return valueOrDefault(limit, fallback);\n}\n\nfunction getRange(scale, pixel0, pixel1) {\n  const v0 = scale.getValueForPixel(pixel0);\n  const v1 = scale.getValueForPixel(pixel1);\n  return {\n    min: Math.min(v0, v1),\n    max: Math.max(v0, v1)\n  };\n}\n\nfunction updateRange(scale, {min, max}, limits, zoom = false) {\n  const state = getState(scale.chart);\n  const {id, axis, options: scaleOpts} = scale;\n\n  const scaleLimits = limits && (limits[id] || limits[axis]) || {};\n  const {minRange = 0} = scaleLimits;\n  const minLimit = getLimit(state, scale, scaleLimits, 'min', -Infinity);\n  const maxLimit = getLimit(state, scale, scaleLimits, 'max', Infinity);\n\n  const range = zoom ? Math.max(max - min, minRange) : scale.max - scale.min;\n  const offset = (range - max + min) / 2;\n  min -= offset;\n  max += offset;\n\n  if (min < minLimit) {\n    min = minLimit;\n    max = Math.min(minLimit + range, maxLimit);\n  } else if (max > maxLimit) {\n    max = maxLimit;\n    min = Math.max(maxLimit - range, minLimit);\n  }\n  scaleOpts.min = min;\n  scaleOpts.max = max;\n\n  state.updatedScaleLimits[scale.id] = {min, max};\n\n  // return true if the scale range is changed\n  return scale.parse(min) !== scale.min || scale.parse(max) !== scale.max;\n}\n\nfunction zoomNumericalScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  const newRange = {min: scale.min + delta.min, max: scale.max - delta.max};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction zoomRectNumericalScale(scale, from, to, limits) {\n  updateRange(scale, getRange(scale, from, to), limits, true);\n}\n\nconst integerChange = (v) => v === 0 || isNaN(v) ? 0 : v < 0 ? Math.min(Math.round(v), -1) : Math.max(Math.round(v), 1);\n\nfunction existCategoryFromMaxZoom(scale) {\n  const labels = scale.getLabels();\n  const maxIndex = labels.length - 1;\n\n  if (scale.min > 0) {\n    scale.min -= 1;\n  }\n  if (scale.max < maxIndex) {\n    scale.max += 1;\n  }\n}\n\nfunction zoomCategoryScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  if (scale.min === scale.max && zoom < 1) {\n    existCategoryFromMaxZoom(scale);\n  }\n  const newRange = {min: scale.min + integerChange(delta.min), max: scale.max - integerChange(delta.max)};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction scaleLength(scale) {\n  return scale.isHorizontal() ? scale.width : scale.height;\n}\n\nfunction panCategoryScale(scale, delta, limits) {\n  const labels = scale.getLabels();\n  const lastLabelIndex = labels.length - 1;\n  let {min, max} = scale;\n  // The visible range. Ticks can be skipped, and thus not reliable.\n  const range = Math.max(max - min, 1);\n  // How many pixels of delta is required before making a step. stepSize, but limited to max 1/10 of the scale length.\n  const stepDelta = Math.round(scaleLength(scale) / Math.max(range, 10));\n  const stepSize = Math.round(Math.abs(delta / stepDelta));\n  let applied;\n  if (delta < -stepDelta) {\n    max = Math.min(max + stepSize, lastLabelIndex);\n    min = range === 1 ? max : max - range;\n    applied = max === lastLabelIndex;\n  } else if (delta > stepDelta) {\n    min = Math.max(0, min - stepSize);\n    max = range === 1 ? min : min + range;\n    applied = min === 0;\n  }\n\n  return updateRange(scale, {min, max}, limits) || applied;\n}\n\nconst OFFSETS = {\n  second: 500, // 500 ms\n  minute: 30 * 1000, // 30 s\n  hour: 30 * 60 * 1000, // 30 m\n  day: 12 * 60 * 60 * 1000, // 12 h\n  week: 3.5 * 24 * 60 * 60 * 1000, // 3.5 d\n  month: 15 * 24 * 60 * 60 * 1000, // 15 d\n  quarter: 60 * 24 * 60 * 60 * 1000, // 60 d\n  year: 182 * 24 * 60 * 60 * 1000 // 182 d\n};\n\nfunction panNumericalScale(scale, delta, limits, canZoom = false) {\n  const {min: prevStart, max: prevEnd, options} = scale;\n  const round = options.time && options.time.round;\n  const offset = OFFSETS[round] || 0;\n  const newMin = scale.getValueForPixel(scale.getPixelForValue(prevStart + offset) - delta);\n  const newMax = scale.getValueForPixel(scale.getPixelForValue(prevEnd + offset) - delta);\n  const {min: minLimit = -Infinity, max: maxLimit = Infinity} = canZoom && limits && limits[scale.axis] || {};\n  if (isNaN(newMin) || isNaN(newMax) || newMin < minLimit || newMax > maxLimit) {\n    // At limit: No change but return true to indicate no need to store the delta.\n    // NaN can happen for 0-dimension scales (either because they were configured\n    // with min === max or because the chart has 0 plottable area).\n    return true;\n  }\n  return updateRange(scale, {min: newMin, max: newMax}, limits, canZoom);\n}\n\nfunction panNonLinearScale(scale, delta, limits) {\n  return panNumericalScale(scale, delta, limits, true);\n}\n\nconst zoomFunctions = {\n  category: zoomCategoryScale,\n  default: zoomNumericalScale,\n};\n\nconst zoomRectFunctions = {\n  default: zoomRectNumericalScale,\n};\n\nconst panFunctions = {\n  category: panCategoryScale,\n  default: panNumericalScale,\n  logarithmic: panNonLinearScale,\n  timeseries: panNonLinearScale,\n};\n\nfunction shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits) {\n  const {id, options: {min, max}} = scale;\n  if (!originalScaleLimits[id] || !updatedScaleLimits[id]) {\n    return true;\n  }\n  const previous = updatedScaleLimits[id];\n  return previous.min !== min || previous.max !== max;\n}\n\nfunction removeMissingScales(limits, scales) {\n  each(limits, (opt, key) => {\n    if (!scales[key]) {\n      delete limits[key];\n    }\n  });\n}\n\nfunction storeOriginalScaleLimits(chart, state) {\n  const {scales} = chart;\n  const {originalScaleLimits, updatedScaleLimits} = state;\n\n  each(scales, function(scale) {\n    if (shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits)) {\n      originalScaleLimits[scale.id] = {\n        min: {scale: scale.min, options: scale.options.min},\n        max: {scale: scale.max, options: scale.options.max},\n      };\n    }\n  });\n\n  removeMissingScales(originalScaleLimits, scales);\n  removeMissingScales(updatedScaleLimits, scales);\n  return originalScaleLimits;\n}\n\nfunction doZoom(scale, amount, center, limits) {\n  const fn = zoomFunctions[scale.type] || zoomFunctions.default;\n  callback(fn, [scale, amount, center, limits]);\n}\n\nfunction doZoomRect(scale, amount, from, to, limits) {\n  const fn = zoomRectFunctions[scale.type] || zoomRectFunctions.default;\n  callback(fn, [scale, amount, from, to, limits]);\n}\n\nfunction getCenter(chart) {\n  const ca = chart.chartArea;\n  return {\n    x: (ca.left + ca.right) / 2,\n    y: (ca.top + ca.bottom) / 2,\n  };\n}\n\n/**\n * @param chart The chart instance\n * @param {number | {x?: number, y?: number, focalPoint?: {x: number, y: number}}} amount The zoom percentage or percentages and focal point\n * @param {string} [transition] Which transition mode to use. Defaults to 'none'\n */\nfunction zoom(chart, amount, transition = 'none') {\n  const {x = 1, y = 1, focalPoint = getCenter(chart)} = typeof amount === 'number' ? {x: amount, y: amount} : amount;\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 1;\n  const yEnabled = y !== 1;\n  const enabledScales = getEnabledScalesByPoint(zoomOptions, focalPoint, chart);\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoom(scale, x, focalPoint, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoom(scale, y, focalPoint, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomRect(chart, p0, p1, transition = 'none') {\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n  const {mode = 'xy'} = zoomOptions;\n\n  storeOriginalScaleLimits(chart, state);\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n\n  each(chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoomRect(scale, p0.x, p1.x, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoomRect(scale, p0.y, p1.y, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomScale(chart, scaleId, range, transition = 'none') {\n  storeOriginalScaleLimits(chart, getState(chart));\n  const scale = chart.scales[scaleId];\n  updateRange(scale, range, undefined, true);\n  chart.update(transition);\n}\n\nfunction resetZoom(chart, transition = 'default') {\n  const state = getState(chart);\n  const originalScaleLimits = storeOriginalScaleLimits(chart, state);\n\n  each(chart.scales, function(scale) {\n    const scaleOptions = scale.options;\n    if (originalScaleLimits[scale.id]) {\n      scaleOptions.min = originalScaleLimits[scale.id].min.options;\n      scaleOptions.max = originalScaleLimits[scale.id].max.options;\n    } else {\n      delete scaleOptions.min;\n      delete scaleOptions.max;\n    }\n  });\n  chart.update(transition);\n  callback(state.options.zoom.onZoomComplete, [{chart}]);\n}\n\nfunction getOriginalRange(state, scaleId) {\n  const original = state.originalScaleLimits[scaleId];\n  if (!original) {\n    return;\n  }\n  const {min, max} = original;\n  return valueOrDefault(max.options, max.scale) - valueOrDefault(min.options, min.scale);\n}\n\nfunction getZoomLevel(chart) {\n  const state = getState(chart);\n  let min = 1;\n  let max = 1;\n  each(chart.scales, function(scale) {\n    const origRange = getOriginalRange(state, scale.id);\n    if (origRange) {\n      const level = Math.round(origRange / (scale.max - scale.min) * 100) / 100;\n      min = Math.min(min, level);\n      max = Math.max(max, level);\n    }\n  });\n  return min < 1 ? min : max;\n}\n\nfunction panScale(scale, delta, limits, state) {\n  const {panDelta} = state;\n  // Add possible cumulative delta from previous pan attempts where scale did not change\n  const storedDelta = panDelta[scale.id] || 0;\n  if (sign(storedDelta) === sign(delta)) {\n    delta += storedDelta;\n  }\n  const fn = panFunctions[scale.type] || panFunctions.default;\n  if (callback(fn, [scale, delta, limits])) {\n    // The scale changed, reset cumulative delta\n    panDelta[scale.id] = 0;\n  } else {\n    // The scale did not change, store cumulative delta\n    panDelta[scale.id] = delta;\n  }\n}\n\nfunction pan(chart, delta, enabledScales, transition = 'none') {\n  const {x = 0, y = 0} = typeof delta === 'number' ? {x: delta, y: delta} : delta;\n  const state = getState(chart);\n  const {options: {pan: panOptions, limits}} = state;\n  const {onPan} = panOptions || {};\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 0;\n  const yEnabled = y !== 0;\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      panScale(scale, x, limits, state);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      panScale(scale, y, limits, state);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(onPan, [{chart}]);\n}\n\nfunction getInitialScaleBounds(chart) {\n  const state = getState(chart);\n  storeOriginalScaleLimits(chart, state);\n  const scaleBounds = {};\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min, max} = state.originalScaleLimits[scaleId] || {min: {}, max: {}};\n    scaleBounds[scaleId] = {min: min.scale, max: max.scale};\n  }\n\n  return scaleBounds;\n}\n\nfunction isZoomedOrPanned(chart) {\n  const scaleBounds = getInitialScaleBounds(chart);\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min: originalMin, max: originalMax} = scaleBounds[scaleId];\n\n    if (originalMin !== undefined && chart.scales[scaleId].min !== originalMin) {\n      return true;\n    }\n\n    if (originalMax !== undefined && chart.scales[scaleId].max !== originalMax) {\n      return true;\n    }\n  }\n\n  return false;\n}\n\nfunction removeHandler(chart, type) {\n  const {handlers} = getState(chart);\n  const handler = handlers[type];\n  if (handler && handler.target) {\n    handler.target.removeEventListener(type, handler);\n    delete handlers[type];\n  }\n}\n\nfunction addHandler(chart, target, type, handler) {\n  const {handlers, options} = getState(chart);\n  const oldHandler = handlers[type];\n  if (oldHandler && oldHandler.target === target) {\n    // already attached\n    return;\n  }\n  removeHandler(chart, type);\n  handlers[type] = (event) => handler(chart, event, options);\n  handlers[type].target = target;\n  target.addEventListener(type, handlers[type]);\n}\n\nfunction mouseMove(chart, event) {\n  const state = getState(chart);\n  if (state.dragStart) {\n    state.dragging = true;\n    state.dragEnd = event;\n    chart.update('none');\n  }\n}\n\nfunction keyDown(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart || event.key !== 'Escape') {\n    return;\n  }\n\n  removeHandler(chart, 'keydown');\n  state.dragging = false;\n  state.dragStart = state.dragEnd = null;\n  chart.update('none');\n}\n\nfunction zoomStart(chart, event, zoomOptions) {\n  const {onZoomStart, onZoomRejected} = zoomOptions;\n  if (onZoomStart) {\n    const point = getRelativePosition(event, chart);\n    if (callback(onZoomStart, [{chart, event, point}]) === false) {\n      callback(onZoomRejected, [{chart, event}]);\n      return false;\n    }\n  }\n}\n\nfunction mouseDown(chart, event) {\n  const state = getState(chart);\n  const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n  if (\n    event.button !== 0 ||\n    keyPressed(getModifierKey(panOptions), event) ||\n    keyNotPressed(getModifierKey(zoomOptions.drag), event)\n  ) {\n    return callback(zoomOptions.onZoomRejected, [{chart, event}]);\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n  state.dragStart = event;\n\n  addHandler(chart, chart.canvas, 'mousemove', mouseMove);\n  addHandler(chart, window.document, 'keydown', keyDown);\n}\n\nfunction computeDragRect(chart, mode, beginPointEvent, endPointEvent) {\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n  let {top, left, right, bottom, width: chartWidth, height: chartHeight} = chart.chartArea;\n\n  const beginPoint = getRelativePosition(beginPointEvent, chart);\n  const endPoint = getRelativePosition(endPointEvent, chart);\n\n  if (xEnabled) {\n    left = Math.min(beginPoint.x, endPoint.x);\n    right = Math.max(beginPoint.x, endPoint.x);\n  }\n\n  if (yEnabled) {\n    top = Math.min(beginPoint.y, endPoint.y);\n    bottom = Math.max(beginPoint.y, endPoint.y);\n  }\n  const width = right - left;\n  const height = bottom - top;\n\n  return {\n    left,\n    top,\n    right,\n    bottom,\n    width,\n    height,\n    zoomX: xEnabled && width ? 1 + ((chartWidth - width) / chartWidth) : 1,\n    zoomY: yEnabled && height ? 1 + ((chartHeight - height) / chartHeight) : 1\n  };\n}\n\nfunction mouseUp(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart) {\n    return;\n  }\n\n  removeHandler(chart, 'mousemove');\n  const {mode, onZoomComplete, drag: {threshold = 0}} = state.options.zoom;\n  const rect = computeDragRect(chart, mode, state.dragStart, event);\n  const distanceX = directionEnabled(mode, 'x', chart) ? rect.width : 0;\n  const distanceY = directionEnabled(mode, 'y', chart) ? rect.height : 0;\n  const distance = Math.sqrt(distanceX * distanceX + distanceY * distanceY);\n\n  // Remove drag start and end before chart update to stop drawing selected area\n  state.dragStart = state.dragEnd = null;\n\n  if (distance <= threshold) {\n    state.dragging = false;\n    chart.update('none');\n    return;\n  }\n\n  zoomRect(chart, {x: rect.left, y: rect.top}, {x: rect.right, y: rect.bottom}, 'zoom');\n\n  setTimeout(() => (state.dragging = false), 500);\n  callback(onZoomComplete, [{chart}]);\n}\n\nfunction wheelPreconditions(chart, event, zoomOptions) {\n  // Before preventDefault, check if the modifier key required and pressed\n  if (keyNotPressed(getModifierKey(zoomOptions.wheel), event)) {\n    callback(zoomOptions.onZoomRejected, [{chart, event}]);\n    return;\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n\n  // Prevent the event from triggering the default behavior (e.g. content scrolling).\n  if (event.cancelable) {\n    event.preventDefault();\n  }\n\n  // Firefox always fires the wheel event twice:\n  // First without the delta and right after that once with the delta properties.\n  if (event.deltaY === undefined) {\n    return;\n  }\n  return true;\n}\n\nfunction wheel(chart, event) {\n  const {handlers: {onZoomComplete}, options: {zoom: zoomOptions}} = getState(chart);\n\n  if (!wheelPreconditions(chart, event, zoomOptions)) {\n    return;\n  }\n\n  const rect = event.target.getBoundingClientRect();\n  const speed = 1 + (event.deltaY >= 0 ? -zoomOptions.wheel.speed : zoomOptions.wheel.speed);\n  const amount = {\n    x: speed,\n    y: speed,\n    focalPoint: {\n      x: event.clientX - rect.left,\n      y: event.clientY - rect.top\n    }\n  };\n\n  zoom(chart, amount);\n\n  if (onZoomComplete) {\n    onZoomComplete();\n  }\n}\n\nfunction addDebouncedHandler(chart, name, handler, delay) {\n  if (handler) {\n    getState(chart).handlers[name] = debounce(() => callback(handler, [{chart}]), delay);\n  }\n}\n\nfunction addListeners(chart, options) {\n  const canvas = chart.canvas;\n  const {wheel: wheelOptions, drag: dragOptions, onZoomComplete} = options.zoom;\n\n  // Install listeners. Do this dynamically based on options so that we can turn zoom on and off\n  // We also want to make sure listeners aren't always on. E.g. if you're scrolling down a page\n  // and the mouse goes over a chart you don't want it intercepted unless the plugin is enabled\n  if (wheelOptions.enabled) {\n    addHandler(chart, canvas, 'wheel', wheel);\n    addDebouncedHandler(chart, 'onZoomComplete', onZoomComplete, 250);\n  } else {\n    removeHandler(chart, 'wheel');\n  }\n  if (dragOptions.enabled) {\n    addHandler(chart, canvas, 'mousedown', mouseDown);\n    addHandler(chart, canvas.ownerDocument, 'mouseup', mouseUp);\n  } else {\n    removeHandler(chart, 'mousedown');\n    removeHandler(chart, 'mousemove');\n    removeHandler(chart, 'mouseup');\n    removeHandler(chart, 'keydown');\n  }\n}\n\nfunction removeListeners(chart) {\n  removeHandler(chart, 'mousedown');\n  removeHandler(chart, 'mousemove');\n  removeHandler(chart, 'mouseup');\n  removeHandler(chart, 'wheel');\n  removeHandler(chart, 'click');\n  removeHandler(chart, 'keydown');\n}\n\nfunction createEnabler(chart, state) {\n  return function(recognizer, event) {\n    const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n    if (!panOptions || !panOptions.enabled) {\n      return false;\n    }\n    const srcEvent = event && event.srcEvent;\n    if (!srcEvent) { // Sometimes Hammer queries this with a null event.\n      return true;\n    }\n    if (!state.panning && event.pointerType === 'mouse' && (\n      keyNotPressed(getModifierKey(panOptions), srcEvent) || keyPressed(getModifierKey(zoomOptions.drag), srcEvent))\n    ) {\n      callback(panOptions.onPanRejected, [{chart, event}]);\n      return false;\n    }\n    return true;\n  };\n}\n\nfunction pinchAxes(p0, p1) {\n  // fingers position difference\n  const pinchX = Math.abs(p0.clientX - p1.clientX);\n  const pinchY = Math.abs(p0.clientY - p1.clientY);\n\n  // diagonal fingers will change both (xy) axes\n  const p = pinchX / pinchY;\n  let x, y;\n  if (p > 0.3 && p < 1.7) {\n    x = y = true;\n  } else if (pinchX > pinchY) {\n    x = true;\n  } else {\n    y = true;\n  }\n  return {x, y};\n}\n\nfunction handlePinch(chart, state, e) {\n  if (state.scale) {\n    const {center, pointers} = e;\n    // Hammer reports the total scaling. We need the incremental amount\n    const zoomPercent = 1 / state.scale * e.scale;\n    const rect = e.target.getBoundingClientRect();\n    const pinch = pinchAxes(pointers[0], pointers[1]);\n    const mode = state.options.zoom.mode;\n    const amount = {\n      x: pinch.x && directionEnabled(mode, 'x', chart) ? zoomPercent : 1,\n      y: pinch.y && directionEnabled(mode, 'y', chart) ? zoomPercent : 1,\n      focalPoint: {\n        x: center.x - rect.left,\n        y: center.y - rect.top\n      }\n    };\n\n    zoom(chart, amount);\n\n    // Keep track of overall scale\n    state.scale = e.scale;\n  }\n}\n\nfunction startPinch(chart, state) {\n  if (state.options.zoom.pinch.enabled) {\n    state.scale = 1;\n  }\n}\n\nfunction endPinch(chart, state, e) {\n  if (state.scale) {\n    handlePinch(chart, state, e);\n    state.scale = null; // reset\n    callback(state.options.zoom.onZoomComplete, [{chart}]);\n  }\n}\n\nfunction handlePan(chart, state, e) {\n  const delta = state.delta;\n  if (delta) {\n    state.panning = true;\n    pan(chart, {x: e.deltaX - delta.x, y: e.deltaY - delta.y}, state.panScales);\n    state.delta = {x: e.deltaX, y: e.deltaY};\n  }\n}\n\nfunction startPan(chart, state, event) {\n  const {enabled, onPanStart, onPanRejected} = state.options.pan;\n  if (!enabled) {\n    return;\n  }\n  const rect = event.target.getBoundingClientRect();\n  const point = {\n    x: event.center.x - rect.left,\n    y: event.center.y - rect.top\n  };\n\n  if (callback(onPanStart, [{chart, event, point}]) === false) {\n    return callback(onPanRejected, [{chart, event}]);\n  }\n\n  state.panScales = getEnabledScalesByPoint(state.options.pan, point, chart);\n  state.delta = {x: 0, y: 0};\n  clearTimeout(state.panEndTimeout);\n  handlePan(chart, state, event);\n}\n\nfunction endPan(chart, state) {\n  state.delta = null;\n  if (state.panning) {\n    state.panEndTimeout = setTimeout(() => (state.panning = false), 500);\n    callback(state.options.pan.onPanComplete, [{chart}]);\n  }\n}\n\nconst hammers = new WeakMap();\nfunction startHammer(chart, options) {\n  const state = getState(chart);\n  const canvas = chart.canvas;\n  const {pan: panOptions, zoom: zoomOptions} = options;\n\n  const mc = new Hammer.Manager(canvas);\n  if (zoomOptions && zoomOptions.pinch.enabled) {\n    mc.add(new Hammer.Pinch());\n    mc.on('pinchstart', () => startPinch(chart, state));\n    mc.on('pinch', (e) => handlePinch(chart, state, e));\n    mc.on('pinchend', (e) => endPinch(chart, state, e));\n  }\n\n  if (panOptions && panOptions.enabled) {\n    mc.add(new Hammer.Pan({\n      threshold: panOptions.threshold,\n      enable: createEnabler(chart, state)\n    }));\n    mc.on('panstart', (e) => startPan(chart, state, e));\n    mc.on('panmove', (e) => handlePan(chart, state, e));\n    mc.on('panend', () => endPan(chart, state));\n  }\n\n  hammers.set(chart, mc);\n}\n\nfunction stopHammer(chart) {\n  const mc = hammers.get(chart);\n  if (mc) {\n    mc.remove('pinchstart');\n    mc.remove('pinch');\n    mc.remove('pinchend');\n    mc.remove('panstart');\n    mc.remove('pan');\n    mc.remove('panend');\n    mc.destroy();\n    hammers.delete(chart);\n  }\n}\n\nvar version = \"2.0.1\";\n\nfunction draw(chart, caller, options) {\n  const dragOptions = options.zoom.drag;\n  const {dragStart, dragEnd} = getState(chart);\n\n  if (dragOptions.drawTime !== caller || !dragEnd) {\n    return;\n  }\n  const {left, top, width, height} = computeDragRect(chart, options.zoom.mode, dragStart, dragEnd);\n  const ctx = chart.ctx;\n\n  ctx.save();\n  ctx.beginPath();\n  ctx.fillStyle = dragOptions.backgroundColor || 'rgba(225,225,225,0.3)';\n  ctx.fillRect(left, top, width, height);\n\n  if (dragOptions.borderWidth > 0) {\n    ctx.lineWidth = dragOptions.borderWidth;\n    ctx.strokeStyle = dragOptions.borderColor || 'rgba(225,225,225)';\n    ctx.strokeRect(left, top, width, height);\n  }\n  ctx.restore();\n}\n\nvar plugin = {\n  id: 'zoom',\n\n  version,\n\n  defaults: {\n    pan: {\n      enabled: false,\n      mode: 'xy',\n      threshold: 10,\n      modifierKey: null,\n    },\n    zoom: {\n      wheel: {\n        enabled: false,\n        speed: 0.1,\n        modifierKey: null\n      },\n      drag: {\n        enabled: false,\n        drawTime: 'beforeDatasetsDraw',\n        modifierKey: null\n      },\n      pinch: {\n        enabled: false\n      },\n      mode: 'xy',\n    }\n  },\n\n  start: function(chart, _args, options) {\n    const state = getState(chart);\n    state.options = options;\n\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'enabled')) {\n      console.warn('The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`.');\n    }\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'overScaleMode')\n      || Object.prototype.hasOwnProperty.call(options.pan, 'overScaleMode')) {\n      console.warn('The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired).');\n    }\n\n    if (Hammer) {\n      startHammer(chart, options);\n    }\n\n    chart.pan = (delta, panScales, transition) => pan(chart, delta, panScales, transition);\n    chart.zoom = (args, transition) => zoom(chart, args, transition);\n    chart.zoomRect = (p0, p1, transition) => zoomRect(chart, p0, p1, transition);\n    chart.zoomScale = (id, range, transition) => zoomScale(chart, id, range, transition);\n    chart.resetZoom = (transition) => resetZoom(chart, transition);\n    chart.getZoomLevel = () => getZoomLevel(chart);\n    chart.getInitialScaleBounds = () => getInitialScaleBounds(chart);\n    chart.isZoomedOrPanned = () => isZoomedOrPanned(chart);\n  },\n\n  beforeEvent(chart) {\n    const state = getState(chart);\n    if (state.panning || state.dragging) {\n      // cancel any event handling while panning or dragging\n      return false;\n    }\n  },\n\n  beforeUpdate: function(chart, args, options) {\n    const state = getState(chart);\n    state.options = options;\n    addListeners(chart, options);\n  },\n\n  beforeDatasetsDraw(chart, _args, options) {\n    draw(chart, 'beforeDatasetsDraw', options);\n  },\n\n  afterDatasetsDraw(chart, _args, options) {\n    draw(chart, 'afterDatasetsDraw', options);\n  },\n\n  beforeDraw(chart, _args, options) {\n    draw(chart, 'beforeDraw', options);\n  },\n\n  afterDraw(chart, _args, options) {\n    draw(chart, 'afterDraw', options);\n  },\n\n  stop: function(chart) {\n    removeListeners(chart);\n\n    if (Hammer) {\n      stopHammer(chart);\n    }\n    removeState(chart);\n  },\n\n  panFunctions,\n  zoomFunctions,\n  zoomRectFunctions,\n};\n\nexport { plugin as default, pan, resetZoom, zoom, zoomRect, zoomScale };\n",
         "import type { MouseEvent } from 'react';\nimport type {\n  ChartType,\n  ChartData,\n  DefaultDataPoint,\n  ChartDataset,\n  ChartOptions,\n  Chart,\n} from 'chart.js';\n\nimport type { ForwardedRef } from './types.js';\n\nconst defaultDatasetIdKey = 'label';\n\nexport function reforwardRef<T>(ref: ForwardedRef<T>, value: T) {\n  if (typeof ref === 'function') {\n    ref(value);\n  } else if (ref) {\n    ref.current = value;\n  }\n}\n\nexport function setOptions<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(chart: Chart<TType, TData, TLabel>, nextOptions: ChartOptions<TType>) {\n  const options = chart.options;\n\n  if (options && nextOptions) {\n    Object.assign(options, nextOptions);\n  }\n}\n\nexport function setLabels<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  currentData: ChartData<TType, TData, TLabel>,\n  nextLabels: TLabel[] | undefined\n) {\n  currentData.labels = nextLabels;\n}\n\nexport function setDatasets<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  currentData: ChartData<TType, TData, TLabel>,\n  nextDatasets: ChartDataset<TType, TData>[],\n  datasetIdKey = defaultDatasetIdKey\n) {\n  const addedDatasets: ChartDataset<TType, TData>[] = [];\n\n  currentData.datasets = nextDatasets.map(\n    (nextDataset: Record<string, unknown>) => {\n      // given the new set, find it's current match\n      const currentDataset = currentData.datasets.find(\n        (dataset: Record<string, unknown>) =>\n          dataset[datasetIdKey] === nextDataset[datasetIdKey]\n      );\n\n      // There is no original to update, so simply add new one\n      if (\n        !currentDataset ||\n        !nextDataset.data ||\n        addedDatasets.includes(currentDataset)\n      ) {\n        return { ...nextDataset } as ChartDataset<TType, TData>;\n      }\n\n      addedDatasets.push(currentDataset);\n\n      Object.assign(currentDataset, nextDataset);\n\n      return currentDataset;\n    }\n  );\n}\n\nexport function cloneData<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(data: ChartData<TType, TData, TLabel>, datasetIdKey = defaultDatasetIdKey) {\n  const nextData: ChartData<TType, TData, TLabel> = {\n    labels: [],\n    datasets: [],\n  };\n\n  setLabels(nextData, data.labels);\n  setDatasets(nextData, data.datasets, datasetIdKey);\n\n  return nextData;\n}\n\n/**\n * Get dataset from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getDatasetAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'dataset',\n    { intersect: true },\n    false\n  );\n}\n\n/**\n * Get single dataset element from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getElementAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'nearest',\n    { intersect: true },\n    false\n  );\n}\n\n/**\n * Get all dataset elements from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getElementsAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'index',\n    { intersect: true },\n    false\n  );\n}\n",
         "import React, { useEffect, useRef, forwardRef } from 'react';\nimport { Chart as ChartJS } from 'chart.js';\nimport type { ChartType, DefaultDataPoint } from 'chart.js';\n\nimport type { ForwardedRef, ChartProps, BaseChartComponent } from './types.js';\nimport {\n  reforwardRef,\n  cloneData,\n  setOptions,\n  setLabels,\n  setDatasets,\n} from './utils.js';\n\nfunction ChartComponent<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  props: ChartProps<TType, TData, TLabel>,\n  ref: ForwardedRef<ChartJS<TType, TData, TLabel>>\n) {\n  const {\n    height = 150,\n    width = 300,\n    redraw = false,\n    datasetIdKey,\n    type,\n    data,\n    options,\n    plugins = [],\n    fallbackContent,\n    updateMode,\n    ...canvasProps\n  } = props as ChartProps;\n  const canvasRef = useRef<HTMLCanvasElement>(null);\n  const chartRef = useRef<ChartJS | null>();\n\n  const renderChart = () => {\n    if (!canvasRef.current) return;\n\n    chartRef.current = new ChartJS(canvasRef.current, {\n      type,\n      data: cloneData(data, datasetIdKey),\n      options: options && { ...options },\n      plugins,\n    });\n\n    reforwardRef(ref, chartRef.current);\n  };\n\n  const destroyChart = () => {\n    reforwardRef(ref, null);\n\n    if (chartRef.current) {\n      chartRef.current.destroy();\n      chartRef.current = null;\n    }\n  };\n\n  useEffect(() => {\n    if (!redraw && chartRef.current && options) {\n      setOptions(chartRef.current, options);\n    }\n  }, [redraw, options]);\n\n  useEffect(() => {\n    if (!redraw && chartRef.current) {\n      setLabels(chartRef.current.config.data, data.labels);\n    }\n  }, [redraw, data.labels]);\n\n  useEffect(() => {\n    if (!redraw && chartRef.current && data.datasets) {\n      setDatasets(chartRef.current.config.data, data.datasets, datasetIdKey);\n    }\n  }, [redraw, data.datasets]);\n\n  useEffect(() => {\n    if (!chartRef.current) return;\n\n    if (redraw) {\n      destroyChart();\n      setTimeout(renderChart);\n    } else {\n      chartRef.current.update(updateMode);\n    }\n  }, [redraw, options, data.labels, data.datasets, updateMode]);\n\n  useEffect(() => {\n    if (!chartRef.current) return;\n\n    destroyChart();\n    setTimeout(renderChart);\n  }, [type]);\n\n  useEffect(() => {\n    renderChart();\n\n    return () => destroyChart();\n  }, []);\n\n  return (\n    <canvas\n      ref={canvasRef}\n      role='img'\n      height={height}\n      width={width}\n      {...canvasProps}\n    >\n      {fallbackContent}\n    </canvas>\n  );\n}\n\nexport const Chart = forwardRef(ChartComponent) as BaseChartComponent;\n",
         "import React, { forwardRef } from 'react';\nimport {\n  Chart as ChartJS,\n  LineController,\n  BarController,\n  RadarController,\n  DoughnutController,\n  PolarAreaController,\n  BubbleController,\n  PieController,\n  ScatterController,\n} from 'chart.js';\nimport type { ChartType, ChartComponentLike } from 'chart.js';\n\nimport type {\n  ChartProps,\n  ChartJSOrUndefined,\n  TypedChartComponent,\n} from './types.js';\nimport { Chart } from './chart.js';\n\nfunction createTypedChart<T extends ChartType>(\n  type: T,\n  registerables: ChartComponentLike\n) {\n  ChartJS.register(registerables);\n\n  return forwardRef<ChartJSOrUndefined<T>, Omit<ChartProps<T>, 'type'>>(\n    (props, ref) => <Chart {...props} ref={ref} type={type} />\n  ) as TypedChartComponent<T>;\n}\n\nexport const Line = /* #__PURE__ */ createTypedChart('line', LineController);\n\nexport const Bar = /* #__PURE__ */ createTypedChart('bar', BarController);\n\nexport const Radar = /* #__PURE__ */ createTypedChart('radar', RadarController);\n\nexport const Doughnut = /* #__PURE__ */ createTypedChart(\n  'doughnut',\n  DoughnutController\n);\n\nexport const PolarArea = /* #__PURE__ */ createTypedChart(\n  'polarArea',\n  PolarAreaController\n);\n\nexport const Bubble = /* #__PURE__ */ createTypedChart(\n  'bubble',\n  BubbleController\n);\n\nexport const Pie = /* #__PURE__ */ createTypedChart('pie', PieController);\n\nexport const Scatter = /* #__PURE__ */ createTypedChart(\n  'scatter',\n  ScatterController\n);\n",
         "export function createChartData(data, options) {\r\n  const xLabels = Object.keys(data[Object.keys(data)[0]].data)\r\n  const datasets = Object.entries(data).map(([colName, colData], index) => {\r\n    return {\r\n      showLine: options.show_line,\r\n      data: colData.data,\r\n      label: colName,\r\n      lineTension: options.tension,\r\n      cubicInterpolationMode: \"default\",\r\n      spanGaps: options.fill_gaps,\r\n      backgroundColor: colData.color,\r\n      borderColor: colData.color,\r\n      pointRadius: colData.point_radius,\r\n      borderDash: colData.border_dash,\r\n    }\r\n  })\r\n\r\n  return {\r\n    labels: xLabels,\r\n    datasets: datasets,\r\n  }\r\n}\r\n",
-        "import { Chart } from \"chart.js\"\r\n\r\nexport function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    indexAxis: \"x\",\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    onHover: createHoverOptions(options),\r\n    plugins: {\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(options),\r\n      tooltip: createTooltipOptions(options, theme),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions(options) {\r\n  return (event, chartElement) => {\r\n    let cursorStyle = \"default\"\r\n    if (chartElement.length > 0) {\r\n      const datasets = event.chart.data.datasets\r\n      const label = datasets[chartElement[0].datasetIndex].label\r\n      cursorStyle = determineCursorStyle(label, options)\r\n    }\r\n    event.native.target.style.cursor = cursorStyle\r\n  }\r\n}\r\n\r\nfunction determineCursorStyle(label, options) {\r\n  if (options.fixed_lines.includes(label)) {\r\n    return \"default\"\r\n  }\r\n  return \"crosshair\"\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"xy\",\r\n    },\r\n    pan: {\r\n      enabled: true,\r\n    },\r\n    limits: {\r\n      x: { min: \"original\", max: \"original\" },\r\n      y: { min: \"original\", max: \"original\" },\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: Boolean(options.title),\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions(options) {\r\n  return {\r\n    display: options.legend,\r\n    position: options.legend_position,\r\n    align: options.legend_align,\r\n    labels: {\r\n      boxWidth: 16,\r\n      boxHeight: 8,\r\n      padding: 8,\r\n      generateLabels: function (chart) {\r\n        const labels =\r\n          Chart.defaults.plugins.legend.labels.generateLabels(chart)\r\n        labels.forEach((label) => {\r\n          if (options.labels.hasOwnProperty(label.text)) {\r\n            label.text = options.labels[label.text]\r\n          }\r\n          if (\r\n            options.labels.hasOwnProperty(label.text.replace(\" (bezier)\", \"\"))\r\n          ) {\r\n            label.text =\r\n              options.labels[label.text.replace(\" (bezier)\", \"\")] + \" (bezier)\"\r\n          }\r\n        })\r\n        return labels\r\n      },\r\n    },\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  const xScaleOptions = {\r\n    display: true,\r\n    type: options.x_type,\r\n    title: {\r\n      display: Boolean(options.x_label),\r\n      text: options.x_label,\r\n    },\r\n    grid: {\r\n      display: options.x_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.x_labels) {\r\n    xScaleOptions.min = options.x_labels[0]\r\n    xScaleOptions.max = options.x_labels[options.x_labels.length - 1]\r\n  }\r\n\r\n  const yScaleOptions = {\r\n    display: true,\r\n    type: options.y_type,\r\n    title: {\r\n      display: Boolean(options.y_label),\r\n      text: options.y_label,\r\n    },\r\n    grid: {\r\n      display: options.y_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.y_labels) {\r\n    yScaleOptions.labels = options.y_labels\r\n    yScaleOptions.min = options.y_labels[0]\r\n    yScaleOptions.max = options.y_labels[options.y_labels.length - 1]\r\n  }\r\n\r\n  return {\r\n    x: xScaleOptions,\r\n    y: yScaleOptions,\r\n  }\r\n}\r\n\r\nfunction createTooltipOptions(options, theme) {\r\n  return {\r\n    filter: function (data) {\r\n      const pointRadius = data.dataset.pointRadius\r\n      return pointRadius !== 0\r\n    },\r\n    callbacks: {\r\n      title: function (data) {\r\n        if (data.length === 0) {\r\n          return \"\"\r\n        }\r\n        const label = data[0].dataset.label\r\n        if (options.labels.hasOwnProperty(label)) {\r\n          return `${options.labels[label]}`\r\n        }\r\n        return `${label}`\r\n      },\r\n      label: function (event) {\r\n        const Xvalue = event.parsed.x.toFixed(2)\r\n        const Yvalue = event.parsed.y.toFixed(2)\r\n        return `${Xvalue}, ${Yvalue}`\r\n      },\r\n    },\r\n  }\r\n}\r\n",
+        "import { Chart } from \"chart.js\"\r\nimport millify from \"millify\"\r\n\r\nexport function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    indexAxis: \"x\",\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    onHover: createHoverOptions(options),\r\n    plugins: {\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(options),\r\n      tooltip: createTooltipOptions(options, theme),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions(options) {\r\n  return (event, chartElement) => {\r\n    let cursorStyle = \"default\"\r\n    if (chartElement.length > 0) {\r\n      const datasets = event.chart.data.datasets\r\n      const label = datasets[chartElement[0].datasetIndex].label\r\n      cursorStyle = determineCursorStyle(label, options)\r\n    }\r\n    event.native.target.style.cursor = cursorStyle\r\n  }\r\n}\r\n\r\nfunction determineCursorStyle(label, options) {\r\n  if (options.fixed_lines.includes(label)) {\r\n    return \"default\"\r\n  }\r\n  return \"crosshair\"\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"xy\",\r\n    },\r\n    pan: {\r\n      enabled: true,\r\n    },\r\n    limits: {\r\n      x: { min: \"original\", max: \"original\" },\r\n      y: { min: \"original\", max: \"original\" },\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: Boolean(options.title),\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions(options) {\r\n  return {\r\n    display: options.legend,\r\n    position: options.legend_position,\r\n    align: options.legend_align,\r\n    labels: {\r\n      boxWidth: 16,\r\n      boxHeight: 8,\r\n      padding: 8,\r\n      generateLabels: function (chart) {\r\n        const labels =\r\n          Chart.defaults.plugins.legend.labels.generateLabels(chart)\r\n        labels.forEach((label) => {\r\n          if (options.labels.hasOwnProperty(label.text)) {\r\n            label.text = options.labels[label.text]\r\n          }\r\n          if (\r\n            options.labels.hasOwnProperty(label.text.replace(\" (bezier)\", \"\"))\r\n          ) {\r\n            label.text =\r\n              options.labels[label.text.replace(\" (bezier)\", \"\")] + \" (bezier)\"\r\n          }\r\n        })\r\n        return labels\r\n      },\r\n    },\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction formatTickValue(val, index, options) {\r\n  if (options.x_type === \"linear\") {\r\n    return millify(val);\r\n  }\r\n  return this.getLabelForValue(val);\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  const xScaleOptions = {\r\n    display: true,\r\n    type: options.x_type,\r\n    ticks: {\r\n      callback: function(val, index) {\r\n        return formatTickValue.call(this, val, index, options);\r\n      },\r\n    },\r\n    title: {\r\n      display: Boolean(options.x_label),\r\n      text: options.x_label,\r\n    },\r\n    grid: {\r\n      display: options.x_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.x_labels) {\r\n    xScaleOptions.min = options.x_labels[0]\r\n    xScaleOptions.max = options.x_labels[options.x_labels.length - 1]\r\n  }\r\n\r\n  const yScaleOptions = {\r\n    display: true,\r\n    type: options.y_type,\r\n    ticks: {\r\n      callback: function(val, index) {\r\n        return formatTickValue.call(this, val, index, options);\r\n      },\r\n    },\r\n    title: {\r\n      display: Boolean(options.y_label),\r\n      text: options.y_label,\r\n    },\r\n    grid: {\r\n      display: options.y_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.y_labels) {\r\n    yScaleOptions.labels = options.y_labels\r\n    yScaleOptions.min = options.y_labels[0]\r\n    yScaleOptions.max = options.y_labels[options.y_labels.length - 1]\r\n  }\r\n\r\n  return {\r\n    x: xScaleOptions,\r\n    y: yScaleOptions,\r\n  }\r\n}\r\n\r\nfunction createTooltipOptions(options, theme) {\r\n  return {\r\n    filter: function (data) {\r\n      const pointRadius = data.dataset.pointRadius\r\n      return pointRadius !== 0\r\n    },\r\n    callbacks: {\r\n      title: function (data) {\r\n        if (data.length === 0) {\r\n          return \"\"\r\n        }\r\n        const label = data[0].dataset.label\r\n        if (options.labels.hasOwnProperty(label)) {\r\n          return `${options.labels[label]}`\r\n        }\r\n        return `${label}`\r\n      },\r\n      label: function (event) {\r\n        const Xvalue = event.parsed.x.toFixed(2)\r\n        const Yvalue = event.parsed.y.toFixed(2)\r\n        return `${Xvalue}, ${Yvalue}`\r\n      },\r\n    },\r\n  }\r\n}\r\n",
         "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\nimport { Line, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass LineChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const datasetLabel =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex].label\r\n      if (\r\n        this.props.args.options.fixed_lines &&\r\n        this.props.args.options.fixed_lines.includes(datasetLabel)\r\n      ) {\r\n        // This line is fixed, so don't allow it to be moved\r\n        return\r\n      }\r\n      this.setState({ activePoint: points[0] })\r\n      this.togglePan(false)\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n      const yAxis = chart.scales.y\r\n      const yValue = this.map(\r\n        position.y,\r\n        chartArea.bottom,\r\n        chartArea.top,\r\n        yAxis.min,\r\n        yAxis.max\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ] = yValue\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const datasetIndex = this.state.activePoint.datasetIndex\r\n      const pointIndex = this.state.activePoint.index\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xLabel = this.state.chartData.labels[pointIndex]\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex]\r\n\r\n      this.state.originalData[datasetLabel][\"data\"][xLabel] = yValue\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n      Streamlit.setComponentValue(this.state.originalData)\r\n    }\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Line\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default LineChart\r\n",
         "export function createChartData(data, options) {\r\n  const xLabels = options && options.x_labels ? options.x_labels : []\r\n  const datasets = Object.entries(data).map(([colName, colData], index) => {\r\n    const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n    return {\r\n      showLine: options.show_line,\r\n      data: data,\r\n      label: colName,\r\n      lineTension: options.tension,\r\n      cubicInterpolationMode: \"default\",\r\n      spanGaps: options.fill_gaps,\r\n      backgroundColor: colData.color,\r\n      borderColor: colData.color,\r\n      pointRadius: colData.point_radius,\r\n      borderDash: colData.border_dash,\r\n    }\r\n  })\r\n\r\n  return {\r\n    labels: xLabels,\r\n    datasets: datasets,\r\n  }\r\n}\r\n",
         "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass ScatterChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const datasetLabel =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex].label\r\n      if (\r\n        this.props.args.options.fixed_lines &&\r\n        this.props.args.options.fixed_lines.includes(datasetLabel)\r\n      ) {\r\n        // This line is fixed, so don't allow it to be moved\r\n        return\r\n      }\r\n      this.setState({ activePoint: points[0] })\r\n      this.togglePan(false)\r\n    }\r\n  }\r\n\r\n  calculateNewYValue = (position, chartArea, yAxis) => {\r\n    if (this.props.args.options.y_type === \"category\") {\r\n      const categories = yAxis.getLabels()\r\n      const categoryIndex = Math.round(\r\n        this.map(\r\n          position.y,\r\n          chartArea.top,\r\n          chartArea.bottom,\r\n          0,\r\n          categories.length - 1\r\n        )\r\n      )\r\n      return categories[categoryIndex]\r\n    } else {\r\n      return this.map(\r\n        position.y,\r\n        chartArea.bottom,\r\n        chartArea.top,\r\n        yAxis.min,\r\n        yAxis.max\r\n      )\r\n    }\r\n  }\r\n\r\n  calculateNewXValue = (position, chartArea, xAxis) => {\r\n    if (this.props.args.options.x_type === \"category\") {\r\n      const categories = xAxis.getLabels()\r\n      const categoryIndex = Math.round(\r\n        this.map(\r\n          position.x,\r\n          chartArea.left,\r\n          chartArea.right,\r\n          0,\r\n          categories.length - 1\r\n        )\r\n      )\r\n      return categories[categoryIndex]\r\n    } else {\r\n      return this.map(\r\n        position.x,\r\n        chartArea.left,\r\n        chartArea.right,\r\n        xAxis.min,\r\n        xAxis.max\r\n      )\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = this.calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y\r\n      )\r\n\r\n      const newXValue = this.calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ].y = newYValue\r\n\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ].x = newXValue\r\n\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const datasetIndex = this.state.activePoint.datasetIndex\r\n      const pointIndex = this.state.activePoint.index\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n\r\n      this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n      this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n      Streamlit.setComponentValue(this.state.originalData)\r\n\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default ScatterChart\r\n",
         "import { Bezier } from \"./bezier.js\";\n\n// math-inlining.\nconst { abs, cos, sin, acos, atan2, sqrt, pow } = Math;\n\n// cube root function yielding real roots\nfunction crt(v) {\n  return v < 0 ? -pow(-v, 1 / 3) : pow(v, 1 / 3);\n}\n\n// trig constants\nconst pi = Math.PI,\n  tau = 2 * pi,\n  quart = pi / 2,\n  // float precision significant decimal\n  epsilon = 0.000001,\n  // extremas used in bbox calculation and similar algorithms\n  nMax = Number.MAX_SAFE_INTEGER || 9007199254740991,\n  nMin = Number.MIN_SAFE_INTEGER || -9007199254740991,\n  // a zero coordinate, which is surprisingly useful\n  ZERO = { x: 0, y: 0, z: 0 };\n\n// Bezier utility functions\nconst utils = {\n  // Legendre-Gauss abscissae with n=24 (x_i values, defined at i=n as the roots of the nth order Legendre polynomial Pn(x))\n  Tvalues: [\n    -0.0640568928626056260850430826247450385909,\n    0.0640568928626056260850430826247450385909,\n    -0.1911188674736163091586398207570696318404,\n    0.1911188674736163091586398207570696318404,\n    -0.3150426796961633743867932913198102407864,\n    0.3150426796961633743867932913198102407864,\n    -0.4337935076260451384870842319133497124524,\n    0.4337935076260451384870842319133497124524,\n    -0.5454214713888395356583756172183723700107,\n    0.5454214713888395356583756172183723700107,\n    -0.6480936519369755692524957869107476266696,\n    0.6480936519369755692524957869107476266696,\n    -0.7401241915785543642438281030999784255232,\n    0.7401241915785543642438281030999784255232,\n    -0.8200019859739029219539498726697452080761,\n    0.8200019859739029219539498726697452080761,\n    -0.8864155270044010342131543419821967550873,\n    0.8864155270044010342131543419821967550873,\n    -0.9382745520027327585236490017087214496548,\n    0.9382745520027327585236490017087214496548,\n    -0.9747285559713094981983919930081690617411,\n    0.9747285559713094981983919930081690617411,\n    -0.9951872199970213601799974097007368118745,\n    0.9951872199970213601799974097007368118745,\n  ],\n\n  // Legendre-Gauss weights with n=24 (w_i values, defined by a function linked to in the Bezier primer article)\n  Cvalues: [\n    0.1279381953467521569740561652246953718517,\n    0.1279381953467521569740561652246953718517,\n    0.1258374563468282961213753825111836887264,\n    0.1258374563468282961213753825111836887264,\n    0.121670472927803391204463153476262425607,\n    0.121670472927803391204463153476262425607,\n    0.1155056680537256013533444839067835598622,\n    0.1155056680537256013533444839067835598622,\n    0.1074442701159656347825773424466062227946,\n    0.1074442701159656347825773424466062227946,\n    0.0976186521041138882698806644642471544279,\n    0.0976186521041138882698806644642471544279,\n    0.086190161531953275917185202983742667185,\n    0.086190161531953275917185202983742667185,\n    0.0733464814110803057340336152531165181193,\n    0.0733464814110803057340336152531165181193,\n    0.0592985849154367807463677585001085845412,\n    0.0592985849154367807463677585001085845412,\n    0.0442774388174198061686027482113382288593,\n    0.0442774388174198061686027482113382288593,\n    0.0285313886289336631813078159518782864491,\n    0.0285313886289336631813078159518782864491,\n    0.0123412297999871995468056670700372915759,\n    0.0123412297999871995468056670700372915759,\n  ],\n\n  arcfn: function (t, derivativeFn) {\n    const d = derivativeFn(t);\n    let l = d.x * d.x + d.y * d.y;\n    if (typeof d.z !== \"undefined\") {\n      l += d.z * d.z;\n    }\n    return sqrt(l);\n  },\n\n  compute: function (t, points, _3d) {\n    // shortcuts\n    if (t === 0) {\n      points[0].t = 0;\n      return points[0];\n    }\n\n    const order = points.length - 1;\n\n    if (t === 1) {\n      points[order].t = 1;\n      return points[order];\n    }\n\n    const mt = 1 - t;\n    let p = points;\n\n    // constant?\n    if (order === 0) {\n      points[0].t = t;\n      return points[0];\n    }\n\n    // linear?\n    if (order === 1) {\n      const ret = {\n        x: mt * p[0].x + t * p[1].x,\n        y: mt * p[0].y + t * p[1].y,\n        t: t,\n      };\n      if (_3d) {\n        ret.z = mt * p[0].z + t * p[1].z;\n      }\n      return ret;\n    }\n\n    // quadratic/cubic curve?\n    if (order < 4) {\n      let mt2 = mt * mt,\n        t2 = t * t,\n        a,\n        b,\n        c,\n        d = 0;\n      if (order === 2) {\n        p = [p[0], p[1], p[2], ZERO];\n        a = mt2;\n        b = mt * t * 2;\n        c = t2;\n      } else if (order === 3) {\n        a = mt2 * mt;\n        b = mt2 * t * 3;\n        c = mt * t2 * 3;\n        d = t * t2;\n      }\n      const ret = {\n        x: a * p[0].x + b * p[1].x + c * p[2].x + d * p[3].x,\n        y: a * p[0].y + b * p[1].y + c * p[2].y + d * p[3].y,\n        t: t,\n      };\n      if (_3d) {\n        ret.z = a * p[0].z + b * p[1].z + c * p[2].z + d * p[3].z;\n      }\n      return ret;\n    }\n\n    // higher order curves: use de Casteljau's computation\n    const dCpts = JSON.parse(JSON.stringify(points));\n    while (dCpts.length > 1) {\n      for (let i = 0; i < dCpts.length - 1; i++) {\n        dCpts[i] = {\n          x: dCpts[i].x + (dCpts[i + 1].x - dCpts[i].x) * t,\n          y: dCpts[i].y + (dCpts[i + 1].y - dCpts[i].y) * t,\n        };\n        if (typeof dCpts[i].z !== \"undefined\") {\n          dCpts[i].z = dCpts[i].z + (dCpts[i + 1].z - dCpts[i].z) * t;\n        }\n      }\n      dCpts.splice(dCpts.length - 1, 1);\n    }\n    dCpts[0].t = t;\n    return dCpts[0];\n  },\n\n  computeWithRatios: function (t, points, ratios, _3d) {\n    const mt = 1 - t,\n      r = ratios,\n      p = points;\n\n    let f1 = r[0],\n      f2 = r[1],\n      f3 = r[2],\n      f4 = r[3],\n      d;\n\n    // spec for linear\n    f1 *= mt;\n    f2 *= t;\n\n    if (p.length === 2) {\n      d = f1 + f2;\n      return {\n        x: (f1 * p[0].x + f2 * p[1].x) / d,\n        y: (f1 * p[0].y + f2 * p[1].y) / d,\n        z: !_3d ? false : (f1 * p[0].z + f2 * p[1].z) / d,\n        t: t,\n      };\n    }\n\n    // upgrade to quadratic\n    f1 *= mt;\n    f2 *= 2 * mt;\n    f3 *= t * t;\n\n    if (p.length === 3) {\n      d = f1 + f2 + f3;\n      return {\n        x: (f1 * p[0].x + f2 * p[1].x + f3 * p[2].x) / d,\n        y: (f1 * p[0].y + f2 * p[1].y + f3 * p[2].y) / d,\n        z: !_3d ? false : (f1 * p[0].z + f2 * p[1].z + f3 * p[2].z) / d,\n        t: t,\n      };\n    }\n\n    // upgrade to cubic\n    f1 *= mt;\n    f2 *= 1.5 * mt;\n    f3 *= 3 * mt;\n    f4 *= t * t * t;\n\n    if (p.length === 4) {\n      d = f1 + f2 + f3 + f4;\n      return {\n        x: (f1 * p[0].x + f2 * p[1].x + f3 * p[2].x + f4 * p[3].x) / d,\n        y: (f1 * p[0].y + f2 * p[1].y + f3 * p[2].y + f4 * p[3].y) / d,\n        z: !_3d\n          ? false\n          : (f1 * p[0].z + f2 * p[1].z + f3 * p[2].z + f4 * p[3].z) / d,\n        t: t,\n      };\n    }\n  },\n\n  derive: function (points, _3d) {\n    const dpoints = [];\n    for (let p = points, d = p.length, c = d - 1; d > 1; d--, c--) {\n      const list = [];\n      for (let j = 0, dpt; j < c; j++) {\n        dpt = {\n          x: c * (p[j + 1].x - p[j].x),\n          y: c * (p[j + 1].y - p[j].y),\n        };\n        if (_3d) {\n          dpt.z = c * (p[j + 1].z - p[j].z);\n        }\n        list.push(dpt);\n      }\n      dpoints.push(list);\n      p = list;\n    }\n    return dpoints;\n  },\n\n  between: function (v, m, M) {\n    return (\n      (m <= v && v <= M) ||\n      utils.approximately(v, m) ||\n      utils.approximately(v, M)\n    );\n  },\n\n  approximately: function (a, b, precision) {\n    return abs(a - b) <= (precision || epsilon);\n  },\n\n  length: function (derivativeFn) {\n    const z = 0.5,\n      len = utils.Tvalues.length;\n\n    let sum = 0;\n\n    for (let i = 0, t; i < len; i++) {\n      t = z * utils.Tvalues[i] + z;\n      sum += utils.Cvalues[i] * utils.arcfn(t, derivativeFn);\n    }\n    return z * sum;\n  },\n\n  map: function (v, ds, de, ts, te) {\n    const d1 = de - ds,\n      d2 = te - ts,\n      v2 = v - ds,\n      r = v2 / d1;\n    return ts + d2 * r;\n  },\n\n  lerp: function (r, v1, v2) {\n    const ret = {\n      x: v1.x + r * (v2.x - v1.x),\n      y: v1.y + r * (v2.y - v1.y),\n    };\n    if (v1.z !== undefined && v2.z !== undefined) {\n      ret.z = v1.z + r * (v2.z - v1.z);\n    }\n    return ret;\n  },\n\n  pointToString: function (p) {\n    let s = p.x + \"/\" + p.y;\n    if (typeof p.z !== \"undefined\") {\n      s += \"/\" + p.z;\n    }\n    return s;\n  },\n\n  pointsToString: function (points) {\n    return \"[\" + points.map(utils.pointToString).join(\", \") + \"]\";\n  },\n\n  copy: function (obj) {\n    return JSON.parse(JSON.stringify(obj));\n  },\n\n  angle: function (o, v1, v2) {\n    const dx1 = v1.x - o.x,\n      dy1 = v1.y - o.y,\n      dx2 = v2.x - o.x,\n      dy2 = v2.y - o.y,\n      cross = dx1 * dy2 - dy1 * dx2,\n      dot = dx1 * dx2 + dy1 * dy2;\n    return atan2(cross, dot);\n  },\n\n  // round as string, to avoid rounding errors\n  round: function (v, d) {\n    const s = \"\" + v;\n    const pos = s.indexOf(\".\");\n    return parseFloat(s.substring(0, pos + 1 + d));\n  },\n\n  dist: function (p1, p2) {\n    const dx = p1.x - p2.x,\n      dy = p1.y - p2.y;\n    return sqrt(dx * dx + dy * dy);\n  },\n\n  closest: function (LUT, point) {\n    let mdist = pow(2, 63),\n      mpos,\n      d;\n    LUT.forEach(function (p, idx) {\n      d = utils.dist(point, p);\n      if (d < mdist) {\n        mdist = d;\n        mpos = idx;\n      }\n    });\n    return { mdist: mdist, mpos: mpos };\n  },\n\n  abcratio: function (t, n) {\n    // see ratio(t) note on http://pomax.github.io/bezierinfo/#abc\n    if (n !== 2 && n !== 3) {\n      return false;\n    }\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    } else if (t === 0 || t === 1) {\n      return t;\n    }\n    const bottom = pow(t, n) + pow(1 - t, n),\n      top = bottom - 1;\n    return abs(top / bottom);\n  },\n\n  projectionratio: function (t, n) {\n    // see u(t) note on http://pomax.github.io/bezierinfo/#abc\n    if (n !== 2 && n !== 3) {\n      return false;\n    }\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    } else if (t === 0 || t === 1) {\n      return t;\n    }\n    const top = pow(1 - t, n),\n      bottom = pow(t, n) + top;\n    return top / bottom;\n  },\n\n  lli8: function (x1, y1, x2, y2, x3, y3, x4, y4) {\n    const nx =\n        (x1 * y2 - y1 * x2) * (x3 - x4) - (x1 - x2) * (x3 * y4 - y3 * x4),\n      ny = (x1 * y2 - y1 * x2) * (y3 - y4) - (y1 - y2) * (x3 * y4 - y3 * x4),\n      d = (x1 - x2) * (y3 - y4) - (y1 - y2) * (x3 - x4);\n    if (d == 0) {\n      return false;\n    }\n    return { x: nx / d, y: ny / d };\n  },\n\n  lli4: function (p1, p2, p3, p4) {\n    const x1 = p1.x,\n      y1 = p1.y,\n      x2 = p2.x,\n      y2 = p2.y,\n      x3 = p3.x,\n      y3 = p3.y,\n      x4 = p4.x,\n      y4 = p4.y;\n    return utils.lli8(x1, y1, x2, y2, x3, y3, x4, y4);\n  },\n\n  lli: function (v1, v2) {\n    return utils.lli4(v1, v1.c, v2, v2.c);\n  },\n\n  makeline: function (p1, p2) {\n    return new Bezier(\n      p1.x,\n      p1.y,\n      (p1.x + p2.x) / 2,\n      (p1.y + p2.y) / 2,\n      p2.x,\n      p2.y\n    );\n  },\n\n  findbbox: function (sections) {\n    let mx = nMax,\n      my = nMax,\n      MX = nMin,\n      MY = nMin;\n    sections.forEach(function (s) {\n      const bbox = s.bbox();\n      if (mx > bbox.x.min) mx = bbox.x.min;\n      if (my > bbox.y.min) my = bbox.y.min;\n      if (MX < bbox.x.max) MX = bbox.x.max;\n      if (MY < bbox.y.max) MY = bbox.y.max;\n    });\n    return {\n      x: { min: mx, mid: (mx + MX) / 2, max: MX, size: MX - mx },\n      y: { min: my, mid: (my + MY) / 2, max: MY, size: MY - my },\n    };\n  },\n\n  shapeintersections: function (\n    s1,\n    bbox1,\n    s2,\n    bbox2,\n    curveIntersectionThreshold\n  ) {\n    if (!utils.bboxoverlap(bbox1, bbox2)) return [];\n    const intersections = [];\n    const a1 = [s1.startcap, s1.forward, s1.back, s1.endcap];\n    const a2 = [s2.startcap, s2.forward, s2.back, s2.endcap];\n    a1.forEach(function (l1) {\n      if (l1.virtual) return;\n      a2.forEach(function (l2) {\n        if (l2.virtual) return;\n        const iss = l1.intersects(l2, curveIntersectionThreshold);\n        if (iss.length > 0) {\n          iss.c1 = l1;\n          iss.c2 = l2;\n          iss.s1 = s1;\n          iss.s2 = s2;\n          intersections.push(iss);\n        }\n      });\n    });\n    return intersections;\n  },\n\n  makeshape: function (forward, back, curveIntersectionThreshold) {\n    const bpl = back.points.length;\n    const fpl = forward.points.length;\n    const start = utils.makeline(back.points[bpl - 1], forward.points[0]);\n    const end = utils.makeline(forward.points[fpl - 1], back.points[0]);\n    const shape = {\n      startcap: start,\n      forward: forward,\n      back: back,\n      endcap: end,\n      bbox: utils.findbbox([start, forward, back, end]),\n    };\n    shape.intersections = function (s2) {\n      return utils.shapeintersections(\n        shape,\n        shape.bbox,\n        s2,\n        s2.bbox,\n        curveIntersectionThreshold\n      );\n    };\n    return shape;\n  },\n\n  getminmax: function (curve, d, list) {\n    if (!list) return { min: 0, max: 0 };\n    let min = nMax,\n      max = nMin,\n      t,\n      c;\n    if (list.indexOf(0) === -1) {\n      list = [0].concat(list);\n    }\n    if (list.indexOf(1) === -1) {\n      list.push(1);\n    }\n    for (let i = 0, len = list.length; i < len; i++) {\n      t = list[i];\n      c = curve.get(t);\n      if (c[d] < min) {\n        min = c[d];\n      }\n      if (c[d] > max) {\n        max = c[d];\n      }\n    }\n    return { min: min, mid: (min + max) / 2, max: max, size: max - min };\n  },\n\n  align: function (points, line) {\n    const tx = line.p1.x,\n      ty = line.p1.y,\n      a = -atan2(line.p2.y - ty, line.p2.x - tx),\n      d = function (v) {\n        return {\n          x: (v.x - tx) * cos(a) - (v.y - ty) * sin(a),\n          y: (v.x - tx) * sin(a) + (v.y - ty) * cos(a),\n        };\n      };\n    return points.map(d);\n  },\n\n  roots: function (points, line) {\n    line = line || { p1: { x: 0, y: 0 }, p2: { x: 1, y: 0 } };\n\n    const order = points.length - 1;\n    const aligned = utils.align(points, line);\n    const reduce = function (t) {\n      return 0 <= t && t <= 1;\n    };\n\n    if (order === 2) {\n      const a = aligned[0].y,\n        b = aligned[1].y,\n        c = aligned[2].y,\n        d = a - 2 * b + c;\n      if (d !== 0) {\n        const m1 = -sqrt(b * b - a * c),\n          m2 = -a + b,\n          v1 = -(m1 + m2) / d,\n          v2 = -(-m1 + m2) / d;\n        return [v1, v2].filter(reduce);\n      } else if (b !== c && d === 0) {\n        return [(2 * b - c) / (2 * b - 2 * c)].filter(reduce);\n      }\n      return [];\n    }\n\n    // see http://www.trans4mind.com/personal_development/mathematics/polynomials/cubicAlgebra.htm\n    const pa = aligned[0].y,\n      pb = aligned[1].y,\n      pc = aligned[2].y,\n      pd = aligned[3].y;\n\n    let d = -pa + 3 * pb - 3 * pc + pd,\n      a = 3 * pa - 6 * pb + 3 * pc,\n      b = -3 * pa + 3 * pb,\n      c = pa;\n\n    if (utils.approximately(d, 0)) {\n      // this is not a cubic curve.\n      if (utils.approximately(a, 0)) {\n        // in fact, this is not a quadratic curve either.\n        if (utils.approximately(b, 0)) {\n          // in fact in fact, there are no solutions.\n          return [];\n        }\n        // linear solution:\n        return [-c / b].filter(reduce);\n      }\n      // quadratic solution:\n      const q = sqrt(b * b - 4 * a * c),\n        a2 = 2 * a;\n      return [(q - b) / a2, (-b - q) / a2].filter(reduce);\n    }\n\n    // at this point, we know we need a cubic solution:\n\n    a /= d;\n    b /= d;\n    c /= d;\n\n    const p = (3 * b - a * a) / 3,\n      p3 = p / 3,\n      q = (2 * a * a * a - 9 * a * b + 27 * c) / 27,\n      q2 = q / 2,\n      discriminant = q2 * q2 + p3 * p3 * p3;\n\n    let u1, v1, x1, x2, x3;\n    if (discriminant < 0) {\n      const mp3 = -p / 3,\n        mp33 = mp3 * mp3 * mp3,\n        r = sqrt(mp33),\n        t = -q / (2 * r),\n        cosphi = t < -1 ? -1 : t > 1 ? 1 : t,\n        phi = acos(cosphi),\n        crtr = crt(r),\n        t1 = 2 * crtr;\n      x1 = t1 * cos(phi / 3) - a / 3;\n      x2 = t1 * cos((phi + tau) / 3) - a / 3;\n      x3 = t1 * cos((phi + 2 * tau) / 3) - a / 3;\n      return [x1, x2, x3].filter(reduce);\n    } else if (discriminant === 0) {\n      u1 = q2 < 0 ? crt(-q2) : -crt(q2);\n      x1 = 2 * u1 - a / 3;\n      x2 = -u1 - a / 3;\n      return [x1, x2].filter(reduce);\n    } else {\n      const sd = sqrt(discriminant);\n      u1 = crt(-q2 + sd);\n      v1 = crt(q2 + sd);\n      return [u1 - v1 - a / 3].filter(reduce);\n    }\n  },\n\n  droots: function (p) {\n    // quadratic roots are easy\n    if (p.length === 3) {\n      const a = p[0],\n        b = p[1],\n        c = p[2],\n        d = a - 2 * b + c;\n      if (d !== 0) {\n        const m1 = -sqrt(b * b - a * c),\n          m2 = -a + b,\n          v1 = -(m1 + m2) / d,\n          v2 = -(-m1 + m2) / d;\n        return [v1, v2];\n      } else if (b !== c && d === 0) {\n        return [(2 * b - c) / (2 * (b - c))];\n      }\n      return [];\n    }\n\n    // linear roots are even easier\n    if (p.length === 2) {\n      const a = p[0],\n        b = p[1];\n      if (a !== b) {\n        return [a / (a - b)];\n      }\n      return [];\n    }\n\n    return [];\n  },\n\n  curvature: function (t, d1, d2, _3d, kOnly) {\n    let num,\n      dnm,\n      adk,\n      dk,\n      k = 0,\n      r = 0;\n\n    //\n    // We're using the following formula for curvature:\n    //\n    //              x'y\" - y'x\"\n    //   k(t) = ------------------\n    //           (x'\u00b2 + y'\u00b2)^(3/2)\n    //\n    // from https://en.wikipedia.org/wiki/Radius_of_curvature#Definition\n    //\n    // With it corresponding 3D counterpart:\n    //\n    //          sqrt( (y'z\" - y\"z')\u00b2 + (z'x\" - z\"x')\u00b2 + (x'y\" - x\"y')\u00b2)\n    //   k(t) = -------------------------------------------------------\n    //                     (x'\u00b2 + y'\u00b2 + z'\u00b2)^(3/2)\n    //\n\n    const d = utils.compute(t, d1);\n    const dd = utils.compute(t, d2);\n    const qdsum = d.x * d.x + d.y * d.y;\n\n    if (_3d) {\n      num = sqrt(\n        pow(d.y * dd.z - dd.y * d.z, 2) +\n          pow(d.z * dd.x - dd.z * d.x, 2) +\n          pow(d.x * dd.y - dd.x * d.y, 2)\n      );\n      dnm = pow(qdsum + d.z * d.z, 3 / 2);\n    } else {\n      num = d.x * dd.y - d.y * dd.x;\n      dnm = pow(qdsum, 3 / 2);\n    }\n\n    if (num === 0 || dnm === 0) {\n      return { k: 0, r: 0 };\n    }\n\n    k = num / dnm;\n    r = dnm / num;\n\n    // We're also computing the derivative of kappa, because\n    // there is value in knowing the rate of change for the\n    // curvature along the curve. And we're just going to\n    // ballpark it based on an epsilon.\n    if (!kOnly) {\n      // compute k'(t) based on the interval before, and after it,\n      // to at least try to not introduce forward/backward pass bias.\n      const pk = utils.curvature(t - 0.001, d1, d2, _3d, true).k;\n      const nk = utils.curvature(t + 0.001, d1, d2, _3d, true).k;\n      dk = (nk - k + (k - pk)) / 2;\n      adk = (abs(nk - k) + abs(k - pk)) / 2;\n    }\n\n    return { k: k, r: r, dk: dk, adk: adk };\n  },\n\n  inflections: function (points) {\n    if (points.length < 4) return [];\n\n    // FIXME: TODO: add in inflection abstraction for quartic+ curves?\n\n    const p = utils.align(points, { p1: points[0], p2: points.slice(-1)[0] }),\n      a = p[2].x * p[1].y,\n      b = p[3].x * p[1].y,\n      c = p[1].x * p[2].y,\n      d = p[3].x * p[2].y,\n      v1 = 18 * (-3 * a + 2 * b + 3 * c - d),\n      v2 = 18 * (3 * a - b - 3 * c),\n      v3 = 18 * (c - a);\n\n    if (utils.approximately(v1, 0)) {\n      if (!utils.approximately(v2, 0)) {\n        let t = -v3 / v2;\n        if (0 <= t && t <= 1) return [t];\n      }\n      return [];\n    }\n\n    const d2 = 2 * v1;\n\n    if (utils.approximately(d2, 0)) return [];\n\n    const trm = v2 * v2 - 4 * v1 * v3;\n\n    if (trm < 0) return [];\n\n    const sq = Math.sqrt(trm);\n\n    return [(sq - v2) / d2, -(v2 + sq) / d2].filter(function (r) {\n      return 0 <= r && r <= 1;\n    });\n  },\n\n  bboxoverlap: function (b1, b2) {\n    const dims = [\"x\", \"y\"],\n      len = dims.length;\n\n    for (let i = 0, dim, l, t, d; i < len; i++) {\n      dim = dims[i];\n      l = b1[dim].mid;\n      t = b2[dim].mid;\n      d = (b1[dim].size + b2[dim].size) / 2;\n      if (abs(l - t) >= d) return false;\n    }\n    return true;\n  },\n\n  expandbox: function (bbox, _bbox) {\n    if (_bbox.x.min < bbox.x.min) {\n      bbox.x.min = _bbox.x.min;\n    }\n    if (_bbox.y.min < bbox.y.min) {\n      bbox.y.min = _bbox.y.min;\n    }\n    if (_bbox.z && _bbox.z.min < bbox.z.min) {\n      bbox.z.min = _bbox.z.min;\n    }\n    if (_bbox.x.max > bbox.x.max) {\n      bbox.x.max = _bbox.x.max;\n    }\n    if (_bbox.y.max > bbox.y.max) {\n      bbox.y.max = _bbox.y.max;\n    }\n    if (_bbox.z && _bbox.z.max > bbox.z.max) {\n      bbox.z.max = _bbox.z.max;\n    }\n    bbox.x.mid = (bbox.x.min + bbox.x.max) / 2;\n    bbox.y.mid = (bbox.y.min + bbox.y.max) / 2;\n    if (bbox.z) {\n      bbox.z.mid = (bbox.z.min + bbox.z.max) / 2;\n    }\n    bbox.x.size = bbox.x.max - bbox.x.min;\n    bbox.y.size = bbox.y.max - bbox.y.min;\n    if (bbox.z) {\n      bbox.z.size = bbox.z.max - bbox.z.min;\n    }\n  },\n\n  pairiteration: function (c1, c2, curveIntersectionThreshold) {\n    const c1b = c1.bbox(),\n      c2b = c2.bbox(),\n      r = 100000,\n      threshold = curveIntersectionThreshold || 0.5;\n\n    if (\n      c1b.x.size + c1b.y.size < threshold &&\n      c2b.x.size + c2b.y.size < threshold\n    ) {\n      return [\n        (((r * (c1._t1 + c1._t2)) / 2) | 0) / r +\n          \"/\" +\n          (((r * (c2._t1 + c2._t2)) / 2) | 0) / r,\n      ];\n    }\n\n    let cc1 = c1.split(0.5),\n      cc2 = c2.split(0.5),\n      pairs = [\n        { left: cc1.left, right: cc2.left },\n        { left: cc1.left, right: cc2.right },\n        { left: cc1.right, right: cc2.right },\n        { left: cc1.right, right: cc2.left },\n      ];\n\n    pairs = pairs.filter(function (pair) {\n      return utils.bboxoverlap(pair.left.bbox(), pair.right.bbox());\n    });\n\n    let results = [];\n\n    if (pairs.length === 0) return results;\n\n    pairs.forEach(function (pair) {\n      results = results.concat(\n        utils.pairiteration(pair.left, pair.right, threshold)\n      );\n    });\n\n    results = results.filter(function (v, i) {\n      return results.indexOf(v) === i;\n    });\n\n    return results;\n  },\n\n  getccenter: function (p1, p2, p3) {\n    const dx1 = p2.x - p1.x,\n      dy1 = p2.y - p1.y,\n      dx2 = p3.x - p2.x,\n      dy2 = p3.y - p2.y,\n      dx1p = dx1 * cos(quart) - dy1 * sin(quart),\n      dy1p = dx1 * sin(quart) + dy1 * cos(quart),\n      dx2p = dx2 * cos(quart) - dy2 * sin(quart),\n      dy2p = dx2 * sin(quart) + dy2 * cos(quart),\n      // chord midpoints\n      mx1 = (p1.x + p2.x) / 2,\n      my1 = (p1.y + p2.y) / 2,\n      mx2 = (p2.x + p3.x) / 2,\n      my2 = (p2.y + p3.y) / 2,\n      // midpoint offsets\n      mx1n = mx1 + dx1p,\n      my1n = my1 + dy1p,\n      mx2n = mx2 + dx2p,\n      my2n = my2 + dy2p,\n      // intersection of these lines:\n      arc = utils.lli8(mx1, my1, mx1n, my1n, mx2, my2, mx2n, my2n),\n      r = utils.dist(arc, p1);\n\n    // arc start/end values, over mid point:\n    let s = atan2(p1.y - arc.y, p1.x - arc.x),\n      m = atan2(p2.y - arc.y, p2.x - arc.x),\n      e = atan2(p3.y - arc.y, p3.x - arc.x),\n      _;\n\n    // determine arc direction (cw/ccw correction)\n    if (s < e) {\n      // if s<m<e, arc(s, e)\n      // if m<s<e, arc(e, s + tau)\n      // if s<e<m, arc(e, s + tau)\n      if (s > m || m > e) {\n        s += tau;\n      }\n      if (s > e) {\n        _ = e;\n        e = s;\n        s = _;\n      }\n    } else {\n      // if e<m<s, arc(e, s)\n      // if m<e<s, arc(s, e + tau)\n      // if e<s<m, arc(s, e + tau)\n      if (e < m && m < s) {\n        _ = e;\n        e = s;\n        s = _;\n      } else {\n        e += tau;\n      }\n    }\n    // assign and done.\n    arc.s = s;\n    arc.e = e;\n    arc.r = r;\n    return arc;\n  },\n\n  numberSort: function (a, b) {\n    return a - b;\n  },\n};\n\nexport { utils };\n",
         "import { utils } from \"./utils.js\";\n\n/**\n * Poly Bezier\n * @param {[type]} curves [description]\n */\nclass PolyBezier {\n  constructor(curves) {\n    this.curves = [];\n    this._3d = false;\n    if (!!curves) {\n      this.curves = curves;\n      this._3d = this.curves[0]._3d;\n    }\n  }\n\n  valueOf() {\n    return this.toString();\n  }\n\n  toString() {\n    return (\n      \"[\" +\n      this.curves\n        .map(function (curve) {\n          return utils.pointsToString(curve.points);\n        })\n        .join(\", \") +\n      \"]\"\n    );\n  }\n\n  addCurve(curve) {\n    this.curves.push(curve);\n    this._3d = this._3d || curve._3d;\n  }\n\n  length() {\n    return this.curves\n      .map(function (v) {\n        return v.length();\n      })\n      .reduce(function (a, b) {\n        return a + b;\n      });\n  }\n\n  curve(idx) {\n    return this.curves[idx];\n  }\n\n  bbox() {\n    const c = this.curves;\n    var bbox = c[0].bbox();\n    for (var i = 1; i < c.length; i++) {\n      utils.expandbox(bbox, c[i].bbox());\n    }\n    return bbox;\n  }\n\n  offset(d) {\n    const offset = [];\n    this.curves.forEach(function (v) {\n      offset.push(...v.offset(d));\n    });\n    return new PolyBezier(offset);\n  }\n}\n\nexport { PolyBezier };\n",
         "/**\n  A javascript Bezier curve library by Pomax.\n\n  Based on http://pomax.github.io/bezierinfo\n\n  This code is MIT licensed.\n**/\n\nimport { utils } from \"./utils.js\";\nimport { PolyBezier } from \"./poly-bezier.js\";\n\n// math-inlining.\nconst { abs, min, max, cos, sin, acos, sqrt } = Math;\nconst pi = Math.PI;\n// a zero coordinate, which is surprisingly useful\nconst ZERO = { x: 0, y: 0, z: 0 };\n\n/**\n * Bezier curve constructor.\n *\n * ...docs pending...\n */\nclass Bezier {\n  constructor(coords) {\n    let args =\n      coords && coords.forEach ? coords : Array.from(arguments).slice();\n    let coordlen = false;\n\n    if (typeof args[0] === \"object\") {\n      coordlen = args.length;\n      const newargs = [];\n      args.forEach(function (point) {\n        [\"x\", \"y\", \"z\"].forEach(function (d) {\n          if (typeof point[d] !== \"undefined\") {\n            newargs.push(point[d]);\n          }\n        });\n      });\n      args = newargs;\n    }\n\n    let higher = false;\n    const len = args.length;\n\n    if (coordlen) {\n      if (coordlen > 4) {\n        if (arguments.length !== 1) {\n          throw new Error(\n            \"Only new Bezier(point[]) is accepted for 4th and higher order curves\"\n          );\n        }\n        higher = true;\n      }\n    } else {\n      if (len !== 6 && len !== 8 && len !== 9 && len !== 12) {\n        if (arguments.length !== 1) {\n          throw new Error(\n            \"Only new Bezier(point[]) is accepted for 4th and higher order curves\"\n          );\n        }\n      }\n    }\n\n    const _3d = (this._3d =\n      (!higher && (len === 9 || len === 12)) ||\n      (coords && coords[0] && typeof coords[0].z !== \"undefined\"));\n\n    const points = (this.points = []);\n    for (let idx = 0, step = _3d ? 3 : 2; idx < len; idx += step) {\n      var point = {\n        x: args[idx],\n        y: args[idx + 1],\n      };\n      if (_3d) {\n        point.z = args[idx + 2];\n      }\n      points.push(point);\n    }\n    const order = (this.order = points.length - 1);\n\n    const dims = (this.dims = [\"x\", \"y\"]);\n    if (_3d) dims.push(\"z\");\n    this.dimlen = dims.length;\n\n    // is this curve, practically speaking, a straight line?\n    const aligned = utils.align(points, { p1: points[0], p2: points[order] });\n    const baselength = utils.dist(points[0], points[order]);\n    this._linear = aligned.reduce((t, p) => t + abs(p.y), 0) < baselength / 50;\n\n    this._lut = [];\n    this._t1 = 0;\n    this._t2 = 1;\n    this.update();\n  }\n\n  static quadraticFromPoints(p1, p2, p3, t) {\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    }\n    // shortcuts, although they're really dumb\n    if (t === 0) {\n      return new Bezier(p2, p2, p3);\n    }\n    if (t === 1) {\n      return new Bezier(p1, p2, p2);\n    }\n    // real fitting.\n    const abc = Bezier.getABC(2, p1, p2, p3, t);\n    return new Bezier(p1, abc.A, p3);\n  }\n\n  static cubicFromPoints(S, B, E, t, d1) {\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    }\n    const abc = Bezier.getABC(3, S, B, E, t);\n    if (typeof d1 === \"undefined\") {\n      d1 = utils.dist(B, abc.C);\n    }\n    const d2 = (d1 * (1 - t)) / t;\n\n    const selen = utils.dist(S, E),\n      lx = (E.x - S.x) / selen,\n      ly = (E.y - S.y) / selen,\n      bx1 = d1 * lx,\n      by1 = d1 * ly,\n      bx2 = d2 * lx,\n      by2 = d2 * ly;\n    // derivation of new hull coordinates\n    const e1 = { x: B.x - bx1, y: B.y - by1 },\n      e2 = { x: B.x + bx2, y: B.y + by2 },\n      A = abc.A,\n      v1 = { x: A.x + (e1.x - A.x) / (1 - t), y: A.y + (e1.y - A.y) / (1 - t) },\n      v2 = { x: A.x + (e2.x - A.x) / t, y: A.y + (e2.y - A.y) / t },\n      nc1 = { x: S.x + (v1.x - S.x) / t, y: S.y + (v1.y - S.y) / t },\n      nc2 = {\n        x: E.x + (v2.x - E.x) / (1 - t),\n        y: E.y + (v2.y - E.y) / (1 - t),\n      };\n    // ...done\n    return new Bezier(S, nc1, nc2, E);\n  }\n\n  static getUtils() {\n    return utils;\n  }\n\n  getUtils() {\n    return Bezier.getUtils();\n  }\n\n  static get PolyBezier() {\n    return PolyBezier;\n  }\n\n  valueOf() {\n    return this.toString();\n  }\n\n  toString() {\n    return utils.pointsToString(this.points);\n  }\n\n  toSVG() {\n    if (this._3d) return false;\n    const p = this.points,\n      x = p[0].x,\n      y = p[0].y,\n      s = [\"M\", x, y, this.order === 2 ? \"Q\" : \"C\"];\n    for (let i = 1, last = p.length; i < last; i++) {\n      s.push(p[i].x);\n      s.push(p[i].y);\n    }\n    return s.join(\" \");\n  }\n\n  setRatios(ratios) {\n    if (ratios.length !== this.points.length) {\n      throw new Error(\"incorrect number of ratio values\");\n    }\n    this.ratios = ratios;\n    this._lut = []; //  invalidate any precomputed LUT\n  }\n\n  verify() {\n    const print = this.coordDigest();\n    if (print !== this._print) {\n      this._print = print;\n      this.update();\n    }\n  }\n\n  coordDigest() {\n    return this.points\n      .map(function (c, pos) {\n        return \"\" + pos + c.x + c.y + (c.z ? c.z : 0);\n      })\n      .join(\"\");\n  }\n\n  update() {\n    // invalidate any precomputed LUT\n    this._lut = [];\n    this.dpoints = utils.derive(this.points, this._3d);\n    this.computedirection();\n  }\n\n  computedirection() {\n    const points = this.points;\n    const angle = utils.angle(points[0], points[this.order], points[1]);\n    this.clockwise = angle > 0;\n  }\n\n  length() {\n    return utils.length(this.derivative.bind(this));\n  }\n\n  static getABC(order = 2, S, B, E, t = 0.5) {\n    const u = utils.projectionratio(t, order),\n      um = 1 - u,\n      C = {\n        x: u * S.x + um * E.x,\n        y: u * S.y + um * E.y,\n      },\n      s = utils.abcratio(t, order),\n      A = {\n        x: B.x + (B.x - C.x) / s,\n        y: B.y + (B.y - C.y) / s,\n      };\n    return { A, B, C, S, E };\n  }\n\n  getABC(t, B) {\n    B = B || this.get(t);\n    let S = this.points[0];\n    let E = this.points[this.order];\n    return Bezier.getABC(this.order, S, B, E, t);\n  }\n\n  getLUT(steps) {\n    this.verify();\n    steps = steps || 100;\n    if (this._lut.length === steps + 1) {\n      return this._lut;\n    }\n    this._lut = [];\n    // n steps means n+1 points\n    steps++;\n    this._lut = [];\n    for (let i = 0, p, t; i < steps; i++) {\n      t = i / (steps - 1);\n      p = this.compute(t);\n      p.t = t;\n      this._lut.push(p);\n    }\n    return this._lut;\n  }\n\n  on(point, error) {\n    error = error || 5;\n    const lut = this.getLUT(),\n      hits = [];\n    for (let i = 0, c, t = 0; i < lut.length; i++) {\n      c = lut[i];\n      if (utils.dist(c, point) < error) {\n        hits.push(c);\n        t += i / lut.length;\n      }\n    }\n    if (!hits.length) return false;\n    return (t /= hits.length);\n  }\n\n  project(point) {\n    // step 1: coarse check\n    const LUT = this.getLUT(),\n      l = LUT.length - 1,\n      closest = utils.closest(LUT, point),\n      mpos = closest.mpos,\n      t1 = (mpos - 1) / l,\n      t2 = (mpos + 1) / l,\n      step = 0.1 / l;\n\n    // step 2: fine check\n    let mdist = closest.mdist,\n      t = t1,\n      ft = t,\n      p;\n    mdist += 1;\n    for (let d; t < t2 + step; t += step) {\n      p = this.compute(t);\n      d = utils.dist(point, p);\n      if (d < mdist) {\n        mdist = d;\n        ft = t;\n      }\n    }\n    ft = ft < 0 ? 0 : ft > 1 ? 1 : ft;\n    p = this.compute(ft);\n    p.t = ft;\n    p.d = mdist;\n    return p;\n  }\n\n  get(t) {\n    return this.compute(t);\n  }\n\n  point(idx) {\n    return this.points[idx];\n  }\n\n  compute(t) {\n    if (this.ratios) {\n      return utils.computeWithRatios(t, this.points, this.ratios, this._3d);\n    }\n    return utils.compute(t, this.points, this._3d, this.ratios);\n  }\n\n  raise() {\n    const p = this.points,\n      np = [p[0]],\n      k = p.length;\n    for (let i = 1, pi, pim; i < k; i++) {\n      pi = p[i];\n      pim = p[i - 1];\n      np[i] = {\n        x: ((k - i) / k) * pi.x + (i / k) * pim.x,\n        y: ((k - i) / k) * pi.y + (i / k) * pim.y,\n      };\n    }\n    np[k] = p[k - 1];\n    return new Bezier(np);\n  }\n\n  derivative(t) {\n    return utils.compute(t, this.dpoints[0], this._3d);\n  }\n\n  dderivative(t) {\n    return utils.compute(t, this.dpoints[1], this._3d);\n  }\n\n  align() {\n    let p = this.points;\n    return new Bezier(utils.align(p, { p1: p[0], p2: p[p.length - 1] }));\n  }\n\n  curvature(t) {\n    return utils.curvature(t, this.dpoints[0], this.dpoints[1], this._3d);\n  }\n\n  inflections() {\n    return utils.inflections(this.points);\n  }\n\n  normal(t) {\n    return this._3d ? this.__normal3(t) : this.__normal2(t);\n  }\n\n  __normal2(t) {\n    const d = this.derivative(t);\n    const q = sqrt(d.x * d.x + d.y * d.y);\n    return { t, x: -d.y / q, y: d.x / q };\n  }\n\n  __normal3(t) {\n    // see http://stackoverflow.com/questions/25453159\n    const r1 = this.derivative(t),\n      r2 = this.derivative(t + 0.01),\n      q1 = sqrt(r1.x * r1.x + r1.y * r1.y + r1.z * r1.z),\n      q2 = sqrt(r2.x * r2.x + r2.y * r2.y + r2.z * r2.z);\n    r1.x /= q1;\n    r1.y /= q1;\n    r1.z /= q1;\n    r2.x /= q2;\n    r2.y /= q2;\n    r2.z /= q2;\n    // cross product\n    const c = {\n      x: r2.y * r1.z - r2.z * r1.y,\n      y: r2.z * r1.x - r2.x * r1.z,\n      z: r2.x * r1.y - r2.y * r1.x,\n    };\n    const m = sqrt(c.x * c.x + c.y * c.y + c.z * c.z);\n    c.x /= m;\n    c.y /= m;\n    c.z /= m;\n    // rotation matrix\n    const R = [\n      c.x * c.x,\n      c.x * c.y - c.z,\n      c.x * c.z + c.y,\n      c.x * c.y + c.z,\n      c.y * c.y,\n      c.y * c.z - c.x,\n      c.x * c.z - c.y,\n      c.y * c.z + c.x,\n      c.z * c.z,\n    ];\n    // normal vector:\n    const n = {\n      t,\n      x: R[0] * r1.x + R[1] * r1.y + R[2] * r1.z,\n      y: R[3] * r1.x + R[4] * r1.y + R[5] * r1.z,\n      z: R[6] * r1.x + R[7] * r1.y + R[8] * r1.z,\n    };\n    return n;\n  }\n\n  hull(t) {\n    let p = this.points,\n      _p = [],\n      q = [],\n      idx = 0;\n    q[idx++] = p[0];\n    q[idx++] = p[1];\n    q[idx++] = p[2];\n    if (this.order === 3) {\n      q[idx++] = p[3];\n    }\n    // we lerp between all points at each iteration, until we have 1 point left.\n    while (p.length > 1) {\n      _p = [];\n      for (let i = 0, pt, l = p.length - 1; i < l; i++) {\n        pt = utils.lerp(t, p[i], p[i + 1]);\n        q[idx++] = pt;\n        _p.push(pt);\n      }\n      p = _p;\n    }\n    return q;\n  }\n\n  split(t1, t2) {\n    // shortcuts\n    if (t1 === 0 && !!t2) {\n      return this.split(t2).left;\n    }\n    if (t2 === 1) {\n      return this.split(t1).right;\n    }\n\n    // no shortcut: use \"de Casteljau\" iteration.\n    const q = this.hull(t1);\n    const result = {\n      left:\n        this.order === 2\n          ? new Bezier([q[0], q[3], q[5]])\n          : new Bezier([q[0], q[4], q[7], q[9]]),\n      right:\n        this.order === 2\n          ? new Bezier([q[5], q[4], q[2]])\n          : new Bezier([q[9], q[8], q[6], q[3]]),\n      span: q,\n    };\n\n    // make sure we bind _t1/_t2 information!\n    result.left._t1 = utils.map(0, 0, 1, this._t1, this._t2);\n    result.left._t2 = utils.map(t1, 0, 1, this._t1, this._t2);\n    result.right._t1 = utils.map(t1, 0, 1, this._t1, this._t2);\n    result.right._t2 = utils.map(1, 0, 1, this._t1, this._t2);\n\n    // if we have no t2, we're done\n    if (!t2) {\n      return result;\n    }\n\n    // if we have a t2, split again:\n    t2 = utils.map(t2, t1, 1, 0, 1);\n    return result.right.split(t2).left;\n  }\n\n  extrema() {\n    const result = {};\n    let roots = [];\n\n    this.dims.forEach(\n      function (dim) {\n        let mfn = function (v) {\n          return v[dim];\n        };\n        let p = this.dpoints[0].map(mfn);\n        result[dim] = utils.droots(p);\n        if (this.order === 3) {\n          p = this.dpoints[1].map(mfn);\n          result[dim] = result[dim].concat(utils.droots(p));\n        }\n        result[dim] = result[dim].filter(function (t) {\n          return t >= 0 && t <= 1;\n        });\n        roots = roots.concat(result[dim].sort(utils.numberSort));\n      }.bind(this)\n    );\n\n    result.values = roots.sort(utils.numberSort).filter(function (v, idx) {\n      return roots.indexOf(v) === idx;\n    });\n\n    return result;\n  }\n\n  bbox() {\n    const extrema = this.extrema(),\n      result = {};\n    this.dims.forEach(\n      function (d) {\n        result[d] = utils.getminmax(this, d, extrema[d]);\n      }.bind(this)\n    );\n    return result;\n  }\n\n  overlaps(curve) {\n    const lbbox = this.bbox(),\n      tbbox = curve.bbox();\n    return utils.bboxoverlap(lbbox, tbbox);\n  }\n\n  offset(t, d) {\n    if (typeof d !== \"undefined\") {\n      const c = this.get(t),\n        n = this.normal(t);\n      const ret = {\n        c: c,\n        n: n,\n        x: c.x + n.x * d,\n        y: c.y + n.y * d,\n      };\n      if (this._3d) {\n        ret.z = c.z + n.z * d;\n      }\n      return ret;\n    }\n    if (this._linear) {\n      const nv = this.normal(0),\n        coords = this.points.map(function (p) {\n          const ret = {\n            x: p.x + t * nv.x,\n            y: p.y + t * nv.y,\n          };\n          if (p.z && nv.z) {\n            ret.z = p.z + t * nv.z;\n          }\n          return ret;\n        });\n      return [new Bezier(coords)];\n    }\n    return this.reduce().map(function (s) {\n      if (s._linear) {\n        return s.offset(t)[0];\n      }\n      return s.scale(t);\n    });\n  }\n\n  simple() {\n    if (this.order === 3) {\n      const a1 = utils.angle(this.points[0], this.points[3], this.points[1]);\n      const a2 = utils.angle(this.points[0], this.points[3], this.points[2]);\n      if ((a1 > 0 && a2 < 0) || (a1 < 0 && a2 > 0)) return false;\n    }\n    const n1 = this.normal(0);\n    const n2 = this.normal(1);\n    let s = n1.x * n2.x + n1.y * n2.y;\n    if (this._3d) {\n      s += n1.z * n2.z;\n    }\n    return abs(acos(s)) < pi / 3;\n  }\n\n  reduce() {\n    // TODO: examine these var types in more detail...\n    let i,\n      t1 = 0,\n      t2 = 0,\n      step = 0.01,\n      segment,\n      pass1 = [],\n      pass2 = [];\n    // first pass: split on extrema\n    let extrema = this.extrema().values;\n    if (extrema.indexOf(0) === -1) {\n      extrema = [0].concat(extrema);\n    }\n    if (extrema.indexOf(1) === -1) {\n      extrema.push(1);\n    }\n\n    for (t1 = extrema[0], i = 1; i < extrema.length; i++) {\n      t2 = extrema[i];\n      segment = this.split(t1, t2);\n      segment._t1 = t1;\n      segment._t2 = t2;\n      pass1.push(segment);\n      t1 = t2;\n    }\n\n    // second pass: further reduce these segments to simple segments\n    pass1.forEach(function (p1) {\n      t1 = 0;\n      t2 = 0;\n      while (t2 <= 1) {\n        for (t2 = t1 + step; t2 <= 1 + step; t2 += step) {\n          segment = p1.split(t1, t2);\n          if (!segment.simple()) {\n            t2 -= step;\n            if (abs(t1 - t2) < step) {\n              // we can never form a reduction\n              return [];\n            }\n            segment = p1.split(t1, t2);\n            segment._t1 = utils.map(t1, 0, 1, p1._t1, p1._t2);\n            segment._t2 = utils.map(t2, 0, 1, p1._t1, p1._t2);\n            pass2.push(segment);\n            t1 = t2;\n            break;\n          }\n        }\n      }\n      if (t1 < 1) {\n        segment = p1.split(t1, 1);\n        segment._t1 = utils.map(t1, 0, 1, p1._t1, p1._t2);\n        segment._t2 = p1._t2;\n        pass2.push(segment);\n      }\n    });\n    return pass2;\n  }\n\n  translate(v, d1, d2) {\n    d2 = typeof d2 === \"number\" ? d2 : d1;\n\n    // TODO: make this take curves with control points outside\n    //       of the start-end interval into account\n\n    const o = this.order;\n    let d = this.points.map((_, i) => (1 - i / o) * d1 + (i / o) * d2);\n    return new Bezier(\n      this.points.map((p, i) => ({\n        x: p.x + v.x * d[i],\n        y: p.y + v.y * d[i],\n      }))\n    );\n  }\n\n  scale(d) {\n    const order = this.order;\n    let distanceFn = false;\n    if (typeof d === \"function\") {\n      distanceFn = d;\n    }\n    if (distanceFn && order === 2) {\n      return this.raise().scale(distanceFn);\n    }\n\n    // TODO: add special handling for non-linear degenerate curves.\n\n    const clockwise = this.clockwise;\n    const points = this.points;\n\n    if (this._linear) {\n      return this.translate(\n        this.normal(0),\n        distanceFn ? distanceFn(0) : d,\n        distanceFn ? distanceFn(1) : d\n      );\n    }\n\n    const r1 = distanceFn ? distanceFn(0) : d;\n    const r2 = distanceFn ? distanceFn(1) : d;\n    const v = [this.offset(0, 10), this.offset(1, 10)];\n    const np = [];\n    const o = utils.lli4(v[0], v[0].c, v[1], v[1].c);\n\n    if (!o) {\n      throw new Error(\"cannot scale this curve. Try reducing it first.\");\n    }\n\n    // move all points by distance 'd' wrt the origin 'o',\n    // and move end points by fixed distance along normal.\n    [0, 1].forEach(function (t) {\n      const p = (np[t * order] = utils.copy(points[t * order]));\n      p.x += (t ? r2 : r1) * v[t].n.x;\n      p.y += (t ? r2 : r1) * v[t].n.y;\n    });\n\n    if (!distanceFn) {\n      // move control points to lie on the intersection of the offset\n      // derivative vector, and the origin-through-control vector\n      [0, 1].forEach((t) => {\n        if (order === 2 && !!t) return;\n        const p = np[t * order];\n        const d = this.derivative(t);\n        const p2 = { x: p.x + d.x, y: p.y + d.y };\n        np[t + 1] = utils.lli4(p, p2, o, points[t + 1]);\n      });\n      return new Bezier(np);\n    }\n\n    // move control points by \"however much necessary to\n    // ensure the correct tangent to endpoint\".\n    [0, 1].forEach(function (t) {\n      if (order === 2 && !!t) return;\n      var p = points[t + 1];\n      var ov = {\n        x: p.x - o.x,\n        y: p.y - o.y,\n      };\n      var rc = distanceFn ? distanceFn((t + 1) / order) : d;\n      if (distanceFn && !clockwise) rc = -rc;\n      var m = sqrt(ov.x * ov.x + ov.y * ov.y);\n      ov.x /= m;\n      ov.y /= m;\n      np[t + 1] = {\n        x: p.x + rc * ov.x,\n        y: p.y + rc * ov.y,\n      };\n    });\n    return new Bezier(np);\n  }\n\n  outline(d1, d2, d3, d4) {\n    d2 = d2 === undefined ? d1 : d2;\n\n    if (this._linear) {\n      // TODO: find the actual extrema, because they might\n      //       be before the start, or past the end.\n\n      const n = this.normal(0);\n      const start = this.points[0];\n      const end = this.points[this.points.length - 1];\n      let s, mid, e;\n\n      if (d3 === undefined) {\n        d3 = d1;\n        d4 = d2;\n      }\n\n      s = { x: start.x + n.x * d1, y: start.y + n.y * d1 };\n      e = { x: end.x + n.x * d3, y: end.y + n.y * d3 };\n      mid = { x: (s.x + e.x) / 2, y: (s.y + e.y) / 2 };\n      const fline = [s, mid, e];\n\n      s = { x: start.x - n.x * d2, y: start.y - n.y * d2 };\n      e = { x: end.x - n.x * d4, y: end.y - n.y * d4 };\n      mid = { x: (s.x + e.x) / 2, y: (s.y + e.y) / 2 };\n      const bline = [e, mid, s];\n\n      const ls = utils.makeline(bline[2], fline[0]);\n      const le = utils.makeline(fline[2], bline[0]);\n      const segments = [ls, new Bezier(fline), le, new Bezier(bline)];\n      return new PolyBezier(segments);\n    }\n\n    const reduced = this.reduce(),\n      len = reduced.length,\n      fcurves = [];\n\n    let bcurves = [],\n      p,\n      alen = 0,\n      tlen = this.length();\n\n    const graduated = typeof d3 !== \"undefined\" && typeof d4 !== \"undefined\";\n\n    function linearDistanceFunction(s, e, tlen, alen, slen) {\n      return function (v) {\n        const f1 = alen / tlen,\n          f2 = (alen + slen) / tlen,\n          d = e - s;\n        return utils.map(v, 0, 1, s + f1 * d, s + f2 * d);\n      };\n    }\n\n    // form curve oulines\n    reduced.forEach(function (segment) {\n      const slen = segment.length();\n      if (graduated) {\n        fcurves.push(\n          segment.scale(linearDistanceFunction(d1, d3, tlen, alen, slen))\n        );\n        bcurves.push(\n          segment.scale(linearDistanceFunction(-d2, -d4, tlen, alen, slen))\n        );\n      } else {\n        fcurves.push(segment.scale(d1));\n        bcurves.push(segment.scale(-d2));\n      }\n      alen += slen;\n    });\n\n    // reverse the \"return\" outline\n    bcurves = bcurves\n      .map(function (s) {\n        p = s.points;\n        if (p[3]) {\n          s.points = [p[3], p[2], p[1], p[0]];\n        } else {\n          s.points = [p[2], p[1], p[0]];\n        }\n        return s;\n      })\n      .reverse();\n\n    // form the endcaps as lines\n    const fs = fcurves[0].points[0],\n      fe = fcurves[len - 1].points[fcurves[len - 1].points.length - 1],\n      bs = bcurves[len - 1].points[bcurves[len - 1].points.length - 1],\n      be = bcurves[0].points[0],\n      ls = utils.makeline(bs, fs),\n      le = utils.makeline(fe, be),\n      segments = [ls].concat(fcurves).concat([le]).concat(bcurves);\n\n    return new PolyBezier(segments);\n  }\n\n  outlineshapes(d1, d2, curveIntersectionThreshold) {\n    d2 = d2 || d1;\n    const outline = this.outline(d1, d2).curves;\n    const shapes = [];\n    for (let i = 1, len = outline.length; i < len / 2; i++) {\n      const shape = utils.makeshape(\n        outline[i],\n        outline[len - i],\n        curveIntersectionThreshold\n      );\n      shape.startcap.virtual = i > 1;\n      shape.endcap.virtual = i < len / 2 - 1;\n      shapes.push(shape);\n    }\n    return shapes;\n  }\n\n  intersects(curve, curveIntersectionThreshold) {\n    if (!curve) return this.selfintersects(curveIntersectionThreshold);\n    if (curve.p1 && curve.p2) {\n      return this.lineIntersects(curve);\n    }\n    if (curve instanceof Bezier) {\n      curve = curve.reduce();\n    }\n    return this.curveintersects(\n      this.reduce(),\n      curve,\n      curveIntersectionThreshold\n    );\n  }\n\n  lineIntersects(line) {\n    const mx = min(line.p1.x, line.p2.x),\n      my = min(line.p1.y, line.p2.y),\n      MX = max(line.p1.x, line.p2.x),\n      MY = max(line.p1.y, line.p2.y);\n    return utils.roots(this.points, line).filter((t) => {\n      var p = this.get(t);\n      return utils.between(p.x, mx, MX) && utils.between(p.y, my, MY);\n    });\n  }\n\n  selfintersects(curveIntersectionThreshold) {\n    // \"simple\" curves cannot intersect with their direct\n    // neighbour, so for each segment X we check whether\n    // it intersects [0:x-2][x+2:last].\n\n    const reduced = this.reduce(),\n      len = reduced.length - 2,\n      results = [];\n\n    for (let i = 0, result, left, right; i < len; i++) {\n      left = reduced.slice(i, i + 1);\n      right = reduced.slice(i + 2);\n      result = this.curveintersects(left, right, curveIntersectionThreshold);\n      results.push(...result);\n    }\n    return results;\n  }\n\n  curveintersects(c1, c2, curveIntersectionThreshold) {\n    const pairs = [];\n    // step 1: pair off any overlapping segments\n    c1.forEach(function (l) {\n      c2.forEach(function (r) {\n        if (l.overlaps(r)) {\n          pairs.push({ left: l, right: r });\n        }\n      });\n    });\n    // step 2: for each pairing, run through the convergence algorithm.\n    let intersections = [];\n    pairs.forEach(function (pair) {\n      const result = utils.pairiteration(\n        pair.left,\n        pair.right,\n        curveIntersectionThreshold\n      );\n      if (result.length > 0) {\n        intersections = intersections.concat(result);\n      }\n    });\n    return intersections;\n  }\n\n  arcs(errorThreshold) {\n    errorThreshold = errorThreshold || 0.5;\n    return this._iterate(errorThreshold, []);\n  }\n\n  _error(pc, np1, s, e) {\n    const q = (e - s) / 4,\n      c1 = this.get(s + q),\n      c2 = this.get(e - q),\n      ref = utils.dist(pc, np1),\n      d1 = utils.dist(pc, c1),\n      d2 = utils.dist(pc, c2);\n    return abs(d1 - ref) + abs(d2 - ref);\n  }\n\n  _iterate(errorThreshold, circles) {\n    let t_s = 0,\n      t_e = 1,\n      safety;\n    // we do a binary search to find the \"good `t` closest to no-longer-good\"\n    do {\n      safety = 0;\n\n      // step 1: start with the maximum possible arc\n      t_e = 1;\n\n      // points:\n      let np1 = this.get(t_s),\n        np2,\n        np3,\n        arc,\n        prev_arc;\n\n      // booleans:\n      let curr_good = false,\n        prev_good = false,\n        done;\n\n      // numbers:\n      let t_m = t_e,\n        prev_e = 1,\n        step = 0;\n\n      // step 2: find the best possible arc\n      do {\n        prev_good = curr_good;\n        prev_arc = arc;\n        t_m = (t_s + t_e) / 2;\n        step++;\n\n        np2 = this.get(t_m);\n        np3 = this.get(t_e);\n\n        arc = utils.getccenter(np1, np2, np3);\n\n        //also save the t values\n        arc.interval = {\n          start: t_s,\n          end: t_e,\n        };\n\n        let error = this._error(arc, np1, t_s, t_e);\n        curr_good = error <= errorThreshold;\n\n        done = prev_good && !curr_good;\n        if (!done) prev_e = t_e;\n\n        // this arc is fine: we can move 'e' up to see if we can find a wider arc\n        if (curr_good) {\n          // if e is already at max, then we're done for this arc.\n          if (t_e >= 1) {\n            // make sure we cap at t=1\n            arc.interval.end = prev_e = 1;\n            prev_arc = arc;\n            // if we capped the arc segment to t=1 we also need to make sure that\n            // the arc's end angle is correct with respect to the bezier end point.\n            if (t_e > 1) {\n              let d = {\n                x: arc.x + arc.r * cos(arc.e),\n                y: arc.y + arc.r * sin(arc.e),\n              };\n              arc.e += utils.angle({ x: arc.x, y: arc.y }, d, this.get(1));\n            }\n            break;\n          }\n          // if not, move it up by half the iteration distance\n          t_e = t_e + (t_e - t_s) / 2;\n        } else {\n          // this is a bad arc: we need to move 'e' down to find a good arc\n          t_e = t_m;\n        }\n      } while (!done && safety++ < 100);\n\n      if (safety >= 100) {\n        break;\n      }\n\n      // console.log(\"L835: [F] arc found\", t_s, prev_e, prev_arc.x, prev_arc.y, prev_arc.s, prev_arc.e);\n\n      prev_arc = prev_arc ? prev_arc : arc;\n      circles.push(prev_arc);\n      t_s = prev_e;\n    } while (t_e < 1);\n    return circles;\n  }\n}\n\nexport { Bezier };\n",
         "export default {\n\taliceblue: [240, 248, 255],\n\tantiquewhite: [250, 235, 215],\n\taqua: [0, 255, 255],\n\taquamarine: [127, 255, 212],\n\tazure: [240, 255, 255],\n\tbeige: [245, 245, 220],\n\tbisque: [255, 228, 196],\n\tblack: [0, 0, 0],\n\tblanchedalmond: [255, 235, 205],\n\tblue: [0, 0, 255],\n\tblueviolet: [138, 43, 226],\n\tbrown: [165, 42, 42],\n\tburlywood: [222, 184, 135],\n\tcadetblue: [95, 158, 160],\n\tchartreuse: [127, 255, 0],\n\tchocolate: [210, 105, 30],\n\tcoral: [255, 127, 80],\n\tcornflowerblue: [100, 149, 237],\n\tcornsilk: [255, 248, 220],\n\tcrimson: [220, 20, 60],\n\tcyan: [0, 255, 255],\n\tdarkblue: [0, 0, 139],\n\tdarkcyan: [0, 139, 139],\n\tdarkgoldenrod: [184, 134, 11],\n\tdarkgray: [169, 169, 169],\n\tdarkgreen: [0, 100, 0],\n\tdarkgrey: [169, 169, 169],\n\tdarkkhaki: [189, 183, 107],\n\tdarkmagenta: [139, 0, 139],\n\tdarkolivegreen: [85, 107, 47],\n\tdarkorange: [255, 140, 0],\n\tdarkorchid: [153, 50, 204],\n\tdarkred: [139, 0, 0],\n\tdarksalmon: [233, 150, 122],\n\tdarkseagreen: [143, 188, 143],\n\tdarkslateblue: [72, 61, 139],\n\tdarkslategray: [47, 79, 79],\n\tdarkslategrey: [47, 79, 79],\n\tdarkturquoise: [0, 206, 209],\n\tdarkviolet: [148, 0, 211],\n\tdeeppink: [255, 20, 147],\n\tdeepskyblue: [0, 191, 255],\n\tdimgray: [105, 105, 105],\n\tdimgrey: [105, 105, 105],\n\tdodgerblue: [30, 144, 255],\n\tfirebrick: [178, 34, 34],\n\tfloralwhite: [255, 250, 240],\n\tforestgreen: [34, 139, 34],\n\tfuchsia: [255, 0, 255],\n\tgainsboro: [220, 220, 220],\n\tghostwhite: [248, 248, 255],\n\tgold: [255, 215, 0],\n\tgoldenrod: [218, 165, 32],\n\tgray: [128, 128, 128],\n\tgreen: [0, 128, 0],\n\tgreenyellow: [173, 255, 47],\n\tgrey: [128, 128, 128],\n\thoneydew: [240, 255, 240],\n\thotpink: [255, 105, 180],\n\tindianred: [205, 92, 92],\n\tindigo: [75, 0, 130],\n\tivory: [255, 255, 240],\n\tkhaki: [240, 230, 140],\n\tlavender: [230, 230, 250],\n\tlavenderblush: [255, 240, 245],\n\tlawngreen: [124, 252, 0],\n\tlemonchiffon: [255, 250, 205],\n\tlightblue: [173, 216, 230],\n\tlightcoral: [240, 128, 128],\n\tlightcyan: [224, 255, 255],\n\tlightgoldenrodyellow: [250, 250, 210],\n\tlightgray: [211, 211, 211],\n\tlightgreen: [144, 238, 144],\n\tlightgrey: [211, 211, 211],\n\tlightpink: [255, 182, 193],\n\tlightsalmon: [255, 160, 122],\n\tlightseagreen: [32, 178, 170],\n\tlightskyblue: [135, 206, 250],\n\tlightslategray: [119, 136, 153],\n\tlightslategrey: [119, 136, 153],\n\tlightsteelblue: [176, 196, 222],\n\tlightyellow: [255, 255, 224],\n\tlime: [0, 255, 0],\n\tlimegreen: [50, 205, 50],\n\tlinen: [250, 240, 230],\n\tmagenta: [255, 0, 255],\n\tmaroon: [128, 0, 0],\n\tmediumaquamarine: [102, 205, 170],\n\tmediumblue: [0, 0, 205],\n\tmediumorchid: [186, 85, 211],\n\tmediumpurple: [147, 112, 219],\n\tmediumseagreen: [60, 179, 113],\n\tmediumslateblue: [123, 104, 238],\n\tmediumspringgreen: [0, 250, 154],\n\tmediumturquoise: [72, 209, 204],\n\tmediumvioletred: [199, 21, 133],\n\tmidnightblue: [25, 25, 112],\n\tmintcream: [245, 255, 250],\n\tmistyrose: [255, 228, 225],\n\tmoccasin: [255, 228, 181],\n\tnavajowhite: [255, 222, 173],\n\tnavy: [0, 0, 128],\n\toldlace: [253, 245, 230],\n\tolive: [128, 128, 0],\n\tolivedrab: [107, 142, 35],\n\torange: [255, 165, 0],\n\torangered: [255, 69, 0],\n\torchid: [218, 112, 214],\n\tpalegoldenrod: [238, 232, 170],\n\tpalegreen: [152, 251, 152],\n\tpaleturquoise: [175, 238, 238],\n\tpalevioletred: [219, 112, 147],\n\tpapayawhip: [255, 239, 213],\n\tpeachpuff: [255, 218, 185],\n\tperu: [205, 133, 63],\n\tpink: [255, 192, 203],\n\tplum: [221, 160, 221],\n\tpowderblue: [176, 224, 230],\n\tpurple: [128, 0, 128],\n\trebeccapurple: [102, 51, 153],\n\tred: [255, 0, 0],\n\trosybrown: [188, 143, 143],\n\troyalblue: [65, 105, 225],\n\tsaddlebrown: [139, 69, 19],\n\tsalmon: [250, 128, 114],\n\tsandybrown: [244, 164, 96],\n\tseagreen: [46, 139, 87],\n\tseashell: [255, 245, 238],\n\tsienna: [160, 82, 45],\n\tsilver: [192, 192, 192],\n\tskyblue: [135, 206, 235],\n\tslateblue: [106, 90, 205],\n\tslategray: [112, 128, 144],\n\tslategrey: [112, 128, 144],\n\tsnow: [255, 250, 250],\n\tspringgreen: [0, 255, 127],\n\tsteelblue: [70, 130, 180],\n\ttan: [210, 180, 140],\n\tteal: [0, 128, 128],\n\tthistle: [216, 191, 216],\n\ttomato: [255, 99, 71],\n\tturquoise: [64, 224, 208],\n\tviolet: [238, 130, 238],\n\twheat: [245, 222, 179],\n\twhite: [255, 255, 255],\n\twhitesmoke: [245, 245, 245],\n\tyellow: [255, 255, 0],\n\tyellowgreen: [154, 205, 50]\n}\n",
```

### Comparing `draggable-charts-1.2.4/draggable_charts/utils/callback.py` & `draggable-charts-1.2.5/draggable_charts/utils/callback.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/utils/component_func.py` & `draggable-charts-1.2.5/draggable_charts/utils/component_func.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/utils/options.py` & `draggable-charts-1.2.5/draggable_charts/utils/options.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/widgets/bezierchart.py` & `draggable-charts-1.2.5/draggable_charts/widgets/bezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/widgets/cubicbezierchart.py` & `draggable-charts-1.2.5/draggable_charts/widgets/cubicbezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/widgets/linechart.py` & `draggable-charts-1.2.5/draggable_charts/widgets/linechart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts/widgets/scatterchart.py` & `draggable-charts-1.2.5/draggable_charts/widgets/scatterchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.4/draggable_charts.egg-info/PKG-INFO` & `draggable-charts-1.2.5/draggable_charts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.2.4/draggable_charts.egg-info/SOURCES.txt` & `draggable-charts-1.2.5/draggable_charts.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 draggable_charts.egg-info/SOURCES.txt
 draggable_charts.egg-info/dependency_links.txt
 draggable_charts.egg-info/requires.txt
 draggable_charts.egg-info/top_level.txt
 draggable_charts/frontend/build/asset-manifest.json
 draggable_charts/frontend/build/bootstrap.min.css
 draggable_charts/frontend/build/index.html
-draggable_charts/frontend/build/static/js/main.c3c91322.js
-draggable_charts/frontend/build/static/js/main.c3c91322.js.LICENSE.txt
-draggable_charts/frontend/build/static/js/main.c3c91322.js.map
+draggable_charts/frontend/build/static/js/main.41dd267d.js
+draggable_charts/frontend/build/static/js/main.41dd267d.js.LICENSE.txt
+draggable_charts/frontend/build/static/js/main.41dd267d.js.map
 draggable_charts/utils/__init__.py
 draggable_charts/utils/callback.py
 draggable_charts/utils/component_func.py
 draggable_charts/utils/options.py
 draggable_charts/widgets/__init__.py
 draggable_charts/widgets/bezierchart.py
 draggable_charts/widgets/cubicbezierchart.py
```

### Comparing `draggable-charts-1.2.4/setup.py` & `draggable-charts-1.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-charts",
-    version="1.2.4",
+    version="1.2.5",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/draggable-charts",
     packages=setuptools.find_packages(),
```
