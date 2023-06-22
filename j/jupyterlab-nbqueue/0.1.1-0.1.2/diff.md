# Comparing `tmp/jupyterlab_nbqueue-0.1.1.tar.gz` & `tmp/jupyterlab_nbqueue-0.1.2.tar.gz`

## Comparing `jupyterlab_nbqueue-0.1.1.tar` & `jupyterlab_nbqueue-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,154 @@
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/.jupyterlab-nbqueue.db
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/install.json
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/setup.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/yarn.lock
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyter-config/nb-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyter-config/server-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/_version.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/db_handler.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/handlers.py
--rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/build_log.json
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/package.json
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
--rw-r--r--   0        0        0    46224 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.dfa9e385d8336e1bc16c.js
--rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.dfa9e385d8336e1bc16c.js.map
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/lib_index_js.6a4e4d2a1cfd99ae049d.js
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/lib_index_js.6a4e4d2a1cfd99ae049d.js.map
--rw-r--r--   0        0        0    26908 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/remoteEntry.b9120c81f33bd5a84514.js.map
--rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/remoteEntry.f60060dfd6edb1319777.js
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/remoteEntry.f60060dfd6edb1319777.js.map
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/style.js
--rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
--rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
--rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
--rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
--rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
--rw-r--r--   0        0        0   332370 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/handler.ts
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/index.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/components/CustomProps.tsx
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/components/RunComponent.tsx
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/components/RunsContext.tsx
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/components/RunsPanelComponent.tsx
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/components/runs.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/src/widgets/RunsPanelWidget.tsx
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/index.js
--rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/css/all.css
--rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/css/fontawesome.css
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/css/solid.css
--rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/js/fontawesome.js
--rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/js/pro.js
--rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/js/solid.js
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/style/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/LICENSE
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/README.md
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.jupyterlab-nbqueue.db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/install.json
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/setup.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/yarn.lock
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyter-config/nb-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyter-config/server-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/_version.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/db_handler.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/handlers.py
+-rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/build_log.json
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/package.json
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
+-rw-r--r--   0        0        0    47311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js
+-rw-r--r--   0        0        0    18284 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js.map
+-rw-r--r--   0        0        0    48985 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.2724577231114db8dca3.js
+-rw-r--r--   0        0        0    19687 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.2724577231114db8dca3.js.map
+-rw-r--r--   0        0        0    52386 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.4e3c890a49308e4d5db4.js
+-rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.4e3c890a49308e4d5db4.js.map
+-rw-r--r--   0        0        0    63535 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.5d0ad4afe884aa708c22.js
+-rw-r--r--   0        0        0    34622 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.5d0ad4afe884aa708c22.js.map
+-rw-r--r--   0        0        0    63553 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.634752f692d503c6101d.js
+-rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.634752f692d503c6101d.js.map
+-rw-r--r--   0        0        0    63535 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.65bf61ee25313e3ee42f.js
+-rw-r--r--   0        0        0    34621 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.65bf61ee25313e3ee42f.js.map
+-rw-r--r--   0        0        0   144526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.73d3a3c0c8299a970d71.js
+-rw-r--r--   0        0        0   116947 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.73d3a3c0c8299a970d71.js.map
+-rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js
+-rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map
+-rw-r--r--   0        0        0    63552 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78e9c95f849f06d3b986.js
+-rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78e9c95f849f06d3b986.js.map
+-rw-r--r--   0        0        0    63553 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bc1f17109c578fd2c2b.js
+-rw-r--r--   0        0        0    34640 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bc1f17109c578fd2c2b.js.map
+-rw-r--r--   0        0        0    47311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bdfa0f8f502c09ba050.js
+-rw-r--r--   0        0        0    18284 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bdfa0f8f502c09ba050.js.map
+-rw-r--r--   0        0        0    63524 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7c8f2dc70352938a3d2d.js
+-rw-r--r--   0        0        0    34608 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7c8f2dc70352938a3d2d.js.map
+-rw-r--r--   0        0        0    47311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.8e15078a7af71e5c27f3.js
+-rw-r--r--   0        0        0    18284 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.8e15078a7af71e5c27f3.js.map
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9a521c3e0452d2c575dd.js
+-rw-r--r--   0        0        0    34621 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9a521c3e0452d2c575dd.js.map
+-rw-r--r--   0        0        0    81134 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9c42f23f2ca0899d925f.js
+-rw-r--r--   0        0        0    51953 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9c42f23f2ca0899d925f.js.map
+-rw-r--r--   0        0        0    63524 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9db362ed0cd5de83c4ff.js
+-rw-r--r--   0        0        0    34651 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9db362ed0cd5de83c4ff.js.map
+-rw-r--r--   0        0        0    64695 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.a39b226218658706a104.js
+-rw-r--r--   0        0        0    35753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.a39b226218658706a104.js.map
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.ab48e277a648e1eb9459.js
+-rw-r--r--   0        0        0    35748 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.ab48e277a648e1eb9459.js.map
+-rw-r--r--   0        0        0    48985 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.b3d7c6a5fa739a71ab91.js
+-rw-r--r--   0        0        0    19695 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.b3d7c6a5fa739a71ab91.js.map
+-rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.bc5073b762b2799baf2d.js
+-rw-r--r--   0        0        0    34640 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.bc5073b762b2799baf2d.js.map
+-rw-r--r--   0        0        0    52393 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c2bac3e77e187661465f.js
+-rw-r--r--   0        0        0    23450 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c2bac3e77e187661465f.js.map
+-rw-r--r--   0        0        0    52393 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c7ce8bed2c64290cde14.js
+-rw-r--r--   0        0        0    23451 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c7ce8bed2c64290cde14.js.map
+-rw-r--r--   0        0        0    64695 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.cfc5655624a4f827853b.js
+-rw-r--r--   0        0        0    35742 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.cfc5655624a4f827853b.js.map
+-rw-r--r--   0        0        0    63552 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d7142ae030373bc07d59.js
+-rw-r--r--   0        0        0    34622 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d7142ae030373bc07d59.js.map
+-rw-r--r--   0        0        0    52386 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d80038fa11375409ce91.js
+-rw-r--r--   0        0        0    23167 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d80038fa11375409ce91.js.map
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d99557b1553264e1f51e.js
+-rw-r--r--   0        0        0    34611 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d99557b1553264e1f51e.js.map
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.e8b3b45040a4af100b2e.js
+-rw-r--r--   0        0        0    35748 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.e8b3b45040a4af100b2e.js.map
+-rw-r--r--   0        0        0   144526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f95bd611aa60234e4f29.js
+-rw-r--r--   0        0        0   116944 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f95bd611aa60234e4f29.js.map
+-rw-r--r--   0        0        0   144526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f991ed7948b7bf891549.js
+-rw-r--r--   0        0        0   116947 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f991ed7948b7bf891549.js.map
+-rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.fffc8902b7b81746fe22.js
+-rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.fffc8902b7b81746fe22.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.0d4a29b3c23d232e97db.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.144efd145178595f0377.js.map
+-rw-r--r--   0        0        0    28507 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.158206971a084a36156d.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.1624be3501a9e12030d2.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.2018b34df243f9fedf3f.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.25cc9b1a1a145c3b88a8.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.2baa197656ade62a5cc3.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.376989fbb715f1b9ea1e.js.map
+-rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.386184b399a7a26bbfe6.js
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.386184b399a7a26bbfe6.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.447cbd569c4938bf49f7.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.48747736a93f4631050e.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.5763d893f0cb4a371ca9.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.59a24d8eaac1602b2340.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.5b252688f9affca54bc4.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.823dee75784ce4edca11.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.8a4ecaf13ffba72c4570.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.8d50aab740e9b8654c43.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.8f78e1adb6bc44518617.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.90eee843417add461073.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.9c5f21006540e759f069.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.a4c0e0994ff2f73ff5f3.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.b6ae8b0d850f3d51ba6e.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.b9ae4ec13d2cab6718c1.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.c662eec8eff500213ecb.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.ca79b65b71518690e478.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d673a697ae8e2330837f.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d7d9808378d65b484124.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d92c4a074743e9ae43ac.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d954f1ac91a58d251f88.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.e660b2dffe760079d5e8.js.map
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.ec91fff4ed20ba232f14.js.map
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style.js
+-rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
+-rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
+-rw-r--r--   0        0        0    19674 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js.07200853a72a491c7e0d.js
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js.07200853a72a491c7e0d.js.map
+-rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
+-rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
+-rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
+-rw-r--r--   0        0        0   332370 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
+-rw-r--r--   0        0        0  1500401 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.fa1f0281bb8cb7a915f1.js
+-rw-r--r--   0        0        0  1643592 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.fa1f0281bb8cb7a915f1.js.map
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/handler.ts
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/index.ts
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/svg.d.ts
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/CustomProps.tsx
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/RunComponent.tsx
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/RunsContext.tsx
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/RunsPanelComponent.tsx
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/runs.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/style/IconsStyle.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/widgets/RunsPanelWidget.tsx
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/index.js
+-rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/nbqueue_logo_v1.svg
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/nbqueue_logo_v2.svg
+-rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/css/all.css
+-rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/css/fontawesome.css
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/css/solid.css
+-rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/js/fontawesome.js
+-rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/js/pro.js
+-rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/js/solid.js
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/README.md
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/PKG-INFO
```

### Comparing `jupyterlab_nbqueue-0.1.1/.jupyterlab-nbqueue.db` & `jupyterlab_nbqueue-0.1.2/.jupyterlab-nbqueue.db`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/RELEASE.md` & `jupyterlab_nbqueue-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/package.json` & `jupyterlab_nbqueue-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -183,9 +183,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.1/tsconfig.json` & `jupyterlab_nbqueue-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/yarn.lock` & `jupyterlab_nbqueue-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/__init__.py` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/db_handler.py` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/db_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/handlers.py` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/build_log.json` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993110670194%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'jupyterlab-nbqueue': {'version': '0.1.1'}}}}}}"}*

```diff
@@ -588,15 +588,15 @@
                             "requiredVersion": "^1.33.0",
                             "singleton": true
                         },
                         "bootstrap": {},
                         "jupyterlab-nbqueue": {
                             "import": "/Users/luisgleon/Proyectos/Navteca/OpenScienceStudio/jupyterlab_nbqueue/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.0"
+                            "version": "0.1.1"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-bootstrap": {},
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/package.json` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.386184b399a7a26bbfe6.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -106,15 +106,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Navteca/jupyterlab-nbqueue.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f60060dfd6edb1319777.js",
+            "load": "static/remoteEntry.386184b399a7a26bbfe6.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_nbqueue"
                 },
@@ -188,9 +188,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.dfa9e385d8336e1bc16c.js` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.8e15078a7af71e5c27f3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -395,50 +395,49 @@
                 /* harmony import */
                 var _jupyterlab_filebrowser__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_filebrowser__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyterlab/apputils */ "webpack/sharing/consume/default/@jupyterlab/apputils");
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__);
                 /* harmony import */
