# Comparing `tmp/gradio_modal-0.0.2.tar.gz` & `tmp/gradio_modal-0.0.3.tar.gz`

## Comparing `gradio_modal-0.0.2.tar` & `gradio_modal-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/backend/gradio_modal/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/backend/gradio_modal/modal.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/backend/gradio_modal/modal.pyi
--rw-r--r--   0        0        0    20919 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/backend/gradio_modal/templates/component/index.js
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/backend/gradio_modal/templates/component/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/demo/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/demo/css.css
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/demo/space.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/frontend/Index.svelte
--rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/frontend/package-lock.json
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/frontend/package.json
--rw-r--r--   0        0        0    21606 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/.gitignore
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 gradio_modal-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/backend/gradio_modal/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/backend/gradio_modal/modal.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/backend/gradio_modal/modal.pyi
+-rw-r--r--   0        0        0    21118 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/backend/gradio_modal/templates/component/index.js
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/backend/gradio_modal/templates/component/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/demo/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/demo/css.css
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/demo/space.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/frontend/Index.svelte
+-rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/frontend/package-lock.json
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/frontend/package.json
+-rw-r--r--   0        0        0    21606 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/.gitignore
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 gradio_modal-0.0.3/PKG-INFO
```

### Comparing `gradio_modal-0.0.2/backend/gradio_modal/modal.py` & `gradio_modal-0.0.3/backend/gradio_modal/modal.py`

 * *Files identical despite different names*

### Comparing `gradio_modal-0.0.2/backend/gradio_modal/modal.pyi` & `gradio_modal-0.0.3/backend/gradio_modal/modal.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             show_progress: If True, will show progress animation while pending
             queue: If True, will place the request on the queue, if the queue has been enabled. If False, will not put this event on the queue, even if the queue has been enabled. If None, will use the queue setting of the gradio app.
             batch: If True, then the function should process a batch of inputs, meaning that it should accept a list of input values for each parameter. The lists should be of equal length (and be up to length `max_batch_size`). The function is then *required* to return a tuple of lists (even if there is only 1 output component), with each list in the tuple corresponding to one output component.
             max_batch_size: Maximum number of inputs to batch together if this is called from the queue (only relevant if batch=True)
             preprocess: If False, will not run preprocessing of component data before running 'fn' (e.g. leaving it as a base64 string if this method is called with the `Image` component).
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
-            every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds. Queue must be enabled.
-            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` event) would allow a second submission after the pending event is complete.
+            every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
+            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
             show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
```

### Comparing `gradio_modal-0.0.2/backend/gradio_modal/templates/component/index.js` & `gradio_modal-0.0.3/backend/gradio_modal/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 const {
-    SvelteComponent: R,
-    assign: V,
-    create_slot: W,
-    detach: X,
-    element: Y,
-    get_all_dirty_from_scope: Z,
-    get_slot_changes: p,
-    get_spread_update: x,
-    init: $,
-    insert: ee,
-    safe_not_equal: le,
+    SvelteComponent: V,
+    assign: W,
+    create_slot: X,
+    detach: Y,
+    element: Z,
+    get_all_dirty_from_scope: p,
+    get_slot_changes: x,
+    get_spread_update: $,
+    init: ee,
+    insert: le,
+    safe_not_equal: te,
     set_dynamic_element_data: z,
     set_style: m,
     toggle_class: g,
-    transition_in: U,
-    transition_out: F,
-    update_slot_base: te
+    transition_in: F,
+    transition_out: G,
+    update_slot_base: fe
 } = window.__gradio__svelte__internal;
 
