# Comparing `tmp/jupyterlab_nbqueue-0.1.2.tar.gz` & `tmp/jupyterlab_nbqueue-0.1.3.tar.gz`

## Comparing `jupyterlab_nbqueue-0.1.2.tar` & `jupyterlab_nbqueue-0.1.3.tar`

### file list

```diff
@@ -1,154 +1,67 @@
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.jupyterlab-nbqueue.db
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/install.json
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/setup.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/tsconfig.json
--rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/yarn.lock
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyter-config/nb-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyter-config/server-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/_version.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/db_handler.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/handlers.py
--rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/build_log.json
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/package.json
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
--rw-r--r--   0        0        0    47311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js
--rw-r--r--   0        0        0    18284 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.0af14a6a3dd4c7d7d0d9.js.map
--rw-r--r--   0        0        0    48985 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.2724577231114db8dca3.js
--rw-r--r--   0        0        0    19687 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.2724577231114db8dca3.js.map
--rw-r--r--   0        0        0    52386 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.4e3c890a49308e4d5db4.js
--rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.4e3c890a49308e4d5db4.js.map
--rw-r--r--   0        0        0    63535 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.5d0ad4afe884aa708c22.js
--rw-r--r--   0        0        0    34622 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.5d0ad4afe884aa708c22.js.map
--rw-r--r--   0        0        0    63553 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.634752f692d503c6101d.js
--rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.634752f692d503c6101d.js.map
--rw-r--r--   0        0        0    63535 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.65bf61ee25313e3ee42f.js
--rw-r--r--   0        0        0    34621 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.65bf61ee25313e3ee42f.js.map
--rw-r--r--   0        0        0   144526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.73d3a3c0c8299a970d71.js
--rw-r--r--   0        0        0   116947 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.73d3a3c0c8299a970d71.js.map
--rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js
--rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map
--rw-r--r--   0        0        0    63552 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78e9c95f849f06d3b986.js
--rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78e9c95f849f06d3b986.js.map
--rw-r--r--   0        0        0    63553 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bc1f17109c578fd2c2b.js
--rw-r--r--   0        0        0    34640 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bc1f17109c578fd2c2b.js.map
--rw-r--r--   0        0        0    47311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bdfa0f8f502c09ba050.js
--rw-r--r--   0        0        0    18284 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7bdfa0f8f502c09ba050.js.map
--rw-r--r--   0        0        0    63524 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7c8f2dc70352938a3d2d.js
--rw-r--r--   0        0        0    34608 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.7c8f2dc70352938a3d2d.js.map
--rw-r--r--   0        0        0    47311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.8e15078a7af71e5c27f3.js
--rw-r--r--   0        0        0    18284 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.8e15078a7af71e5c27f3.js.map
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9a521c3e0452d2c575dd.js
--rw-r--r--   0        0        0    34621 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9a521c3e0452d2c575dd.js.map
--rw-r--r--   0        0        0    81134 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9c42f23f2ca0899d925f.js
--rw-r--r--   0        0        0    51953 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9c42f23f2ca0899d925f.js.map
--rw-r--r--   0        0        0    63524 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9db362ed0cd5de83c4ff.js
--rw-r--r--   0        0        0    34651 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.9db362ed0cd5de83c4ff.js.map
--rw-r--r--   0        0        0    64695 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.a39b226218658706a104.js
--rw-r--r--   0        0        0    35753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.a39b226218658706a104.js.map
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.ab48e277a648e1eb9459.js
--rw-r--r--   0        0        0    35748 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.ab48e277a648e1eb9459.js.map
--rw-r--r--   0        0        0    48985 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.b3d7c6a5fa739a71ab91.js
--rw-r--r--   0        0        0    19695 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.b3d7c6a5fa739a71ab91.js.map
--rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.bc5073b762b2799baf2d.js
--rw-r--r--   0        0        0    34640 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.bc5073b762b2799baf2d.js.map
--rw-r--r--   0        0        0    52393 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c2bac3e77e187661465f.js
--rw-r--r--   0        0        0    23450 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c2bac3e77e187661465f.js.map
--rw-r--r--   0        0        0    52393 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c7ce8bed2c64290cde14.js
--rw-r--r--   0        0        0    23451 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.c7ce8bed2c64290cde14.js.map
--rw-r--r--   0        0        0    64695 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.cfc5655624a4f827853b.js
--rw-r--r--   0        0        0    35742 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.cfc5655624a4f827853b.js.map
--rw-r--r--   0        0        0    63552 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d7142ae030373bc07d59.js
--rw-r--r--   0        0        0    34622 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d7142ae030373bc07d59.js.map
--rw-r--r--   0        0        0    52386 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d80038fa11375409ce91.js
--rw-r--r--   0        0        0    23167 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d80038fa11375409ce91.js.map
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d99557b1553264e1f51e.js
--rw-r--r--   0        0        0    34611 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.d99557b1553264e1f51e.js.map
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.e8b3b45040a4af100b2e.js
--rw-r--r--   0        0        0    35748 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.e8b3b45040a4af100b2e.js.map
--rw-r--r--   0        0        0   144526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f95bd611aa60234e4f29.js
--rw-r--r--   0        0        0   116944 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f95bd611aa60234e4f29.js.map
--rw-r--r--   0        0        0   144526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f991ed7948b7bf891549.js
--rw-r--r--   0        0        0   116947 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.f991ed7948b7bf891549.js.map
--rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.fffc8902b7b81746fe22.js
--rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.fffc8902b7b81746fe22.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.0d4a29b3c23d232e97db.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.144efd145178595f0377.js.map
--rw-r--r--   0        0        0    28507 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.158206971a084a36156d.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.1624be3501a9e12030d2.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.2018b34df243f9fedf3f.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.25cc9b1a1a145c3b88a8.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.2baa197656ade62a5cc3.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.376989fbb715f1b9ea1e.js.map
--rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.386184b399a7a26bbfe6.js
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.386184b399a7a26bbfe6.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.447cbd569c4938bf49f7.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.48747736a93f4631050e.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.5763d893f0cb4a371ca9.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.59a24d8eaac1602b2340.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.5b252688f9affca54bc4.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.823dee75784ce4edca11.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.8a4ecaf13ffba72c4570.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.8d50aab740e9b8654c43.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.8f78e1adb6bc44518617.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.90eee843417add461073.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.9c5f21006540e759f069.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.a4c0e0994ff2f73ff5f3.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.b6ae8b0d850f3d51ba6e.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.b9ae4ec13d2cab6718c1.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.c662eec8eff500213ecb.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.ca79b65b71518690e478.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d673a697ae8e2330837f.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d7d9808378d65b484124.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d92c4a074743e9ae43ac.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.d954f1ac91a58d251f88.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.e660b2dffe760079d5e8.js.map
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.ec91fff4ed20ba232f14.js.map
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style.js
--rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
--rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
--rw-r--r--   0        0        0    19674 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js.07200853a72a491c7e0d.js
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js.07200853a72a491c7e0d.js.map
--rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
--rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
--rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
--rw-r--r--   0        0        0   332370 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
--rw-r--r--   0        0        0  1500401 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.fa1f0281bb8cb7a915f1.js
--rw-r--r--   0        0        0  1643592 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.fa1f0281bb8cb7a915f1.js.map
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/handler.ts
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/index.ts
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/svg.d.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/CustomProps.tsx
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/RunComponent.tsx
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/RunsContext.tsx
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/RunsPanelComponent.tsx
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/components/runs.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/style/IconsStyle.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/src/widgets/RunsPanelWidget.tsx
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/index.js
--rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/nbqueue_logo_v1.svg
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/nbqueue_logo_v2.svg
--rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/css/all.css
--rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/css/fontawesome.css
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/css/solid.css
--rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/js/fontawesome.js
--rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/js/pro.js
--rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/js/solid.js
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/LICENSE
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/README.md
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.jupyterlab-nbqueue.db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/RunningCode.ipynb
+-rw-r--r--   0        0        0    54279 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/RunningCode.nbconvert.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/install.json
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/setup.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/test04.ipynb
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/test04.nbconvert.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/yarn.lock
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyter-config/nb-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyter-config/server-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/_version.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/cmd_launcher.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/db_handler.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/handlers.py
+-rw-r--r--   0        0        0    22111 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/build_log.json
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/package.json
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
+-rw-r--r--   0        0        0    63567 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js
+-rw-r--r--   0        0        0    34654 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map
+-rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js.map
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style.js
+-rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
+-rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
+-rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
+-rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
+-rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
+-rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/handler.ts
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/index.ts
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/svg.d.ts
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/CustomProps.tsx
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/RunComponent.tsx
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/RunsContext.tsx
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/RunsPanelComponent.tsx
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/components/runs.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/style/IconsStyle.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/src/widgets/RunsPanelWidget.tsx
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/base.css
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/index.js
+-rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v1.svg
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v2.svg
+-rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/css/all.css
+-rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/css/fontawesome.css
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/css/solid.css
+-rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/js/fontawesome.js
+-rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/js/pro.js
+-rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/js/solid.js
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/README.md
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.3/PKG-INFO
```

### Comparing `jupyterlab_nbqueue-0.1.2/RELEASE.md` & `jupyterlab_nbqueue-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/package.json` & `jupyterlab_nbqueue-0.1.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9786931818181818%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^4.0.2'}", "'version'": "'0.1.3'"}*

```diff
@@ -15,15 +15,15 @@
         "@jupyterlab/ui-components": "^4.0.2",
         "bootstrap": "^5.3.0",
         "react-bootstrap": "^2.7.4",
         "react-bootstrap-typeahead": "^6.2.3"
     },
     "description": "A JupyterLab extension for queuing notebooks executions.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.5.3",
+        "@jupyterlab/builder": "^4.0.2",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
@@ -183,9 +183,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.2/tsconfig.json` & `jupyterlab_nbqueue-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/yarn.lock` & `jupyterlab_nbqueue-0.1.3/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1697,17 +1697,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.436"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.436.tgz#2aa6e1644693d25cb438a873fba72ec901e1be30"
-  integrity sha512-aktOxo8fnrMC8vOIBMVS3PXbT1nrPQ+SouUuN7Y0a+Rw3pOMrvIV92Ybnax7x4tugA+ZpYA5fOHTby7ama8OQQ==
+  version "1.4.437"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.437.tgz#d0e73a431a9ade4467f73d48a59d752d91909316"
+  integrity sha512-ZFekRuBOHUXp21wrR5lshT6pZa/KmjkhKBAtmZz4NN5sCWlHOk3kdhiwFINrDBsRLX6FjyBAb1TRN+KBeNlyzQ==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/__init__.py` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/db_handler.py` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/db_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/handlers.py` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/handlers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import tornado
 import shlex
 import sqlalchemy
 import subprocess
