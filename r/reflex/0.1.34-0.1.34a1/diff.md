# Comparing `tmp/reflex-0.1.34.tar.gz` & `tmp/reflex-0.1.34a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.1.34.tar", max compression
+gzip compressed data, was "reflex-0.1.34a1.tar", max compression
```

## Comparing `reflex-0.1.34.tar` & `reflex-0.1.34a1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
--rw-r--r--   0        0        0    11354 2023-06-21 19:40:38.323768 reflex-0.1.34/LICENSE
--rw-r--r--   0        0        0     7927 2023-06-21 22:04:19.230985 reflex-0.1.34/README.md
--rw-r--r--   0        0        0     1856 2023-06-21 19:50:57.355046 reflex-0.1.34/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 19:39:18.143727 reflex-0.1.34/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1336 2023-06-21 19:49:49.379532 reflex-0.1.34/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-06-21 19:39:18.143865 reflex-0.1.34/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-06-21 19:49:49.378868 reflex-0.1.34/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-06-21 19:39:18.144027 reflex-0.1.34/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-06-21 19:49:49.379710 reflex-0.1.34/reflex/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-06-21 19:39:18.144299 reflex-0.1.34/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-06-21 19:39:18.144358 reflex-0.1.34/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-06-21 19:39:18.144413 reflex-0.1.34/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-06-21 19:39:18.144491 reflex-0.1.34/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-06-21 19:39:18.144554 reflex-0.1.34/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-06-21 19:39:18.144609 reflex-0.1.34/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-06-21 19:39:18.144720 reflex-0.1.34/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-06-21 19:39:18.144842 reflex-0.1.34/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-06-21 19:39:18.145610 reflex-0.1.34/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-06-21 19:39:18.145678 reflex-0.1.34/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2023-06-21 19:39:18.145739 reflex-0.1.34/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1141 2023-06-21 19:41:07.668788 reflex-0.1.34/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-06-21 19:39:18.146164 reflex-0.1.34/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-06-21 19:39:18.146237 reflex-0.1.34/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-06-21 19:39:18.146295 reflex-0.1.34/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-06-21 19:39:18.146513 reflex-0.1.34/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-06-21 19:39:18.146586 reflex-0.1.34/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     8836 2023-06-21 19:40:38.483055 reflex-0.1.34/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1634 2023-06-21 19:42:10.850987 reflex-0.1.34/reflex/__init__.py
--rw-r--r--   0        0        0      318 2023-06-21 19:40:38.443773 reflex-0.1.34/reflex/admin.py
--rw-r--r--   0        0        0    21877 2023-06-21 19:42:10.813549 reflex-0.1.34/reflex/app.py
--rw-r--r--   0        0        0     2544 2023-06-21 19:40:38.367059 reflex-0.1.34/reflex/base.py
--rw-r--r--   0        0        0       27 2023-06-21 19:40:38.482980 reflex-0.1.34/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     7317 2023-06-21 19:41:07.668731 reflex-0.1.34/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-06-21 19:41:07.668718 reflex-0.1.34/reflex/compiler/templates.py
--rw-r--r--   0        0        0     7751 2023-06-21 19:41:07.668710 reflex-0.1.34/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7471 2023-06-21 19:39:18.147409 reflex-0.1.34/reflex/components/__init__.py
--rw-r--r--   0        0        0      229 2023-06-21 19:39:18.147494 reflex-0.1.34/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-06-21 19:41:07.668963 reflex-0.1.34/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-06-21 19:41:07.669054 reflex-0.1.34/reflex/components/base/body.py
--rw-r--r--   0        0        0      721 2023-06-21 19:41:07.668989 reflex-0.1.34/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-06-21 19:41:07.669031 reflex-0.1.34/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-06-21 19:41:07.669017 reflex-0.1.34/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-06-21 19:41:07.668976 reflex-0.1.34/reflex/components/base/meta.py
--rw-r--r--   0        0        0    24223 2023-06-21 19:41:07.668808 reflex-0.1.34/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-06-21 19:39:18.148069 reflex-0.1.34/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-06-21 19:41:07.669332 reflex-0.1.34/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2503 2023-06-21 19:41:07.669264 reflex-0.1.34/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     4025 2023-06-21 19:41:07.669313 reflex-0.1.34/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-06-21 19:41:07.669295 reflex-0.1.34/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-06-21 19:41:07.669281 reflex-0.1.34/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-06-21 19:41:07.669365 reflex-0.1.34/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-06-21 19:41:07.669347 reflex-0.1.34/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5785 2023-06-21 19:41:07.669249 reflex-0.1.34/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-06-21 19:42:10.888870 reflex-0.1.34/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-06-21 19:39:18.148895 reflex-0.1.34/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-06-21 19:41:07.670209 reflex-0.1.34/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-06-21 19:41:07.670223 reflex-0.1.34/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-06-21 19:41:07.670268 reflex-0.1.34/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-06-21 19:41:07.670143 reflex-0.1.34/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-06-21 19:39:18.149333 reflex-0.1.34/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1565 2023-06-21 19:41:07.669466 reflex-0.1.34/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-06-21 19:41:07.669534 reflex-0.1.34/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-06-21 19:41:07.669520 reflex-0.1.34/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-06-21 19:41:07.669821 reflex-0.1.34/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-06-21 19:41:07.669478 reflex-0.1.34/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1471 2023-06-21 19:39:18.149718 reflex-0.1.34/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-21 19:41:07.670074 reflex-0.1.34/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-06-21 19:41:07.669880 reflex-0.1.34/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-06-21 19:42:10.907299 reflex-0.1.34/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-06-21 19:41:07.669953 reflex-0.1.34/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-06-21 19:41:07.670059 reflex-0.1.34/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-06-21 19:41:07.670000 reflex-0.1.34/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1943 2023-06-21 19:41:07.670090 reflex-0.1.34/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-06-21 19:41:07.669922 reflex-0.1.34/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-06-21 19:41:07.669937 reflex-0.1.34/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-06-21 19:41:07.670010 reflex-0.1.34/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2872 2023-06-21 19:41:07.670035 reflex-0.1.34/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-06-21 19:41:07.670023 reflex-0.1.34/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-06-21 19:41:07.670161 reflex-0.1.34/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-06-21 19:41:07.669890 reflex-0.1.34/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-06-21 19:41:07.669972 reflex-0.1.34/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-06-21 19:41:07.669857 reflex-0.1.34/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-06-21 19:41:07.669867 reflex-0.1.34/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-06-21 19:41:07.669835 reflex-0.1.34/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-06-21 19:41:07.669900 reflex-0.1.34/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-06-21 19:41:07.670173 reflex-0.1.34/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-06-21 19:41:07.670104 reflex-0.1.34/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-06-21 19:41:07.669986 reflex-0.1.34/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-06-21 19:39:18.151257 reflex-0.1.34/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-06-21 19:41:07.669169 reflex-0.1.34/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-06-21 19:41:07.669218 reflex-0.1.34/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-06-21 19:39:18.151506 reflex-0.1.34/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-06-21 19:41:07.669847 reflex-0.1.34/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-06-21 19:41:07.669800 reflex-0.1.34/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-06-21 19:41:07.669788 reflex-0.1.34/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-06-21 19:41:07.669715 reflex-0.1.34/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-06-21 19:41:07.669669 reflex-0.1.34/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-06-21 19:41:07.669703 reflex-0.1.34/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-06-21 19:41:07.669679 reflex-0.1.34/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-06-21 19:41:07.669758 reflex-0.1.34/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-06-21 19:41:07.669776 reflex-0.1.34/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-06-21 19:41:07.669742 reflex-0.1.34/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-06-21 19:41:07.669728 reflex-0.1.34/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-06-21 19:41:07.669657 reflex-0.1.34/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-06-21 19:41:07.669691 reflex-0.1.34/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-06-21 19:41:07.669646 reflex-0.1.34/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:42:10.888989 reflex-0.1.34/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-06-21 19:39:18.152449 reflex-0.1.34/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-06-21 19:41:07.669444 reflex-0.1.34/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-06-21 19:41:07.669431 reflex-0.1.34/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-21 19:39:18.152655 reflex-0.1.34/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-06-21 19:41:07.669005 reflex-0.1.34/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-06-21 19:41:07.669042 reflex-0.1.34/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-06-21 19:41:07.669084 reflex-0.1.34/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-06-21 19:41:07.669097 reflex-0.1.34/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-06-21 19:41:07.669068 reflex-0.1.34/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-21 19:39:18.153019 reflex-0.1.34/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-06-21 19:41:07.669597 reflex-0.1.34/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1606 2023-06-21 19:41:07.669582 reflex-0.1.34/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-06-21 19:41:07.669611 reflex-0.1.34/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-06-21 19:41:07.669545 reflex-0.1.34/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-06-21 19:41:07.669622 reflex-0.1.34/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-21 19:39:18.153386 reflex-0.1.34/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-06-21 19:41:07.668825 reflex-0.1.34/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-06-21 19:41:07.668846 reflex-0.1.34/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-06-21 19:41:07.668932 reflex-0.1.34/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-06-21 19:41:07.668948 reflex-0.1.34/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-06-21 19:41:07.669505 reflex-0.1.34/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-06-21 19:41:07.668836 reflex-0.1.34/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-06-21 19:41:07.668910 reflex-0.1.34/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-06-21 19:39:18.153921 reflex-0.1.34/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-06-21 19:41:07.669558 reflex-0.1.34/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2294 2023-06-21 19:41:07.669396 reflex-0.1.34/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-06-21 19:41:07.669382 reflex-0.1.34/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-06-21 19:41:07.669414 reflex-0.1.34/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-06-21 19:41:07.669137 reflex-0.1.34/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-06-21 19:41:07.669109 reflex-0.1.34/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-06-21 19:41:07.669124 reflex-0.1.34/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3454 2023-06-21 19:41:07.669153 reflex-0.1.34/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-06-21 19:41:07.669197 reflex-0.1.34/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-06-21 19:41:07.669180 reflex-0.1.34/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7120 2023-06-21 19:41:07.668697 reflex-0.1.34/reflex/config.py
--rw-r--r--   0        0        0    10404 2023-06-21 19:42:10.850909 reflex-0.1.34/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-06-21 19:39:18.154819 reflex-0.1.34/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-06-21 19:41:07.670407 reflex-0.1.34/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-06-21 19:39:18.154965 reflex-0.1.34/reflex/el/constants/html.py
--rw-r--r--   0        0        0     1701 2023-06-21 19:41:07.670396 reflex-0.1.34/reflex/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-06-21 19:39:18.155123 reflex-0.1.34/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1318 2023-06-21 19:41:07.670469 reflex-0.1.34/reflex/el/element.py
--rw-r--r--   0        0        0   108514 2023-06-21 19:41:07.670384 reflex-0.1.34/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2657 2023-06-21 19:41:07.670358 reflex-0.1.34/reflex/el/precompile.py
--rw-r--r--   0        0        0    11866 2023-06-21 19:41:07.668669 reflex-0.1.34/reflex/event.py
--rw-r--r--   0        0        0      111 2023-06-21 19:40:38.482930 reflex-0.1.34/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-06-21 19:41:07.670596 reflex-0.1.34/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-06-21 19:41:07.670487 reflex-0.1.34/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     2382 2023-06-21 19:41:07.668605 reflex-0.1.34/reflex/model.py
--rw-r--r--   0        0        0        0 2023-06-21 19:39:18.155926 reflex-0.1.34/reflex/py.typed
--rw-r--r--   0        0        0     8789 2023-06-21 19:41:54.530268 reflex-0.1.34/reflex/rf.py
--rw-r--r--   0        0        0     4104 2023-06-21 19:42:10.850975 reflex-0.1.34/reflex/route.py
--rw-r--r--   0        0        0    31405 2023-06-21 19:42:10.850962 reflex-0.1.34/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-06-21 19:41:07.668634 reflex-0.1.34/reflex/style.py
--rw-r--r--   0        0        0       24 2023-06-21 19:40:38.483103 reflex-0.1.34/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7849 2023-06-21 19:41:07.670304 reflex-0.1.34/reflex/utils/build.py
--rw-r--r--   0        0        0     1759 2023-06-21 19:39:18.156628 reflex-0.1.34/reflex/utils/console.py
--rw-r--r--   0        0        0     4785 2023-06-21 19:41:07.670343 reflex-0.1.34/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-06-21 19:42:10.888907 reflex-0.1.34/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-06-21 19:41:07.670254 reflex-0.1.34/reflex/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-06-21 19:39:18.156957 reflex-0.1.34/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    10881 2023-06-21 19:41:54.530389 reflex-0.1.34/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     3015 2023-06-21 19:41:07.670281 reflex-0.1.34/reflex/utils/processes.py
--rw-r--r--   0        0        0     2369 2023-06-21 19:41:07.670319 reflex-0.1.34/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-06-21 19:41:07.670193 reflex-0.1.34/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-06-21 19:41:07.670236 reflex-0.1.34/reflex/utils/watch.py
--rw-r--r--   0        0        0    30916 2023-06-21 19:41:07.668571 reflex-0.1.34/reflex/vars.py
--rw-r--r--   0        0        0     9551 1970-01-01 00:00:00.000000 reflex-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0    11354 2023-06-19 22:34:24.681273 reflex-0.1.34a1/LICENSE
+-rw-r--r--   0        0        0     7932 2023-06-19 22:36:51.179169 reflex-0.1.34a1/README.md
+-rw-r--r--   0        0        0     1859 2023-06-19 22:47:24.392655 reflex-0.1.34a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 22:33:46.770141 reflex-0.1.34a1/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-19 22:35:59.095973 reflex-0.1.34a1/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:33:46.770260 reflex-0.1.34a1/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-06-19 22:35:59.096017 reflex-0.1.34a1/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-06-19 22:33:46.770420 reflex-0.1.34a1/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-06-19 22:35:59.096045 reflex-0.1.34a1/reflex/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-06-19 22:33:46.770667 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-06-19 22:33:46.770722 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-06-19 22:33:46.770774 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-19 22:33:46.770836 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-06-19 22:33:46.770901 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-06-19 22:33:46.770962 reflex-0.1.34a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-06-19 22:33:46.771043 reflex-0.1.34a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-06-19 22:33:46.771125 reflex-0.1.34a1/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-06-19 22:33:46.771903 reflex-0.1.34a1/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-06-19 22:33:46.771990 reflex-0.1.34a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2023-06-19 22:33:46.772046 reflex-0.1.34a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1141 2023-06-19 22:35:59.096002 reflex-0.1.34a1/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-06-19 22:33:46.772194 reflex-0.1.34a1/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-06-19 22:33:46.772250 reflex-0.1.34a1/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-06-19 22:33:46.772306 reflex-0.1.34a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-06-19 22:33:46.772513 reflex-0.1.34a1/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-06-19 22:33:46.772579 reflex-0.1.34a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     8836 2023-06-19 22:34:24.888565 reflex-0.1.34a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1634 2023-06-19 22:34:24.831036 reflex-0.1.34a1/reflex/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-19 22:34:24.699927 reflex-0.1.34a1/reflex/admin.py
+-rw-r--r--   0        0        0    21877 2023-06-19 22:35:59.095850 reflex-0.1.34a1/reflex/app.py
+-rw-r--r--   0        0        0     2544 2023-06-19 22:34:24.719267 reflex-0.1.34a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-06-19 22:34:24.870104 reflex-0.1.34a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     7317 2023-06-19 22:35:59.095958 reflex-0.1.34a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-06-19 22:35:59.095943 reflex-0.1.34a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     7751 2023-06-19 22:35:59.095988 reflex-0.1.34a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7471 2023-06-19 22:33:46.773466 reflex-0.1.34a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-19 22:33:46.773564 reflex-0.1.34a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-19 22:35:59.096413 reflex-0.1.34a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-06-19 22:35:59.096444 reflex-0.1.34a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0      721 2023-06-19 22:35:59.096461 reflex-0.1.34a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-06-19 22:35:59.096397 reflex-0.1.34a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-06-19 22:35:59.096774 reflex-0.1.34a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-06-19 22:35:59.096367 reflex-0.1.34a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    24223 2023-06-19 22:35:59.096035 reflex-0.1.34a1/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-06-19 22:33:46.775571 reflex-0.1.34a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-19 22:35:59.096735 reflex-0.1.34a1/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2503 2023-06-19 22:35:59.096726 reflex-0.1.34a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-06-19 22:35:59.096802 reflex-0.1.34a1/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-06-19 22:35:59.096963 reflex-0.1.34a1/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-06-19 22:35:59.097170 reflex-0.1.34a1/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-06-19 22:35:59.096789 reflex-0.1.34a1/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-06-19 22:35:59.096813 reflex-0.1.34a1/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5785 2023-06-19 22:35:59.096689 reflex-0.1.34a1/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-06-19 22:35:59.096714 reflex-0.1.34a1/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-06-19 22:33:46.776227 reflex-0.1.34a1/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-06-19 22:35:59.097561 reflex-0.1.34a1/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-06-19 22:35:59.097606 reflex-0.1.34a1/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-06-19 22:35:59.097594 reflex-0.1.34a1/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-06-19 22:35:59.097898 reflex-0.1.34a1/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-06-19 22:33:46.776580 reflex-0.1.34a1/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1565 2023-06-19 22:35:59.096900 reflex-0.1.34a1/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-06-19 22:35:59.096909 reflex-0.1.34a1/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-06-19 22:35:59.096826 reflex-0.1.34a1/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-06-19 22:35:59.096882 reflex-0.1.34a1/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-06-19 22:35:59.096860 reflex-0.1.34a1/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1471 2023-06-19 22:33:46.776951 reflex-0.1.34a1/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-06-19 22:35:59.097156 reflex-0.1.34a1/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-06-19 22:35:59.096923 reflex-0.1.34a1/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-06-19 22:35:59.097250 reflex-0.1.34a1/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-06-19 22:35:59.097214 reflex-0.1.34a1/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-06-19 22:35:59.097099 reflex-0.1.34a1/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-06-19 22:35:59.097488 reflex-0.1.34a1/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1943 2023-06-19 22:35:59.097191 reflex-0.1.34a1/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-06-19 22:35:59.097108 reflex-0.1.34a1/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-06-19 22:35:59.097052 reflex-0.1.34a1/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-06-19 22:35:59.097201 reflex-0.1.34a1/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2872 2023-06-19 22:35:59.097131 reflex-0.1.34a1/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-06-19 22:35:59.097088 reflex-0.1.34a1/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-06-19 22:35:59.097001 reflex-0.1.34a1/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-06-19 22:35:59.097391 reflex-0.1.34a1/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-06-19 22:35:59.097118 reflex-0.1.34a1/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-06-19 22:35:59.097238 reflex-0.1.34a1/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-06-19 22:35:59.097071 reflex-0.1.34a1/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-06-19 22:35:59.097295 reflex-0.1.34a1/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-06-19 22:35:59.097039 reflex-0.1.34a1/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-06-19 22:35:59.097182 reflex-0.1.34a1/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-06-19 22:35:59.097226 reflex-0.1.34a1/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-06-19 22:35:59.097145 reflex-0.1.34a1/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-06-19 22:33:46.778441 reflex-0.1.34a1/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-06-19 22:35:59.096527 reflex-0.1.34a1/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-06-19 22:35:59.097946 reflex-0.1.34a1/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-06-19 22:33:46.778696 reflex-0.1.34a1/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-19 22:35:59.097415 reflex-0.1.34a1/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-06-19 22:35:59.097509 reflex-0.1.34a1/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-06-19 22:35:59.097305 reflex-0.1.34a1/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-06-19 22:35:59.097347 reflex-0.1.34a1/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-06-19 22:35:59.097704 reflex-0.1.34a1/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-06-19 22:35:59.097321 reflex-0.1.34a1/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-06-19 22:35:59.097277 reflex-0.1.34a1/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-06-19 22:35:59.097333 reflex-0.1.34a1/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-06-19 22:35:59.097526 reflex-0.1.34a1/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-06-19 22:35:59.097545 reflex-0.1.34a1/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-06-19 22:35:59.097451 reflex-0.1.34a1/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-06-19 22:35:59.097261 reflex-0.1.34a1/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-06-19 22:35:59.097576 reflex-0.1.34a1/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-06-19 22:35:59.097437 reflex-0.1.34a1/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-06-19 22:35:59.097268 reflex-0.1.34a1/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-06-19 22:33:46.779636 reflex-0.1.34a1/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-19 22:35:59.096477 reflex-0.1.34a1/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-06-19 22:35:59.096490 reflex-0.1.34a1/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-19 22:33:46.779841 reflex-0.1.34a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-19 22:35:59.096067 reflex-0.1.34a1/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-06-19 22:35:59.096077 reflex-0.1.34a1/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-06-19 22:35:59.096429 reflex-0.1.34a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-06-19 22:35:59.096054 reflex-0.1.34a1/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-06-19 22:35:59.096061 reflex-0.1.34a1/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-19 22:33:46.780197 reflex-0.1.34a1/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-06-19 22:35:59.096547 reflex-0.1.34a1/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1606 2023-06-19 22:35:59.096600 reflex-0.1.34a1/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-06-19 22:35:59.096566 reflex-0.1.34a1/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-06-19 22:35:59.096616 reflex-0.1.34a1/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-06-19 22:35:59.096580 reflex-0.1.34a1/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-19 22:33:46.780630 reflex-0.1.34a1/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-06-19 22:35:59.096337 reflex-0.1.34a1/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-06-19 22:35:59.096326 reflex-0.1.34a1/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-06-19 22:35:59.096353 reflex-0.1.34a1/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-06-19 22:35:59.096282 reflex-0.1.34a1/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-06-19 22:35:59.096302 reflex-0.1.34a1/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-06-19 22:35:59.096382 reflex-0.1.34a1/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-06-19 22:35:59.096313 reflex-0.1.34a1/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-06-19 22:33:46.781218 reflex-0.1.34a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-06-19 22:35:59.096675 reflex-0.1.34a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2294 2023-06-19 22:35:59.096659 reflex-0.1.34a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-06-19 22:35:59.096643 reflex-0.1.34a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-06-19 22:35:59.096705 reflex-0.1.34a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-06-19 22:35:59.096266 reflex-0.1.34a1/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-19 22:35:59.096084 reflex-0.1.34a1/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-06-19 22:35:59.096228 reflex-0.1.34a1/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3454 2023-06-19 22:35:59.096099 reflex-0.1.34a1/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-06-19 22:35:59.096238 reflex-0.1.34a1/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-06-19 22:35:59.096249 reflex-0.1.34a1/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7120 2023-06-19 22:35:59.095927 reflex-0.1.34a1/reflex/config.py
+-rw-r--r--   0        0        0    10382 2023-06-19 22:36:51.202098 reflex-0.1.34a1/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-06-19 22:33:46.782066 reflex-0.1.34a1/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-19 22:35:59.097790 reflex-0.1.34a1/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-06-19 22:33:46.782213 reflex-0.1.34a1/reflex/el/constants/html.py
+-rw-r--r--   0        0        0     1701 2023-06-19 22:35:59.097774 reflex-0.1.34a1/reflex/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-06-19 22:33:46.782376 reflex-0.1.34a1/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1318 2023-06-19 22:35:59.097806 reflex-0.1.34a1/reflex/el/element.py
+-rw-r--r--   0        0        0   108514 2023-06-19 22:35:59.097834 reflex-0.1.34a1/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2657 2023-06-19 22:35:59.097738 reflex-0.1.34a1/reflex/el/precompile.py
+-rw-r--r--   0        0        0    11866 2023-06-19 22:35:59.095898 reflex-0.1.34a1/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-06-19 22:34:24.888652 reflex-0.1.34a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-06-19 22:35:59.097851 reflex-0.1.34a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-06-19 22:35:59.097863 reflex-0.1.34a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     2382 2023-06-19 22:35:59.095833 reflex-0.1.34a1/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:33:46.783154 reflex-0.1.34a1/reflex/py.typed
+-rw-r--r--   0        0        0     4104 2023-06-19 22:35:59.095862 reflex-0.1.34a1/reflex/route.py
+-rw-r--r--   0        0        0     8549 2023-06-19 22:36:51.179201 reflex-0.1.34a1/reflex/rx.py
+-rw-r--r--   0        0        0    30933 2023-06-19 22:35:59.095822 reflex-0.1.34a1/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-06-19 22:35:59.095871 reflex-0.1.34a1/reflex/style.py
+-rw-r--r--   0        0        0       24 2023-06-19 22:34:24.870062 reflex-0.1.34a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7378 2023-06-19 22:35:59.097756 reflex-0.1.34a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-06-19 22:33:46.783773 reflex-0.1.34a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     5305 2023-06-19 22:35:59.098892 reflex-0.1.34a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-06-19 22:35:59.097652 reflex-0.1.34a1/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-06-19 22:35:59.097721 reflex-0.1.34a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-06-19 22:33:46.784040 reflex-0.1.34a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    10881 2023-06-19 22:36:51.202382 reflex-0.1.34a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     3015 2023-06-19 22:35:59.097617 reflex-0.1.34a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2369 2023-06-19 22:35:59.097638 reflex-0.1.34a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-06-19 22:35:59.097667 reflex-0.1.34a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-06-19 22:35:59.097626 reflex-0.1.34a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    30916 2023-06-19 22:35:59.095790 reflex-0.1.34a1/reflex/vars.py
+-rw-r--r--   0        0        0     9559 1970-01-01 00:00:00.000000 reflex-0.1.34a1/PKG-INFO
```

### Comparing `reflex-0.1.34/LICENSE` & `reflex-0.1.34a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/README.md` & `reflex-0.1.34a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <hr>
 
 **✨ Performant, customizable web apps in pure Python. Deploy in seconds.**
 
 📑 [Docs](https://reflex.dev/docs/getting-started/introduction) &nbsp; 📱 [Component Library](https://reflex.dev/docs/library) &nbsp; 🖼️ [Gallery](https://reflex.dev/docs/gallery) &nbsp; 🛸 [Deployment](https://reflex.dev/docs/hosting/deploy)
 
 [![PyPI version](https://badge.fury.io/py/reflex.svg)](https://badge.fury.io/py/reflex)
-![tests](https://github.com/reflex-io/reflex/actions/workflows/build.yml/badge.svg)
+![tests](https://github.com/reflex-dev/reflex/actions/workflows/build.yml/badge.svg)
 ![versions](https://img.shields.io/pypi/pyversions/reflex-io.svg)
 [![Discord](https://img.shields.io/discord/1029853095527727165?color=%237289da&label=Discord)](https://discord.gg/T5WSbC2YtQ)
 
 </div>
 
 ### README in different language
 
@@ -38,27 +38,27 @@
 Installing Reflex also installs the `pc` command line tool. Test that the install was successful by creating a new project.
 
 Replace my_app_name with your project name:
 
 ```
 mkdir my_app_name
 cd my_app_name
-pc init
+rx init
 ```
 
 When you run this command for the first time, we will download and install [bun](https://bun.sh/) automatically.
 
 This command initializes a template app in your new directory.
 
 ## 🏃 3. Run
 
 You can run this app in development mode:
 
 ```
-pc run
+rx run
 ```
 
 You should see your app running at http://localhost:3000.
 
 Now you can modify the source code in `my_app_name/my_app_name.py`. Reflex has fast refreshes so you can see your changes instantly when you save your code.
 
 ## 🫧 Example
@@ -131,15 +131,15 @@
         width="100%",
         height="100vh",
         bg="radial-gradient(circle at 22% 11%,rgba(62, 180, 137,.20),hsla(0,0%,100%,0) 19%)",
     )
 
 # Add state and page to the app.
 app = pc.App(state=State)
-app.add_page(index, title="rx:DALL·E")
+app.add_page(index, title="Reflex:DALL·E")
 app.compile()
 ```
 
 Let's break this down.
 
 ### **UI In Reflex**
```

### Comparing `reflex-0.1.34/pyproject.toml` & `reflex-0.1.34a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "reflex"
-version = "0.1.34"
+version = "0.1.34a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
 ]
 readme = "README.md"
 homepage = "https://reflex.dev"
-repository = "https://github.com/reflex-io/reflex"
+repository = "https://github.com/reflex-dev/reflex"
 documentation = "https://reflex.dev/docs/getting-started/introduction"
 keywords = [
     "web",
     "framework",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -58,15 +58,15 @@
     {version = "^1.5.3", python = ">=3.8,<4.0"},
     {version = "^1.1", python = ">=3.7, <3.8"}
 ]
 asynctest = "^0.13.0"
 pre-commit = {version = "^3.2.1", python = ">=3.8,<4.0"}
 
 [tool.poetry.scripts]
-rf = "reflex.rf:main"
+rx = "reflex.rx:main"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
```

### Comparing `reflex-0.1.34/reflex/.templates/apps/counter/counter.py` & `reflex-0.1.34a1/reflex/.templates/apps/counter/counter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Welcome to Reflex! This file create a counter app."""
 import random
 
-import reflex as rf
+import reflex as pc
 
 
-class State(rf.State):
+class State(pc.State):
     """The app state."""
 
     count = 0
 
     def increment(self):
         """Increment the count."""
         self.count += 1
@@ -18,36 +18,36 @@
         self.count -= 1
 
     def random(self):
         """Randomize the count."""
         self.count = random.randint(0, 100)
 
 
-def index() -> rf.Component:
-    return rf.center(
-        rf.vstack(
-            rf.heading(State.count),
-            rf.hstack(
-                rf.button("Decrement", on_click=State.decrement, color_scheme="red"),
-                rf.button(
+def index() -> pc.Component:
+    return pc.center(
+        pc.vstack(
+            pc.heading(State.count),
+            pc.hstack(
+                pc.button("Decrement", on_click=State.decrement, color_scheme="red"),
+                pc.button(
                     "Randomize",
                     on_click=State.random,
                     background_image="linear-gradient(90deg, rgba(255,0,0,1) 0%, rgba(0,176,34,1) 100%)",
                     color="white",
                 ),
-                rf.button("Increment", on_click=State.increment, color_scheme="green"),
+                pc.button("Increment", on_click=State.increment, color_scheme="green"),
             ),
             padding="1em",
             bg="#ededed",
             border_radius="1em",
             box_shadow="lg",
         ),
         padding_y="5em",
         font_size="2em",
         text_align="center",
     )
 
 
 # Add state and page to the app.
-app = rf.App(state=State)
+app = pc.App(state=State)
 app.add_page(index, title="Counter")
 app.compile()
```

### Comparing `reflex-0.1.34/reflex/.templates/apps/default/default.py` & `reflex-0.1.34a1/reflex/.templates/apps/default/default.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Welcome to Reflex! This file outlines the steps to create a basic app."""
 from pcconfig import config
 
-import reflex as rf
+import reflex as pc
 
 docs_url = "https://reflex.dev/docs/getting-started/introduction"
 filename = f"{config.app_name}/{config.app_name}.py"
 
 
-class State(rf.State):
+class State(pc.State):
     """The app state."""
 
     pass
 
 
-def index() -> rf.Component:
-    return rf.fragment(
-        rf.color_mode_button(rf.color_mode_icon(), float="right"),
-        rf.vstack(
-            rf.heading("Welcome to Reflex!", font_size="2em"),
-            rf.box("Get started by editing ", rf.code(filename, font_size="1em")),
-            rf.link(
+def index() -> pc.Component:
+    return pc.fragment(
+        pc.color_mode_button(pc.color_mode_icon(), float="right"),
+        pc.vstack(
+            pc.heading("Welcome to Reflex!", font_size="2em"),
+            pc.box("Get started by editing ", pc.code(filename, font_size="1em")),
+            pc.link(
                 "Check out our docs!",
                 href=docs_url,
                 border="0.1em solid",
                 padding="0.5em",
                 border_radius="0.5em",
                 _hover={
-                    "color": rf.color_mode_cond(
+                    "color": pc.color_mode_cond(
                         light="rgb(107,99,246)",
                         dark="rgb(179, 175, 255)",
                     )
                 },
             ),
             spacing="1.5em",
             font_size="2em",
             padding_top="10%",
         ),
     )
 
 
 # Add state and page to the app.
-app = rf.App(state=State)
+app = pc.App(state=State)
 app.add_page(index)
 app.compile()
```

### Comparing `reflex-0.1.34/reflex/.templates/assets/favicon.ico` & `reflex-0.1.34a1/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.1.34a1/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.1.34a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/web/bun.lockb` & `reflex-0.1.34a1/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/web/package.json` & `reflex-0.1.34a1/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/web/pages/_app.js` & `reflex-0.1.34a1/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/web/styles/code/prism.js` & `reflex-0.1.34a1/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/.templates/web/utils/state.js` & `reflex-0.1.34a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/__init__.py` & `reflex-0.1.34a1/reflex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Import all classes and functions the end user will need to make an app.
 
-Anything imported here will be available in the default Reflex import as `rf.*`.
+Anything imported here will be available in the default Reflex import as `pc.*`.
 To signal to typecheckers that something should be reexported, 
 we use the Flask "import name as name" syntax.
 """
 
 from . import el as el
 from .admin import AdminDash as AdminDash
 from .app import App as App
```

### Comparing `reflex-0.1.34/reflex/app.py` & `reflex-0.1.34a1/reflex/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
             ):
                 handler_upload_param = (k, v)
                 break
 
         if not handler_upload_param:
             raise ValueError(
                 f"`{handler}` handler should have a parameter annotated as List["
-                f"rf.UploadFile]"
+                f"pc.UploadFile]"
             )
 
         event = Event(
             token=token,
             name=handler,
             payload={handler_upload_param[0]: files},
         )
```

### Comparing `reflex-0.1.34/reflex/base.py` & `reflex-0.1.34a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/compiler/compiler.py` & `reflex-0.1.34a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/compiler/templates.py` & `reflex-0.1.34a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/compiler/utils.py` & `reflex-0.1.34a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/__init__.py` & `reflex-0.1.34a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/base/bare.py` & `reflex-0.1.34a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/base/document.py` & `reflex-0.1.34a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/base/link.py` & `reflex-0.1.34a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/base/meta.py` & `reflex-0.1.34a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/component.py` & `reflex-0.1.34a1/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/code.py` & `reflex-0.1.34a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/datatable.py` & `reflex-0.1.34a1/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/divider.py` & `reflex-0.1.34a1/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/list.py` & `reflex-0.1.34a1/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/stat.py` & `reflex-0.1.34a1/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/table.py` & `reflex-0.1.34a1/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/datadisplay/tag.py` & `reflex-0.1.34a1/reflex/components/datadisplay/tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         close_button: Optional[Component] = None,
         **props
     ) -> Component:
         """Creates a Chakra Tag with a label and optionally left_icon, right_icon, and close_button, and returns it.
 
         Args:
             label (Component): The label of the Tag that will be created.
-            left_icon (Optional[Component]): Should be a rf.TagLeftIcon instance.
-            right_icon (Optional[Component]): Should be a rf.TagRightIcon instance.
-            close_button (Optional[Component]): Should be a rf.TagCloseButton instance.
+            left_icon (Optional[Component]): Should be a pc.TagLeftIcon instance.
+            right_icon (Optional[Component]): Should be a pc.TagRightIcon instance.
+            close_button (Optional[Component]): Should be a pc.TagCloseButton instance.
             props: The properties to be passed to the component.
 
         Returns:
             The `create()` method returns a Tag object.
         """
         children = [
             x for x in (left_icon, label, right_icon, close_button) if x is not None
```

### Comparing `reflex-0.1.34/reflex/components/disclosure/accordion.py` & `reflex-0.1.34a1/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/disclosure/tabs.py` & `reflex-0.1.34a1/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/disclosure/transition.py` & `reflex-0.1.34a1/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/feedback/alert.py` & `reflex-0.1.34a1/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/feedback/circularprogress.py` & `reflex-0.1.34a1/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/feedback/progress.py` & `reflex-0.1.34a1/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/feedback/skeleton.py` & `reflex-0.1.34a1/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/feedback/spinner.py` & `reflex-0.1.34a1/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/__init__.py` & `reflex-0.1.34a1/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/button.py` & `reflex-0.1.34a1/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/checkbox.py` & `reflex-0.1.34a1/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/colormodeswitch.py` & `reflex-0.1.34a1/reflex/components/forms/colormodeswitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """A switch component for toggling color_mode.
 
 To style components based on color mode, use style props with `color_mode_cond`:
 
 ```
-rf.text(
+pc.text(
     "Hover over me",
     _hover={
-        "background": rf.color_mode_cond(
+        "background": pc.color_mode_cond(
             light="var(--chakra-colors-gray-200)",
             dark="var(--chakra-colors-gray-700)",
         ),
     },
 )
 ```
 """
```

### Comparing `reflex-0.1.34/reflex/components/forms/copytoclipboard.py` & `reflex-0.1.34a1/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/editable.py` & `reflex-0.1.34a1/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/form.py` & `reflex-0.1.34a1/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/iconbutton.py` & `reflex-0.1.34a1/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/input.py` & `reflex-0.1.34a1/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/multiselect.py` & `reflex-0.1.34a1/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/numberinput.py` & `reflex-0.1.34a1/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/pininput.py` & `reflex-0.1.34a1/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/radio.py` & `reflex-0.1.34a1/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/rangeslider.py` & `reflex-0.1.34a1/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/select.py` & `reflex-0.1.34a1/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/slider.py` & `reflex-0.1.34a1/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/switch.py` & `reflex-0.1.34a1/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/textarea.py` & `reflex-0.1.34a1/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/forms/upload.py` & `reflex-0.1.34a1/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/graphing/plotly.py` & `reflex-0.1.34a1/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/graphing/victory.py` & `reflex-0.1.34a1/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/__init__.py` & `reflex-0.1.34a1/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/box.py` & `reflex-0.1.34a1/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/card.py` & `reflex-0.1.34a1/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/cond.py` & `reflex-0.1.34a1/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/flex.py` & `reflex-0.1.34a1/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/foreach.py` & `reflex-0.1.34a1/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/grid.py` & `reflex-0.1.34a1/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/html.py` & `reflex-0.1.34a1/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/responsive.py` & `reflex-0.1.34a1/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/stack.py` & `reflex-0.1.34a1/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/layout/wrap.py` & `reflex-0.1.34a1/reflex/components/layout/wrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # The flex direction of the wrap.
     direction: Var[str]
 
     # How to justify the items.
     justify: Var[str]
 
-    # Whether to wrap children in `rf.wrap_item`.
+    # Whether to wrap children in `pc.wrap_item`.
     should_wrap_children: Var[bool]
 
     # The spacing between the items.
     spacing: Var[str]
 
     # The horizontal spacing between the items.
     spacing_x: Var[str]
```

### Comparing `reflex-0.1.34/reflex/components/libs/react_player.py` & `reflex-0.1.34a1/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/media/avatar.py` & `reflex-0.1.34a1/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/media/icon.py` & `reflex-0.1.34a1/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/media/image.py` & `reflex-0.1.34a1/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/navigation/breadcrumb.py` & `reflex-0.1.34a1/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/navigation/link.py` & `reflex-0.1.34a1/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/navigation/linkoverlay.py` & `reflex-0.1.34a1/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/navigation/stepper.py` & `reflex-0.1.34a1/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/__init__.py` & `reflex-0.1.34a1/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/alertdialog.py` & `reflex-0.1.34a1/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/banner.py` & `reflex-0.1.34a1/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/drawer.py` & `reflex-0.1.34a1/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/menu.py` & `reflex-0.1.34a1/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/modal.py` & `reflex-0.1.34a1/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/popover.py` & `reflex-0.1.34a1/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/overlay/tooltip.py` & `reflex-0.1.34a1/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/tags/iter_tag.py` & `reflex-0.1.34a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/tags/tag.py` & `reflex-0.1.34a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/tags/tagless.py` & `reflex-0.1.34a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/typography/highlight.py` & `reflex-0.1.34a1/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/components/typography/markdown.py` & `reflex-0.1.34a1/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/config.py` & `reflex-0.1.34a1/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/constants.py` & `reflex-0.1.34a1/reflex/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 MAX_BUN_VERSION = "0.6.9"
 
 # Files and directories used to init a new project.
 # The root directory of the reflex library.
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # The name of the assets directory.
 APP_ASSETS_DIR = "assets"
-# The template directory used during rf init.
+# The template directory used during rx init.
 TEMPLATE_DIR = os.path.join(ROOT_DIR, MODULE_NAME, ".templates")
 # The web subdirectory of the template directory.
 WEB_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "web")
 # The assets subdirectory of the template directory.
 ASSETS_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, APP_ASSETS_DIR)
 # The jinja template directory.
 JINJA_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "jinja")
@@ -119,15 +119,15 @@
 PING_TIMEOUT = 120
 
 # Compiler variables.
 # The extension for compiled Javascript files.
 JS_EXT = ".js"
 # The extension for python files.
 PY_EXT = ".py"
-# The expected variable name where the rf.App is stored.
+# The expected variable name where the pc.App is stored.
 APP_VAR = "app"
 # The expected variable name where the API object is stored for deployment.
 API_VAR = "api"
 # The name of the router variable.
 ROUTER = "router"
 # The name of the socket variable.
 SOCKET = "socket"
@@ -312,15 +312,14 @@
 
     CLIENT_IP = "ip"
     CLIENT_TOKEN = "token"
     HEADERS = "headers"
     PATH = "pathname"
     SESSION_ID = "sid"
     QUERY = "query"
-    COOKIE = "cookie"
 
 
 class RouteRegex(SimpleNamespace):
     """Regex used for extracting route args in route."""
 
     ARG = re.compile(r"\[(?!\.)([^\[\]]+)\]")
     # group return the catchall pattern (i.e. "[[..slug]]")
```

### Comparing `reflex-0.1.34/reflex/el/constants/html.py` & `reflex-0.1.34a1/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/el/constants/pynecone.py` & `reflex-0.1.34a1/reflex/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/el/constants/react.py` & `reflex-0.1.34a1/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/el/element.py` & `reflex-0.1.34a1/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/el/elements/__init__.py` & `reflex-0.1.34a1/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/el/precompile.py` & `reflex-0.1.34a1/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/event.py` & `reflex-0.1.34a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/middleware/hydrate_middleware.py` & `reflex-0.1.34a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/middleware/middleware.py` & `reflex-0.1.34a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/model.py` & `reflex-0.1.34a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/rf.py` & `reflex-0.1.34a1/reflex/rx.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,63 +106,53 @@
 
     if backend and processes.is_process_on_port(backend_port):
         backend_port = processes.change_or_terminate_port(backend_port, "backend")
 
     # Check that the app is initialized.
     if frontend and not prerequisites.is_initialized():
         console.print(
-            "[red]The app is not initialized. Run [bold]rf init[/bold] first."
+            "[red]The app is not initialized. Run [bold]rx init[/bold] first."
         )
         raise typer.Exit()
 
     # Check that the template is up to date.
     if frontend and not prerequisites.is_latest_template():
         console.print(
-            "[red]The base app template has updated. Run [bold]rf init[/bold] again."
+            "[red]The base app template has updated. Run [bold]rx init[/bold] again."
         )
         raise typer.Exit()
 
     # Get the app module.
     console.rule("[bold]Starting Reflex App")
     app = prerequisites.get_app()
 
     # Check the admin dashboard settings.
     prerequisites.check_admin_settings()
 
     # Get the frontend and backend commands, based on the environment.
-    setup_frontend = frontend_cmd = backend_cmd = None
+    frontend_cmd = backend_cmd = None
     if env == constants.Env.DEV:
-        setup_frontend, frontend_cmd, backend_cmd = (
-            build.setup_frontend,
-            exec.run_frontend,
-            exec.run_backend,
-        )
+        frontend_cmd, backend_cmd = exec.run_frontend, exec.run_backend
     if env == constants.Env.PROD:
-        setup_frontend, frontend_cmd, backend_cmd = (
-            build.setup_frontend_prod,
-            exec.run_frontend_prod,
-            exec.run_backend_prod,
-        )
-    assert setup_frontend and frontend_cmd and backend_cmd, "Invalid env"
+        frontend_cmd, backend_cmd = exec.run_frontend_prod, exec.run_backend_prod
+    assert frontend_cmd and backend_cmd, "Invalid env"
 
     # Post a telemetry event.
     telemetry.send(f"run-{env.value}", get_config().telemetry_enabled)
 
     # Run the frontend and backend.
-    if frontend:
-        setup_frontend(Path.cwd(), loglevel)
-        threading.Thread(
-            target=frontend_cmd, args=(Path.cwd(), frontend_port, loglevel)
-        ).start()
     if backend:
-        build.setup_backend()
         threading.Thread(
             target=backend_cmd,
             args=(app.__name__, backend_host, backend_port, loglevel),
         ).start()
+    if frontend:
+        threading.Thread(
+            target=frontend_cmd, args=(app.app, Path.cwd(), frontend_port)
+        ).start()
 
 
 @cli.command()
 def deploy(dry_run: bool = typer.Option(False, help="Whether to run a dry run.")):
     """Deploy the app to the Reflex hosting service."""
     # Get the app config.
     config = get_config()
@@ -223,15 +213,17 @@
 
     # Compile the app in production mode and export it.
     console.rule("[bold]Compiling production app and preparing for export.")
 
     if frontend:
         build.setup_frontend(Path.cwd())
 
+    app = prerequisites.get_app().app
     build.export_app(
+        app,
         backend=backend,
         frontend=frontend,
         zip=zipping,
         deploy_url=config.deploy_url,
     )
 
     # Post a telemetry event.
```

### Comparing `reflex-0.1.34/reflex/route.py` & `reflex-0.1.34a1/reflex/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     title: Optional[str] = None,
     image: Optional[str] = None,
     description: Optional[str] = None,
     on_load: Optional[Union[EventHandler, List[EventHandler]]] = None,
 ):
     """Decorate a function as a page.
 
-    rf.App() will automatically call add_page() for any method decorated with route
+    pc.App() will automatically call add_page() for any method decorated with route
     when App.compile is called.
 
     All defaults are None because they will use the one from add_page().
 
     Note: the decorated functions still need to be imported.
 
     Args:
```

### Comparing `reflex-0.1.34/reflex/state.py` & `reflex-0.1.34a1/reflex/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         Raises:
             TypeError: if the variable has an incorrect type
         """
         if not types.is_valid_var_type(prop.type_):
             raise TypeError(
                 "State vars must be primitive Python types, "
                 "Plotly figures, Pandas dataframes, "
-                "or subclasses of rf.Base. "
+                "or subclasses of pc.Base. "
                 f'Found var "{prop.name}" with type {prop.type_}.'
             )
         cls._set_var(prop)
         cls._create_setter(prop)
         cls._set_default_value(prop)
 
     @classmethod
@@ -486,30 +486,14 @@
         The query object contains both the URI parameters and the GET parameters.
 
         Returns:
             The dict of query parameters.
         """
         return self.router_data.get(constants.RouteVar.QUERY, {})
 
-    def get_cookies(self) -> Dict[str, str]:
-        """Obtain the cookies of the client stored in the browser.
-
-        Returns:
-                The dict of cookies.
-        """
-        headers = self.get_headers().get(constants.RouteVar.COOKIE)
-        return (
-            {
-                pair[0].strip(): pair[1].strip()
-                for pair in (item.split("=") for item in headers.split(";"))
-            }
-            if headers
-            else {}
-        )
-
     @classmethod
     def setup_dynamic_args(cls, args: dict[str, str]):
         """Set up args for easy access in renderer.
 
         Args:
             args: a dict of args
         """
```

### Comparing `reflex-0.1.34/reflex/style.py` & `reflex-0.1.34a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/build.py` & `reflex-0.1.34a1/reflex/utils/build.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 from __future__ import annotations
 
 import json
 import os
 import random
 import subprocess
 from pathlib import Path
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from rich.progress import Progress
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import path_ops, prerequisites
 
+if TYPE_CHECKING:
+    from reflex.app import App
+
 
 def update_json_file(file_path: str, update_dict: dict[str, Union[int, str]]):
     """Update the contents of a json file.
 
     Args:
         file_path: the path to the JSON file.
         update_dict: object to update json.
@@ -84,23 +87,25 @@
     )
 
     with open(constants.SITEMAP_CONFIG_FILE, "w") as f:
         f.write(templates.SITEMAP_CONFIG(config=config))
 
 
 def export_app(
+    app: App,
     backend: bool = True,
     frontend: bool = True,
     zip: bool = False,
     deploy_url: Optional[str] = None,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Zip up the app for deployment.
 
     Args:
+        app: The app.
         backend: Whether to zip up the backend app.
         frontend: Whether to zip up the frontend app.
         zip: Whether to zip the app.
         deploy_url: The URL of the deployed app.
         loglevel: The log level to use.
     """
     # Remove the static folder.
@@ -112,42 +117,45 @@
 
     # Create a progress object
     progress = Progress()
 
     # Add a single task to the progress object
     task = progress.add_task("Building app... ", total=500)
 
-    # Start the subprocess with the progress bar.
-    with progress, subprocess.Popen(
-        [prerequisites.get_package_manager(), "run", "export"],
-        cwd=constants.WEB_DIR,
-        env=os.environ,
-        stderr=subprocess.STDOUT,
-        stdout=subprocess.PIPE,  # Redirect stdout to a pipe
-        universal_newlines=True,  # Set universal_newlines to True for text mode
-    ) as export_process:
-        assert export_process.stdout is not None, "No stdout for export process."
-        for line in export_process.stdout:
-            # Print the line in debug mode.
-            if loglevel == constants.LogLevel.DEBUG:
-                print(line, end="")
-
-            # Check for special strings and update the progress bar.
-            if "Linting and checking " in line:
-                progress.update(task, advance=100)
-            elif "Compiled successfully" in line:
-                progress.update(task, advance=100)
-            elif "Route (pages)" in line:
-                progress.update(task, advance=100)
-            elif "automatically rendered as static HTML" in line:
-                progress.update(task, advance=100)
-            elif "Export successful" in line:
-                progress.update(task, completed=500)
-                break  # Exit the loop if the completion message is found
+    # Start the progress bar
+    with progress:
+        # Run the subprocess command
+        export_process = subprocess.Popen(
+            [prerequisites.get_package_manager(), "run", "export"],
+            cwd=constants.WEB_DIR,
+            env=os.environ,
+            stderr=subprocess.STDOUT,
+            stdout=subprocess.PIPE,  # Redirect stdout to a pipe
+            universal_newlines=True,  # Set universal_newlines to True for text mode
+        )
+
+        if export_process.stdout:
+            for line in iter(export_process.stdout.readline, ""):
+                if "Linting and checking " in line:
+                    progress.update(task, advance=100)
+                elif "Compiled successfully" in line:
+                    progress.update(task, advance=100)
+                elif "Route (pages)" in line:
+                    progress.update(task, advance=100)
+                elif "automatically rendered as static HTML" in line:
+                    progress.update(task, advance=100)
+                elif "Export successful" in line:
+                    print("DOOE")
+                    progress.update(task, completed=500)
+                    break  # Exit the loop if the completion message is found
+                elif loglevel == constants.LogLevel.DEBUG:
+                    print(line, end="")
 
+        # Wait for the subprocess to complete
+        export_process.wait()
         print("Export process completed.")
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
@@ -182,29 +190,21 @@
         cmd = r"cd .web/_static && zip -r ../../frontend.zip ./*"
         os.system(cmd)
     if backend:
         cmd = r"zip -r backend.zip ./* -x .web/\* ./assets\* ./frontend.zip\* ./backend.zip\*"
         os.system(cmd)
 
 
-def setup_frontend(
-    root: Path,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
-    disable_telemetry: bool = True,
-):
+def setup_frontend(root: Path, disable_telemetry: bool = True):
     """Set up the frontend.
 
     Args:
-        root: The root path of the project.
-        loglevel: The log level to use.
+        root: root path of the project.
         disable_telemetry: Whether to disable the Next telemetry.
     """
-    # Validate bun version.
-    prerequisites.validate_and_install_bun(initialize=False)
-
     # Initialize the web directory if it doesn't exist.
     web_dir = prerequisites.create_web_directory(root)
 
     # Install frontend packages.
     prerequisites.install_frontend_packages(web_dir)
 
     # Copy asset files to public folder.
@@ -229,30 +229,14 @@
             cwd=constants.WEB_DIR,
             env=os.environ,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.STDOUT,
         )
 
 
-def setup_frontend_prod(
-    root: Path,
-    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
-    disable_telemetry: bool = True,
-):
-    """Set up the frontend for prod mode.
-
-    Args:
-        root: The root path of the project.
-        loglevel: The log level to use.
-        disable_telemetry: Whether to disable the Next telemetry.
-    """
-    setup_frontend(root, loglevel, disable_telemetry)
-    export_app(loglevel=loglevel)
-
-
 def setup_backend():
     """Set up backend.
 
     Specifically ensures backend database is updated when running --no-frontend.
     """
     # Import here to avoid circular imports.
     from reflex.model import Model
```

### Comparing `reflex-0.1.34/reflex/utils/console.py` & `reflex-0.1.34a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/exec.py` & `reflex-0.1.34a1/reflex/utils/exec.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,48 @@
 from __future__ import annotations
 
 import os
 import platform
 import subprocess
 from datetime import datetime
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from rich import print
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites, processes
+from reflex.utils.build import export_app, setup_backend, setup_frontend
 from reflex.utils.watch import AssetFolderWatch
 
+if TYPE_CHECKING:
+    from reflex.app import App
+
 
 def start_watching_assets_folder(root):
     """Start watching assets folder.
 
     Args:
         root: root path of the project.
     """
     asset_watch = AssetFolderWatch(root)
     asset_watch.start()
 
 
 def run_process_and_launch_url(
     run_command: list[str],
+    root: Path,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the process and launch the URL.
 
     Args:
         run_command: The command to run.
+        root: root path of the project.
         loglevel: The log level to use.
     """
     process = subprocess.Popen(
         run_command,
         cwd=constants.WEB_DIR,
         env=os.environ,
         stderr=subprocess.STDOUT,
@@ -61,55 +68,71 @@
                     f"[yellow][Updating App][/yellow] Applying changes and refreshing. Time: {current_time}"
                 )
             elif loglevel == constants.LogLevel.DEBUG:
                 print(line, end="")
 
 
 def run_frontend(
+    app: App,
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the frontend.
 
     Args:
-        root: The root path of the project.
-        port: The port to run the frontend on.
+        app: The app.
+        root: root path of the project.
+        port: port of the app.
         loglevel: The log level to use.
     """
+    # validate bun version
+    prerequisites.validate_and_install_bun(initialize=False)
+
+    # Set up the frontend.
+    setup_frontend(root)
+
     # Start watching asset folder.
     start_watching_assets_folder(root)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().frontend_port if port is None else port
     run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "dev"], loglevel
+        [prerequisites.get_package_manager(), "run", "dev"], root, loglevel
     )
 
 
 def run_frontend_prod(
+    app: App,
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the frontend.
 
     Args:
-        root: The root path of the project (to keep same API as run_frontend).
-        port: The port to run the frontend on.
+        app: The app.
+        root: root path of the project.
+        port: port of the app.
         loglevel: The log level to use.
     """
+    # Set up the frontend.
+    setup_frontend(root)
+
+    # Export the app.
+    export_app(app, loglevel=loglevel)
+
     # Set the port.
     os.environ["PORT"] = get_config().frontend_port if port is None else port
 
     # Run the frontend in production mode.
     console.rule("[bold green]App Running")
     run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "prod"], loglevel
+        [prerequisites.get_package_manager(), "run", "prod"], root, loglevel
     )
 
 
 def run_backend(
     app_name: str,
     host: str,
     port: int,
@@ -119,14 +142,16 @@
 
     Args:
         host: The app host
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
+    setup_backend()
+
     cmd = [
         "uvicorn",
         f"{app_name}:{constants.APP_VAR}.{constants.API_VAR}",
         "--host",
         host,
         "--port",
         str(port),
@@ -152,14 +177,16 @@
 
     Args:
         host: The app host
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
+    setup_backend()
+
     num_workers = processes.get_num_workers()
     command = (
         [
             *constants.RUN_BACKEND_PROD_WINDOWS,
             "--host",
             host,
             "--port",
```

### Comparing `reflex-0.1.34/reflex/utils/format.py` & `reflex-0.1.34a1/reflex/utils/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
 
     # Convert Image objects to base64.
     if types.is_image(type(value)):
         return format_image_data(value)  # type: ignore
 
     raise TypeError(
         "State vars must be primitive Python types, "
-        "or subclasses of rf.Base. "
+        "or subclasses of pc.Base. "
         f"Got var of type {type(value)}."
     )
 
 
 def format_ref(ref: str) -> str:
     """Format a ref.
```

### Comparing `reflex-0.1.34/reflex/utils/imports.py` & `reflex-0.1.34a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/path_ops.py` & `reflex-0.1.34a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/prerequisites.py` & `reflex-0.1.34a1/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
     # Add the new files to the .gitignore file.
     with open(constants.GITIGNORE_FILE, "a") as f:
         f.write(f"\n{path_ops.join(files)}")
 
 
 def initialize_app_directory(app_name: str, template: constants.Template):
-    """Initialize the app directory on rf init.
+    """Initialize the app directory on rx init.
 
     Args:
         app_name: The name of the app.
         template: The template to use.
     """
     console.log("Initializing the app directory.")
     path_ops.cp(os.path.join(constants.TEMPLATE_DIR, "apps", template.value), app_name)
@@ -200,15 +200,15 @@
         os.path.join(app_name, template.value + ".py"),
         os.path.join(app_name, app_name + constants.PY_EXT),
     )
     path_ops.cp(constants.ASSETS_TEMPLATE_DIR, constants.APP_ASSETS_DIR)
 
 
 def initialize_web_directory():
-    """Initialize the web directory on rf init."""
+    """Initialize the web directory on rx init."""
     console.log("Initializing the web directory.")
     path_ops.rm(os.path.join(constants.WEB_TEMPLATE_DIR, constants.NODE_MODULES))
     path_ops.rm(os.path.join(constants.WEB_TEMPLATE_DIR, constants.PACKAGE_LOCK))
     path_ops.cp(constants.WEB_TEMPLATE_DIR, constants.WEB_DIR)
     path_ops.mkdir(constants.WEB_ASSETS_DIR)
 
     # Write the current version of distributed reflex package to a PCVERSION_APP_FILE."""
@@ -218,15 +218,15 @@
 
 
 def validate_and_install_bun(initialize=True):
     """Check that bun version requirements are met. If they are not,
     ask user whether to install required version.
 
     Args:
-        initialize: whether this function is called on `rf init` or `rf run`.
+        initialize: whether this function is called on `rx init` or `rx run`.
 
     Raises:
         Exit: If the bun version is not supported.
 
     """
     bun_version = get_bun_version()
     if bun_version is not None and (
```

### Comparing `reflex-0.1.34/reflex/utils/processes.py` & `reflex-0.1.34a1/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/telemetry.py` & `reflex-0.1.34a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/types.py` & `reflex-0.1.34a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/utils/watch.py` & `reflex-0.1.34a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/reflex/vars.py` & `reflex-0.1.34a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.1.34/PKG-INFO` & `reflex-0.1.34a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.1.34
+Version: 0.1.34a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.7,<4.0
@@ -32,28 +32,28 @@
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: starlette-admin (>=0.9.0,<0.10.0)
 Requires-Dist: typer (==0.4.2)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: watchdog (>=2.3.1,<3.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Documentation, https://reflex.dev/docs/getting-started/introduction
-Project-URL: Repository, https://github.com/reflex-io/reflex
+Project-URL: Repository, https://github.com/reflex-dev/reflex
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="docs/images/cones.png">
 <hr>
 
 **✨ Performant, customizable web apps in pure Python. Deploy in seconds.**
 
 📑 [Docs](https://reflex.dev/docs/getting-started/introduction) &nbsp; 📱 [Component Library](https://reflex.dev/docs/library) &nbsp; 🖼️ [Gallery](https://reflex.dev/docs/gallery) &nbsp; 🛸 [Deployment](https://reflex.dev/docs/hosting/deploy)
 
 [![PyPI version](https://badge.fury.io/py/reflex.svg)](https://badge.fury.io/py/reflex)
-![tests](https://github.com/reflex-io/reflex/actions/workflows/build.yml/badge.svg)
+![tests](https://github.com/reflex-dev/reflex/actions/workflows/build.yml/badge.svg)
 ![versions](https://img.shields.io/pypi/pyversions/reflex-io.svg)
 [![Discord](https://img.shields.io/discord/1029853095527727165?color=%237289da&label=Discord)](https://discord.gg/T5WSbC2YtQ)
 
 </div>
 
 ### README in different language
 
@@ -79,27 +79,27 @@
 Installing Reflex also installs the `pc` command line tool. Test that the install was successful by creating a new project.
 
 Replace my_app_name with your project name:
 
 ```
 mkdir my_app_name
 cd my_app_name
-pc init
+rx init
 ```
 
 When you run this command for the first time, we will download and install [bun](https://bun.sh/) automatically.
 
 This command initializes a template app in your new directory.
 
 ## 🏃 3. Run
 
 You can run this app in development mode:
 
 ```
-pc run
+rx run
 ```
 
 You should see your app running at http://localhost:3000.
 
 Now you can modify the source code in `my_app_name/my_app_name.py`. Reflex has fast refreshes so you can see your changes instantly when you save your code.
 
 ## 🫧 Example
@@ -172,15 +172,15 @@
         width="100%",
         height="100vh",
         bg="radial-gradient(circle at 22% 11%,rgba(62, 180, 137,.20),hsla(0,0%,100%,0) 19%)",
     )
 
 # Add state and page to the app.
 app = pc.App(state=State)
-app.add_page(index, title="rx:DALL·E")
+app.add_page(index, title="Reflex:DALL·E")
 app.compile()
 ```
 
 Let's break this down.
 
 ### **UI In Reflex**
```