-                var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
-                /* harmony import */
-                var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_2__);
+                var _style_IconsStyle__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! ./style/IconsStyle */ "./lib/style/IconsStyle.js");
                 /* harmony import */
                 var _handler__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! ./handler */ "./lib/handler.js");
                 /* harmony import */
-                var _widgets_RunsPanelWidget__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! ./widgets/RunsPanelWidget */ "./lib/widgets/RunsPanelWidget.js");
+                var _widgets_RunsPanelWidget__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! ./widgets/RunsPanelWidget */ "./lib/widgets/RunsPanelWidget.js");
 
 
+                // import { runIcon } from '@jupyterlab/ui-components';
 
 
 
                 /**
                  * Initialization data for the jupyterlab-nbqueue extension.
                  */
                 const plugin = {
                     id: 'jupyterlab-nbqueue:plugin',
                     description: 'A JupyterLab extension for queuing notebooks executions.',
                     autoStart: true,
                     requires: [_jupyterlab_filebrowser__WEBPACK_IMPORTED_MODULE_0__.IFileBrowserFactory],
                     activate: (app, factory) => {
-                        const runsContent = new _widgets_RunsPanelWidget__WEBPACK_IMPORTED_MODULE_3__.RunsPanelWidget();
+                        const runsContent = new _widgets_RunsPanelWidget__WEBPACK_IMPORTED_MODULE_2__.RunsPanelWidget();
                         runsContent.addClass('jp-PropertyInspector-placeholderContent');
                         const runsWidget = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.MainAreaWidget({
                             content: runsContent
                         });
                         runsWidget.toolbar.hide();
-                        runsWidget.title.icon = _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_2__.runIcon;
+                        runsWidget.title.icon = _style_IconsStyle__WEBPACK_IMPORTED_MODULE_3__.nbqueueIcon;
                         runsWidget.title.caption = 'Nbconvert runs';
                         app.shell.add(runsWidget, 'right', {
                             rank: 501
                         });
                         app.commands.addCommand('jupyterlab-nbqueue:open', {
                             label: 'Run',
                             caption: "Example context menu button for file browser's items.",
-                            icon: _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_2__.runIcon,
+                            icon: _style_IconsStyle__WEBPACK_IMPORTED_MODULE_3__.nbqueueIcon,
                             execute: () => {
                                 var _a;
                                 console.log('jupyterlab-nbqueue:open');
                                 const file = (_a = factory.tracker.currentWidget) === null || _a === void 0 ? void 0 : _a.selectedItems().next();
                                 console.log(JSON.parse(JSON.stringify(file)));
                                 const obj = JSON.parse(JSON.stringify(file));
                                 if (obj) {
@@ -473,14 +472,53 @@
                 const __WEBPACK_DEFAULT_EXPORT__ = (plugin);
 
 
                 /***/
             }),
 
         /***/
+        "./lib/style/IconsStyle.js":
+            /*!*********************************!*\
+              !*** ./lib/style/IconsStyle.js ***!
+              \*********************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony export */
+                __webpack_require__.d(__webpack_exports__, {
+                    /* harmony export */
+                    nbqueueIcon: () => ( /* binding */ nbqueueIcon)
+                    /* harmony export */
+                });
+                /* harmony import */
+                var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
+                /* harmony import */
+                var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__);
+                Object(function webpackMissingModule() {
+                    var e = new Error("Cannot find module '../../style/nbqueue_logo_v4.svg'");
+                    e.code = 'MODULE_NOT_FOUND';
+                    throw e;
+                }());
+
+
+                const nbqueueIcon = new _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__.LabIcon({
+                    name: 'nbqueue',
+                    svgstr: Object(function webpackMissingModule() {
+                        var e = new Error("Cannot find module '../../style/nbqueue_logo_v4.svg'");
+                        e.code = 'MODULE_NOT_FOUND';
+                        throw e;
+                    }())
+                });
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/widgets/RunsPanelWidget.js":
             /*!****************************************!*\
               !*** ./lib/widgets/RunsPanelWidget.js ***!
               \****************************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
@@ -774,8 +812,8 @@
                 module.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 8 8%27%3e%3cpath fill=%27%23198754%27 d=%27M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z%27/%3e%3c/svg%3e";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.dfa9e385d8336e1bc16c.js.map
+//# sourceMappingURL=lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.8e15078a7af71e5c27f3.js.map
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.dfa9e385d8336e1bc16c.js.map` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8201530612244898%*

 * *Differences: {"'file'": "'lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;;;AAA0C;AACE;AACJ;AACE;AACkB;AACd;AACH;AAGsB;AAM1D,MAAM,YAAY,GAAoB,CAAC,EAAE,GAAG,EAAE,EAAe,EAAE;IACpE,MAAM,EAAE,iBAAiB,EAAE,WAAW,EAAE,GAAG,iDAAU,CACnD,oDAAU,CACO,CAAC;IACpB,MAAM,iBAAiB,GAAG,KAAK,EAC7B,KAAoC,EACpC,EAAU,EACV,GAAW,EACX,EAAE;QACF,KAAK,CAAC,cAAc,EAAE,CAAC;QACvB,iBAAiB,CAAC,EAAE,EAAE,EAAE,GAAG,EAAE,CAAC,CAAC;QAC/B,WAAW,E […]*

```diff
@@ -1,23 +1,25 @@
 {
-    "file": "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.dfa9e385d8336e1bc16c.js",
-    "mappings": "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",
+    "file": "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-nbqueue/./src/components/RunComponent.tsx",
         "webpack://jupyterlab-nbqueue/./src/components/RunsContext.tsx",
         "webpack://jupyterlab-nbqueue/./src/components/RunsPanelComponent.tsx",
         "webpack://jupyterlab-nbqueue/./src/handler.ts",
         "webpack://jupyterlab-nbqueue/./src/index.ts",
+        "webpack://jupyterlab-nbqueue/./src/style/IconsStyle.ts",
         "webpack://jupyterlab-nbqueue/./src/widgets/RunsPanelWidget.tsx"
     ],
     "sourcesContent": [
         "import React, { useContext } from 'react';\nimport Button from 'react-bootstrap/Button';\nimport Card from 'react-bootstrap/Card';\nimport Stack from 'react-bootstrap/Stack';\nimport OverlayTrigger from 'react-bootstrap/OverlayTrigger';\nimport Tooltip from 'react-bootstrap/Tooltip';\nimport { RunContext } from './RunsContext';\nimport { RunContextType } from './runs';\nimport { IRun } from './CustomProps';\nimport '../../node_modules/bootstrap/dist/css/bootstrap.min.css';\n\ninterface Props {\n  run: IRun;\n}\n\nexport const RunComponent: React.FC<Props> = ({ run }): JSX.Element => {\n  const { deleteRunFromList, getRunsList } = useContext(\n    RunContext\n  ) as RunContextType;\n  const handleDeleteClick = async (\n    event: React.MouseEvent<HTMLElement>,\n    id: number,\n    pid: number\n  ) => {\n    event.preventDefault();\n    deleteRunFromList({ id, pid });\n    getRunsList();\n  };\n\n  const removeFromListTooltip = (\n    <Tooltip id=\"remove-from-list\">Remove from list</Tooltip>\n  );\n\n  return (\n    <div>\n      <Card className=\"m-2\">\n        <Card.Body>\n          <Stack gap={1} direction=\"horizontal\">\n            <Stack gap={1}>\n              <span>{run.name}</span>\n              <span>{run.status}</span>\n            </Stack>\n            <OverlayTrigger placement=\"bottom\" overlay={removeFromListTooltip}>\n              <Button\n                className=\"ms-auto\"\n                variant=\"link\"\n                size=\"sm\"\n                onClick={e => handleDeleteClick(e, run.id, run.pid)}\n                disabled={false}\n              >\n                <span\n                  className=\"fa fa-solid fa-xmark m-2\"\n                  aria-hidden=\"true\"\n                ></span>\n              </Button>\n            </OverlayTrigger>\n          </Stack>\n        </Card.Body>\n      </Card>\n    </div>\n  );\n};\n",
         "import React, { useEffect, useState } from 'react';\nimport { RunContextType } from './runs';\nimport { requestAPI } from '../handler';\nimport { IRunsProps, IRun, IDeleteRun } from './CustomProps';\n\ntype RunProviderProps = {\n  children: React.ReactNode;\n};\n\nexport const RunContext = React.createContext<RunContextType | null>(null);\n\nconst RunProvider: React.FC<RunProviderProps> = ({ children }) => {\n  const [runs, setRun] = useState<IRunsProps>([]);\n\n  useEffect(() => {\n    getRunsList();\n  }, []);\n\n  const runObject = async ({\n    id,\n    pid,\n    name,\n    status,\n    message\n  }: IRun): Promise<void> => {\n    try {\n      await requestAPI<any>('run', {\n        method: 'POST',\n        body: JSON.stringify({ id, pid, name, status, message })\n      });\n      getRunsList();\n    } catch (e) {\n      console.log(\n        `There has been an error trying to run an object => ${JSON.stringify(\n          e,\n          null,\n          2\n        )}`\n      );\n    }\n  };\n\n  const deleteRunFromList = async ({\n    id,\n    pid,\n    deleteAll = false\n  }: IDeleteRun): Promise<void> => {\n    try {\n      await requestAPI<any>('run', {\n        method: 'DELETE',\n        body: JSON.stringify({ deleteAll, id, pid })\n      });\n      getRunsList();\n    } catch (e) {\n      console.log(\n        `There has been an error trying to delete an object from the list of runs => ${e}`\n      );\n    }\n  };\n\n  const getRunsList = async (): Promise<void> => {\n    const response = await requestAPI<any>('run');\n    setRun(response.reverse());\n  };\n\n  return (\n    <RunContext.Provider\n      value={{\n        runs,\n        getRunsList,\n        runObject,\n        deleteRunFromList\n      }}\n    >\n      {children}\n    </RunContext.Provider>\n  );\n};\n\nexport default RunProvider;\n",
         "import React, { useEffect, useContext } from 'react';\nimport Stack from 'react-bootstrap/Stack';\nimport Button from 'react-bootstrap/Button';\nimport OverlayTrigger from 'react-bootstrap/OverlayTrigger';\nimport Tooltip from 'react-bootstrap/Tooltip';\nimport ButtonGroup from 'react-bootstrap/ButtonGroup';\nimport { RunComponent } from './RunComponent';\nimport { RunContext } from './RunsContext';\nimport { RunContextType } from './runs';\n\nexport const RunsPanelComponent: React.FC = (): JSX.Element => {\n  const { getRunsList, deleteRunFromList, runs } = useContext(\n    RunContext\n  ) as RunContextType;\n\n  useEffect(() => {\n    getRunsList();\n  }, []);\n\n  const handleDelete = (event: React.MouseEvent<HTMLElement>) => {\n    event.preventDefault();\n    deleteRunFromList({ deleteAll: true });\n    getRunsList();\n  };\n\n  const clearListTooltip = <Tooltip id=\"clear-list\">Clear all</Tooltip>;\n  const refreshTooltip = <Tooltip id=\"refresh\">Refresh</Tooltip>;\n\n  return (\n    <div\n      style={{\n        display: 'flex',\n        flexDirection: 'column',\n        height: '100%',\n        overflowY: 'auto'\n      }}\n    >\n      <Stack gap={2} direction=\"horizontal\">\n        <h4>Nbconvert history</h4>\n        <span style={{ flex: '1 1 auto' }}></span>\n        <ButtonGroup className=\"p-2\" aria-label=\"Runs Utilities\">\n          <OverlayTrigger placement=\"bottom\" overlay={clearListTooltip}>\n            <Button\n              variant=\"link\"\n              size=\"sm\"\n              onClick={e => handleDelete(e)}\n              disabled={!!(runs.length === 0)}\n            >\n              <i\n                className=\"fa fa-solid fa-trash-list m-2 fa-lg\"\n                aria-hidden=\"true\"\n              ></i>\n            </Button>\n          </OverlayTrigger>\n          <OverlayTrigger placement=\"bottom\" overlay={refreshTooltip}>\n            <Button variant=\"link\" size=\"sm\" onClick={getRunsList}>\n              <i\n                className=\"fa fa-solid fa-arrows-rotate m-2 fa-lg\"\n                aria-hidden=\"true\"\n              ></i>\n            </Button>\n          </OverlayTrigger>\n        </ButtonGroup>\n      </Stack>\n      <div>\n        {runs.map(run => {\n          return <RunComponent run={run} />;\n        })}\n      </div>\n    </div>\n  );\n};\n",
         "import { URLExt } from '@jupyterlab/coreutils';\n\nimport { ServerConnection } from '@jupyterlab/services';\n\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI<T>(\n  endPoint = '',\n  init: RequestInit = {}\n): Promise<T> {\n  // Make request to Jupyter API\n  const settings = ServerConnection.makeSettings();\n  const requestUrl = URLExt.join(\n    settings.baseUrl,\n    'jupyterlab-nbqueue', // API Namespace\n    endPoint\n  );\n\n  let response: Response;\n  try {\n    response = await ServerConnection.makeRequest(requestUrl, init, settings);\n  } catch (error) {\n    throw new ServerConnection.NetworkError(error as any);\n  }\n\n  let data: any = await response.text();\n\n  if (data.length > 0) {\n    try {\n      data = JSON.parse(data);\n    } catch (error) {\n      console.log('Not a JSON response body.', response);\n    }\n  }\n\n  if (!response.ok) {\n    throw new ServerConnection.ResponseError(response, data.message || data);\n  }\n\n  return data;\n}\n",
-        "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\nimport { showDialog, Dialog, MainAreaWidget } from '@jupyterlab/apputils';\nimport { runIcon } from '@jupyterlab/ui-components';\n\nimport { requestAPI } from './handler';\n\nimport { RunsPanelWidget } from './widgets/RunsPanelWidget';\n/**\n * Initialization data for the jupyterlab-nbqueue extension.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: 'jupyterlab-nbqueue:plugin',\n  description: 'A JupyterLab extension for queuing notebooks executions.',\n  autoStart: true,\n  requires: [IFileBrowserFactory],\n  activate: (app: JupyterFrontEnd, factory: IFileBrowserFactory) => {\n    const runsContent = new RunsPanelWidget();\n    runsContent.addClass('jp-PropertyInspector-placeholderContent');\n    const runsWidget = new MainAreaWidget<RunsPanelWidget>({\n      content: runsContent\n    });\n    runsWidget.toolbar.hide();\n    runsWidget.title.icon = runIcon;\n    runsWidget.title.caption = 'Nbconvert runs';\n    app.shell.add(runsWidget, 'right', { rank: 501 });\n\n    app.commands.addCommand('jupyterlab-nbqueue:open', {\n      label: 'Run',\n      caption: \"Example context menu button for file browser's items.\",\n      icon: runIcon,\n      execute: () => {\n        console.log('jupyterlab-nbqueue:open');\n        const file = factory.tracker.currentWidget?.selectedItems().next();\n\n        console.log(JSON.parse(JSON.stringify(file)));\n        const obj = JSON.parse(JSON.stringify(file));\n\n        if (obj) {\n          showDialog({\n            title: obj.name,\n            body: `Notebook ${obj.name} running in background.`,\n            buttons: [Dialog.okButton()]\n          }).catch(e => console.log(e));\n        }\n\n        requestAPI<any>('run', {\n          method: 'POST',\n          body: JSON.stringify({ notebook: obj.path })\n        })\n          .then(data => {\n            console.log(data);\n          })\n          .catch(reason => {\n            console.error(\n              `The jupyterlab-nbqueue server extension appears to be missing.\\n${reason}`\n            );\n          });\n      }\n    });\n\n    app.contextMenu.addItem({\n      command: 'jupyterlab-nbqueue:open',\n      selector: '.jp-DirListing-item[data-isdir=\"false\"]',\n      rank: 0\n    });\n  }\n};\nexport default plugin;\n",
+        "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\nimport { showDialog, Dialog, MainAreaWidget } from '@jupyterlab/apputils';\n// import { runIcon } from '@jupyterlab/ui-components';\nimport { nbqueueIcon } from './style/IconsStyle';\n\nimport { requestAPI } from './handler';\n\nimport { RunsPanelWidget } from './widgets/RunsPanelWidget';\n/**\n * Initialization data for the jupyterlab-nbqueue extension.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: 'jupyterlab-nbqueue:plugin',\n  description: 'A JupyterLab extension for queuing notebooks executions.',\n  autoStart: true,\n  requires: [IFileBrowserFactory],\n  activate: (app: JupyterFrontEnd, factory: IFileBrowserFactory) => {\n    const runsContent = new RunsPanelWidget();\n    runsContent.addClass('jp-PropertyInspector-placeholderContent');\n    const runsWidget = new MainAreaWidget<RunsPanelWidget>({\n      content: runsContent\n    });\n    runsWidget.toolbar.hide();\n    runsWidget.title.icon = nbqueueIcon;\n    runsWidget.title.caption = 'Nbconvert runs';\n    app.shell.add(runsWidget, 'right', { rank: 501 });\n\n    app.commands.addCommand('jupyterlab-nbqueue:open', {\n      label: 'Run',\n      caption: \"Example context menu button for file browser's items.\",\n      icon: nbqueueIcon,\n      execute: () => {\n        console.log('jupyterlab-nbqueue:open');\n        const file = factory.tracker.currentWidget?.selectedItems().next();\n\n        console.log(JSON.parse(JSON.stringify(file)));\n        const obj = JSON.parse(JSON.stringify(file));\n\n        if (obj) {\n          showDialog({\n            title: obj.name,\n            body: `Notebook ${obj.name} running in background.`,\n            buttons: [Dialog.okButton()]\n          }).catch(e => console.log(e));\n        }\n\n        requestAPI<any>('run', {\n          method: 'POST',\n          body: JSON.stringify({ notebook: obj.path })\n        })\n          .then(data => {\n            console.log(data);\n          })\n          .catch(reason => {\n            console.error(\n              `The jupyterlab-nbqueue server extension appears to be missing.\\n${reason}`\n            );\n          });\n      }\n    });\n\n    app.contextMenu.addItem({\n      command: 'jupyterlab-nbqueue:open',\n      selector: '.jp-DirListing-item[data-isdir=\"false\"]',\n      rank: 0\n    });\n  }\n};\nexport default plugin;\n",
+        "import { LabIcon } from '@jupyterlab/ui-components';\n\nimport nbqueueSVG from '../../style/nbqueue_logo_v2.svg';\n\nexport const nbqueueIcon = new LabIcon({ name: 'nbqueue', svgstr: nbqueueSVG });\n",
         "import React from 'react';\nimport { ReactWidget } from '@jupyterlab/apputils';\nimport { RunsPanelComponent } from '../components/RunsPanelComponent';\nimport RunProvider from '../components/RunsContext';\n\nexport class RunsPanelWidget extends ReactWidget {\n  constructor() {\n    super();\n  }\n\n  render(): JSX.Element {\n    return (\n      <div\n        style={{\n          minWidth: '400px',\n          display: 'flex',\n          flexDirection: 'column',\n          background: 'var(--jp-layout-color1)'\n        }}\n      >\n        <RunProvider>\n          <RunsPanelComponent />\n        </RunProvider>\n      </div>\n    );\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/remoteEntry.b9120c81f33bd5a84514.js.map` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.158206971a084a36156d.js.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8311688311688312%*

 * *Differences: {"'file'": "'remoteEntry.158206971a084a36156d.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.b9120c81f33bd5a84514.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,kSAAkS;WAChU;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC5KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.158206971a084a36156d.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,oSAAoS;WAClU;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-nbqueue/webpack/container-entry",
         "webpack://jupyterlab-nbqueue/webpack/bootstrap",
         "webpack://jupyterlab-nbqueue/webpack/runtime/compat get default export",
         "webpack://jupyterlab-nbqueue/webpack/runtime/define property getters",
@@ -20,27 +20,27 @@
         "webpack://jupyterlab-nbqueue/webpack/runtime/jsonp chunk loading",
         "webpack://jupyterlab-nbqueue/webpack/runtime/nonce",
         "webpack://jupyterlab-nbqueue/webpack/before-startup",
         "webpack://jupyterlab-nbqueue/webpack/startup",
         "webpack://jupyterlab-nbqueue/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"6a4e4d2a1cfd99ae049d\",\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\":\"103775b5d2edfd3cd852\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\":\"3970d5aff54335b54c0d\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\":\"fa1f0281bb8cb7a915f1\",\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\":\"78207085ee8bf5d10cb1\",\"style_index_js\":\"07200853a72a491c7e0d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-nbqueue:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-nbqueue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-nbqueue\", \"0.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-nbqueue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-nbqueue\", \"0.1.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,3])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,5,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-dom\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-nbqueue\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_nbqueue\"] = self[\"webpackChunkjupyterlab_nbqueue\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-nbqueue\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/remoteEntry.f60060dfd6edb1319777.js` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.386184b399a7a26bbfe6.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -184,15 +184,15 @@
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
                 "vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b": "103775b5d2edfd3cd852",
                 "vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093": "766984a3c69834ca0c09",
-                "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61": "dfa9e385d8336e1bc16c",
+                "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61": "78207085ee8bf5d10cb1",
                 "style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1": "3970d5aff54335b54c0d"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -429,15 +429,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-nbqueue", "0.1.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b"), __webpack_require__.e("vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093"), __webpack_require__.e("lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-nbqueue", "0.1.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b"), __webpack_require__.e("vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093"), __webpack_require__.e("lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -834,44 +834,44 @@
         /******/
         var moduleToHandlerMapping = {
             /******/
             "webpack/sharing/consume/default/@jupyterlab/filebrowser": () => (loadSingletonVersionCheck("default", "@jupyterlab/filebrowser", [1, 3, 5, 3])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 5, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 5, 3])),
-            /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 5, 3])),
             /******/
             "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 5, 3])),
             /******/
