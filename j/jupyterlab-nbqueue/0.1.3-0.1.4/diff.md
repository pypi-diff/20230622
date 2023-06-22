# Comparing `tmp/jupyterlab_nbqueue-0.1.3.tar.gz` & `tmp/jupyterlab_nbqueue-0.1.4.tar.gz`

## Comparing `jupyterlab_nbqueue-0.1.3.tar` & `jupyterlab_nbqueue-0.1.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.jupyterlab-nbqueue.db
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/RELEASE.md
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/RunningCode.ipynb
--rw-r--r--   0        0        0    54279 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/RunningCode.nbconvert.ipynb
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/install.json
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/setup.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/test04.ipynb
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/test04.nbconvert.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/tsconfig.json
--rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/yarn.lock
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyter-config/nb-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyter-config/server-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/_version.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/cmd_launcher.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/db_handler.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/handlers.py
--rw-r--r--   0        0        0    22111 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/build_log.json
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/package.json
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
--rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js
--rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map
--rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js.map
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style.js
--rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
--rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
--rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
--rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
--rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
--rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/handler.ts
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/index.ts
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/svg.d.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/CustomProps.tsx
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/RunComponent.tsx
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/RunsContext.tsx
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/RunsPanelComponent.tsx
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/runs.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/style/IconsStyle.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/widgets/RunsPanelWidget.tsx
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/base.css
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/index.js
--rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v1.svg
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v2.svg
--rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/css/all.css
--rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/css/fontawesome.css
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/css/solid.css
--rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/js/fontawesome.js
--rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/js/pro.js
--rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/js/solid.js
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/LICENSE
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/README.md
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/.jupyterlab-nbqueue.db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/RELEASE.md
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/RunningCode.ipynb
+-rw-r--r--   0        0        0    54279 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/RunningCode.nbconvert.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/install.json
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/setup.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/test04.ipynb
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/test04.nbconvert.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/tsconfig.json
+-rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/yarn.lock
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyter-config/nb-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyter-config/server-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/_version.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/cmd_launcher.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/db_handler.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/handlers.py
+-rw-r--r--   0        0        0    22111 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/build_log.json
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/package.json
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
+-rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js
+-rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map
+-rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js.map
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/style.js
+-rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
+-rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
+-rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
+-rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
+-rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
+-rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/handler.ts
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/index.ts
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/svg.d.ts
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/components/CustomProps.tsx
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/components/RunComponent.tsx
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/components/RunsContext.tsx
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/components/RunsPanelComponent.tsx
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/components/runs.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/style/IconsStyle.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/src/widgets/RunsPanelWidget.tsx
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/base.css
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/index.js
+-rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/nbqueue_logo_v1.svg
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/nbqueue_logo_v2.svg
+-rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/css/all.css
+-rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/css/fontawesome.css
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/css/solid.css
+-rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/js/fontawesome.js
+-rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/js/pro.js
+-rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/js/solid.js
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/style/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/README.md
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.4/PKG-INFO
```

### Comparing `jupyterlab_nbqueue-0.1.3/.jupyterlab-nbqueue.db` & `jupyterlab_nbqueue-0.1.4/.jupyterlab-nbqueue.db`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/RELEASE.md` & `jupyterlab_nbqueue-0.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/RunningCode.ipynb` & `jupyterlab_nbqueue-0.1.4/RunningCode.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/RunningCode.nbconvert.ipynb` & `jupyterlab_nbqueue-0.1.4/RunningCode.nbconvert.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/package.json` & `jupyterlab_nbqueue-0.1.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -183,9 +183,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.3/test04.ipynb` & `jupyterlab_nbqueue-0.1.4/test04.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/test04.nbconvert.ipynb` & `jupyterlab_nbqueue-0.1.4/test04.nbconvert.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/tsconfig.json` & `jupyterlab_nbqueue-0.1.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/yarn.lock` & `jupyterlab_nbqueue-0.1.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/__init__.py` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/cmd_launcher.py` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/cmd_launcher.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/db_handler.py` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/db_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/handlers.py` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/build_log.json` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/package.json` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js.map` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map` & `jupyterlab_nbqueue-0.1.4/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/src/handler.ts` & `jupyterlab_nbqueue-0.1.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/src/index.ts` & `jupyterlab_nbqueue-0.1.4/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     const runsContent = new RunsPanelWidget();
     runsContent.addClass('jp-PropertyInspector-placeholderContent');
     const runsWidget = new MainAreaWidget<RunsPanelWidget>({
       content: runsContent
     });
     runsWidget.toolbar.hide();
     runsWidget.title.icon = nbqueueIcon;
-    runsWidget.title.caption = 'Nbconvert runs';
+    runsWidget.title.caption = 'NBQueue history';
     app.shell.add(runsWidget, 'right', { rank: 501 });
 
     app.commands.addCommand('jupyterlab-nbqueue:open', {
       label: 'Run',
       caption: "Example context menu button for file browser's items.",
       icon: nbqueueIcon,
       execute: () => {
```

### Comparing `jupyterlab_nbqueue-0.1.3/src/components/RunComponent.tsx` & `jupyterlab_nbqueue-0.1.4/src/components/RunComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/src/components/RunsContext.tsx` & `jupyterlab_nbqueue-0.1.4/src/components/RunsContext.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/src/components/RunsPanelComponent.tsx` & `jupyterlab_nbqueue-0.1.4/src/components/RunsPanelComponent.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         display: 'flex',
         flexDirection: 'column',
         height: '100%',
         overflowY: 'auto'
       }}
     >
       <Stack gap={2} direction="horizontal">
-        <h4>Nbconvert history</h4>
+        <h4>NBQueue history</h4>
         <span style={{ flex: '1 1 auto' }}></span>
         <ButtonGroup className="p-2" aria-label="Runs Utilities">
           <OverlayTrigger placement="bottom" overlay={clearListTooltip}>
             <Button
               variant="link"
               size="sm"
               onClick={e => handleDelete(e)}
```

### Comparing `jupyterlab_nbqueue-0.1.3/src/widgets/RunsPanelWidget.tsx` & `jupyterlab_nbqueue-0.1.4/src/widgets/RunsPanelWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v1.svg` & `jupyterlab_nbqueue-0.1.4/style/nbqueue_logo_v1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v2.svg` & `jupyterlab_nbqueue-0.1.4/style/nbqueue_logo_v2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/css/all.css` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/css/fontawesome.css` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/css/solid.css` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/js/fontawesome.js` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/js/pro.js` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/js/pro.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/js/solid.js` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.ttf` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff2` & `jupyterlab_nbqueue-0.1.4/style/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/.gitignore` & `jupyterlab_nbqueue-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/LICENSE` & `jupyterlab_nbqueue-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/README.md` & `jupyterlab_nbqueue-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/pyproject.toml` & `jupyterlab_nbqueue-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.3/PKG-INFO` & `jupyterlab_nbqueue-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbqueue
-Version: 0.1.3
+Version: 0.1.4
 Summary: A JupyterLab extension for queuing notebooks executions.
 Project-URL: Homepage, https://github.com/Navteca/jupyterlab-nbqueue.git
 Project-URL: Bug Tracker, https://github.com/Navteca/jupyterlab-nbqueue.git/issues
 Project-URL: Repository, https://github.com/Navteca/jupyterlab-nbqueue.git.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
```