+import importlib.resources as pkg_resources
 
+from shutil import which
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.utils import url_path_join
 
 from .db_handler import DBHandler, Runs
 
 class RouteHandler(APIHandler):
     db = DBHandler()
@@ -32,53 +34,34 @@
 
     @tornado.web.authenticated
     def post(self):
         try:
             request_data = self.get_json_body()
             notebook = request_data.get('notebook', None)                
             if notebook:
-                cmd_split = shlex.split(f'jupyter nbconvert --to notebook --execute ./{notebook}')
-                process = subprocess.Popen(cmd_split, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-                success = True
+                with pkg_resources.path('jupyterlab_nbqueue', 'cmd_launcher.py') as p:
+                    cmd_split = shlex.split(f"{which('python')} {p} {notebook}")
+                    subprocess.Popen(cmd_split, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            else:
+                self.log.error("The required data has not been received. Please send notebook.")
+                message = "The required data has not been received. Please send notebook."
         except subprocess.CalledProcessError as exc:
             self.log.error(f"Program failed {exc.returncode} - {exc}")
             message = f"Program failed {exc.returncode} - {exc}"
         except subprocess.TimeoutExpired as exc:
             self.log.error(f"Program timed out {exc}")
             message = f"Program timed out {exc}"
         except Exception as exc:
             self.log.error(f"Exception {exc}")
             message = f"Exception {exc}"
         else:
-            success = True
-        finally:
-            with self.db.get_session() as session:
-                if process:
-                    new_process = Runs(pid=process.pid, name=notebook, status='', message='')
-                    new_process.status = 'Running' if success else 'Error'
-                    new_process.message = '' if success else message
-                    session.add(new_process)
-                    session.commit()
-                                
-                    out, error = process.communicate()
-
-                    if error.strip() != '':
-                        session.query(Runs).filter_by(pid=process.pid).update({'status': 'Error', 'message': error.strip().decode('utf-8')})
-
-                    if out.strip() != '':
-                        session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
-
-                    session.commit()
-                else:
-                    self.log.error('It has not been possible to execute the command. It must be related to the OS')
-
-
-        self.finish(json.dumps({
-            "data": "This is /jupyterlab-nbqueue/run endpoint!"
-        }))
+            message = "Your notebook have been sent to the queue."
+            self.finish(json.dumps({
+                "data": message
+            }))
 
     @tornado.web.authenticated  # type: ignore
     def delete(self):
         try:
             request_data = self.get_json_body()
             if request_data:
                 delete_all = request_data['deleteAll']
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/build_log.json` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444437555114639%*

 * *Differences: {'0': "{'bail': True, 'plugins': {1: {'_options': {'shared': {'jupyterlab-nbqueue': {'version': "*

 * *      "'0.1.2'}}}}}}"}*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "bail": false,
+        "bail": true,
         "devtool": "source-map",
         "entry": {},
         "mode": "development",
         "module": {
             "rules": [
                 {
                     "test": {},
@@ -588,15 +588,15 @@
                             "requiredVersion": "^1.33.0",
                             "singleton": true
                         },
                         "bootstrap": {},
                         "jupyterlab-nbqueue": {
                             "import": "/Users/luisgleon/Proyectos/Navteca/OpenScienceStudio/jupyterlab_nbqueue/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.1"
+                            "version": "0.1.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-bootstrap": {},
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/package.json` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b4a869fd4dc07cdda70f.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -106,15 +106,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Navteca/jupyterlab-nbqueue.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.386184b399a7a26bbfe6.js",
+            "load": "static/remoteEntry.b4a869fd4dc07cdda70f.js",
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
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.2724577231114db8dca3.js` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 "use strict";
 (self["webpackChunkjupyterlab_nbqueue"] = self["webpackChunkjupyterlab_nbqueue"] || []).push([
     ["lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61"], {
 
         /***/
-        "./style/queue-solid-svgrepo-com.svg":
-            /*!*******************************************!*\
-              !*** ./style/queue-solid-svgrepo-com.svg ***!
-              \*******************************************/
+        "./style/nbqueue_logo_v2.svg":
+            /*!***********************************!*\
+              !*** ./style/nbqueue_logo_v2.svg ***!
+              \***********************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
                     "default": () => (__WEBPACK_DEFAULT_EXPORT__)
                     /* harmony export */
                 });
                 /* harmony default export */
-                const __WEBPACK_DEFAULT_EXPORT__ = ("<?xml version=\"1.0\" encoding=\"utf-8\"?>\n\r<!-- Uploaded to: SVG Repo, www.svgrepo.com, Generator: SVG Repo Mixer Tools -->\n<svg width=\"800px\" height=\"800px\" viewBox=\"0 0 48 48\" xmlns=\"http://www.w3.org/2000/svg\">\r\n  <title>queue-solid</title>\r\n  <g id=\"Layer_2\" data-name=\"Layer 2\">\r\n    <g id=\"invisible_box\" data-name=\"invisible box\">\r\n      <rect width=\"48\" height=\"48\" fill=\"none\"/>\r\n    </g>\r\n    <g id=\"icons_Q2\" data-name=\"icons Q2\">\r\n      <path d=\"M16,36a2,2,0,0,1-2-2V6a2,2,0,0,1,2-2h0a2,2,0,0,1,2,2V34a2,2,0,0,1-2,2Z\"/>\r\n      <path d=\"M24,36a2,2,0,0,1-2-2V6a2,2,0,0,1,2-2h0a2,2,0,0,1,2,2V34a2,2,0,0,1-2,2Z\"/>\r\n      <path d=\"M32,36a2,2,0,0,1-2-2V6a2,2,0,0,1,2-2h0a2,2,0,0,1,2,2V34a2,2,0,0,1-2,2Z\"/>\r\n      <path d=\"M39.7,26A2.1,2.1,0,0,0,38,28.1V40H10V28.1A2.1,2.1,0,0,0,8.3,26,2,2,0,0,0,6,28V42a2,2,0,0,0,2,2H40a2,2,0,0,0,2-2V28A2,2,0,0,0,39.7,26Z\"/>\r\n      <path d=\"M9.8,15.7,2.5,11.1c-.3-.2-.5-.1-.5.3v9.2c0,.4.2.5.5.3l7.3-4.6Q10.3,16,9.8,15.7Z\"/>\r\n      <path d=\"M45.8,15.7l-7.3-4.6c-.3-.2-.5-.1-.5.3v9.2c0,.4.2.5.5.3l7.3-4.6Q46.3,16,45.8,15.7Z\"/>\r\n    </g>\r\n  </g>\r\n</svg>");
+                const __WEBPACK_DEFAULT_EXPORT__ = ("<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n<!-- Generated by Pixelmator Pro 3.3.6 -->\n<svg width=\"800\" height=\"800\" viewBox=\"0 0 800 800\" xmlns=\"http://www.w3.org/2000/svg\">\n    <g id=\"notebook-svgrepo-com\">\n        <path id=\"Trazado\" fill=\"#69b6a9\" stroke=\"none\" d=\"M 676.253113 127.251587 L 676.253113 742.606262 C 676.253113 774.289063 649.5047 800 616.393738 800 L 59.860939 800 C 58.042187 800 56.225002 799.8703 54.40625 799.740662 C 27.917189 797.403137 6.492188 778.704712 1.16875 754.164063 C 0.65 751.306274 0.259375 748.450012 0.129687 745.46405 C -0 744.554688 -0 743.515625 -0 742.606262 L -0 127.251587 C -0 123.226563 0.389062 119.460938 1.16875 115.695313 C 4.026562 102.710938 11.296875 91.412476 21.554688 83.103149 C 25.190624 80.2453 29.085938 77.648438 33.5 75.701538 C 41.420315 71.935913 50.379688 69.857788 59.859379 69.857788 L 616.392212 69.857788 C 629.117188 69.857788 641.064087 73.623413 650.803162 80.2453 C 655.737488 83.621887 660.15155 87.646851 663.787537 92.190613 C 664.435974 92.970337 665.085938 93.878113 665.734375 94.787476 C 667.553162 97.384399 669.110901 99.981262 670.539063 102.837524 C 671.059387 103.876587 671.578125 104.915649 671.96875 105.954712 C 673.396851 109.459351 674.565613 113.096863 675.215637 116.860962 C 675.474976 118.029663 675.734375 119.198425 675.864075 120.496887 C 676.123413 122.707825 676.253113 124.914063 676.253113 127.251587 Z\"/>\n        <path id=\"path1\" fill=\"#313333\" stroke=\"none\" d=\"M 159.714066 69.859375 L 159.714066 800 L 57.393749 800 C 56.484379 800 55.445313 800 54.535938 799.8703 C 28.046877 798.571899 6.3625 779.354675 1.16875 754.164063 C 0.65 751.306274 0.259375 748.450012 0.129687 745.46405 C 0 744.554688 0 743.515625 0 742.606262 L 0 127.251587 C 0 123.226563 0.389062 119.460938 1.16875 115.695313 C 3.895313 102.320313 11.296875 90.634399 21.554688 82.323425 C 25.320313 79.465637 29.345312 76.868774 33.760937 75.051575 C 39.053123 72.549988 44.940624 71.231262 51.018749 70.546875 C 52.289063 70.367188 53.567188 70.232788 54.862499 70.131226 C 55.721874 70.09375 56.524998 69.857788 57.393749 69.857788 L 159.714066 69.857788 Z\"/>\n        <path id=\"path2\" fill=\"#b2536c\" stroke=\"none\" d=\"M 295.08905 366.078125 L 237.642197 337.581238 L 180.195313 366.078125 L 180.195313 69.868774 L 295.08905 69.868774 Z\"/>\n        <path id=\"path3\" fill=\"#f5e529\" stroke=\"none\" d=\"M 609.865601 33.378113 L 186.943741 33.378113 L 87.414063 33.378113 C 56.546871 33.378113 31.510937 59.104675 31.510937 90.825012 L 31.510937 116.051575 C 31.510937 147.770325 56.546871 173.498413 87.414063 173.498413 L 186.943741 173.498413 L 609.865601 173.498413 C 640.732788 173.498413 665.768738 147.771851 665.768738 116.051575 L 665.768738 90.825012 C 665.768738 59.104675 640.732788 33.378113 609.865601 33.378113 Z\"/>\n        <path id=\"path4\" fill=\"#f2f2f2\" stroke=\"none\" d=\"M 665.768738 98.404663 L 186.943741 98.404663 L 31.510937 98.404663 L 31.510937 745.995361 L 186.943741 745.995361 L 665.768738 745.995361 Z\"/>\n        <linearGradient id=\"linearGradient1\" x1=\"31.510312\" y1=\"742.616719\" x2=\"665.769375\" y2=\"742.616719\" gradientUnits=\"userSpaceOnUse\">\n            <stop offset=\"1e-05\" stop-color=\"#ffffff\" stop-opacity=\"1\"/>\n            <stop offset=\"0.9952\" stop-color=\"#f6f5f5\" stop-opacity=\"1\"/>\n        </linearGradient>\n        <path id=\"path5\" fill=\"url(#linearGradient1)\" stroke=\"none\" d=\"M 634.364075 770.02655 L 53.420311 770.02655 C 41.370312 770.02655 31.509377 760.167175 31.509377 748.115662 L 31.509377 737.117188 C 31.509377 725.0672 41.368752 715.206238 53.420311 715.206238 L 643.857788 715.206238 C 655.907837 715.206238 665.768738 725.065613 665.768738 737.117188 L 665.768738 738.620361 C 665.768738 755.893738 651.637512 770.02655 634.364075 770.02655 Z\"/>\n        <path id=\"path6\" fill=\"#69b6a9\" stroke=\"none\" d=\"M 650.803162 57.523438 L 650.803162 672.748413 C 650.803162 689.628113 643.53125 704.821899 631.974976 715.209412 C 621.846863 724.6875 608.212524 730.271851 593.279724 730.271851 L 57.393749 730.271851 C 49.34375 730.271851 41.81094 728.584351 34.929688 725.596863 C 33.760937 725.206238 32.592186 724.6875 31.554688 724.039063 C 28.048437 722.220337 24.671875 720.143738 21.55625 717.676514 C 21.165625 717.285889 20.646875 717.028137 20.257813 716.637512 C 17.401562 714.170288 14.803125 711.443726 12.467188 708.456238 C 4.675 698.717163 0 686.251526 0 672.748413 L 0 57.523438 C 0 25.709351 25.709375 0 57.393749 0 L 593.279724 0 C 622.885925 0 647.426575 22.46405 650.543762 51.549988 C 650.543762 51.549988 650.543762 51.549988 650.543762 51.679688 C 650.673462 53.628113 650.803162 55.576538 650.803162 57.523438 Z\"/>\n        <path id=\"path7\" fill=\"#d6d7d7\" stroke=\"none\" d=\"M 181.321869 0.032837 L 181.321869 730.226563 L 21.598438 730.226563 L 21.598438 57.478149 C 21.598438 25.757813 47.325001 0.03125 79.045311 0.03125 L 181.321869 0.03125 Z\"/>\n        <path id=\"path8\" fill=\"#505354\" stroke=\"none\" d=\"M 159.714066 0 L 159.714066 730.271851 L 0 730.271851 L 0 57.523438 C 0 25.709351 25.709375 0 57.393749 0 L 159.714066 0 Z\"/>\n        <path id=\"path9\" fill=\"#ebe0ac\" stroke=\"none\" d=\"M 453.770294 194.865601 L 389.565643 160.092163 L 325.360931 194.865601 L 325.360931 0.032837 L 453.770294 0.032837 Z\"/>\n        <path id=\"path10\" fill=\"#bdb595\" stroke=\"none\" d=\"M 418.632782 76.351563 L 396.689056 76.351563 L 394.610931 69.859375 L 389.676575 54.796875 L 389.417206 54.796875 L 384.612488 69.859375 L 382.534393 76.351563 L 360.459381 76.351563 L 360.459381 76.610962 L 378.248444 89.726563 L 375.392212 98.426575 L 371.237488 111.542175 L 371.496857 111.542175 L 389.15625 98.426575 L 389.545319 98.167175 L 389.934387 98.426575 L 407.593719 111.542175 L 407.853119 111.542175 L 403.698456 98.426575 L 400.842194 89.726563 L 418.631256 76.610962 L 418.631256 76.351563 Z\"/>\n        <path id=\"path11\" fill=\"#040000\" stroke=\"none\" opacity=\"0.04\" d=\"M 676.253113 127.251587 L 676.253113 742.606262 C 676.253113 774.289063 649.5047 800 616.393738 800 L 57.393749 800 C 56.484379 800 55.445313 800 54.535938 799.8703 C 28.046877 798.571899 6.3625 779.354675 1.16875 754.164063 C 0.65 751.306274 0.259375 748.450012 0.129687 745.46405 C -0 744.554688 -0 743.515625 -0 742.606262 L -0 720.273438 L 12.465625 708.456238 L 21.554688 699.885925 L 31.553125 690.40625 L 159.714066 569.128113 L 181.268753 548.742188 L 577.957825 173.478149 L 650.803162 104.528137 L 657.165649 98.424988 L 663.787537 92.1922 L 665.734375 90.375 L 665.734375 94.789063 C 667.553162 97.385925 669.110901 99.982788 670.539063 102.83905 C 671.059387 103.878113 671.578125 104.917175 671.96875 105.956238 C 673.396851 109.460938 674.565613 113.09845 675.215637 116.862488 C 675.474976 118.03125 675.734375 119.200012 675.864075 120.498413 C 676.123413 122.707825 676.253113 124.914063 676.253113 127.251587 Z\"/>\n    </g>\n    <g id=\"Circle-icons-gear\">\n        <g id=\"Layer1\">\n            <g id=\"Agrupar\">\n                <path id=\"path12\" fill=\"#76c2af\" stroke=\"none\" d=\"M 589 445 C 589 549.381836 504.381805 634 400 634 C 295.618195 634 211 549.381836 211 445 C 211 340.618195 295.618195 256 400 256 C 504.381805 256 589 340.618195 589 445 Z\"/>\n            </g>\n            <g id=\"g1\" opacity=\"0.2\">\n                <g id=\"g2\">\n                    <path id=\"path13\" fill=\"#231f20\" stroke=\"none\" d=\"M 373.421875 456.8125 C 373.421875 471.578125 385.234375 483.390625 400 483.390625 C 414.765625 483.390625 426.578125 471.578125 426.578125 456.8125 C 426.578125 442.046875 414.765625 430.234375 400 430.234375 C 385.234375 430.234375 373.421875 442.046875 373.421875 456.8125 Z\"/>\n                </g>\n            </g>\n            <g id=\"g3\" opacity=\"0.2\">\n                <path id=\"path14\" fill=\"#231f20\" stroke=\"none\" d=\"M 529.346863 448.543732 C 529.346863 445.590607 526.393738 442.046875 523.440613 440.865631 L 499.225006 432.006256 C 496.271881 430.824982 492.728119 427.28125 491.546875 424.328125 L 487.412506 414.878143 C 486.231232 411.925018 486.231232 407.199982 487.412506 404.246857 L 498.634369 381.212494 C 499.815643 378.259369 499.225006 374.125 497.453125 371.762482 L 485.640625 359.949982 C 483.278107 357.587494 478.553131 356.996857 476.190643 358.768768 L 453.15625 369.990631 C 450.203125 371.171875 445.478119 371.171875 442.524994 369.990631 L 433.074982 365.856232 C 430.121857 364.675018 426.578125 361.131256 425.396881 358.178131 L 416.537506 333.962494 C 415.356232 331.009369 411.8125 328.056244 408.859375 328.056244 C 408.859375 328.056244 405.315643 327.465607 400.590607 327.465607 C 395.865631 327.465607 392.321869 328.056244 392.321869 328.056244 C 389.368744 328.056244 385.825012 331.009369 384.643738 333.962494 L 375.784363 358.178131 C 374.603119 361.131256 371.059387 364.675018 368.106262 365.856232 L 358.65625 369.990631 C 355.703125 371.171875 350.978119 371.171875 348.024994 369.990631 L 324.990631 358.768768 C 322.037506 357.587494 317.903137 358.178131 315.540619 359.949982 L 303.728119 371.762482 C 301.365631 374.125 300.774994 378.850006 302.546875 381.212494 L 313.768738 404.246857 C 314.950012 407.199982 314.950012 411.925018 313.768738 414.878143 L 309.634369 424.328125 C 308.453125 427.28125 304.909363 430.824982 301.956238 432.006256 L 277.740631 440.865631 C 274.787506 442.046875 271.834381 445.590607 271.834381 448.543732 C 271.834381 448.543732 271.243744 452.087494 271.243744 456.8125 C 271.243744 461.537506 271.834381 465.081268 271.834381 465.081268 C 271.834381 468.034393 274.787506 471.578125 277.740631 472.759369 L 301.956238 481.618744 C 304.909363 482.800018 308.453125 486.34375 309.634369 489.296875 L 313.768738 498.746857 C 314.950012 501.699982 314.950012 506.425018 313.768738 509.378143 L 302.546875 532.412476 C 301.365631 535.365601 301.956238 539.5 303.728119 541.862549 L 315.540619 553.674988 C 317.903137 556.037476 322.628113 556.628113 324.990631 554.856262 L 348.024994 543.634399 C 350.978119 542.453125 355.703125 542.453125 358.65625 543.634399 L 368.106262 547.768738 C 371.059387 548.950012 374.603119 552.493774 375.784363 555.446899 L 384.643738 579.662476 C 385.825012 582.615601 389.368744 585.568726 392.321869 585.568726 C 392.321869 585.568726 395.865631 586.159363 400.590607 586.159363 C 405.315643 586.159363 408.859375 585.568726 408.859375 585.568726 C 411.8125 585.568726 415.356232 582.615601 416.537506 579.662476 L 425.396881 555.446899 C 426.578125 552.493774 430.121857 548.950012 433.074982 547.768738 L 442.524994 543.634399 C 445.478119 542.453125 450.203125 542.453125 453.15625 543.634399 L 476.190643 554.856262 C 479.143768 556.037476 483.278107 555.446899 485.640625 553.674988 L 497.453125 541.862549 C 499.815643 539.5 500.40625 534.775024 498.634369 532.412476 L 487.412506 509.378143 C 486.231232 506.425018 486.231232 501.699982 487.412506 498.746857 L 491.546875 489.296875 C 492.728119 486.34375 496.271881 482.800018 499.225006 481.618744 L 523.440613 472.759369 C 526.393738 471.578125 529.346863 468.034393 529.346863 465.081268 C 529.346863 465.081268 529.9375 461.537506 529.9375 456.8125 C 529.9375 452.087494 529.346863 448.543732 529.346863 448.543732 Z M 400 515.875 C 367.515625 515.875 340.9375 489.296875 340.9375 456.8125 C 340.9375 424.328125 367.515625 397.75 400 397.75 C 432.484375 397.75 459.0625 424.328125 459.0625 456.8125 C 459.0625 489.296875 432.484375 515.875 400 515.875 Z\"/>\n            </g>\n            <g id=\"g4\">\n                <g id=\"g5\">\n                    <path id=\"path15\" fill=\"#4f5d73\" stroke=\"none\" d=\"M 373.421875 445 C 373.421875 459.765625 385.234375 471.578125 400 471.578125 C 414.765625 471.578125 426.578125 459.765625 426.578125 445 C 426.578125 430.234375 414.765625 418.421875 400 418.421875 C 385.234375 418.421875 373.421875 430.234375 373.421875 445 Z\"/>\n                </g>\n            </g>\n            <g id=\"g6\">\n                <path id=\"path16\" fill=\"#ffffff\" stroke=\"none\" d=\"M 529.346863 436.731232 C 529.346863 433.778107 526.393738 430.234375 523.440613 429.053131 L 499.225006 420.193756 C 496.271881 419.012482 492.728119 415.46875 491.546875 412.515625 L 487.412506 403.065643 C 486.231232 400.112518 486.231232 395.387482 487.412506 392.434357 L 498.634369 369.399994 C 499.815643 366.446869 499.225006 362.3125 497.453125 359.949982 L 485.640625 348.137482 C 483.278107 345.774994 478.553131 345.184357 476.190643 346.956268 L 453.15625 358.178131 C 450.203125 359.359375 445.478119 359.359375 442.524994 358.178131 L 433.074982 354.043732 C 430.121857 352.862518 426.578125 349.318756 425.396881 346.365631 L 416.537506 322.149994 C 415.356232 319.196869 411.8125 316.243744 408.859375 316.243744 C 408.859375 316.243744 405.315643 315.653107 400.590607 315.653107 C 395.865631 315.653107 392.321869 316.243744 392.321869 316.243744 C 389.368744 316.243744 385.825012 319.196869 384.643738 322.149994 L 375.784363 346.365631 C 374.603119 349.318756 371.059387 352.862518 368.106262 354.043732 L 358.65625 358.178131 C 355.703125 359.359375 350.978119 359.359375 348.024994 358.178131 L 324.990631 346.956268 C 322.037506 345.774994 317.903137 346.365631 315.540619 348.137482 L 303.728119 359.949982 C 301.365631 362.3125 300.774994 367.037506 302.546875 369.399994 L 313.768738 392.434357 C 314.950012 395.387482 314.950012 400.112518 313.768738 403.065643 L 309.634369 412.515625 C 308.453125 415.46875 304.909363 419.012482 301.956238 420.193756 L 277.740631 429.053131 C 274.787506 430.234375 271.834381 433.778107 271.834381 436.731232 C 271.834381 436.731232 271.243744 440.274994 271.243744 445 C 271.243744 449.725006 271.834381 453.268768 271.834381 453.268768 C 271.834381 456.221893 274.787506 459.765625 277.740631 460.946869 L 301.956238 469.806244 C 304.909363 470.987518 308.453125 474.53125 309.634369 477.484375 L 313.768738 486.934357 C 314.950012 489.887482 314.950012 494.612518 313.768738 497.565643 L 302.546875 520.599976 C 301.365631 523.553101 301.956238 527.6875 303.728119 530.050049 L 315.540619 541.862549 C 317.903137 544.224976 322.628113 544.815613 324.990631 543.043701 L 348.024994 531.821899 C 350.978119 530.640625 355.703125 530.640625 358.65625 531.821899 L 368.106262 535.956299 C 371.059387 537.137451 374.603119 540.681274 375.784363 543.634399 L 384.643738 567.849976 C 385.825012 570.803101 389.368744 573.756226 392.321869 573.756226 C 392.321869 573.756226 395.865631 574.346863 400.590607 574.346863 C 405.315643 574.346863 408.859375 573.756226 408.859375 573.756226 C 411.8125 573.756226 415.356232 570.803101 416.537506 567.849976 L 425.396881 543.634399 C 426.578125 540.681274 430.121857 537.137451 433.074982 535.956299 L 442.524994 531.821899 C 445.478119 530.640625 450.203125 530.640625 453.15625 531.821899 L 476.190643 543.043701 C 479.143768 544.224976 483.278107 543.634399 485.640625 541.862549 L 497.453125 530.050049 C 499.815643 527.6875 500.40625 522.962524 498.634369 520.599976 L 487.412506 497.565643 C 486.231232 494.612518 486.231232 489.887482 487.412506 486.934357 L 491.546875 477.484375 C 492.728119 474.53125 496.271881 470.987518 499.225006 469.806244 L 523.440613 460.946869 C 526.393738 459.765625 529.346863 456.221893 529.346863 453.268768 C 529.346863 453.268768 529.9375 449.725006 529.9375 445 C 529.9375 440.274994 529.346863 436.731232 529.346863 436.731232 Z M 400 504.0625 C 367.515625 504.0625 340.9375 477.484375 340.9375 445 C 340.9375 412.515625 367.515625 385.9375 400 385.9375 C 432.484375 385.9375 459.0625 412.515625 459.0625 445 C 459.0625 477.484375 432.484375 504.0625 400 504.0625 Z\"/>\n            </g>\n        </g>\n        <g id=\"Layer2\"/>\n    </g>\n</svg>\n");
 
                 /***/
             }),
 
         /***/
         "./lib/components/RunComponent.js":
             /*!****************************************!*\
@@ -512,20 +512,20 @@
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
-                var _style_queue_solid_svgrepo_com_svg__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! ../../style/queue-solid-svgrepo-com.svg */ "./style/queue-solid-svgrepo-com.svg");
+                var _style_nbqueue_logo_v2_svg__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! ../../style/nbqueue_logo_v2.svg */ "./style/nbqueue_logo_v2.svg");
 
 
                 const nbqueueIcon = new _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_0__.LabIcon({
                     name: 'nbqueue',
-                    svgstr: _style_queue_solid_svgrepo_com_svg__WEBPACK_IMPORTED_MODULE_1__["default"]
+                    svgstr: _style_nbqueue_logo_v2_svg__WEBPACK_IMPORTED_MODULE_1__["default"]
                 });
 
 
                 /***/
             }),
 
         /***/
@@ -826,8 +826,8 @@
                 module.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 8 8%27%3e%3cpath fill=%27%23198754%27 d=%27M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z%27/%3e%3c/svg%3e";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.2724577231114db8dca3.js.map
+//# sourceMappingURL=lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.5d0ad4afe884aa708c22.js.map` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8412698412698413%*

 * *Differences: {"'file'": "'lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;AAAA,iEAAe,k8eAAk8e;;;;;;;;;;;;;;;;;;;;;;;ACAv6e;AACE;AACJ;AACE;AACkB;AACd;AACH;AAGsB;AAM1D,MAAM,YAAY,GAAoB,CAAC,EAAE,GAAG,EAAE,EAAe,EAAE;IACpE,MAAM,EAAE,iBAAiB,EAAE,WAAW,EAAE,GAAG,iDAAU,CACnD,oDAAU,CACO,CAAC;IACpB,MAAM,iBAAiB,GAAG,KAAK,EAC7B,KAAoC,EACpC,EAAU,EACV,GAAW,EACX,EAAE;QACF,KAAK,CAAC,cAAc,EAAE,CAAC;QACvB,iBAAiB,CAAC,EAAE,EAAE,EAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.5d0ad4afe884aa708c22.js",
-    "mappings": "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",
+    "file": "lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.78207085ee8bf5d10cb1.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-nbqueue/./style/nbqueue_logo_v2.svg",
         "webpack://jupyterlab-nbqueue/./src/components/RunComponent.tsx",
         "webpack://jupyterlab-nbqueue/./src/components/RunsContext.tsx",
         "webpack://jupyterlab-nbqueue/./src/components/RunsPanelComponent.tsx",
@@ -13,15 +13,15 @@
         "webpack://jupyterlab-nbqueue/./src/style/IconsStyle.ts",
         "webpack://jupyterlab-nbqueue/./src/widgets/RunsPanelWidget.tsx"
     ],
     "sourcesContent": [
         "export default \"<?xml version=\\\"1.0\\\" encoding=\\\"UTF-8\\\"?>\\n<!-- Generated by Pixelmator Pro 3.3.6 -->\\n<svg width=\\\"800\\\" height=\\\"800\\\" viewBox=\\\"0 0 800 800\\\" xmlns=\\\"http://www.w3.org/2000/svg\\\">\\n    <g id=\\\"notebook-svgrepo-com\\\">\\n        <path id=\\\"Trazado\\\" fill=\\\"#69b6a9\\\" stroke=\\\"none\\\" d=\\\"M 676.253113 127.251587 L 676.253113 742.606262 C 676.253113 774.289063 649.5047 800 616.393738 800 L 59.860939 800 C 58.042187 800 56.225002 799.8703 54.40625 799.740662 C 27.917189 797.403137 6.492188 778.704712 1.16875 754.164063 C 0.65 751.306274 0.259375 748.450012 0.129687 745.46405 C -0 744.554688 -0 743.515625 -0 742.606262 L -0 127.251587 C -0 123.226563 0.389062 119.460938 1.16875 115.695313 C 4.026562 102.710938 11.296875 91.412476 21.554688 83.103149 C 25.190624 80.2453 29.085938 77.648438 33.5 75.701538 C 41.420315 71.935913 50.379688 69.857788 59.859379 69.857788 L 616.392212 69.857788 C 629.117188 69.857788 641.064087 73.623413 650.803162 80.2453 C 655.737488 83.621887 660.15155 87.646851 663.787537 92.190613 C 664.435974 92.970337 665.085938 93.878113 665.734375 94.787476 C 667.553162 97.384399 669.110901 99.981262 670.539063 102.837524 C 671.059387 103.876587 671.578125 104.915649 671.96875 105.954712 C 673.396851 109.459351 674.565613 113.096863 675.215637 116.860962 C 675.474976 118.029663 675.734375 119.198425 675.864075 120.496887 C 676.123413 122.707825 676.253113 124.914063 676.253113 127.251587 Z\\\"/>\\n        <path id=\\\"path1\\\" fill=\\\"#313333\\\" stroke=\\\"none\\\" d=\\\"M 159.714066 69.859375 L 159.714066 800 L 57.393749 800 C 56.484379 800 55.445313 800 54.535938 799.8703 C 28.046877 798.571899 6.3625 779.354675 1.16875 754.164063 C 0.65 751.306274 0.259375 748.450012 0.129687 745.46405 C 0 744.554688 0 743.515625 0 742.606262 L 0 127.251587 C 0 123.226563 0.389062 119.460938 1.16875 115.695313 C 3.895313 102.320313 11.296875 90.634399 21.554688 82.323425 C 25.320313 79.465637 29.345312 76.868774 33.760937 75.051575 C 39.053123 72.549988 44.940624 71.231262 51.018749 70.546875 C 52.289063 70.367188 53.567188 70.232788 54.862499 70.131226 C 55.721874 70.09375 56.524998 69.857788 57.393749 69.857788 L 159.714066 69.857788 Z\\\"/>\\n        <path id=\\\"path2\\\" fill=\\\"#b2536c\\\" stroke=\\\"none\\\" d=\\\"M 295.08905 366.078125 L 237.642197 337.581238 L 180.195313 366.078125 L 180.195313 69.868774 L 295.08905 69.868774 Z\\\"/>\\n        <path id=\\\"path3\\\" fill=\\\"#f5e529\\\" stroke=\\\"none\\\" d=\\\"M 609.865601 33.378113 L 186.943741 33.378113 L 87.414063 33.378113 C 56.546871 33.378113 31.510937 59.104675 31.510937 90.825012 L 31.510937 116.051575 C 31.510937 147.770325 56.546871 173.498413 87.414063 173.498413 L 186.943741 173.498413 L 609.865601 173.498413 C 640.732788 173.498413 665.768738 147.771851 665.768738 116.051575 L 665.768738 90.825012 C 665.768738 59.104675 640.732788 33.378113 609.865601 33.378113 Z\\\"/>\\n        <path id=\\\"path4\\\" fill=\\\"#f2f2f2\\\" stroke=\\\"none\\\" d=\\\"M 665.768738 98.404663 L 186.943741 98.404663 L 31.510937 98.404663 L 31.510937 745.995361 L 186.943741 745.995361 L 665.768738 745.995361 Z\\\"/>\\n        <linearGradient id=\\\"linearGradient1\\\" x1=\\\"31.510312\\\" y1=\\\"742.616719\\\" x2=\\\"665.769375\\\" y2=\\\"742.616719\\\" gradientUnits=\\\"userSpaceOnUse\\\">\\n            <stop offset=\\\"1e-05\\\" stop-color=\\\"#ffffff\\\" stop-opacity=\\\"1\\\"/>\\n            <stop offset=\\\"0.9952\\\" stop-color=\\\"#f6f5f5\\\" stop-opacity=\\\"1\\\"/>\\n        </linearGradient>\\n        <path id=\\\"path5\\\" fill=\\\"url(#linearGradient1)\\\" stroke=\\\"none\\\" d=\\\"M 634.364075 770.02655 L 53.420311 770.02655 C 41.370312 770.02655 31.509377 760.167175 31.509377 748.115662 L 31.509377 737.117188 C 31.509377 725.0672 41.368752 715.206238 53.420311 715.206238 L 643.857788 715.206238 C 655.907837 715.206238 665.768738 725.065613 665.768738 737.117188 L 665.768738 738.620361 C 665.768738 755.893738 651.637512 770.02655 634.364075 770.02655 Z\\\"/>\\n        <path id=\\\"path6\\\" fill=\\\"#69b6a9\\\" stroke=\\\"none\\\" d=\\\"M 650.803162 57.523438 L 650.803162 672.748413 C 650.803162 689.628113 643.53125 704.821899 631.974976 715.209412 C 621.846863 724.6875 608.212524 730.271851 593.279724 730.271851 L 57.393749 730.271851 C 49.34375 730.271851 41.81094 728.584351 34.929688 725.596863 C 33.760937 725.206238 32.592186 724.6875 31.554688 724.039063 C 28.048437 722.220337 24.671875 720.143738 21.55625 717.676514 C 21.165625 717.285889 20.646875 717.028137 20.257813 716.637512 C 17.401562 714.170288 14.803125 711.443726 12.467188 708.456238 C 4.675 698.717163 0 686.251526 0 672.748413 L 0 57.523438 C 0 25.709351 25.709375 0 57.393749 0 L 593.279724 0 C 622.885925 0 647.426575 22.46405 650.543762 51.549988 C 650.543762 51.549988 650.543762 51.549988 650.543762 51.679688 C 650.673462 53.628113 650.803162 55.576538 650.803162 57.523438 Z\\\"/>\\n        <path id=\\\"path7\\\" fill=\\\"#d6d7d7\\\" stroke=\\\"none\\\" d=\\\"M 181.321869 0.032837 L 181.321869 730.226563 L 21.598438 730.226563 L 21.598438 57.478149 C 21.598438 25.757813 47.325001 0.03125 79.045311 0.03125 L 181.321869 0.03125 Z\\\"/>\\n        <path id=\\\"path8\\\" fill=\\\"#505354\\\" stroke=\\\"none\\\" d=\\\"M 159.714066 0 L 159.714066 730.271851 L 0 730.271851 L 0 57.523438 C 0 25.709351 25.709375 0 57.393749 0 L 159.714066 0 Z\\\"/>\\n        <path id=\\\"path9\\\" fill=\\\"#ebe0ac\\\" stroke=\\\"none\\\" d=\\\"M 453.770294 194.865601 L 389.565643 160.092163 L 325.360931 194.865601 L 325.360931 0.032837 L 453.770294 0.032837 Z\\\"/>\\n        <path id=\\\"path10\\\" fill=\\\"#bdb595\\\" stroke=\\\"none\\\" d=\\\"M 418.632782 76.351563 L 396.689056 76.351563 L 394.610931 69.859375 L 389.676575 54.796875 L 389.417206 54.796875 L 384.612488 69.859375 L 382.534393 76.351563 L 360.459381 76.351563 L 360.459381 76.610962 L 378.248444 89.726563 L 375.392212 98.426575 L 371.237488 111.542175 L 371.496857 111.542175 L 389.15625 98.426575 L 389.545319 98.167175 L 389.934387 98.426575 L 407.593719 111.542175 L 407.853119 111.542175 L 403.698456 98.426575 L 400.842194 89.726563 L 418.631256 76.610962 L 418.631256 76.351563 Z\\\"/>\\n        <path id=\\\"path11\\\" fill=\\\"#040000\\\" stroke=\\\"none\\\" opacity=\\\"0.04\\\" d=\\\"M 676.253113 127.251587 L 676.253113 742.606262 C 676.253113 774.289063 649.5047 800 616.393738 800 L 57.393749 800 C 56.484379 800 55.445313 800 54.535938 799.8703 C 28.046877 798.571899 6.3625 779.354675 1.16875 754.164063 C 0.65 751.306274 0.259375 748.450012 0.129687 745.46405 C -0 744.554688 -0 743.515625 -0 742.606262 L -0 720.273438 L 12.465625 708.456238 L 21.554688 699.885925 L 31.553125 690.40625 L 159.714066 569.128113 L 181.268753 548.742188 L 577.957825 173.478149 L 650.803162 104.528137 L 657.165649 98.424988 L 663.787537 92.1922 L 665.734375 90.375 L 665.734375 94.789063 C 667.553162 97.385925 669.110901 99.982788 670.539063 102.83905 C 671.059387 103.878113 671.578125 104.917175 671.96875 105.956238 C 673.396851 109.460938 674.565613 113.09845 675.215637 116.862488 C 675.474976 118.03125 675.734375 119.200012 675.864075 120.498413 C 676.123413 122.707825 676.253113 124.914063 676.253113 127.251587 Z\\\"/>\\n    </g>\\n    <g id=\\\"Circle-icons-gear\\\">\\n        <g id=\\\"Layer1\\\">\\n            <g id=\\\"Agrupar\\\">\\n                <path id=\\\"path12\\\" fill=\\\"#76c2af\\\" stroke=\\\"none\\\" d=\\\"M 589 445 C 589 549.381836 504.381805 634 400 634 C 295.618195 634 211 549.381836 211 445 C 211 340.618195 295.618195 256 400 256 C 504.381805 256 589 340.618195 589 445 Z\\\"/>\\n            </g>\\n            <g id=\\\"g1\\\" opacity=\\\"0.2\\\">\\n                <g id=\\\"g2\\\">\\n                    <path id=\\\"path13\\\" fill=\\\"#231f20\\\" stroke=\\\"none\\\" d=\\\"M 373.421875 456.8125 C 373.421875 471.578125 385.234375 483.390625 400 483.390625 C 414.765625 483.390625 426.578125 471.578125 426.578125 456.8125 C 426.578125 442.046875 414.765625 430.234375 400 430.234375 C 385.234375 430.234375 373.421875 442.046875 373.421875 456.8125 Z\\\"/>\\n                </g>\\n            </g>\\n            <g id=\\\"g3\\\" opacity=\\\"0.2\\\">\\n                <path id=\\\"path14\\\" fill=\\\"#231f20\\\" stroke=\\\"none\\\" d=\\\"M 529.346863 448.543732 C 529.346863 445.590607 526.393738 442.046875 523.440613 440.865631 L 499.225006 432.006256 C 496.271881 430.824982 492.728119 427.28125 491.546875 424.328125 L 487.412506 414.878143 C 486.231232 411.925018 486.231232 407.199982 487.412506 404.246857 L 498.634369 381.212494 C 499.815643 378.259369 499.225006 374.125 497.453125 371.762482 L 485.640625 359.949982 C 483.278107 357.587494 478.553131 356.996857 476.190643 358.768768 L 453.15625 369.990631 C 450.203125 371.171875 445.478119 371.171875 442.524994 369.990631 L 433.074982 365.856232 C 430.121857 364.675018 426.578125 361.131256 425.396881 358.178131 L 416.537506 333.962494 C 415.356232 331.009369 411.8125 328.056244 408.859375 328.056244 C 408.859375 328.056244 405.315643 327.465607 400.590607 327.465607 C 395.865631 327.465607 392.321869 328.056244 392.321869 328.056244 C 389.368744 328.056244 385.825012 331.009369 384.643738 333.962494 L 375.784363 358.178131 C 374.603119 361.131256 371.059387 364.675018 368.106262 365.856232 L 358.65625 369.990631 C 355.703125 371.171875 350.978119 371.171875 348.024994 369.990631 L 324.990631 358.768768 C 322.037506 357.587494 317.903137 358.178131 315.540619 359.949982 L 303.728119 371.762482 C 301.365631 374.125 300.774994 378.850006 302.546875 381.212494 L 313.768738 404.246857 C 314.950012 407.199982 314.950012 411.925018 313.768738 414.878143 L 309.634369 424.328125 C 308.453125 427.28125 304.909363 430.824982 301.956238 432.006256 L 277.740631 440.865631 C 274.787506 442.046875 271.834381 445.590607 271.834381 448.543732 C 271.834381 448.543732 271.243744 452.087494 271.243744 456.8125 C 271.243744 461.537506 271.834381 465.081268 271.834381 465.081268 C 271.834381 468.034393 274.787506 471.578125 277.740631 472.759369 L 301.956238 481.618744 C 304.909363 482.800018 308.453125 486.34375 309.634369 489.296875 L 313.768738 498.746857 C 314.950012 501.699982 314.950012 506.425018 313.768738 509.378143 L 302.546875 532.412476 C 301.365631 535.365601 301.956238 539.5 303.728119 541.862549 L 315.540619 553.674988 C 317.903137 556.037476 322.628113 556.628113 324.990631 554.856262 L 348.024994 543.634399 C 350.978119 542.453125 355.703125 542.453125 358.65625 543.634399 L 368.106262 547.768738 C 371.059387 548.950012 374.603119 552.493774 375.784363 555.446899 L 384.643738 579.662476 C 385.825012 582.615601 389.368744 585.568726 392.321869 585.568726 C 392.321869 585.568726 395.865631 586.159363 400.590607 586.159363 C 405.315643 586.159363 408.859375 585.568726 408.859375 585.568726 C 411.8125 585.568726 415.356232 582.615601 416.537506 579.662476 L 425.396881 555.446899 C 426.578125 552.493774 430.121857 548.950012 433.074982 547.768738 L 442.524994 543.634399 C 445.478119 542.453125 450.203125 542.453125 453.15625 543.634399 L 476.190643 554.856262 C 479.143768 556.037476 483.278107 555.446899 485.640625 553.674988 L 497.453125 541.862549 C 499.815643 539.5 500.40625 534.775024 498.634369 532.412476 L 487.412506 509.378143 C 486.231232 506.425018 486.231232 501.699982 487.412506 498.746857 L 491.546875 489.296875 C 492.728119 486.34375 496.271881 482.800018 499.225006 481.618744 L 523.440613 472.759369 C 526.393738 471.578125 529.346863 468.034393 529.346863 465.081268 C 529.346863 465.081268 529.9375 461.537506 529.9375 456.8125 C 529.9375 452.087494 529.346863 448.543732 529.346863 448.543732 Z M 400 515.875 C 367.515625 515.875 340.9375 489.296875 340.9375 456.8125 C 340.9375 424.328125 367.515625 397.75 400 397.75 C 432.484375 397.75 459.0625 424.328125 459.0625 456.8125 C 459.0625 489.296875 432.484375 515.875 400 515.875 Z\\\"/>\\n            </g>\\n            <g id=\\\"g4\\\">\\n                <g id=\\\"g5\\\">\\n                    <path id=\\\"path15\\\" fill=\\\"#4f5d73\\\" stroke=\\\"none\\\" d=\\\"M 373.421875 445 C 373.421875 459.765625 385.234375 471.578125 400 471.578125 C 414.765625 471.578125 426.578125 459.765625 426.578125 445 C 426.578125 430.234375 414.765625 418.421875 400 418.421875 C 385.234375 418.421875 373.421875 430.234375 373.421875 445 Z\\\"/>\\n                </g>\\n            </g>\\n            <g id=\\\"g6\\\">\\n                <path id=\\\"path16\\\" fill=\\\"#ffffff\\\" stroke=\\\"none\\\" d=\\\"M 529.346863 436.731232 C 529.346863 433.778107 526.393738 430.234375 523.440613 429.053131 L 499.225006 420.193756 C 496.271881 419.012482 492.728119 415.46875 491.546875 412.515625 L 487.412506 403.065643 C 486.231232 400.112518 486.231232 395.387482 487.412506 392.434357 L 498.634369 369.399994 C 499.815643 366.446869 499.225006 362.3125 497.453125 359.949982 L 485.640625 348.137482 C 483.278107 345.774994 478.553131 345.184357 476.190643 346.956268 L 453.15625 358.178131 C 450.203125 359.359375 445.478119 359.359375 442.524994 358.178131 L 433.074982 354.043732 C 430.121857 352.862518 426.578125 349.318756 425.396881 346.365631 L 416.537506 322.149994 C 415.356232 319.196869 411.8125 316.243744 408.859375 316.243744 C 408.859375 316.243744 405.315643 315.653107 400.590607 315.653107 C 395.865631 315.653107 392.321869 316.243744 392.321869 316.243744 C 389.368744 316.243744 385.825012 319.196869 384.643738 322.149994 L 375.784363 346.365631 C 374.603119 349.318756 371.059387 352.862518 368.106262 354.043732 L 358.65625 358.178131 C 355.703125 359.359375 350.978119 359.359375 348.024994 358.178131 L 324.990631 346.956268 C 322.037506 345.774994 317.903137 346.365631 315.540619 348.137482 L 303.728119 359.949982 C 301.365631 362.3125 300.774994 367.037506 302.546875 369.399994 L 313.768738 392.434357 C 314.950012 395.387482 314.950012 400.112518 313.768738 403.065643 L 309.634369 412.515625 C 308.453125 415.46875 304.909363 419.012482 301.956238 420.193756 L 277.740631 429.053131 C 274.787506 430.234375 271.834381 433.778107 271.834381 436.731232 C 271.834381 436.731232 271.243744 440.274994 271.243744 445 C 271.243744 449.725006 271.834381 453.268768 271.834381 453.268768 C 271.834381 456.221893 274.787506 459.765625 277.740631 460.946869 L 301.956238 469.806244 C 304.909363 470.987518 308.453125 474.53125 309.634369 477.484375 L 313.768738 486.934357 C 314.950012 489.887482 314.950012 494.612518 313.768738 497.565643 L 302.546875 520.599976 C 301.365631 523.553101 301.956238 527.6875 303.728119 530.050049 L 315.540619 541.862549 C 317.903137 544.224976 322.628113 544.815613 324.990631 543.043701 L 348.024994 531.821899 C 350.978119 530.640625 355.703125 530.640625 358.65625 531.821899 L 368.106262 535.956299 C 371.059387 537.137451 374.603119 540.681274 375.784363 543.634399 L 384.643738 567.849976 C 385.825012 570.803101 389.368744 573.756226 392.321869 573.756226 C 392.321869 573.756226 395.865631 574.346863 400.590607 574.346863 C 405.315643 574.346863 408.859375 573.756226 408.859375 573.756226 C 411.8125 573.756226 415.356232 570.803101 416.537506 567.849976 L 425.396881 543.634399 C 426.578125 540.681274 430.121857 537.137451 433.074982 535.956299 L 442.524994 531.821899 C 445.478119 530.640625 450.203125 530.640625 453.15625 531.821899 L 476.190643 543.043701 C 479.143768 544.224976 483.278107 543.634399 485.640625 541.862549 L 497.453125 530.050049 C 499.815643 527.6875 500.40625 522.962524 498.634369 520.599976 L 487.412506 497.565643 C 486.231232 494.612518 486.231232 489.887482 487.412506 486.934357 L 491.546875 477.484375 C 492.728119 474.53125 496.271881 470.987518 499.225006 469.806244 L 523.440613 460.946869 C 526.393738 459.765625 529.346863 456.221893 529.346863 453.268768 C 529.346863 453.268768 529.9375 449.725006 529.9375 445 C 529.9375 440.274994 529.346863 436.731232 529.346863 436.731232 Z M 400 504.0625 C 367.515625 504.0625 340.9375 477.484375 340.9375 445 C 340.9375 412.515625 367.515625 385.9375 400 385.9375 C 432.484375 385.9375 459.0625 412.515625 459.0625 445 C 459.0625 477.484375 432.484375 504.0625 400 504.0625 Z\\\"/>\\n            </g>\\n        </g>\\n        <g id=\\\"Layer2\\\"/>\\n    </g>\\n</svg>\\n\";",
         "import React, { useContext } from 'react';\nimport Button from 'react-bootstrap/Button';\nimport Card from 'react-bootstrap/Card';\nimport Stack from 'react-bootstrap/Stack';\nimport OverlayTrigger from 'react-bootstrap/OverlayTrigger';\nimport Tooltip from 'react-bootstrap/Tooltip';\nimport { RunContext } from './RunsContext';\nimport { RunContextType } from './runs';\nimport { IRun } from './CustomProps';\nimport '../../node_modules/bootstrap/dist/css/bootstrap.min.css';\n\ninterface Props {\n  run: IRun;\n}\n\nexport const RunComponent: React.FC<Props> = ({ run }): JSX.Element => {\n  const { deleteRunFromList, getRunsList } = useContext(\n    RunContext\n  ) as RunContextType;\n  const handleDeleteClick = async (\n    event: React.MouseEvent<HTMLElement>,\n    id: number,\n    pid: number\n  ) => {\n    event.preventDefault();\n    deleteRunFromList({ id, pid });\n    getRunsList();\n  };\n\n  const removeFromListTooltip = (\n    <Tooltip id=\"remove-from-list\">Remove from list</Tooltip>\n  );\n\n  return (\n    <div>\n      <Card className=\"m-2\">\n        <Card.Body>\n          <Stack gap={1} direction=\"horizontal\">\n            <Stack gap={1}>\n              <span>{run.name}</span>\n              <span>{run.status}</span>\n            </Stack>\n            <OverlayTrigger placement=\"bottom\" overlay={removeFromListTooltip}>\n              <Button\n                className=\"ms-auto\"\n                variant=\"link\"\n                size=\"sm\"\n                onClick={e => handleDeleteClick(e, run.id, run.pid)}\n                disabled={false}\n              >\n                <span\n                  className=\"fa fa-solid fa-xmark m-2\"\n                  aria-hidden=\"true\"\n                ></span>\n              </Button>\n            </OverlayTrigger>\n          </Stack>\n        </Card.Body>\n      </Card>\n    </div>\n  );\n};\n",
         "import React, { useEffect, useState } from 'react';\nimport { RunContextType } from './runs';\nimport { requestAPI } from '../handler';\nimport { IRunsProps, IRun, IDeleteRun } from './CustomProps';\n\ntype RunProviderProps = {\n  children: React.ReactNode;\n};\n\nexport const RunContext = React.createContext<RunContextType | null>(null);\n\nconst RunProvider: React.FC<RunProviderProps> = ({ children }) => {\n  const [runs, setRun] = useState<IRunsProps>([]);\n\n  useEffect(() => {\n    getRunsList();\n  }, []);\n\n  const runObject = async ({\n    id,\n    pid,\n    name,\n    status,\n    message\n  }: IRun): Promise<void> => {\n    try {\n      await requestAPI<any>('run', {\n        method: 'POST',\n        body: JSON.stringify({ id, pid, name, status, message })\n      });\n      getRunsList();\n    } catch (e) {\n      console.log(\n        `There has been an error trying to run an object => ${JSON.stringify(\n          e,\n          null,\n          2\n        )}`\n      );\n    }\n  };\n\n  const deleteRunFromList = async ({\n    id,\n    pid,\n    deleteAll = false\n  }: IDeleteRun): Promise<void> => {\n    try {\n      await requestAPI<any>('run', {\n        method: 'DELETE',\n        body: JSON.stringify({ deleteAll, id, pid })\n      });\n      getRunsList();\n    } catch (e) {\n      console.log(\n        `There has been an error trying to delete an object from the list of runs => ${e}`\n      );\n    }\n  };\n\n  const getRunsList = async (): Promise<void> => {\n    const response = await requestAPI<any>('run');\n    setRun(response.reverse());\n  };\n\n  return (\n    <RunContext.Provider\n      value={{\n        runs,\n        getRunsList,\n        runObject,\n        deleteRunFromList\n      }}\n    >\n      {children}\n    </RunContext.Provider>\n  );\n};\n\nexport default RunProvider;\n",
-        "import React, { useEffect, useContext } from 'react';\nimport Stack from 'react-bootstrap/Stack';\nimport Button from 'react-bootstrap/Button';\nimport OverlayTrigger from 'react-bootstrap/OverlayTrigger';\nimport Tooltip from 'react-bootstrap/Tooltip';\nimport ButtonGroup from 'react-bootstrap/ButtonGroup';\nimport { RunComponent } from './RunComponent';\nimport { RunContext } from './RunsContext';\nimport { RunContextType } from './runs';\n\nexport const RunsPanelComponent: React.FC = (): JSX.Element => {\n  const { getRunsList, deleteRunFromList, runs } = useContext(\n    RunContext\n  ) as RunContextType;\n\n  useEffect(() => {\n    getRunsList();\n  }, []);\n\n  const handleDelete = (event: React.MouseEvent<HTMLElement>) => {\n    event.preventDefault();\n    deleteRunFromList({ deleteAll: true });\n    getRunsList();\n  };\n\n  const clearListTooltip = <Tooltip id=\"clear-list\">Clear all</Tooltip>;\n  const refreshTooltip = <Tooltip id=\"refresh\">Refresh</Tooltip>;\n\n  return (\n    <div\n      style={{\n        display: 'flex',\n        flexDirection: 'column',\n        height: '100%',\n        overflowY: 'auto'\n      }}\n    >\n      <Stack gap={2} direction=\"horizontal\">\n        <h4>Nbconvert history</h4>\n        <span style={{ flex: '1 1 auto' }}></span>\n        <ButtonGroup className=\"p-2\" aria-label=\"Runs Utilities\">\n          <OverlayTrigger placement=\"bottom\" overlay={clearListTooltip}>\n            <Button\n              variant=\"link\"\n              size=\"sm\"\n              onClick={e => handleDelete(e)}\n              disabled={!!(runs.length === 0)}\n            >\n              <i\n                className=\"fa fa-user m-2 fa-lg\"\n                aria-hidden=\"true\"\n              ></i>\n            </Button>\n          </OverlayTrigger>\n          <OverlayTrigger placement=\"bottom\" overlay={refreshTooltip}>\n            <Button variant=\"link\" size=\"sm\" onClick={getRunsList}>\n              <i\n                className=\"fas fa-user m-2 fa-lg\"\n                aria-hidden=\"true\"\n              ></i>\n            </Button>\n          </OverlayTrigger>\n        </ButtonGroup>\n      </Stack>\n      <div>\n        {runs.map(run => {\n          return <RunComponent run={run} />;\n        })}\n      </div>\n    </div>\n  );\n};\n",
+        "import React, { useEffect, useContext } from 'react';\nimport Stack from 'react-bootstrap/Stack';\nimport Button from 'react-bootstrap/Button';\nimport OverlayTrigger from 'react-bootstrap/OverlayTrigger';\nimport Tooltip from 'react-bootstrap/Tooltip';\nimport ButtonGroup from 'react-bootstrap/ButtonGroup';\nimport { RunComponent } from './RunComponent';\nimport { RunContext } from './RunsContext';\nimport { RunContextType } from './runs';\n\nexport const RunsPanelComponent: React.FC = (): JSX.Element => {\n  const { getRunsList, deleteRunFromList, runs } = useContext(\n    RunContext\n  ) as RunContextType;\n\n  useEffect(() => {\n    getRunsList();\n  }, []);\n\n  const handleDelete = (event: React.MouseEvent<HTMLElement>) => {\n    event.preventDefault();\n    deleteRunFromList({ deleteAll: true });\n    getRunsList();\n  };\n\n  const clearListTooltip = <Tooltip id=\"clear-list\">Clear all</Tooltip>;\n  const refreshTooltip = <Tooltip id=\"refresh\">Refresh</Tooltip>;\n\n  return (\n    <div\n      style={{\n        display: 'flex',\n        flexDirection: 'column',\n        height: '100%',\n        overflowY: 'auto'\n      }}\n    >\n      <Stack gap={2} direction=\"horizontal\">\n        <h4>Nbconvert history</h4>\n        <span style={{ flex: '1 1 auto' }}></span>\n        <ButtonGroup className=\"p-2\" aria-label=\"Runs Utilities\">\n          <OverlayTrigger placement=\"bottom\" overlay={clearListTooltip}>\n            <Button\n              variant=\"link\"\n              size=\"sm\"\n              onClick={e => handleDelete(e)}\n              disabled={!!(runs.length === 0)}\n            >\n              <i\n                className=\"fa fa-solid fa-trash-list m-2 fa-lg\"\n                aria-hidden=\"true\"\n              ></i>\n            </Button>\n          </OverlayTrigger>\n          <OverlayTrigger placement=\"bottom\" overlay={refreshTooltip}>\n            <Button variant=\"link\" size=\"sm\" onClick={getRunsList}>\n              <i\n                className=\"fa fa-solid fa-arrows-rotate m-2 fa-lg\"\n                aria-hidden=\"true\"\n              ></i>\n            </Button>\n          </OverlayTrigger>\n        </ButtonGroup>\n      </Stack>\n      <div>\n        {runs.map(run => {\n          return <RunComponent run={run} />;\n        })}\n      </div>\n    </div>\n  );\n};\n",
         "import { URLExt } from '@jupyterlab/coreutils';\n\nimport { ServerConnection } from '@jupyterlab/services';\n\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI<T>(\n  endPoint = '',\n  init: RequestInit = {}\n): Promise<T> {\n  // Make request to Jupyter API\n  const settings = ServerConnection.makeSettings();\n  const requestUrl = URLExt.join(\n    settings.baseUrl,\n    'jupyterlab-nbqueue', // API Namespace\n    endPoint\n  );\n\n  let response: Response;\n  try {\n    response = await ServerConnection.makeRequest(requestUrl, init, settings);\n  } catch (error) {\n    throw new ServerConnection.NetworkError(error as any);\n  }\n\n  let data: any = await response.text();\n\n  if (data.length > 0) {\n    try {\n      data = JSON.parse(data);\n    } catch (error) {\n      console.log('Not a JSON response body.', response);\n    }\n  }\n\n  if (!response.ok) {\n    throw new ServerConnection.ResponseError(response, data.message || data);\n  }\n\n  return data;\n}\n",
         "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\nimport { showDialog, Dialog, MainAreaWidget } from '@jupyterlab/apputils';\n// import { runIcon } from '@jupyterlab/ui-components';\nimport { nbqueueIcon } from './style/IconsStyle';\n\nimport { requestAPI } from './handler';\n\nimport { RunsPanelWidget } from './widgets/RunsPanelWidget';\n/**\n * Initialization data for the jupyterlab-nbqueue extension.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: 'jupyterlab-nbqueue:plugin',\n  description: 'A JupyterLab extension for queuing notebooks executions.',\n  autoStart: true,\n  requires: [IFileBrowserFactory],\n  activate: (app: JupyterFrontEnd, factory: IFileBrowserFactory) => {\n    const runsContent = new RunsPanelWidget();\n    runsContent.addClass('jp-PropertyInspector-placeholderContent');\n    const runsWidget = new MainAreaWidget<RunsPanelWidget>({\n      content: runsContent\n    });\n    runsWidget.toolbar.hide();\n    runsWidget.title.icon = nbqueueIcon;\n    runsWidget.title.caption = 'Nbconvert runs';\n    app.shell.add(runsWidget, 'right', { rank: 501 });\n\n    app.commands.addCommand('jupyterlab-nbqueue:open', {\n      label: 'Run',\n      caption: \"Example context menu button for file browser's items.\",\n      icon: nbqueueIcon,\n      execute: () => {\n        console.log('jupyterlab-nbqueue:open');\n        const file = factory.tracker.currentWidget?.selectedItems().next();\n\n        console.log(JSON.parse(JSON.stringify(file)));\n        const obj = JSON.parse(JSON.stringify(file));\n\n        if (obj) {\n          showDialog({\n            title: obj.name,\n            body: `Notebook ${obj.name} running in background.`,\n            buttons: [Dialog.okButton()]\n          }).catch(e => console.log(e));\n        }\n\n        requestAPI<any>('run', {\n          method: 'POST',\n          body: JSON.stringify({ notebook: obj.path })\n        })\n          .then(data => {\n            console.log(data);\n          })\n          .catch(reason => {\n            console.error(\n              `The jupyterlab-nbqueue server extension appears to be missing.\\n${reason}`\n            );\n          });\n      }\n    });\n\n    app.contextMenu.addItem({\n      command: 'jupyterlab-nbqueue:open',\n      selector: '.jp-DirListing-item[data-isdir=\"false\"]',\n      rank: 0\n    });\n  }\n};\nexport default plugin;\n",
         "import { LabIcon } from '@jupyterlab/ui-components';\n\nimport nbqueueSVG from '../../style/nbqueue_logo_v2.svg';\n\nexport const nbqueueIcon = new LabIcon({ name: 'nbqueue', svgstr: nbqueueSVG });\n",
         "import React from 'react';\nimport { ReactWidget } from '@jupyterlab/apputils';\nimport { RunsPanelComponent } from '../components/RunsPanelComponent';\nimport RunProvider from '../components/RunsContext';\n\nexport class RunsPanelWidget extends ReactWidget {\n  constructor() {\n    super();\n  }\n\n  render(): JSX.Element {\n    return (\n      <div\n        style={{\n          minWidth: '400px',\n          display: 'flex',\n          flexDirection: 'column',\n          background: 'var(--jp-layout-color1)'\n        }}\n      >\n        <RunProvider>\n          <RunsPanelComponent />\n        </RunProvider>\n      </div>\n    );\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.0d4a29b3c23d232e97db.js.map` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.b4a869fd4dc07cdda70f.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b":"103775b5d2edfd3cd852","vendors-node_modules_react-bootstrap_esm_Button_j […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.0d4a29b3c23d232e97db.js",
+    "file": "remoteEntry.b4a869fd4dc07cdda70f.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,wfAAwf;WACthB;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-nbqueue/webpack/container-entry",
         "webpack://jupyterlab-nbqueue/webpack/bootstrap",
         "webpack://jupyterlab-nbqueue/webpack/runtime/compat get default export",
@@ -25,20 +25,20 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\":\"103775b5d2edfd3cd852\",\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\":\"766984a3c69834ca0c09\",\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\":\"7bdfa0f8f502c09ba050\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\":\"3970d5aff54335b54c0d\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\":\"103775b5d2edfd3cd852\",\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\":\"766984a3c69834ca0c09\",\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\":\"78207085ee8bf5d10cb1\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1\":\"3970d5aff54335b54c0d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-nbqueue:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-nbqueue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-nbqueue\", \"0.1.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-nbqueue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-nbqueue\", \"0.1.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b\"), __webpack_require__.e(\"vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093\"), __webpack_require__.e(\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,3])),\n\t\"webpack/sharing/consume/default/react-dom\": () => (loadSingletonVersionCheck(\"default\", \"react-dom\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,5,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react-dom\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-nbqueue\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_nbqueue\"] = self[\"webpackChunkjupyterlab_nbqueue\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-nbqueue\");\n",
         ""
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/remoteEntry.386184b399a7a26bbfe6.js` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/remoteEntry.b4a869fd4dc07cdda70f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -429,15 +429,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-nbqueue", "0.1.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b"), __webpack_require__.e("vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093"), __webpack_require__.e("lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-nbqueue", "0.1.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b"), __webpack_require__.e("vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093"), __webpack_require__.e("lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1099,8 +1099,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-nbqueue");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-nbqueue"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.386184b399a7a26bbfe6.js.map
+//# sourceMappingURL=remoteEntry.b4a869fd4dc07cdda70f.js.map
```

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map` & `jupyterlab_nbqueue-0.1.3/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990147783251232%*

 * *Differences: {"'sources'": '{insert: [(143, '*

 * *              "'webpack://jupyterlab-nbqueue/./node_modules/bootstrap/dist/css/bootstrap.min.css?2e79')], "*

 * *              'delete: [143]}'}*

```diff
@@ -143,15 +143,15 @@
         "webpack://jupyterlab-nbqueue/./node_modules/react/cjs/react-jsx-runtime.development.js",
         "webpack://jupyterlab-nbqueue/./node_modules/react/jsx-runtime.js",
         "webpack://jupyterlab-nbqueue/./node_modules/uncontrollable/lib/esm/hook.js",
         "webpack://jupyterlab-nbqueue/./node_modules/uncontrollable/lib/esm/index.js",
         "webpack://jupyterlab-nbqueue/./node_modules/uncontrollable/lib/esm/uncontrollable.js",
         "webpack://jupyterlab-nbqueue/./node_modules/uncontrollable/lib/esm/utils.js",
         "webpack://jupyterlab-nbqueue/./node_modules/warning/warning.js",
-        "webpack://jupyterlab-nbqueue/./node_modules/bootstrap/dist/css/bootstrap.min.css"
+        "webpack://jupyterlab-nbqueue/./node_modules/bootstrap/dist/css/bootstrap.min.css?2e79"
     ],
     "sourcesContent": [
         "var has = Object.prototype.hasOwnProperty;\n\nfunction find(iter, tar, key) {\n\tfor (key of iter.keys()) {\n\t\tif (dequal(key, tar)) return key;\n\t}\n}\n\nexport function dequal(foo, bar) {\n\tvar ctor, len, tmp;\n\tif (foo === bar) return true;\n\n\tif (foo && bar && (ctor=foo.constructor) === bar.constructor) {\n\t\tif (ctor === Date) return foo.getTime() === bar.getTime();\n\t\tif (ctor === RegExp) return foo.toString() === bar.toString();\n\n\t\tif (ctor === Array) {\n\t\t\tif ((len=foo.length) === bar.length) {\n\t\t\t\twhile (len-- && dequal(foo[len], bar[len]));\n\t\t\t}\n\t\t\treturn len === -1;\n\t\t}\n\n\t\tif (ctor === Set) {\n\t\t\tif (foo.size !== bar.size) {\n\t\t\t\treturn false;\n\t\t\t}\n\t\t\tfor (len of foo) {\n\t\t\t\ttmp = len;\n\t\t\t\tif (tmp && typeof tmp === 'object') {\n\t\t\t\t\ttmp = find(bar, tmp);\n\t\t\t\t\tif (!tmp) return false;\n\t\t\t\t}\n\t\t\t\tif (!bar.has(tmp)) return false;\n\t\t\t}\n\t\t\treturn true;\n\t\t}\n\n\t\tif (ctor === Map) {\n\t\t\tif (foo.size !== bar.size) {\n\t\t\t\treturn false;\n\t\t\t}\n\t\t\tfor (len of foo) {\n\t\t\t\ttmp = len[0];\n\t\t\t\tif (tmp && typeof tmp === 'object') {\n\t\t\t\t\ttmp = find(bar, tmp);\n\t\t\t\t\tif (!tmp) return false;\n\t\t\t\t}\n\t\t\t\tif (!dequal(len[1], bar.get(tmp))) {\n\t\t\t\t\treturn false;\n\t\t\t\t}\n\t\t\t}\n\t\t\treturn true;\n\t\t}\n\n\t\tif (ctor === ArrayBuffer) {\n\t\t\tfoo = new Uint8Array(foo);\n\t\t\tbar = new Uint8Array(bar);\n\t\t} else if (ctor === DataView) {\n\t\t\tif ((len=foo.byteLength) === bar.byteLength) {\n\t\t\t\twhile (len-- && foo.getInt8(len) === bar.getInt8(len));\n\t\t\t}\n\t\t\treturn len === -1;\n\t\t}\n\n\t\tif (ArrayBuffer.isView(foo)) {\n\t\t\tif ((len=foo.byteLength) === bar.byteLength) {\n\t\t\t\twhile (len-- && foo[len] === bar[len]);\n\t\t\t}\n\t\t\treturn len === -1;\n\t\t}\n\n\t\tif (!ctor || typeof foo === 'object') {\n\t\t\tlen = 0;\n\t\t\tfor (ctor in foo) {\n\t\t\t\tif (has.call(foo, ctor) && ++len && !has.call(bar, ctor)) return false;\n\t\t\t\tif (!(ctor in bar) || !dequal(foo[ctor], bar[ctor])) return false;\n\t\t\t}\n\t\t\treturn Object.keys(bar).length === len;\n\t\t}\n\t}\n\n\treturn foo !== foo && bar !== bar;\n}\n",
         "export default function _extends() {\n  _extends = Object.assign ? Object.assign.bind() : function (target) {\n    for (var i = 1; i < arguments.length; i++) {\n      var source = arguments[i];\n      for (var key in source) {\n        if (Object.prototype.hasOwnProperty.call(source, key)) {\n          target[key] = source[key];\n        }\n      }\n    }\n    return target;\n  };\n  return _extends.apply(this, arguments);\n}",
         "import setPrototypeOf from \"./setPrototypeOf.js\";\nexport default function _inheritsLoose(subClass, superClass) {\n  subClass.prototype = Object.create(superClass.prototype);\n  subClass.prototype.constructor = subClass;\n  setPrototypeOf(subClass, superClass);\n}",
         "export default function _objectWithoutPropertiesLoose(source, excluded) {\n  if (source == null) return {};\n  var target = {};\n  var sourceKeys = Object.keys(source);\n  var key, i;\n  for (i = 0; i < sourceKeys.length; i++) {\n    key = sourceKeys[i];\n    if (excluded.indexOf(key) >= 0) continue;\n    target[key] = source[key];\n  }\n  return target;\n}",
         "export default function _setPrototypeOf(o, p) {\n  _setPrototypeOf = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function _setPrototypeOf(o, p) {\n    o.__proto__ = p;\n    return o;\n  };\n  return _setPrototypeOf(o, p);\n}",
```

### Comparing `jupyterlab_nbqueue-0.1.2/src/handler.ts` & `jupyterlab_nbqueue-0.1.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/src/index.ts` & `jupyterlab_nbqueue-0.1.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/src/components/RunComponent.tsx` & `jupyterlab_nbqueue-0.1.3/src/components/RunComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/src/components/RunsContext.tsx` & `jupyterlab_nbqueue-0.1.3/src/components/RunsContext.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/src/components/RunsPanelComponent.tsx` & `jupyterlab_nbqueue-0.1.3/src/components/RunsPanelComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/src/widgets/RunsPanelWidget.tsx` & `jupyterlab_nbqueue-0.1.3/src/widgets/RunsPanelWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/nbqueue_logo_v1.svg` & `jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/nbqueue_logo_v2.svg` & `jupyterlab_nbqueue-0.1.3/style/nbqueue_logo_v2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/css/all.css` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/css/fontawesome.css` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/css/solid.css` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/js/fontawesome.js` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/js/pro.js` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/js/pro.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/js/solid.js` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.ttf` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/style/fontawesome/webfonts/fa-solid-900.woff2` & `jupyterlab_nbqueue-0.1.3/style/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/.gitignore` & `jupyterlab_nbqueue-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/LICENSE` & `jupyterlab_nbqueue-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/README.md` & `jupyterlab_nbqueue-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.2/pyproject.toml` & `jupyterlab_nbqueue-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=2.0.1,<3",
-    "sqlalchemy>=2.0.16,<3"
+    "jupyter_server>=2.0.1,<3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
```

### Comparing `jupyterlab_nbqueue-0.1.2/PKG-INFO` & `jupyterlab_nbqueue-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbqueue
-Version: 0.1.2
+Version: 0.1.3
 Summary: A JupyterLab extension for queuing notebooks executions.
 Project-URL: Homepage, https://github.com/Navteca/jupyterlab-nbqueue.git
 Project-URL: Bug Tracker, https://github.com/Navteca/jupyterlab-nbqueue.git/issues
 Project-URL: Repository, https://github.com/Navteca/jupyterlab-nbqueue.git.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
         
@@ -46,15 +46,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server<3,>=2.0.1
-Requires-Dist: sqlalchemy<3,>=2.0.16
 Description-Content-Type: text/markdown
 
 # jupyterlab_nbqueue
 
 [![Github Actions Status](https://github.com/Navteca/jupyterlab-nbqueue.git/workflows/Build/badge.svg)](https://github.com/Navteca/jupyterlab-nbqueue.git/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Navteca/jupyterlab-nbqueue.git/main?urlpath=lab)
 A JupyterLab extension for queuing notebooks executions.
```