-            "webpack/sharing/consume/default/react-dom": () => (loadSingletonVersionCheck("default", "react-dom", [1, 17, 0, 1]))
+            "webpack/sharing/consume/default/react-dom": () => (loadSingletonVersionCheck("default", "react-dom", [1, 17, 0, 1])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 5, 3]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61": [
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/filebrowser",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/apputils",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/ui-components",
-                /******/
                 "webpack/sharing/consume/default/react",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/coreutils",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/services",
                 /******/
-                "webpack/sharing/consume/default/react-dom"
+                "webpack/sharing/consume/default/react-dom",
+                /******/
+                "webpack/sharing/consume/default/@jupyterlab/ui-components"
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -1099,8 +1099,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-nbqueue");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-nbqueue"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.f60060dfd6edb1319777.js.map
+//# sourceMappingURL=remoteEntry.386184b399a7a26bbfe6.js.map
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/remoteEntry.f60060dfd6edb1319777.js.map` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.48747736a93f4631050e.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9081632653061226%*

 * *Differences: {"'file'": "'remoteEntry.48747736a93f4631050e.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b":"103775b5d2edfd3cd852","vendors-node_modules_react-bootstrap_esm_Button_j […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.f60060dfd6edb1319777.js",
+    "file": "remoteEntry.48747736a93f4631050e.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,wfAAwf;WACthB;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-nbqueue/webpack/container-entry",
         "webpack://jupyterlab-nbqueue/webpack/bootstrap",
         "webpack://jupyterlab-nbqueue/webpack/runtime/compat get default export",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\":\"103775b5d2edfd3cd852\",\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\":\"766984a3c69834ca0c09\",\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\":\"dfa9e385d8336e1bc16c\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\":\"3970d5aff54335b54c0d\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\":\"103775b5d2edfd3cd852\",\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\":\"766984a3c69834ca0c09\",\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\":\"2724577231114db8dca3\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\":\"3970d5aff54335b54c0d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-nbqueue:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-nbqueue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-nbqueue\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-nbqueue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-nbqueue\", \"0.1.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,3])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-dom\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,3])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,5,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-dom\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-nbqueue\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_nbqueue\"] = self[\"webpackChunkjupyterlab_nbqueue\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-nbqueue\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map` & `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/src/handler.ts` & `jupyterlab_nbqueue-0.1.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/src/index.ts` & `jupyterlab_nbqueue-0.1.2/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 import { showDialog, Dialog, MainAreaWidget } from '@jupyterlab/apputils';
-import { runIcon } from '@jupyterlab/ui-components';
+// import { runIcon } from '@jupyterlab/ui-components';
+import { nbqueueIcon } from './style/IconsStyle';
 
 import { requestAPI } from './handler';
 
 import { RunsPanelWidget } from './widgets/RunsPanelWidget';
 /**
  * Initialization data for the jupyterlab-nbqueue extension.
  */
@@ -20,22 +21,22 @@
   activate: (app: JupyterFrontEnd, factory: IFileBrowserFactory) => {
     const runsContent = new RunsPanelWidget();
     runsContent.addClass('jp-PropertyInspector-placeholderContent');
     const runsWidget = new MainAreaWidget<RunsPanelWidget>({
       content: runsContent
     });
     runsWidget.toolbar.hide();
-    runsWidget.title.icon = runIcon;
+    runsWidget.title.icon = nbqueueIcon;
     runsWidget.title.caption = 'Nbconvert runs';
     app.shell.add(runsWidget, 'right', { rank: 501 });
 
     app.commands.addCommand('jupyterlab-nbqueue:open', {
       label: 'Run',
       caption: "Example context menu button for file browser's items.",
-      icon: runIcon,
+      icon: nbqueueIcon,
       execute: () => {
         console.log('jupyterlab-nbqueue:open');
         const file = factory.tracker.currentWidget?.selectedItems().next();
 
         console.log(JSON.parse(JSON.stringify(file)));
         const obj = JSON.parse(JSON.stringify(file));
```