-function fe(f) {
+function ne(f) {
     let e, l, a;
     const n = (
             /*#slots*/
             f[18].default
         ),
-        i = W(
+        i = X(
             n,
             f,
             /*$$scope*/
             f[17],
             null
         );
     let d = [{
@@ -43,18 +43,18 @@
             )
         }, {
             class: l = "block " + /*elem_classes*/
                 f[3].join(" ") + " svelte-1t38q2d"
         }],
         s = {};
     for (let t = 0; t < d.length; t += 1)
-        s = V(s, d[t]);
+        s = W(s, d[t]);
     return {
         c() {
-            e = Y(
+            e = Z(
                 /*tag*/
                 f[14]
             ), i && i.c(), z(
                 /*tag*/
                 f[14]
             )(e, s), g(
                 e,
@@ -103,39 +103,39 @@
                 "flex-grow",
                 /*scale*/
                 f[12]
             ), m(e, "min-width", `calc(min(${/*min_width*/
       f[13]}px, 100%))`), m(e, "border-width", "var(--block-border-width)");
         },
         m(t, o) {
-            ee(t, e, o), i && i.m(e, null), a = !0;
+            le(t, e, o), i && i.m(e, null), a = !0;
         },
         p(t, o) {
             i && i.p && (!a || o & /*$$scope*/
-                    131072) && te(
+                    131072) && fe(
                     i,
                     n,
                     t,
                     /*$$scope*/
                     t[17],
-                    a ? p(
+                    a ? x(
                         n,
                         /*$$scope*/
                         t[17],
                         o,
                         null
-                    ) : Z(
+                    ) : p(
                         /*$$scope*/
                         t[17]
                     ),
                     null
                 ), z(
                     /*tag*/
                     t[14]
-                )(e, s = x(d, [
+                )(e, s = $(d, [
                     (!a || o & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
                             t[7]
                         )
                     },
@@ -204,54 +204,54 @@
                     /*scale*/
                     t[12]
                 ), o & /*min_width*/
                 8192 && m(e, "min-width", `calc(min(${/*min_width*/
       t[13]}px, 100%))`);
         },
         i(t) {
-            a || (U(i, t), a = !0);
+            a || (F(i, t), a = !0);
         },
         o(t) {
-            F(i, t), a = !1;
+            G(i, t), a = !1;
         },
         d(t) {
-            t && X(e), i && i.d(t);
+            t && Y(e), i && i.d(t);
         }
     };
 }
 
-function ne(f) {
+function ae(f) {
     let e, l = (
         /*tag*/
-        f[14] && fe(f)
+        f[14] && ne(f)
     );
     return {
         c() {
             l && l.c();
         },
         m(a, n) {
             l && l.m(a, n), e = !0;
         },
         p(a, [n]) {
             /*tag*/
             a[14] && l.p(a, n);
         },
         i(a) {
-            e || (U(l, a), e = !0);
+            e || (F(l, a), e = !0);
         },
         o(a) {
-            F(l, a), e = !1;
+            G(l, a), e = !1;
         },
         d(a) {
             l && l.d(a);
         }
     };
 }
 
-function ae(f, e, l) {
+function ie(f, e, l) {
     let {
         $$slots: a = {},
         $$scope: n
     } = e, {
         height: i = void 0
     } = e, {
         width: d = void 0
@@ -262,65 +262,65 @@
     } = e, {
         variant: o = "solid"
     } = e, {
         border_mode: u = "base"
     } = e, {
         padding: b = !0
     } = e, {
-        type: c = "normal"
+        type: r = "normal"
     } = e, {
-        test_id: w = void 0
+        test_id: v = void 0
     } = e, {
-        explicit_call: r = !1
+        explicit_call: y = !1
     } = e, {
-        container: B = !0
+        container: k = !0
     } = e, {
-        visible: L = !0
+        visible: c = !0
     } = e, {
         allow_overflow: T = !0
     } = e, {
         scale: E = null
     } = e, {
         min_width: M = 0
-    } = e, P = c === "fieldset" ? "fieldset" : "div";
-    const Q = (_) => {
+    } = e, Q = r === "fieldset" ? "fieldset" : "div";
+    const R = (_) => {
         if (_ !== void 0) {
             if (typeof _ == "number")
                 return _ + "px";
             if (typeof _ == "string")
                 return _;
         }
     };
     return f.$$set = (_) => {
-        "height" in _ && l(0, i = _.height), "width" in _ && l(1, d = _.width), "elem_id" in _ && l(2, s = _.elem_id), "elem_classes" in _ && l(3, t = _.elem_classes), "variant" in _ && l(4, o = _.variant), "border_mode" in _ && l(5, u = _.border_mode), "padding" in _ && l(6, b = _.padding), "type" in _ && l(16, c = _.type), "test_id" in _ && l(7, w = _.test_id), "explicit_call" in _ && l(8, r = _.explicit_call), "container" in _ && l(9, B = _.container), "visible" in _ && l(10, L = _.visible), "allow_overflow" in _ && l(11, T = _.allow_overflow), "scale" in _ && l(12, E = _.scale), "min_width" in _ && l(13, M = _.min_width), "$$scope" in _ && l(17, n = _.$$scope);
+        "height" in _ && l(0, i = _.height), "width" in _ && l(1, d = _.width), "elem_id" in _ && l(2, s = _.elem_id), "elem_classes" in _ && l(3, t = _.elem_classes), "variant" in _ && l(4, o = _.variant), "border_mode" in _ && l(5, u = _.border_mode), "padding" in _ && l(6, b = _.padding), "type" in _ && l(16, r = _.type), "test_id" in _ && l(7, v = _.test_id), "explicit_call" in _ && l(8, y = _.explicit_call), "container" in _ && l(9, k = _.container), "visible" in _ && l(10, c = _.visible), "allow_overflow" in _ && l(11, T = _.allow_overflow), "scale" in _ && l(12, E = _.scale), "min_width" in _ && l(13, M = _.min_width), "$$scope" in _ && l(17, n = _.$$scope);
     }, [
         i,
         d,
         s,
         t,
         o,
         u,
         b,
-        w,
-        r,
-        B,
-        L,
+        v,
+        y,
+        k,
+        c,
         T,
         E,
         M,
-        P,
         Q,
-        c,
+        R,
+        r,
         n,
         a
     ];
 }
-class ie extends R {
+class se extends V {
     constructor(e) {
-        super(), $(this, e, ae, ne, le, {
+        super(), ee(this, e, ie, ae, te, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -331,15 +331,15 @@
             visible: 10,
             allow_overflow: 11,
             scale: 12,
             min_width: 13
         });
     }
 }
-const se = [{
+const _e = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -665,69 +665,69 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
-se.reduce(
+_e.reduce(
     (f, {
         color: e,
         primary: l,
         secondary: a
     }) => ({
         ...f,
         [e]: {
             primary: A[e][l],
             secondary: A[e][a]
         }
     }), {}
 );
 const {
-    SvelteComponent: _e,
-    attr: y,
-    create_slot: de,
-    detach: oe,
-    element: ce,
-    get_all_dirty_from_scope: re,
-    get_slot_changes: ue,
-    init: me,
-    insert: be,
+    SvelteComponent: de,
+    attr: j,
+    create_slot: oe,
+    detach: ce,
+    element: re,
+    get_all_dirty_from_scope: ue,
+    get_slot_changes: me,
+    init: be,
+    insert: ge,
     null_to_empty: D,
-    safe_not_equal: ge,
-    set_style: k,
+    safe_not_equal: he,
+    set_style: C,
     toggle_class: h,
-    transition_in: he,
+    transition_in: we,
     transition_out: ve,
-    update_slot_base: we
+    update_slot_base: ye
 } = window.__gradio__svelte__internal;
 
-function ye(f) {
+function ke(f) {
     let e, l, a = `calc(min(${/*min_width*/
   f[2]}px, 100%))`,
         n;
     const i = (
             /*#slots*/
             f[8].default
         ),
-        d = de(
+        d = oe(
             i,
             f,
             /*$$scope*/
             f[7],
             null
         );
     return {
         c() {
-            e = ce("div"), d && d.c(), y(
+            e = re("div"), d && d.c(), j(
                 e,
                 "id",
                 /*elem_id*/
                 f[3]
-            ), y(e, "class", l = D(
+            ), j(e, "class", l = D(
                 /*elem_classes*/
                 f[4].join(" ")
             ) + " svelte-1m1obck"), h(
                 e,
                 "gap",
                 /*gap*/
                 f[1]
@@ -738,54 +738,54 @@
                 f[6] === "compact"
             ), h(
                 e,
                 "panel",
                 /*variant*/
                 f[6] === "panel"
             ), h(e, "hide", ! /*visible*/
-                f[5]), k(
+                f[5]), C(
                 e,
                 "flex-grow",
                 /*scale*/
                 f[0]
-            ), k(e, "min-width", a);
+            ), C(e, "min-width", a);
         },
         m(s, t) {
-            be(s, e, t), d && d.m(e, null), n = !0;
+            ge(s, e, t), d && d.m(e, null), n = !0;
         },
         p(s, [t]) {
             d && d.p && (!n || t & /*$$scope*/
-                    128) && we(
+                    128) && ye(
                     d,
                     i,
                     s,
                     /*$$scope*/
                     s[7],
-                    n ? ue(
+                    n ? me(
                         i,
                         /*$$scope*/
                         s[7],
                         t,
                         null
-                    ) : re(
+                    ) : ue(
                         /*$$scope*/
                         s[7]
                     ),
                     null
                 ), (!n || t & /*elem_id*/
-                    8) && y(
+                    8) && j(
                     e,
                     "id",
                     /*elem_id*/
                     s[3]
                 ), (!n || t & /*elem_classes*/
                     16 && l !== (l = D(
                         /*elem_classes*/
                         s[4].join(" ")
-                    ) + " svelte-1m1obck")) && y(e, "class", l), (!n || t & /*elem_classes, gap*/
+                    ) + " svelte-1m1obck")) && j(e, "class", l), (!n || t & /*elem_classes, gap*/
                     18) && h(
                     e,
                     "gap",
                     /*gap*/
                     s[1]
                 ), (!n || t & /*elem_classes, variant*/
                     80) && h(
@@ -798,36 +798,36 @@
                     e,
                     "panel",
                     /*variant*/
                     s[6] === "panel"
                 ), (!n || t & /*elem_classes, visible*/
                     48) && h(e, "hide", ! /*visible*/
                     s[5]), t & /*scale*/
-                1 && k(
+                1 && C(
                     e,
                     "flex-grow",
                     /*scale*/
                     s[0]
                 ), t & /*min_width*/
                 4 && a !== (a = `calc(min(${/*min_width*/
-      s[2]}px, 100%))`) && k(e, "min-width", a);
+      s[2]}px, 100%))`) && C(e, "min-width", a);
         },
         i(s) {
-            n || (he(d, s), n = !0);
+            n || (we(d, s), n = !0);
         },
         o(s) {
             ve(d, s), n = !1;
         },
         d(s) {
-            s && oe(e), d && d.d(s);
+            s && ce(e), d && d.d(s);
         }
     };
 }
 
-function ke(f, e, l) {
+function je(f, e, l) {
     let {
         $$slots: a = {},
         $$scope: n
     } = e, {
         scale: i = null
     } = e, {
         gap: d = !0
@@ -838,230 +838,231 @@
     } = e, {
         elem_classes: o = []
     } = e, {
         visible: u = !0
     } = e, {
         variant: b = "default"
     } = e;
-    return f.$$set = (c) => {
-        "scale" in c && l(0, i = c.scale), "gap" in c && l(1, d = c.gap), "min_width" in c && l(2, s = c.min_width), "elem_id" in c && l(3, t = c.elem_id), "elem_classes" in c && l(4, o = c.elem_classes), "visible" in c && l(5, u = c.visible), "variant" in c && l(6, b = c.variant), "$$scope" in c && l(7, n = c.$$scope);
+    return f.$$set = (r) => {
+        "scale" in r && l(0, i = r.scale), "gap" in r && l(1, d = r.gap), "min_width" in r && l(2, s = r.min_width), "elem_id" in r && l(3, t = r.elem_id), "elem_classes" in r && l(4, o = r.elem_classes), "visible" in r && l(5, u = r.visible), "variant" in r && l(6, b = r.variant), "$$scope" in r && l(7, n = r.$$scope);
     }, [i, d, s, t, o, u, b, n, a];
 }
-let je = class extends _e {
+let Ce = class extends de {
     constructor(e) {
-        super(), me(this, e, ke, ye, ge, {
+        super(), be(this, e, je, ke, he, {
             scale: 0,
             gap: 1,
             min_width: 2,
             elem_id: 3,
             elem_classes: 4,
             visible: 5,
             variant: 6
         });
     }
 };
 const {
-    SvelteComponent: Ce,
-    append: qe,
-    attr: v,
-    binding_callbacks: Ie,
-    create_component: G,
+    SvelteComponent: qe,
+    append: Ie,
+    attr: w,
+    binding_callbacks: H,
+    create_component: J,
     create_slot: Se,
-    destroy_component: J,
-    detach: C,
-    element: j,
+    destroy_component: K,
+    detach: I,
+    element: q,
     get_all_dirty_from_scope: Be,
     get_slot_changes: Le,
     init: Te,
-    insert: q,
-    listen: K,
-    mount_component: O,
+    insert: S,
+    listen: O,
+    mount_component: P,
     noop: Ee,
     safe_not_equal: Me,
     space: ze,
-    toggle_class: H,
-    transition_in: I,
-    transition_out: S,
+    toggle_class: N,
+    transition_in: B,
+    transition_out: L,
     update_slot_base: Ae
 } = window.__gradio__svelte__internal;
 
-function N(f) {
+function U(f) {
     let e, l, a;
     return {
         c() {
-            e = j("div"), e.innerHTML = '<svg width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 1L9 9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path><path d="M9 1L1 9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path></svg>', v(e, "class", "close svelte-ra5mg6");
+            e = q("div"), e.innerHTML = '<svg width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 1L9 9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path><path d="M9 1L1 9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path></svg>', w(e, "class", "close svelte-7knbu5");
         },
         m(n, i) {
-            q(n, e, i), l || (a = K(
+            S(n, e, i), l || (a = O(
                 e,
                 "click",
                 /*close*/
-                f[5]
+                f[6]
             ), l = !0);
         },
         p: Ee,
         d(n) {
-            n && C(e), l = !1, a();
+            n && I(e), l = !1, a();
         }
     };
 }
 
 function De(f) {
     let e;
     const l = (
             /*#slots*/
-            f[7].default
+            f[8].default
         ),
         a = Se(
             l,
             f,
             /*$$scope*/
-            f[10],
+            f[12],
             null
         );
     return {
         c() {
             a && a.c();
         },
         m(n, i) {
             a && a.m(n, i), e = !0;
         },
         p(n, i) {
             a && a.p && (!e || i & /*$$scope*/
-                1024) && Ae(
+                4096) && Ae(
                 a,
                 l,
                 n,
                 /*$$scope*/
-                n[10],
+                n[12],
                 e ? Le(
                     l,
                     /*$$scope*/
-                    n[10],
+                    n[12],
                     i,
                     null
                 ) : Be(
                     /*$$scope*/
-                    n[10]
+                    n[12]
                 ),
                 null
             );
         },
         i(n) {
-            e || (I(a, n), e = !0);
+            e || (B(a, n), e = !0);
         },
         o(n) {
-            S(a, n), e = !1;
+            L(a, n), e = !1;
         },
         d(n) {
             a && a.d(n);
         }
     };
 }
 
 function He(f) {
     let e, l, a, n = (
         /*allow_user_close*/
-        f[3] && N(f)
+        f[3] && U(f)
     );
-    return l = new je({
+    return l = new Ce({
         props: {
             $$slots: {
                 default: [De]
             },
             $$scope: {
                 ctx: f
             }
         }
     }), {
         c() {
-            n && n.c(), e = ze(), G(l.$$.fragment);
+            n && n.c(), e = ze(), J(l.$$.fragment);
         },
         m(i, d) {
-            n && n.m(i, d), q(i, e, d), O(l, i, d), a = !0;
+            n && n.m(i, d), S(i, e, d), P(l, i, d), a = !0;
         },
         p(i, d) {
             /*allow_user_close*/
-            i[3] ? n ? n.p(i, d) : (n = N(i), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null);
+            i[3] ? n ? n.p(i, d) : (n = U(i), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null);
             const s = {};
             d & /*$$scope*/
-                1024 && (s.$$scope = {
+                4096 && (s.$$scope = {
                     dirty: d,
                     ctx: i
                 }), l.$set(s);
         },
         i(i) {
-            a || (I(l.$$.fragment, i), a = !0);
+            a || (B(l.$$.fragment, i), a = !0);
         },
         o(i) {
-            S(l.$$.fragment, i), a = !1;
+            L(l.$$.fragment, i), a = !1;
         },
         d(i) {
-            i && C(e), n && n.d(i), J(l, i);
+            i && I(e), n && n.d(i), K(l, i);
         }
     };
 }
 
 function Ne(f) {
     let e, l, a, n, i, d, s;
-    return a = new ie({
+    return a = new se({
         props: {
-            height: "100%",
+            allow_overflow: !1,
+            elem_classes: ["modal-block"],
             $$slots: {
                 default: [He]
             },
             $$scope: {
                 ctx: f
             }
         }
     }), {
         c() {
-            e = j("div"), l = j("div"), G(a.$$.fragment), v(l, "class", "modal-container svelte-ra5mg6"), v(e, "class", n = "modal " + /*elem_classes*/
-                f[2].join(" ") + " svelte-ra5mg6"), v(
+            e = q("div"), l = q("div"), J(a.$$.fragment), w(l, "class", "modal-container svelte-7knbu5"), w(e, "class", n = "modal " + /*elem_classes*/
+                f[2].join(" ") + " svelte-7knbu5"), w(
                 e,
                 "id",
                 /*elem_id*/
                 f[1]
-            ), H(e, "hide", ! /*visible*/
+            ), N(e, "hide", ! /*visible*/
                 f[0]);
         },
         m(t, o) {
-            q(t, e, o), qe(e, l), O(a, l, null), f[8](e), i = !0, d || (s = K(
+            S(t, e, o), Ie(e, l), P(a, l, null), f[9](l), f[10](e), i = !0, d || (s = O(
                 e,
                 "click",
                 /*click_handler*/
-                f[9]
+                f[11]
             ), d = !0);
         },
         p(t, [o]) {
             const u = {};
             o & /*$$scope, allow_user_close*/
-                1032 && (u.$$scope = {
+                4104 && (u.$$scope = {
                     dirty: o,
                     ctx: t
                 }), a.$set(u), (!i || o & /*elem_classes*/
                     4 && n !== (n = "modal " + /*elem_classes*/
-                        t[2].join(" ") + " svelte-ra5mg6")) && v(e, "class", n), (!i || o & /*elem_id*/
-                    2) && v(
+                        t[2].join(" ") + " svelte-7knbu5")) && w(e, "class", n), (!i || o & /*elem_id*/
+                    2) && w(
                     e,
                     "id",
                     /*elem_id*/
                     t[1]
                 ), (!i || o & /*elem_classes, visible*/
-                    5) && H(e, "hide", ! /*visible*/
+                    5) && N(e, "hide", ! /*visible*/
                     t[0]);
         },
         i(t) {
-            i || (I(a.$$.fragment, t), i = !0);
+            i || (B(a.$$.fragment, t), i = !0);
         },
         o(t) {
-            S(a.$$.fragment, t), i = !1;
+            L(a.$$.fragment, t), i = !1;
         },
         d(t) {
-            t && C(e), J(a), f[8](null), d = !1, s();
+            t && I(e), K(a), f[9](null), f[10](null), d = !1, s();
         }
     };
 }
 
 function Ue(f, e, l) {
     let {
         $$slots: a = {},
@@ -1072,54 +1073,62 @@
         elem_classes: d = []
     } = e, {
         visible: s = !1
     } = e, {
         allow_user_close: t = !0
     } = e, {
         gradio: o
-    } = e, u = null;
-    const b = () => {
+    } = e, u = null, b = null;
+    const r = () => {
         l(0, s = !1), o.dispatch("blur");
     };
-    document.addEventListener("keydown", (r) => {
-        t && r.key === "Escape" && b();
+    document.addEventListener("keydown", (c) => {
+        t && c.key === "Escape" && r();
     });
 
-    function c(r) {
-        Ie[r ? "unshift" : "push"](() => {
-            u = r, l(4, u);
+    function v(c) {
+        H[c ? "unshift" : "push"](() => {
+            b = c, l(5, b);
+        });
+    }
+
+    function y(c) {
+        H[c ? "unshift" : "push"](() => {
+            u = c, l(4, u);
         });
     }
-    const w = (r) => {
-        t && r.target === u && b();
+    const k = (c) => {
+        t && (c.target === u || c.target === b) && r();
     };
-    return f.$$set = (r) => {
-        "elem_id" in r && l(1, i = r.elem_id), "elem_classes" in r && l(2, d = r.elem_classes), "visible" in r && l(0, s = r.visible), "allow_user_close" in r && l(3, t = r.allow_user_close), "gradio" in r && l(6, o = r.gradio), "$$scope" in r && l(10, n = r.$$scope);
+    return f.$$set = (c) => {
+        "elem_id" in c && l(1, i = c.elem_id), "elem_classes" in c && l(2, d = c.elem_classes), "visible" in c && l(0, s = c.visible), "allow_user_close" in c && l(3, t = c.allow_user_close), "gradio" in c && l(7, o = c.gradio), "$$scope" in c && l(12, n = c.$$scope);
     }, [
         s,
         i,
         d,
         t,
         u,
         b,
+        r,
         o,
         a,
-        c,
-        w,
+        v,
+        y,
+        k,
         n
     ];
 }
-class Ge extends Ce {
+class Ge extends qe {
     constructor(e) {
         super(), Te(this, e, Ue, Ne, Me, {
             elem_id: 1,
             elem_classes: 2,
             visible: 0,
             allow_user_close: 3,
-            gradio: 6
+            gradio: 7
         });
     }
 }
 export {
     Ge as
     default
 };
```

### Comparing `gradio_modal-0.0.2/backend/gradio_modal/templates/component/style.css` & `gradio_modal-0.0.3/backend/gradio_modal/templates/component/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-.block.svelte-1t38q2d{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-1t38q2d{border-color:var(--color-accent)}.padded.svelte-1t38q2d{padding:var(--block-padding)}.hidden.svelte-1t38q2d{display:none}.hide-container.svelte-1t38q2d{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}div.svelte-1m1obck{display:flex;position:relative;flex-direction:column}div.svelte-1m1obck>*,div.svelte-1m1obck>.form>*{width:var(--size-full)}.gap.svelte-1m1obck{gap:var(--layout-gap)}.hide.svelte-1m1obck{display:none}.compact.svelte-1m1obck>*,.compact.svelte-1m1obck .box{border-radius:0}.compact.svelte-1m1obck,.panel.svelte-1m1obck{border:solid var(--panel-border-width) var(--panel-border-color);border-radius:var(--container-radius);background:var(--panel-background-fill);padding:var(--spacing-lg)}@media (min-width: 640px){.modal-container.svelte-ra5mg6{max-width:640px}}@media (min-width: 768px){.modal-container.svelte-ra5mg6{max-width:768px}}@media (min-width: 1024px){.modal-container.svelte-ra5mg6{max-width:1024px}}@media (min-width: 1280px){.modal-container.svelte-ra5mg6{max-width:1280px}}@media (min-width: 1536px){.modal-container.svelte-ra5mg6{max-width:1536px}}.modal.svelte-ra5mg6{position:fixed;left:0;top:0;width:100%;height:100%;z-index:100;background-color:#000;background-color:#0006;-webkit-backdrop-filter:blur(4px);backdrop-filter:blur(4px)}.modal-container.svelte-ra5mg6{padding:0 var(--size-8);margin:var(--size-8) auto;max-height:calc(100% - var(--size-8));overflow-y:hidden}.close.svelte-ra5mg6{display:flex;position:absolute;top:var(--block-label-margin);right:var(--block-label-margin);align-items:center;box-shadow:var(--shadow-drop);border:1px solid var(--border-color-primary);border-top:none;border-right:none;border-radius:var(--block-label-right-radius);background:var(--block-label-background-fill);padding:6px;height:24px;overflow:hidden;color:var(--block-label-text-color);font:var(--font);font-size:var(--button-small-text-size);cursor:pointer}.hide.svelte-ra5mg6{display:none}
+.block.svelte-1t38q2d{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-1t38q2d{border-color:var(--color-accent)}.padded.svelte-1t38q2d{padding:var(--block-padding)}.hidden.svelte-1t38q2d{display:none}.hide-container.svelte-1t38q2d{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}div.svelte-1m1obck{display:flex;position:relative;flex-direction:column}div.svelte-1m1obck>*,div.svelte-1m1obck>.form>*{width:var(--size-full)}.gap.svelte-1m1obck{gap:var(--layout-gap)}.hide.svelte-1m1obck{display:none}.compact.svelte-1m1obck>*,.compact.svelte-1m1obck .box{border-radius:0}.compact.svelte-1m1obck,.panel.svelte-1m1obck{border:solid var(--panel-border-width) var(--panel-border-color);border-radius:var(--container-radius);background:var(--panel-background-fill);padding:var(--spacing-lg)}@media (min-width: 640px){.modal-container.svelte-7knbu5{max-width:640px}}@media (min-width: 768px){.modal-container.svelte-7knbu5{max-width:768px}}@media (min-width: 1024px){.modal-container.svelte-7knbu5{max-width:1024px}}@media (min-width: 1280px){.modal-container.svelte-7knbu5{max-width:1280px}}@media (min-width: 1536px){.modal-container.svelte-7knbu5{max-width:1536px}}.modal.svelte-7knbu5{position:fixed;left:0;top:0;width:100%;height:100%;z-index:100;background-color:#000;background-color:#0006;-webkit-backdrop-filter:blur(4px);backdrop-filter:blur(4px)}.modal-container.svelte-7knbu5{position:relative;padding:0 var(--size-8);margin:var(--size-8) auto;height:100%;max-height:calc(100% - var(--size-16));overflow-y:hidden}.close.svelte-7knbu5{display:flex;position:absolute;top:var(--block-label-margin);right:var(--block-label-margin);align-items:center;box-shadow:var(--shadow-drop);border:1px solid var(--border-color-primary);border-top:none;border-right:none;border-radius:var(--block-label-right-radius);background:var(--block-label-background-fill);padding:6px;height:24px;overflow:hidden;color:var(--block-label-text-color);font:var(--font);font-size:var(--button-small-text-size);cursor:pointer}.modal.svelte-7knbu5 .modal-block{max-height:100%;overflow-y:auto!important}.hide.svelte-7knbu5{display:none}
```

### Comparing `gradio_modal-0.0.2/demo/app.py` & `gradio_modal-0.0.3/demo/app.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Tab 1"):
         text_1 = gr.Textbox(label="Input 1")
         text_2 = gr.Textbox(label="Input 2")
         text_1.submit(lambda x:x, text_1, text_2)
         show_btn = gr.Button("Show Modal")
+        show_btn2 = gr.Button("Show Modal 2")
         gr.Examples(
             [["Text 1", "Text 2"], ["Text 3", "Text 4"]],
             inputs=[text_1, text_2],
         )
     with gr.Tab("Tab 2"):
         gr.Markdown("This is tab 2")
     with Modal(visible=False) as modal:
-        gr.Markdown("Hello world!")
+        for i in range(5):
+            gr.Markdown("Hello world!")
+    with Modal(visible=False) as modal2:
+        for i in range(100):
+            gr.Markdown("Hello world!")
     show_btn.click(lambda: Modal(visible=True), None, modal)
+    show_btn2.click(lambda: Modal(visible=True), None, modal2)
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_modal-0.0.2/demo/css.css` & `gradio_modal-0.0.3/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_modal-0.0.2/demo/space.py` & `gradio_modal-0.0.3/demo/space.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import gradio as gr
 from app import demo as app
 import os
 
 _docs = {'Modal': {'description': 'Modal is a layout element within Blocks that will show its content in a popup above other content.\n    from gradio_modal import Modal\n    with gr.Blocks() as demo:\n        with Modal():\n            text1 = gr.Textbox()\n            text2 = gr.Textbox()\n            btn = gr.Button("Button")', 'members': {'__init__': {'visible': {'type': 'bool', 'default': 'False', 'description': 'If False, modal will be hidden.'}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': 'An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': 'An optional string or list of strings that are assigned as the class of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'allow_user_close': {'type': 'bool', 'default': 'True', 'description': 'If True, user can close the modal (by clicking outside, clicking the X, or the escape key).'}, 'render': {'type': 'bool', 'default': 'True', 'description': 'If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.'}}, 'postprocess': {}}, 'events': {'blur': {'type': None, 'default': None, 'description': 'This listener is triggered when the Modal is unfocused/blurred.'}}}, '__meta__': {'additional_interfaces': {}}}
-    
+
 abs_path = os.path.join(os.path.dirname(__file__), "css.css")
 
 with gr.Blocks(
     css=abs_path,
     theme=gr.themes.Default(
         font_mono=[
             gr.themes.GoogleFont("Inconsolata"),
@@ -43,23 +43,29 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Tab 1"):
         text_1 = gr.Textbox(label="Input 1")
         text_2 = gr.Textbox(label="Input 2")
         text_1.submit(lambda x:x, text_1, text_2)
         show_btn = gr.Button("Show Modal")
+        show_btn2 = gr.Button("Show Modal 2")
         gr.Examples(
             [["Text 1", "Text 2"], ["Text 3", "Text 4"]],
             inputs=[text_1, text_2],
         )
     with gr.Tab("Tab 2"):
         gr.Markdown("This is tab 2")
     with Modal(visible=False) as modal:
-        gr.Markdown("Hello world!")
+        for i in range(5):
+            gr.Markdown("Hello world!")
+    with Modal(visible=False) as modal2:
+        for i in range(100):
+            gr.Markdown("Hello world!")
     show_btn.click(lambda: Modal(visible=True), None, modal)
+    show_btn2.click(lambda: Modal(visible=True), None, modal2)
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
 """, elem_classes=["md-custom"], header_links=True)
 
@@ -95,15 +101,15 @@
                     el.innerHTML = el.innerHTML.replace(
                         new RegExp("\\b"+ref+"\\b", "g"),
                         `<a href="#h-${ref.toLowerCase()}">${ref}</a>`
                     );
                 })
             }
         })
-        
+
         Object.entries(refs).forEach(([key, refs]) => {
             if (refs.length > 0) {
                 const el = document.querySelector(`.${key}`);
                 if (!el) return;
                 refs.forEach(ref => {
                     el.innerHTML = el.innerHTML.replace(
                         new RegExp("\\b"+ref+"\\b", "g"),
```

### Comparing `gradio_modal-0.0.2/frontend/Index.svelte` & `gradio_modal-0.0.3/frontend/Index.svelte`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 	export let visible = false;
 	export let allow_user_close = true;
 	export let gradio: Gradio<{
 		blur: never;
 	}>;
 
 	let element: HTMLElement | null = null;
+	let inner_element: HTMLElement | null = null;
 	const close = () => {
 		visible = false;
 		gradio.dispatch("blur");
 	};
 
 	document.addEventListener("keydown", (evt: KeyboardEvent) => {
 		if (allow_user_close && evt.key === "Escape") {
@@ -26,21 +27,21 @@
 <!-- svelte-ignore a11y-click-events-have-key-events -->
 <div
 	class="modal {elem_classes.join(' ')}"
 	bind:this={element}
 	class:hide={!visible}
 	id={elem_id}
 	on:click={(evt) => {
-		if (allow_user_close && evt.target === element) {
+		if (allow_user_close && (evt.target === element || evt.target === inner_element)) {
 			close();
 		}
 	}}
 >
-	<div class="modal-container">
-		<Block height="100%">
+	<div class="modal-container" bind:this={inner_element}	>
+		<Block allow_overflow={false} elem_classes={["modal-block"]}>
 			{#if allow_user_close}
 				<div class="close" on:click={close}>
 					<svg
 						width="10"
 						height="10"
 						viewBox="0 0 10 10"
 						fill="none"
@@ -110,17 +111,19 @@
 		height: 100%; /* Full height */
 		z-index: 100;
 		background-color: rgb(0, 0, 0); /* Fallback color */
 		background-color: rgba(0, 0, 0, 0.4); /* Black w/ opacity */
 		backdrop-filter: blur(4px);
 	}
 	.modal-container {
+		position: relative;
 		padding: 0 var(--size-8);
 		margin: var(--size-8) auto;
-		max-height: calc(100% - var(--size-8));
+		height: 100%;
+		max-height: calc(100% - var(--size-16));
 		overflow-y: hidden;
 	}
 	.close {
 		display: flex;
 		position: absolute;
 		top: var(--block-label-margin);
 		right: var(--block-label-margin);
@@ -135,12 +138,16 @@
 		height: 24px;
 		overflow: hidden;
 		color: var(--block-label-text-color);
 		font: var(--font);
 		font-size: var(--button-small-text-size);
 		cursor: pointer;
 	}
+	.modal :global(.modal-block) {
+		max-height: 100%;
+		overflow-y: auto !important;
+	}
 
 	.hide {
 		display: none;
 	}
 </style>
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
-> { if (allow_user_close && evt.target === element) { close(); } }} >
+> { if (allow_user_close && (evt.target === element || evt.target ===
+inner_element)) { close(); } }} >
 {#if allow_user_close}
 {/if}
```

### Comparing `gradio_modal-0.0.2/frontend/package-lock.json` & `gradio_modal-0.0.3/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_modal-0.0.2/frontend/pnpm-lock.yaml` & `gradio_modal-0.0.3/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `gradio_modal-0.0.2/README.md` & `gradio_modal-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 # `gradio_modal`
 <a href="https://pypi.org/project/gradio_modal/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_modal"></a>  
 
 A popup modal component
 
 ## Installation
-    
-```bash 
+
+```bash
 pip install gradio_modal
 ```
 
 ## Usage
 
 ```python
 import gradio as gr
@@ -18,23 +18,29 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Tab 1"):
         text_1 = gr.Textbox(label="Input 1")
         text_2 = gr.Textbox(label="Input 2")
         text_1.submit(lambda x:x, text_1, text_2)
         show_btn = gr.Button("Show Modal")
+        show_btn2 = gr.Button("Show Modal 2")
         gr.Examples(
             [["Text 1", "Text 2"], ["Text 3", "Text 4"]],
             inputs=[text_1, text_2],
         )
     with gr.Tab("Tab 2"):
         gr.Markdown("This is tab 2")
     with Modal(visible=False) as modal:
-        gr.Markdown("Hello world!")
+        for i in range(5):
+            gr.Markdown("Hello world!")
+    with Modal(visible=False) as modal2:
+        for i in range(100):
+            gr.Markdown("Hello world!")
     show_btn.click(lambda: Modal(visible=True), None, modal)
+    show_btn2.click(lambda: Modal(visible=True), None, modal2)
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
 
 ## `Modal`
```

### Comparing `gradio_modal-0.0.2/pyproject.toml` & `gradio_modal-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_modal"
-version = "0.0.2"
+version = "0.0.3"
 description = "A popup modal component"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Column", "Modal, Popup"]
 # Add dependencies here
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_modal/templates", "*.pyi", "backend/gradio_modal/templates", "backend/gradio_modal/templates", "backend/gradio_modal/templates", "backend/gradio_modal/templates"]
+artifacts = ["/backend/gradio_modal/templates", "*.pyi", "backend/gradio_modal/templates", "backend/gradio_modal/templates", "backend/gradio_modal/templates", "backend/gradio_modal/templates", "backend/gradio_modal/templates", "backend/gradio_modal/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_modal"]
```

### Comparing `gradio_modal-0.0.2/PKG-INFO` & `gradio_modal-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gradio_modal
-Version: 0.0.2
+Version: 0.0.3
 Summary: A popup modal component
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: MIT
 Keywords: Modal, Popup,gradio-custom-component,gradio-template-Column
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,16 @@
 
 # `gradio_modal`
 <a href="https://pypi.org/project/gradio_modal/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_modal"></a>  
 
 A popup modal component
 
 ## Installation
-    
-```bash 
+
+```bash
 pip install gradio_modal
 ```
 
 ## Usage
 
 ```python
 import gradio as gr
@@ -44,23 +44,29 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Tab 1"):
         text_1 = gr.Textbox(label="Input 1")
         text_2 = gr.Textbox(label="Input 2")
         text_1.submit(lambda x:x, text_1, text_2)
         show_btn = gr.Button("Show Modal")
+        show_btn2 = gr.Button("Show Modal 2")
         gr.Examples(
             [["Text 1", "Text 2"], ["Text 3", "Text 4"]],
             inputs=[text_1, text_2],
         )
     with gr.Tab("Tab 2"):
         gr.Markdown("This is tab 2")
     with Modal(visible=False) as modal:
-        gr.Markdown("Hello world!")
+        for i in range(5):
+            gr.Markdown("Hello world!")
+    with Modal(visible=False) as modal2:
+        for i in range(100):
+            gr.Markdown("Hello world!")
     show_btn.click(lambda: Modal(visible=True), None, modal)
+    show_btn2.click(lambda: Modal(visible=True), None, modal2)
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
 
 ## `Modal`
```

