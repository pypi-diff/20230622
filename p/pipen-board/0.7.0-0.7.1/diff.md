# Comparing `tmp/pipen_board-0.7.0.tar.gz` & `tmp/pipen_board-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.7.0.tar", max compression
+gzip compressed data, was "pipen_board-0.7.1.tar", max compression
```

## Comparing `pipen_board-0.7.0.tar` & `pipen_board-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6884 2023-06-22 04:12:28.680642 pipen_board-0.7.0/README.md
--rw-r--r--   0        0        0      269 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/__init__.py
--rw-r--r--   0        0        0      517 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/additional_auto.toml
--rw-r--r--   0        0        0    15248 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/apis.py
--rw-r--r--   0        0        0     4594 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/cli.py
--rw-r--r--   0        0        0    31722 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/data_manager.py
--rw-r--r--   0        0        0     6233 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   625768 2023-06-22 04:12:28.684642 pipen_board-0.7.0/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   770030 2023-06-22 04:12:28.688642 pipen_board-0.7.0/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-06-22 04:12:28.688642 pipen_board-0.7.0/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-06-22 04:12:28.688642 pipen_board-0.7.0/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7742 2023-06-22 04:12:28.692642 pipen_board-0.7.0/pipen_board/plugin.py
--rw-r--r--   0        0        0     3831 2023-06-22 04:12:28.692642 pipen_board-0.7.0/pipen_board/quart_app.py
--rw-r--r--   0        0        0       22 2023-06-22 04:12:28.692642 pipen_board-0.7.0/pipen_board/version.py
--rw-r--r--   0        0        0      890 2023-06-22 04:12:28.696642 pipen_board-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 pipen_board-0.7.0/setup.py
--rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 pipen_board-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     6884 2023-06-22 17:45:33.467335 pipen_board-0.7.1/README.md
+-rw-r--r--   0        0        0      269 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/additional_auto.toml
+-rw-r--r--   0        0        0    15248 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/apis.py
+-rw-r--r--   0        0        0     4594 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/cli.py
+-rw-r--r--   0        0        0    31722 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     6233 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-06-22 17:45:33.467335 pipen_board-0.7.1/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   625768 2023-06-22 17:45:33.471335 pipen_board-0.7.1/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   770013 2023-06-22 17:45:33.475335 pipen_board-0.7.1/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-06-22 17:45:33.475335 pipen_board-0.7.1/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-06-22 17:45:33.475335 pipen_board-0.7.1/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7742 2023-06-22 17:45:33.479335 pipen_board-0.7.1/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3831 2023-06-22 17:45:33.479335 pipen_board-0.7.1/pipen_board/quart_app.py
+-rw-r--r--   0        0        0       22 2023-06-22 17:45:33.479335 pipen_board-0.7.1/pipen_board/version.py
+-rw-r--r--   0        0        0      890 2023-06-22 17:45:33.479335 pipen_board-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 pipen_board-0.7.1/setup.py
+-rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 pipen_board-0.7.1/PKG-INFO
```

### Comparing `pipen_board-0.7.0/README.md` & `pipen_board-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/additional_auto.toml` & `pipen_board-0.7.1/pipen_board/additional_auto.toml`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/apis.py` & `pipen_board-0.7.1/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/cli.py` & `pipen_board-0.7.1/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/data_manager.py` & `pipen_board-0.7.1/pipen_board/data_manager.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/defaults.py` & `pipen_board-0.7.1/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.7.1/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.7.1/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.7.1/pipen_board/frontend/build/assets/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4716,15 +4716,15 @@
         r = r[l] && r[l].value
     }
     return r
 }
 const IS_DEV = window.location.search.includes("dev=1"),
     storedGlobalChanged = writable(!1),
     storedErrors = writable({}),
-    storedConfigfile = writable(localStorage.getItem("configfile") || ""),
+    storedConfigfile = writable(localStorage.getItem("configfile") === "undefined" ? void 0 : localStorage.getItem("configfile")),
     descFocused = writable(!1),
     setError = (t, e) => {
         storedErrors.update(n => ({
             ...n,
             [t]: e
         }))
     },
@@ -9836,18 +9836,18 @@
     l = new Dashboard({});
     let S = t[3] && create_if_block$P(t);
     return {
         c() {
             e = element("header"), n = element("div"), r = element("div"), create_component(l.$$.fragment), a = space(), o = element("a"), o.textContent = "PIPEN BOARD", u = space(), s = element("em"), c = text("v"), _ = new HtmlTag(!1), d = space(), g = element("h1"), h = text(t[1]), p = space(), m = element("div"), k = text(v), b = space(), E = element("div"), S && S.c(), attr(o, "href", "https://github.com/pwwang/pipen-board"), attr(o, "target", "_blank"), attr(o, "class", "svelte-1fqt7sq"), _.a = null, attr(r, "class", "wizard-desc svelte-1fqt7sq"), attr(g, "class", "svelte-1fqt7sq"), attr(n, "class", "header-left svelte-1fqt7sq"), attr(E, "class", "header-right svelte-1fqt7sq"), attr(e, "class", "svelte-1fqt7sq")
         },
         m(I, D) {
-            insert(I, e, D), append(e, n), append(n, r), mount_component(l, r, null), append(r, a), append(r, o), append(r, u), append(r, s), append(s, c), _.m(t[6], s), append(n, d), append(n, g), append(g, h), append(n, p), append(n, m), append(m, k), append(e, b), append(e, E), S && S.m(E, null), w = !0
+            insert(I, e, D), append(e, n), append(n, r), mount_component(l, r, null), append(r, a), append(r, o), append(r, u), append(r, s), append(s, c), _.m(t[5], s), append(n, d), append(n, g), append(g, h), append(n, p), append(n, m), append(m, k), append(e, b), append(e, E), S && S.m(E, null), w = !0
         },
         p(I, [D]) {
-            (!w || D & 64) && _.p(I[6]), (!w || D & 2) && set_data(h, I[1]), (!w || D & 4) && v !== (v = (I[2] ? I[2] : "") + "") && set_data(k, v), I[3] ? S ? (S.p(I, D), D & 8 && transition_in(S, 1)) : (S = create_if_block$P(I), S.c(), transition_in(S, 1), S.m(E, null)) : S && (group_outros(), transition_out(S, 1, 1, () => {
+            (!w || D & 32) && _.p(I[5]), (!w || D & 2) && set_data(h, I[1]), (!w || D & 4) && v !== (v = (I[2] ? I[2] : "") + "") && set_data(k, v), I[3] ? S ? (S.p(I, D), D & 8 && transition_in(S, 1)) : (S = create_if_block$P(I), S.c(), transition_in(S, 1), S.m(E, null)) : S && (group_outros(), transition_out(S, 1, 1, () => {
                 S = null
             }), check_outros())
         },
         i(I) {
             w || (transition_in(l.$$.fragment, I), transition_in(S), w = !0)
         },
         o(I) {
@@ -9857,15 +9857,15 @@
             I && detach(e), destroy_component(l), S && S.d()
         }
     }
 }
 
 function instance$1d(t, e, n) {
     let r;
-    component_subscribe(t, storedGlobalChanged, h => n(7, r = h));
+    component_subscribe(t, storedGlobalChanged, h => n(6, r = h));
     let {
         pipelineName: l
     } = e, {
         pipelineDesc: a = void 0
     } = e, {
         backToHistory: o = !1
     } = e, {
@@ -9873,35 +9873,35 @@
     } = e, {
         histories: s
     } = e, {
         isRunning: c = !1
     } = e, _ = "0.0.0";
     onMount(async function() {
         try {
-            n(6, _ = await fetchAPI("/api/version", {}, "text"))
+            n(5, _ = await fetchAPI("/api/version", {}, "text"))
         } catch {
-            n(6, _ = '<font style="color:red">Error</font>')
+            n(5, _ = '<font style="color:red">Error</font>')
         }
     });
     const g = () => {
-        c ? alert("Please wait until the pipeline is finished or stop it before switching to a different configuration") : s.length > 0 ? (!r || confirm("You have unsaved changes. Are you sure to discard them?")) && (n(0, u = void 0), storedConfigfile.set(void 0)) : alert("No history available")
+        c ? alert("Please wait until the pipeline is finished or stop it before switching to a different configuration") : (!r || confirm("You have unsaved changes. Are you sure to discard them?")) && (n(0, u = void 0), storedConfigfile.set(void 0))
     };
     return t.$$set = h => {
-        "pipelineName" in h && n(1, l = h.pipelineName), "pipelineDesc" in h && n(2, a = h.pipelineDesc), "backToHistory" in h && n(3, o = h.backToHistory), "configfile" in h && n(0, u = h.configfile), "histories" in h && n(4, s = h.histories), "isRunning" in h && n(5, c = h.isRunning)
-    }, [u, l, a, o, s, c, _, r, g]
+        "pipelineName" in h && n(1, l = h.pipelineName), "pipelineDesc" in h && n(2, a = h.pipelineDesc), "backToHistory" in h && n(3, o = h.backToHistory), "configfile" in h && n(0, u = h.configfile), "histories" in h && n(7, s = h.histories), "isRunning" in h && n(4, c = h.isRunning)
+    }, [u, l, a, o, c, _, r, s, g]
 }
 class Header extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1d, create_fragment$1d, safe_not_equal, {
             pipelineName: 1,
             pipelineDesc: 2,
             backToHistory: 3,
             configfile: 0,
-            histories: 4,
-            isRunning: 5
+            histories: 7,
+            isRunning: 4
         })
     }
 }
 const History_svelte_svelte_type_style_lang = "";
 
 function create_if_block_1$l(t) {
     let e, n;
@@ -10499,15 +10499,15 @@
                 n(3, u = "Cancelled creating a new instance.");
                 return
             }
             if (O === "" && (O = _), a.find(B => B.is_current && B.name === O)) {
                 n(3, u = `The name "${O}" is already used under current working directory.`);
                 return
             }
-            storedGlobalChanged.set(!1), updateErrors({}), updateConfigfile(""), n(1, o = `new:${O}`)
+            storedGlobalChanged.set(!1), updateErrors({}), updateConfigfile(void 0), n(1, o = `new:${O}`)
         }, w = O => {
             storedGlobalChanged.set(!1), updateErrors({}), updateConfigfile(O.value[1]), n(1, o = O.value[1])
         }, S = O => {
             n(4, s = O.value[0]), h(...O.value)
         }, I = O => {
             n(4, s = O.value[0]), p(...O.value)
         }, D = O => {
@@ -28890,15 +28890,15 @@
                 </ul>
             `, b);
                 return
             }
             n(6, p = !0), n(5, h = stringify(finalizeConfig(d)))
         },
         O = async function(H = !1) {
-            if (!a) return;
+            if (!a && !H) return;
             if (Object.keys(l).length > 0) {
                 const _e = Object.keys(l);
                 n(8, b.kind = "error", b), n(8, b.subtitle = `
                 There are errors in the configuration. Please fix them before saving:
                 <br />
                 <ul>
                     ${_e.map(he=>`<li>${he}: ${l[he]}</li>`).join("")}
@@ -28937,15 +28937,15 @@
             }
             if (b.kind !== "error") {
                 n(1, u = se.configfile), n(8, b.kind = "success", b), n(8, b.subtitle = `Saved to ${u}`, b);
                 const _e = s.find(he => he.configfile === u);
                 _e ? n(20, s = [...s.filter(he => he.configfile !== u), {
                     ..._e,
                     ...se
-                }]) : n(20, s = [...s, se]), storedGlobalChanged.set(!1)
+                }]) : n(20, s = [...s, se]), storedGlobalChanged.set(!1), updateConfigfile(u)
             }
         }, B = function() {
             const H = document.createElement("a"),
                 x = new Blob([h], {
                     type: "text/plain"
                 });
             H.href = URL.createObjectURL(x), H.download = `${d[SECTION_PIPELINE_OPTS].name.value}config.toml`, document.body.appendChild(H), H.click(), H.remove()
@@ -33139,15 +33139,15 @@
             create_component(e.$$.fragment)
         },
         m(r, l) {
             mount_component(e, r, l), n = !0
         },
         p(r, l) {
             const a = {};
-            l & 8388739 && (a.$$scope = {
+            l & 8388737 && (a.$$scope = {
                 dirty: l,
                 ctx: r
             }), e.$set(a)
         },
         i(r) {
             n || (transition_in(e.$$.fragment, r), n = !0)
         },
@@ -33610,15 +33610,15 @@
             n(7, _ = `<strong>Failed to fetch or parse data:</strong> <br /><br /><pre>${G}</pre>`)
         } finally {
             n(6, c = !1)
         }
         _ || (IS_DEV && (window.data = L), n(2, a = L.runStarted + 0), n(4, u = L.config), n(5, s = L.run), n(8, d = u[SECTION_PIPELINE_OPTS].name.value), n(9, g = u[SECTION_PIPELINE_OPTS].desc.value), n(10, h = getStatusPercentage(s))), storedGlobalChanged.set(!1)
     });
     const v = () => {
-        l.length > 0 ? n(0, r = void 0) : alert("No history available")
+        n(0, r = void 0)
     };
 
     function k(L) {
         r = L, n(0, r)
     }
 
     function b(L) {
@@ -33857,15 +33857,15 @@
 
 function create_fragment(t) {
     let e, n, r, l, a, o, u;
     const s = [create_if_block, create_if_block_1, create_if_block_2, create_else_block],
         c = [];
 
     function _(d, g) {
-        return d[4] ? 0 : d[3] ? 1 : d[1].length > 0 && d[2] === void 0 ? 2 : 3
+        return d[4] ? 0 : d[3] ? 1 : d[2] === void 0 ? 2 : 3
     }
     return n = _(t), r = c[n] = s[n](t), {
         c() {
             e = space(), r.c(), l = empty(), document.title = "PIPEN BOARD"
         },
         m(d, g) {
             insert(d, e, g), c[n].m(d, g), insert(d, l, g), a = !0, o || (u = listen(window, "beforeunload", t[5]), o = !0)
```

### Comparing `pipen_board-0.7.0/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.7.1/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/plugin.py` & `pipen_board-0.7.1/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pipen_board/quart_app.py` & `pipen_board-0.7.1/pipen_board/quart_app.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.0/pyproject.toml` & `pipen_board-0.7.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.7.0"
+version = "0.7.1"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
```

### Comparing `pipen_board-0.7.0/setup.py` & `pipen_board-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': '# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nConfigure and run pipen pipelines from the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline.\n                        For the pipeline either\n                        `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an\n                        instance of `Pipen` and running the pipeline should be\n                        called under `__name__ == \'__main__\'.\n\nOptions:\n  -h, --help            show help message and exit\n  -p PORT, --port PORT  Port to serve the UI wizard [default: 18521]\n  -a FILE, --additional FILE\n                        Additional arguments for the pipeline, in YAML, INI,\n                        JSON or TOML format. Can have sections\n                        `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`. It can also\n                        have other sections and items to override the\n                        configurations generated from the pipeline. If the\n                        pipeline is provided as a python script, such as\n                        `/path/to/pipeline.py:<pipeline>`, and `<pipeline>`\n                        runs under `__name__ == \'__main__\'`, the additional\n                        file can also be specified as `auto` to generate a\n                        `RUNNING OPTIONS/Local` section to run the pipeline\n                        locally.\n  --loglevel {auto,debug,info,warning,error,critical}\n                        The logging level. If `auto`, it will be set to `debug`\n                        if `--dev` is set, otherwise `info`. [default: auto]\n  --dev                 Run the pipeline in development/debug mode. This will\n                        reload the server when changes are made to this package\n                        and reload the pipeline when page reloads for new\n                        configurations. Page cache is also disabled in this\n                        mode.\n  -w WORKDIR, --workdir WORKDIR\n                        The working directory of the pipeline. [default:\n                        .pipen]\n```\n\n## Describing arguments in docstring\n\n### Docstring schema\n\n```python\nclass ProcessOrProcessGroup:\n    """Short summary\n\n    Long description\n    Long description\n\n    Args:\n        arg1 (<metadata>): description\n            - subarg1 (<metadata>): description\n            - subarg2 (<metadata>): description\n        arg2 (<metadata>): description\n\n    <Other Sections>:\n        <content>\n    """\n```\n\nThe metadata can have multiple attributes, separated by semicolon (`;`). For example:\n\n```\narg1 (action=ns;required): description\n```\n\n### Marks\n\nYou can mark a process using `pipen.utils.mark(<mark>=<value>)` as a decorator to decorate a process. For example:\n\n```python\nfrom pipen import Proc\nfrom pipen.utils import mark\n\n@mark(board_config_no_input=True)\nclass MyProc(Proc):\n    pass\n```\n\nAvailable marks:\n\n- `board_config_no_input`: Whether to show the input section for the process in configuation page. Only affects the start processes. Default to `False`.\n- `board_config_hidden`: Whether to hide the process options in the configuration page. Note that the process is still visible in the process list. Default to `False`.\n\n### Metadata for arguments\n\n\n| Name     | Description | Allowed values |\n| -------- | ----------- | -------------- |\n| `action` | Like the `action` argument in [`argx`][2]*. | `store_true`, `store_false`, `ns`, `namespace`, `append`, `extend`, `clear_append`, `clear_extend` (other values are allowed but ignore, they may be effective for CLI use) |\n| `btype`  | Board type (option type specified directly). If specified, `action` will be ignored | `ns`, `choice`, `mchoice`, `array`, `list`, `json`, `int`, `float`, `bool`, `str`, `text`, `auto`* |\n| `type` | Fallback for `action` and `btype` | Same as `btype` |\n| `flag` | Fallback for `action=store_true` | No values needed |\n| `text`/`mline`/`mlines` | Shortcut for `btype=text` | No values needed |\n| `ns`/`namespace` | Shortcut for `btype=ns` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `array`/`list` | Shortcut for `btype=array`/`btype=list` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `order` | The order of the argument in the UI. | Any integer |\n| `readonly` | Whether the argument is readonly. | No values needed (True if specified, otherwise False) |\n| `required` | Whether the argument is required. | No values needed (True if specified, otherwise False) |\n| `placeholder` | The placeholder in the UI for the argument. | Any string |\n| `bitype` | The type of the elements in an array or list. | `int`, `float`, `bool`, `str`, `json`, `auto`* |\n| `itype` | Fallback for `bitype` | Same as `bitype` |\n\n- `argx*`: An argument parser for Python, compatible with `argparse`.\n- `auto*`: Automatically infer the type from a string value.\n  - Any of `True`, `TRUE`, `true`, `False`, `FALSE`, `false` will be inferred as a `bool` value.\n  - Any of `None`, `NONE`, `none`, `null`, `NULL` will be inferred as `None`.\n  - Any integers will be inferred as `int`.\n  - Any floats will be inferred as `float`.\n  - Try to parse the value as JSON. If succeed, the value will be inferred as `json`.\n  - Otherwise, the value will be inferred as `str`.\n\n### Types of options in the UI\n\nThe type of an option in the UI is determined by the `btype`, `action` or `type` metadata. If neither is specified, a `PlainText` will be used.\n\n- `BoolOption`: Shown as a switch\n- `TextOption`: Shown as a textarea (allow multiple lines)\n- `ChoiceOption`: Shown as a dropdown list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `MChoiceOption`: Shown as a multiple choice list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `JsonOption`: Shown as a textarea, but the value will be validated and parsed as JSON\n- `ArrayOption`: Shown as a tag input. Items can be added or removed.\n- `AutoOption`: Shown as a 1-row textarea, and the value will be parsed automatically\n- `PlainText`: Shown as a plain text. No validation or parsing will be performed.\n- `MoreLikeOption`: Show as a box with buttons to add or remove sub-options. It\'s usally used together with `ns` type. If there is a sub-option under the option in the docstring wrapped by `<...>`, it indicates that we may have more sub-options.\n\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://github.com/pwwang/argx\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.7.0/PKG-INFO` & `pipen_board-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.7.0
+Version: 0.7.1
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