### Comparing `jupyterlab_nbqueue-0.1.1/src/components/RunComponent.tsx` & `jupyterlab_nbqueue-0.1.2/src/components/RunComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/src/components/RunsContext.tsx` & `jupyterlab_nbqueue-0.1.2/src/components/RunsContext.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/src/components/RunsPanelComponent.tsx` & `jupyterlab_nbqueue-0.1.2/src/components/RunsPanelComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/src/widgets/RunsPanelWidget.tsx` & `jupyterlab_nbqueue-0.1.2/src/widgets/RunsPanelWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/css/all.css` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/css/fontawesome.css` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/css/solid.css` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/js/fontawesome.js` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/js/pro.js` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/js/pro.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/js/solid.js` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/webfonts/fa-solid-900.ttf` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/webfonts/fa-solid-900.woff` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/style/fontawesome/webfonts/fa-solid-900.woff2` & `jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/.gitignore` & `jupyterlab_nbqueue-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/LICENSE` & `jupyterlab_nbqueue-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/README.md` & `jupyterlab_nbqueue-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.1/pyproject.toml` & `jupyterlab_nbqueue-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=2.0.1,<3"
+    "jupyter_server>=2.0.1,<3",
+    "sqlalchemy>=2.0.16,<3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
```

### Comparing `jupyterlab_nbqueue-0.1.1/PKG-INFO` & `jupyterlab_nbqueue-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbqueue
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab extension for queuing notebooks executions.
 Project-URL: Homepage, https://github.com/Navteca/jupyterlab-nbqueue.git
 Project-URL: Bug Tracker, https://github.com/Navteca/jupyterlab-nbqueue.git/issues
 Project-URL: Repository, https://github.com/Navteca/jupyterlab-nbqueue.git.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
         
@@ -46,14 +46,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server<3,>=2.0.1
+Requires-Dist: sqlalchemy<3,>=2.0.16
 Description-Content-Type: text/markdown
 
 # jupyterlab_nbqueue
 
 [![Github Actions Status](https://github.com/Navteca/jupyterlab-nbqueue.git/workflows/Build/badge.svg)](https://github.com/Navteca/jupyterlab-nbqueue.git/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Navteca/jupyterlab-nbqueue.git/main?urlpath=lab)
 A JupyterLab extension for queuing notebooks executions.
```

