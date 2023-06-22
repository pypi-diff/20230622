# Comparing `tmp/markdown2-2.4.8.tar.gz` & `tmp/markdown2-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/markdown2-2.4.8.tar", last modified: Sun Feb 12 22:36:43 2023, max compression
+gzip compressed data, was "dist/markdown2-2.4.9.tar", last modified: Thu Jun 22 20:13:34 2023, max compression
```

## Comparing `markdown2-2.4.8.tar` & `markdown2-2.4.9.tar`

### file list

```diff
@@ -1,523 +1,539 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-12 22:36:43.552903 markdown2-2.4.8/
--rw-r--r--   0 root         (0) staff       (20)    23670 2023-02-12 22:36:38.000000 markdown2-2.4.8/CHANGES.md
--rw-r--r--   0 root         (0) staff       (20)     2292 2023-02-12 22:32:18.000000 markdown2-2.4.8/CONTRIBUTORS.txt
--rw-r--r--   0 root         (0) staff       (20)     2313 2023-02-12 22:32:18.000000 markdown2-2.4.8/LICENSE.txt
--rw-r--r--   0 root         (0) staff       (20)      261 2023-02-12 22:32:18.000000 markdown2-2.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      908 2023-02-12 22:32:18.000000 markdown2-2.4.8/Makefile
--rw-r--r--   0 root         (0) staff       (20)     1808 2023-02-12 22:36:43.553196 markdown2-2.4.8/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     5360 2023-02-12 22:32:18.000000 markdown2-2.4.8/README.md
--rw-r--r--   0 root         (0) staff       (20)     3324 2023-02-12 22:32:18.000000 markdown2-2.4.8/TODO.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-12 22:36:43.285390 markdown2-2.4.8/lib/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-12 22:36:43.288154 markdown2-2.4.8/lib/markdown2.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1808 2023-02-12 22:36:43.000000 markdown2-2.4.8/lib/markdown2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    19731 2023-02-12 22:36:43.000000 markdown2-2.4.8/lib/markdown2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-02-12 22:36:43.000000 markdown2-2.4.8/lib/markdown2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:36:43.000000 markdown2-2.4.8/lib/markdown2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)      164 2023-02-12 22:36:43.000000 markdown2-2.4.8/lib/markdown2.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:36:43.000000 markdown2-2.4.8/lib/markdown2.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) staff       (20)   126519 2023-02-12 22:32:18.000000 markdown2-2.4.8/lib/markdown2.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:36:43.554172 markdown2-2.4.8/setup.cfg
--rwxr-xr-x   0 root         (0) staff       (20)     2337 2023-02-12 22:32:18.000000 markdown2-2.4.8/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-12 22:36:43.290394 markdown2-2.4.8/test/
--rw-r--r--   0 root         (0) staff       (20)      355 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/api.doctests
--rwxr-xr-x   0 root         (0) staff       (20)     1813 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/test.py
--rwxr-xr-x   0 root         (0) staff       (20)    20451 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/test_markdown2.py
--rw-r--r--   0 root         (0) staff       (20)     1570 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/testall.py
--rw-r--r--   0 root         (0) staff       (20)    25924 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/testlib.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-12 22:36:43.552398 markdown2-2.4.8/test/tm-cases/
--rw-r--r--   0 root         (0) staff       (20)      181 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/CVE-2018-5773.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/CVE-2018-5773.opts
--rw-r--r--   0 root         (0) staff       (20)      141 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/CVE-2018-5773.text
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions.html
--rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions.opts
--rw-r--r--   0 root         (0) staff       (20)      955 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions.text
--rw-r--r--   0 root         (0) staff       (20)     1541 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions_with_fenced_code_blocks.html
--rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions_with_fenced_code_blocks.opts
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions_with_fenced_code_blocks.tags
--rw-r--r--   0 root         (0) staff       (20)      470 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/admonitions_with_fenced_code_blocks.text
--rw-r--r--   0 root         (0) staff       (20)       89 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ampersands.html
--rw-r--r--   0 root         (0) staff       (20)       13 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ampersands.tags
--rw-r--r--   0 root         (0) staff       (20)       38 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ampersands.text
--rw-r--r--   0 root         (0) staff       (20)      395 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link.html
--rw-r--r--   0 root         (0) staff       (20)       91 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link.text
--rw-r--r--   0 root         (0) staff       (20)     1443 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_email_with_underscore.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_email_with_underscore.tags
--rw-r--r--   0 root         (0) staff       (20)      207 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_email_with_underscore.text
--rw-r--r--   0 root         (0) staff       (20)      395 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_safe_mode.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_safe_mode.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_safe_mode.tags
--rw-r--r--   0 root         (0) staff       (20)       91 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/auto_link_safe_mode.text
--rw-r--r--   0 root         (0) staff       (20)      550 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/backslash_escape_html_tags.html
--rw-r--r--   0 root         (0) staff       (20)      448 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/backslash_escape_html_tags.text
--rw-r--r--   0 root         (0) staff       (20)      207 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/backslash_removed_by_adjacent_backtick.html
--rw-r--r--   0 root         (0) staff       (20)      145 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/backslash_removed_by_adjacent_backtick.text
--rw-r--r--   0 root         (0) staff       (20)     1114 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode.html
--rw-r--r--   0 root         (0) staff       (20)       91 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode.tags
--rw-r--r--   0 root         (0) staff       (20)      865 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode.text
--rw-r--r--   0 root         (0) staff       (20)       97 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode_escape.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode_escape.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode_escape.tags
--rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/basic_safe_mode_escape.text
--rw-r--r--   0 root         (0) staff       (20)      127 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote.html
--rw-r--r--   0 root         (0) staff       (20)       43 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote.text
--rw-r--r--   0 root         (0) staff       (20)       59 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote_containing_empty_lines.html
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote_containing_empty_lines.text
--rw-r--r--   0 root         (0) staff       (20)       84 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote_two_in_a_row.html
--rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote_two_in_a_row.text
--rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote_with_pre.html
--rw-r--r--   0 root         (0) staff       (20)      154 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/blockquote_with_pre.text
--rw-r--r--   0 root         (0) staff       (20)      205 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/break_on_newline.html
--rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/break_on_newline.opts
--rw-r--r--   0 root         (0) staff       (20)      154 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/break_on_newline.text
--rw-r--r--   0 root         (0) staff       (20)      993 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.html
--rw-r--r--   0 root         (0) staff       (20)       32 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.opts
--rw-r--r--   0 root         (0) staff       (20)      820 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.text
--rw-r--r--   0 root         (0) staff       (20)      126 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_block_with_tabs.html
--rw-r--r--   0 root         (0) staff       (20)       63 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_block_with_tabs.tags
--rw-r--r--   0 root         (0) staff       (20)       74 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_block_with_tabs.text
--rw-r--r--   0 root         (0) staff       (20)      144 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_blocks_leading_line.html
--rw-r--r--   0 root         (0) staff       (20)      110 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_blocks_leading_line.text
--rw-r--r--   0 root         (0) staff       (20)      142 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_safe_emphasis.html
--rw-r--r--   0 root         (0) staff       (20)       30 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_safe_emphasis.opts
--rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_safe_emphasis.tags
--rw-r--r--   0 root         (0) staff       (20)      117 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/code_safe_emphasis.text
--rw-r--r--   0 root         (0) staff       (20)      109 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codeblock.html
--rw-r--r--   0 root         (0) staff       (20)       62 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codeblock.text
--rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans.html
--rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans.text
--rw-r--r--   0 root         (0) staff       (20)      131 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans_inside_link_text.html
--rw-r--r--   0 root         (0) staff       (20)       72 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans_inside_link_text.text
--rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans_safe_mode.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans_safe_mode.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans_safe_mode.tags
--rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/codespans_safe_mode.text
--rw-r--r--   0 root         (0) staff       (20)      651 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/consecutive_image_links_issue498.html
--rw-r--r--   0 root         (0) staff       (20)      535 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/consecutive_image_links_issue498.text
--rw-r--r--   0 root         (0) staff       (20)      226 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_list_indented.html
--rw-r--r--   0 root         (0) staff       (20)       30 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_list_indented.opts
--rw-r--r--   0 root         (0) staff       (20)       36 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_list_indented.tags
--rw-r--r--   0 root         (0) staff       (20)      146 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_list_indented.text
--rw-r--r--   0 root         (0) staff       (20)      640 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_para_and_list.html
--rw-r--r--   0 root         (0) staff       (20)       30 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_para_and_list.opts
--rw-r--r--   0 root         (0) staff       (20)       36 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_para_and_list.tags
--rw-r--r--   0 root         (0) staff       (20)      436 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_para_and_list.text
--rw-r--r--   0 root         (0) staff       (20)      664 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_with_para.html
--rw-r--r--   0 root         (0) staff       (20)      581 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/cuddled_with_para.text
--rw-r--r--   0 root         (0) staff       (20)      175 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/demote_headers.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/demote_headers.opts
--rw-r--r--   0 root         (0) staff       (20)      155 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/demote_headers.text
--rw-r--r--   0 root         (0) staff       (20)      171 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_file_vars.html
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_file_vars.opts
--rw-r--r--   0 root         (0) staff       (20)      147 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_file_vars.text
--rw-r--r--   0 root         (0) staff       (20)       44 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_file_vars_with_metadata.html
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_file_vars_with_metadata.opts
--rw-r--r--   0 root         (0) staff       (20)       53 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_file_vars_with_metadata.text
--rw-r--r--   0 root         (0) staff       (20)      168 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_head_vars.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_head_vars.opts
--rw-r--r--   0 root         (0) staff       (20)        6 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_head_vars.tags
--rw-r--r--   0 root         (0) staff       (20)      161 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_head_vars.text
--rw-r--r--   0 root         (0) staff       (20)      190 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_tail_vars.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_tail_vars.opts
--rw-r--r--   0 root         (0) staff       (20)        6 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_tail_vars.tags
--rw-r--r--   0 root         (0) staff       (20)      183 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emacs_tail_vars.text
--rw-r--r--   0 root         (0) staff       (20)      130 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emphasis.html
--rw-r--r--   0 root         (0) staff       (20)       85 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/emphasis.text
--rw-r--r--   0 root         (0) staff       (20)     1648 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/escapes.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/escapes.tags
--rw-r--r--   0 root         (0) staff       (20)     1331 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/escapes.text
--rw-r--r--   0 root         (0) staff       (20)      353 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue113.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue113.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue113.tags
--rw-r--r--   0 root         (0) staff       (20)      312 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue113.text
--rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue127.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue127.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue127.tags
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue127.text
--rw-r--r--   0 root         (0) staff       (20)       32 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue135.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue135.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue135.tags
--rw-r--r--   0 root         (0) staff       (20)       15 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue135.text
--rw-r--r--   0 root         (0) staff       (20)      277 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue161.html
--rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue161.opts
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue161.tags
--rw-r--r--   0 root         (0) staff       (20)      197 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue161.text
--rw-r--r--   0 root         (0) staff       (20)      270 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue327.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue327.opts
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue327.tags
--rw-r--r--   0 root         (0) staff       (20)      203 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue327.text
--rw-r--r--   0 root         (0) staff       (20)      264 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue355.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue355.opts
--rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue355.tags
--rw-r--r--   0 root         (0) staff       (20)       94 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue355.text
--rw-r--r--   0 root         (0) staff       (20)       31 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue396.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue396.opts
--rw-r--r--   0 root         (0) staff       (20)       13 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue396.text
--rw-r--r--   0 root         (0) staff       (20)     2553 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue426.html
--rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue426.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue426.tags
--rw-r--r--   0 root         (0) staff       (20)      891 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue426.text
--rw-r--r--   0 root         (0) staff       (20)      205 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue462.html
--rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue462.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue462.tags
--rw-r--r--   0 root         (0) staff       (20)       65 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue462.text
--rw-r--r--   0 root         (0) staff       (20)      190 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue86.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue86.opts
--rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue86.tags
--rw-r--r--   0 root         (0) staff       (20)      139 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue86.text
--rw-r--r--   0 root         (0) staff       (20)      222 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_lang_space.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_lang_space.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_lang_space.tags
--rw-r--r--   0 root         (0) staff       (20)       39 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_lang_space.text
--rw-r--r--   0 root         (0) staff       (20)      144 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_line.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_line.opts
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_line.tags
--rw-r--r--   0 root         (0) staff       (20)      114 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_line.text
--rw-r--r--   0 root         (0) staff       (20)       68 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_paragraph.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_paragraph.opts
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_paragraph.tags
--rw-r--r--   0 root         (0) staff       (20)       43 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_leading_paragraph.text
--rw-r--r--   0 root         (0) staff       (20)      764 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight.html
--rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight.opts
--rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight.tags
--rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight.text
--rw-r--r--   0 root         (0) staff       (20)      695 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight_old.html
--rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight_old.opts
--rw-r--r--   0 root         (0) staff       (20)       48 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight_old.tags
--rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight_old.text
--rw-r--r--   0 root         (0) staff       (20)      277 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_simple.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_simple.opts
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_simple.tags
--rw-r--r--   0 root         (0) staff       (20)      197 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_simple.text
--rw-r--r--   0 root         (0) staff       (20)      764 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting.opts
--rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting.tags
--rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting.text
--rw-r--r--   0 root         (0) staff       (20)      695 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.opts
--rw-r--r--   0 root         (0) staff       (20)       48 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.tags
--rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.text
--rw-r--r--   0 root         (0) staff       (20)      300 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_indentation.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_indentation.opts
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_indentation.tags
--rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_indentation.text
--rw-r--r--   0 root         (0) staff       (20)     1196 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes.opts
--rw-r--r--   0 root         (0) staff       (20)      378 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes.text
--rw-r--r--   0 root         (0) staff       (20)     1184 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_custom.html
--rw-r--r--   0 root         (0) staff       (20)       85 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_custom.opts
--rw-r--r--   0 root         (0) staff       (20)      378 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_custom.text
--rw-r--r--   0 root         (0) staff       (20)     1004 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_letters.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_letters.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_letters.tags
--rw-r--r--   0 root         (0) staff       (20)      339 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_letters.text
--rw-r--r--   0 root         (0) staff       (20)      802 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_markup.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_markup.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_markup.tags
--rw-r--r--   0 root         (0) staff       (20)      301 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_markup.text
--rw-r--r--   0 root         (0) staff       (20)      469 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_safe_mode_escape.html
--rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_safe_mode_escape.opts
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_safe_mode_escape.tags
--rw-r--r--   0 root         (0) staff       (20)      185 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_safe_mode_escape.text
--rw-r--r--   0 root         (0) staff       (20)      429 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_smarty-pants.html
--rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_smarty-pants.opts
--rw-r--r--   0 root         (0) staff       (20)      184 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_smarty-pants.text
--rw-r--r--   0 root         (0) staff       (20)      788 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_underscores.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_underscores.opts
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_underscores.tags
--rw-r--r--   0 root         (0) staff       (20)      130 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/footnotes_underscores.text
--rw-r--r--   0 root         (0) staff       (20)      178 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hash_nested_html_blocks.html
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hash_nested_html_blocks.opts
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hash_nested_html_blocks.tags
--rw-r--r--   0 root         (0) staff       (20)       50 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hash_nested_html_blocks.text
--rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header.html
--rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header.text
--rw-r--r--   0 root         (0) staff       (20)       31 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_atx_no_preceeding_space.html
--rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_atx_no_preceeding_space.text
--rw-r--r--   0 root         (0) staff       (20)      185 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_1.html
--rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_1.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_1.tags
--rw-r--r--   0 root         (0) staff       (20)       81 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_1.text
--rw-r--r--   0 root         (0) staff       (20)      193 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_2.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_2.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_2.tags
--rw-r--r--   0 root         (0) staff       (20)       81 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_2.text
--rw-r--r--   0 root         (0) staff       (20)      185 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_3.html
--rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_3.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_3.tags
--rw-r--r--   0 root         (0) staff       (20)      109 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_3.text
--rw-r--r--   0 root         (0) staff       (20)      292 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_4.html
--rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_4.opts
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_4.tags
--rw-r--r--   0 root         (0) staff       (20)      151 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_4.text
--rw-r--r--   0 root         (0) staff       (20)      238 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_5.html
--rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_5.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_5.tags
--rw-r--r--   0 root         (0) staff       (20)       90 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/header_ids_5.text
--rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/headers_tag_friendly.html
--rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/headers_tag_friendly.opts
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/headers_tag_friendly.tags
--rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/headers_tag_friendly.text
--rw-r--r--   0 root         (0) staff       (20)      484 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/highlightjs_lang.html
--rw-r--r--   0 root         (0) staff       (20)       55 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/highlightjs_lang.opts
--rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/highlightjs_lang.tags
--rw-r--r--   0 root         (0) staff       (20)      284 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/highlightjs_lang.text
--rw-r--r--   0 root         (0) staff       (20)       77 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr.html
--rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr.text
--rw-r--r--   0 root         (0) staff       (20)      146 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr_length.html
--rw-r--r--   0 root         (0) staff       (20)       88 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr_length.text
--rw-r--r--   0 root         (0) staff       (20)      661 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr_spaces.html
--rw-r--r--   0 root         (0) staff       (20)      630 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr_spaces.text
--rw-r--r--   0 root         (0) staff       (20)      384 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr_uniform_characters.html
--rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/hr_uniform_characters.text
--rw-r--r--   0 root         (0) staff       (20)      173 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html5_block_tags.html
--rw-r--r--   0 root         (0) staff       (20)        7 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html5_block_tags.tags
--rw-r--r--   0 root         (0) staff       (20)      159 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html5_block_tags.text
--rw-r--r--   0 root         (0) staff       (20)     1433 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes.html
--rw-r--r--   0 root         (0) staff       (20)      355 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes.opts
--rw-r--r--   0 root         (0) staff       (20)       32 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes.tags
--rw-r--r--   0 root         (0) staff       (20)      473 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes.text
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes_is_none.html
--rw-r--r--   0 root         (0) staff       (20)       50 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes_is_none.opts
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes_is_none.tags
--rw-r--r--   0 root         (0) staff       (20)       28 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/html_classes_is_none.text
--rw-r--r--   0 root         (0) staff       (20)      319 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/img_in_link.html
--rw-r--r--   0 root         (0) staff       (20)      235 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/img_in_link.text
--rw-r--r--   0 root         (0) staff       (20)      310 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/incorrect_list_parse.html
--rw-r--r--   0 root         (0) staff       (20)        9 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/incorrect_list_parse.tags
--rw-r--r--   0 root         (0) staff       (20)      219 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/incorrect_list_parse.text
--rw-r--r--   0 root         (0) staff       (20)      348 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/inline_code_pipe_within_table.html
--rw-r--r--   0 root         (0) staff       (20)       22 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/inline_code_pipe_within_table.opts
--rw-r--r--   0 root         (0) staff       (20)       12 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/inline_code_pipe_within_table.tags
--rw-r--r--   0 root         (0) staff       (20)      176 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/inline_code_pipe_within_table.text
--rw-r--r--   0 root         (0) staff       (20)      476 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/inline_links.html
--rw-r--r--   0 root         (0) staff       (20)      278 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/inline_links.text
--rw-r--r--   0 root         (0) staff       (20)      117 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue21_gt_escaping.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue21_gt_escaping.opts
--rw-r--r--   0 root         (0) staff       (20)       15 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue21_gt_escaping.tags
--rw-r--r--   0 root         (0) staff       (20)       74 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue21_gt_escaping.text
--rw-r--r--   0 root         (0) staff       (20)      517 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue276_fenced_code_blocks_in_lists.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue276_fenced_code_blocks_in_lists.opts
--rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue276_fenced_code_blocks_in_lists.tags
--rw-r--r--   0 root         (0) staff       (20)      314 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue276_fenced_code_blocks_in_lists.text
--rw-r--r--   0 root         (0) staff       (20)      174 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue2_safe_mode_borks_markup.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue2_safe_mode_borks_markup.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue2_safe_mode_borks_markup.tags
--rw-r--r--   0 root         (0) staff       (20)      120 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue2_safe_mode_borks_markup.text
--rw-r--r--   0 root         (0) staff       (20)      294 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue341_xss.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue341_xss.opts
--rw-r--r--   0 root         (0) staff       (20)      193 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue341_xss.text
--rw-r--r--   0 root         (0) staff       (20)       70 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue348_incomplete_tag.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue348_incomplete_tag.opts
--rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue348_incomplete_tag.text
--rw-r--r--   0 root         (0) staff       (20)        5 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue52_hang.html
--rw-r--r--   0 root         (0) staff       (20)       21 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue52_hang.tags
--rw-r--r--   0 root         (0) staff       (20)      286 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue52_hang.text
--rw-r--r--   0 root         (0) staff       (20)      535 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue54_escape_link_title.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue54_escape_link_title.tags
--rw-r--r--   0 root         (0) staff       (20)      379 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/issue54_escape_link_title.text
--rw-r--r--   0 root         (0) staff       (20)      408 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_defn_alt_title_delims.html
--rw-r--r--   0 root         (0) staff       (20)      396 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_defn_alt_title_delims.text
--rw-r--r--   0 root         (0) staff       (20)      301 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_defn_spaces_in_url.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_defn_spaces_in_url.tags
--rw-r--r--   0 root         (0) staff       (20)      251 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_defn_spaces_in_url.text
--rw-r--r--   0 root         (0) staff       (20)      798 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_nofollow.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_nofollow.opts
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_nofollow.tags
--rw-r--r--   0 root         (0) staff       (20)      576 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_nofollow.text
--rw-r--r--   0 root         (0) staff       (20)      259 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns.html
--rw-r--r--   0 root         (0) staff       (20)      358 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns.opts
--rw-r--r--   0 root         (0) staff       (20)       72 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns.text
--rw-r--r--   0 root         (0) staff       (20)      186 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_double_hit.html
--rw-r--r--   0 root         (0) staff       (20)      262 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_double_hit.opts
--rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_double_hit.tags
--rw-r--r--   0 root         (0) staff       (20)       55 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_double_hit.text
--rw-r--r--   0 root         (0) staff       (20)      307 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_edge_cases.html
--rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_edge_cases.opts
--rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_edge_cases.tags
--rw-r--r--   0 root         (0) staff       (20)      153 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_edge_cases.text
--rw-r--r--   0 root         (0) staff       (20)      472 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_escape.html
--rw-r--r--   0 root         (0) staff       (20)      358 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_escape.opts
--rw-r--r--   0 root         (0) staff       (20)      461 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_escape.text
--rw-r--r--   0 root         (0) staff       (20)      238 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_markdown_syntax.html
--rw-r--r--   0 root         (0) staff       (20)      141 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_markdown_syntax.opts
--rw-r--r--   0 root         (0) staff       (20)      126 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_patterns_markdown_syntax.text
--rw-r--r--   0 root         (0) staff       (20)      288 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_safe_urls.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_safe_urls.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_safe_urls.tags
--rw-r--r--   0 root         (0) staff       (20)      210 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_safe_urls.text
--rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank.html
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank.opts
--rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank.tags
--rw-r--r--   0 root         (0) staff       (20)       84 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank.text
--rw-r--r--   0 root         (0) staff       (20)      218 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank_nofollow.html
--rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank_nofollow.opts
--rw-r--r--   0 root         (0) staff       (20)       22 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank_nofollow.tags
--rw-r--r--   0 root         (0) staff       (20)       84 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/link_with_blank_nofollow.text
--rw-r--r--   0 root         (0) staff       (20)      145 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists.html
--rw-r--r--   0 root         (0) staff       (20)       70 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists.text
--rw-r--r--   0 root         (0) staff       (20)      162 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists2.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists2.tags
--rw-r--r--   0 root         (0) staff       (20)       69 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists2.text
--rw-r--r--   0 root         (0) staff       (20)     1626 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists3.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists3.tags
--rw-r--r--   0 root         (0) staff       (20)     1188 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/lists3.text
--rw-r--r--   0 root         (0) staff       (20)     1104 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/long_link.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/long_link.tags
--rw-r--r--   0 root         (0) staff       (20)     1037 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/long_link.text
--rw-r--r--   0 root         (0) staff       (20)      739 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/markdown_in_html.html
--rw-r--r--   0 root         (0) staff       (20)       40 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/markdown_in_html.opts
--rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/markdown_in_html.tags
--rw-r--r--   0 root         (0) staff       (20)      549 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/markdown_in_html.text
--rw-r--r--   0 root         (0) staff       (20)      218 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mermaid.html
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mermaid.opts
--rw-r--r--   0 root         (0) staff       (20)       15 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mermaid.tags
--rw-r--r--   0 root         (0) staff       (20)      140 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mermaid.text
--rw-r--r--   0 root         (0) staff       (20)      121 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata.opts
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata.tags
--rw-r--r--   0 root         (0) staff       (20)      628 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata.text
--rw-r--r--   0 root         (0) staff       (20)      121 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata2.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata2.opts
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata2.tags
--rw-r--r--   0 root         (0) staff       (20)      327 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata2.text
--rw-r--r--   0 root         (0) staff       (20)      107 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata3.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata3.opts
--rw-r--r--   0 root         (0) staff       (20)      719 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/metadata3.text
--rw-r--r--   0 root         (0) staff       (20)      650 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mismatched_footnotes.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mismatched_footnotes.opts
--rw-r--r--   0 root         (0) staff       (20)      250 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mismatched_footnotes.text
--rw-r--r--   0 root         (0) staff       (20)       87 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/missing_link_defn.html
--rw-r--r--   0 root         (0) staff       (20)      111 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/missing_link_defn.text
--rw-r--r--   0 root         (0) staff       (20)      261 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mix-ordered-and-unordered-lists.html
--rw-r--r--   0 root         (0) staff       (20)      149 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/mix-ordered-and-unordered-lists.text
--rw-r--r--   0 root         (0) staff       (20)      211 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_incomplete_tags_xss.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_incomplete_tags_xss.opts
--rw-r--r--   0 root         (0) staff       (20)      156 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_incomplete_tags_xss.text
--rw-r--r--   0 root         (0) staff       (20)      456 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_list.html
--rw-r--r--   0 root         (0) staff       (20)      281 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_list.text
--rw-r--r--   0 root         (0) staff       (20)      182 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_list_safe_mode.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_list_safe_mode.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_list_safe_mode.tags
--rw-r--r--   0 root         (0) staff       (20)      106 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/nested_list_safe_mode.text
--rw-r--r--   0 root         (0) staff       (20)      393 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/not_quite_a_list.html
--rw-r--r--   0 root         (0) staff       (20)      282 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/not_quite_a_list.text
--rw-r--r--   0 root         (0) staff       (20)     1270 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/numbering.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/numbering.opts
--rw-r--r--   0 root         (0) staff       (20)     1269 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/numbering.text
--rw-r--r--   0 root         (0) staff       (20)      429 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering.html
--rw-r--r--   0 root         (0) staff       (20)      286 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering.text
--rw-r--r--   0 root         (0) staff       (20)     2792 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering_issue471.html
--rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering_issue471.opts
--rw-r--r--   0 root         (0) staff       (20)     2539 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering_issue471.text
--rw-r--r--   0 root         (0) staff       (20)       85 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/parens_in_url_4.html
--rw-r--r--   0 root         (0) staff       (20)       63 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/parens_in_url_4.tags
--rw-r--r--   0 root         (0) staff       (20)       63 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/parens_in_url_4.text
--rw-r--r--   0 root         (0) staff       (20)      207 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pi_and_xinclude.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pi_and_xinclude.opts
--rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pi_and_xinclude.tags
--rw-r--r--   0 root         (0) staff       (20)      203 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pi_and_xinclude.text
--rw-r--r--   0 root         (0) staff       (20)      380 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell.opts
--rw-r--r--   0 root         (0) staff       (20)      242 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell.text
--rw-r--r--   0 root         (0) staff       (20)     1517 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell_and_fenced_code_blocks.html
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell_and_fenced_code_blocks.opts
--rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell_and_fenced_code_blocks.tags
--rw-r--r--   0 root         (0) staff       (20)      280 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/pyshell_and_fenced_code_blocks.text
--rw-r--r--   0 root         (0) staff       (20)      438 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.opts
--rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.tags
--rw-r--r--   0 root         (0) staff       (20)      107 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.text
--rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/raw_html.html
--rw-r--r--   0 root         (0) staff       (20)       86 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/raw_html.text
--rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ref_links.html
--rw-r--r--   0 root         (0) staff       (20)       88 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/ref_links.text
--rw-r--r--   0 root         (0) staff       (20)     3807 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants.html
--rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants.opts
--rw-r--r--   0 root         (0) staff       (20)       21 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants.tags
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants.text
--rw-r--r--   0 root         (0) staff       (20)      315 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants_image_links.html
--rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants_image_links.opts
--rw-r--r--   0 root         (0) staff       (20)       21 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants_image_links.tags
--rw-r--r--   0 root         (0) staff       (20)      222 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/smarty_pants_image_links.text
--rw-r--r--   0 root         (0) staff       (20)      511 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/spoiler.html
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/spoiler.opts
--rw-r--r--   0 root         (0) staff       (20)      225 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/spoiler.text
--rw-r--r--   0 root         (0) staff       (20)       67 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/strike.html
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/strike.opts
--rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/strike.tags
--rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/strike.text
--rw-r--r--   0 root         (0) staff       (20)      403 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/sublist-ordered-para.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/sublist-ordered-para.tags
--rw-r--r--   0 root         (0) staff       (20)      205 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/sublist-ordered-para.text
--rw-r--r--   0 root         (0) staff       (20)      637 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/sublist-para.html
--rw-r--r--   0 root         (0) staff       (20)       77 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/sublist-para.tags
--rw-r--r--   0 root         (0) staff       (20)      531 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/sublist-para.text
--rw-r--r--   0 root         (0) staff       (20)     4633 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tables.html
--rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tables.opts
--rw-r--r--   0 root         (0) staff       (20)       13 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tables.tags
--rw-r--r--   0 root         (0) staff       (20)     2318 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tables.text
--rw-r--r--   0 root         (0) staff       (20)      267 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/task_list.html
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/task_list.opts
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/task_list.tags
--rw-r--r--   0 root         (0) staff       (20)       39 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/task_list.text
--rw-r--r--   0 root         (0) staff       (20)      242 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tg-spoiler.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tg-spoiler.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tg-spoiler.tags
--rw-r--r--   0 root         (0) staff       (20)      140 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tg-spoiler.text
--rw-r--r--   0 root         (0) staff       (20)      148 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_1.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_1.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_1.tags
--rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_1.text
--rw-r--r--   0 root         (0) staff       (20)      377 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_2.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_2.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_2.tags
--rw-r--r--   0 root         (0) staff       (20)      162 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_2.text
--rw-r--r--   0 root         (0) staff       (20)      377 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_3.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_3.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_3.tags
--rw-r--r--   0 root         (0) staff       (20)      182 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_3.text
--rw-r--r--   0 root         (0) staff       (20)      217 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_4.html
--rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_4.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_4.tags
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_4.text
--rw-r--r--   0 root         (0) staff       (20)      148 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_5.html
--rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_5.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_5.tags
--rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_5.text
--rw-r--r--   0 root         (0) staff       (20)      377 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_depth.html
--rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_depth.opts
--rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_depth.tags
--rw-r--r--   0 root         (0) staff       (20)      162 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/toc_depth.text
--rw-r--r--   0 root         (0) staff       (20)      402 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tricky_anchors.html
--rw-r--r--   0 root         (0) staff       (20)      268 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/tricky_anchors.text
--rw-r--r--   0 root         (0) staff       (20)       86 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/two_comments.html
--rw-r--r--   0 root         (0) staff       (20)       72 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/two_comments.text
--rw-r--r--   0 root         (0) staff       (20)       43 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline.tags
--rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline.text
--rw-r--r--   0 root         (0) staff       (20)      300 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline_html_comment.html
--rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline_html_comment.opts
--rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline_html_comment.tags
--rw-r--r--   0 root         (0) staff       (20)      225 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline_html_comment.text
--rw-r--r--   0 root         (0) staff       (20)      231 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline_in_autolink.html
--rw-r--r--   0 root         (0) staff       (20)      148 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/underline_in_autolink.text
--rw-r--r--   0 root         (0) staff       (20)    99243 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom.html
--rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom.opts
--rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom.tags
--rw-r--r--   0 root         (0) staff       (20)      710 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom.text
--rwxr-xr-x   0 root         (0) staff       (20)      754 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom_no_embed.html
--rw-r--r--   0 root         (0) staff       (20)       53 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom_no_embed.opts
--rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom_no_embed.tags
--rw-r--r--   0 root         (0) staff       (20)      710 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wavedrom_no_embed.text
--rw-r--r--   0 root         (0) staff       (20)     2456 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wiki_tables.html
--rw-r--r--   0 root         (0) staff       (20)       28 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wiki_tables.opts
--rw-r--r--   0 root         (0) staff       (20)       18 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wiki_tables.tags
--rw-r--r--   0 root         (0) staff       (20)      691 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/wiki_tables.text
--rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/xss_issue_362.html
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/xss_issue_362.opts
--rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/xss_issue_362.text
--rw-r--r--   0 root         (0) staff       (20)      124 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/xss_quotes.html
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/xss_quotes.tags
--rw-r--r--   0 root         (0) staff       (20)       98 2023-02-12 22:32:18.000000 markdown2-2.4.8/test/tm-cases/xss_quotes.text
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-22 20:13:34.451449 markdown2-2.4.9/
+-rw-r--r--   0 root         (0) staff       (20)    24221 2023-06-22 20:13:30.000000 markdown2-2.4.9/CHANGES.md
+-rw-r--r--   0 root         (0) staff       (20)     2327 2023-02-21 04:53:57.000000 markdown2-2.4.9/CONTRIBUTORS.txt
+-rw-r--r--   0 root         (0) staff       (20)     2313 2023-02-12 22:32:18.000000 markdown2-2.4.9/LICENSE.txt
+-rw-r--r--   0 root         (0) staff       (20)      261 2023-02-12 22:32:18.000000 markdown2-2.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      908 2023-02-12 22:32:18.000000 markdown2-2.4.9/Makefile
+-rw-r--r--   0 root         (0) staff       (20)     1808 2023-06-22 20:13:34.451566 markdown2-2.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     5360 2023-02-12 22:32:18.000000 markdown2-2.4.9/README.md
+-rw-r--r--   0 root         (0) staff       (20)     3324 2023-02-12 22:32:18.000000 markdown2-2.4.9/TODO.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-22 20:13:34.387184 markdown2-2.4.9/lib/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-22 20:13:34.388017 markdown2-2.4.9/lib/markdown2.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1808 2023-06-22 20:13:34.000000 markdown2-2.4.9/lib/markdown2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    20470 2023-06-22 20:13:34.000000 markdown2-2.4.9/lib/markdown2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-22 20:13:34.000000 markdown2-2.4.9/lib/markdown2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-06-22 20:13:34.000000 markdown2-2.4.9/lib/markdown2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      164 2023-06-22 20:13:34.000000 markdown2-2.4.9/lib/markdown2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-06-22 20:13:34.000000 markdown2-2.4.9/lib/markdown2.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) staff       (20)   130109 2023-06-22 20:10:35.000000 markdown2-2.4.9/lib/markdown2.py
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-06-22 20:13:34.451847 markdown2-2.4.9/setup.cfg
+-rwxr-xr-x   0 root         (0) staff       (20)     2337 2023-02-12 22:32:18.000000 markdown2-2.4.9/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-22 20:13:34.388567 markdown2-2.4.9/test/
+-rw-r--r--   0 root         (0) staff       (20)      355 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/api.doctests
+-rwxr-xr-x   0 root         (0) staff       (20)     1813 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/test.py
+-rwxr-xr-x   0 root         (0) staff       (20)    20451 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/test_markdown2.py
+-rw-r--r--   0 root         (0) staff       (20)     1570 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/testall.py
+-rw-r--r--   0 root         (0) staff       (20)    25846 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/testlib.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-22 20:13:34.451317 markdown2-2.4.9/test/tm-cases/
+-rw-r--r--   0 root         (0) staff       (20)      181 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/CVE-2018-5773.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/CVE-2018-5773.opts
+-rw-r--r--   0 root         (0) staff       (20)      141 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/CVE-2018-5773.text
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions.html
+-rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions.opts
+-rw-r--r--   0 root         (0) staff       (20)      955 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions.text
+-rw-r--r--   0 root         (0) staff       (20)     1541 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions_with_fenced_code_blocks.html
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions_with_fenced_code_blocks.opts
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions_with_fenced_code_blocks.tags
+-rw-r--r--   0 root         (0) staff       (20)      470 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/admonitions_with_fenced_code_blocks.text
+-rw-r--r--   0 root         (0) staff       (20)       89 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ampersands.html
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ampersands.tags
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ampersands.text
+-rw-r--r--   0 root         (0) staff       (20)      395 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link.html
+-rw-r--r--   0 root         (0) staff       (20)       91 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link.text
+-rw-r--r--   0 root         (0) staff       (20)     1443 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_email_with_underscore.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_email_with_underscore.tags
+-rw-r--r--   0 root         (0) staff       (20)      207 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_email_with_underscore.text
+-rw-r--r--   0 root         (0) staff       (20)      395 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_safe_mode.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_safe_mode.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_safe_mode.tags
+-rw-r--r--   0 root         (0) staff       (20)       91 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/auto_link_safe_mode.text
+-rw-r--r--   0 root         (0) staff       (20)      550 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/backslash_escape_html_tags.html
+-rw-r--r--   0 root         (0) staff       (20)      448 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/backslash_escape_html_tags.text
+-rw-r--r--   0 root         (0) staff       (20)      207 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/backslash_removed_by_adjacent_backtick.html
+-rw-r--r--   0 root         (0) staff       (20)      145 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/backslash_removed_by_adjacent_backtick.text
+-rw-r--r--   0 root         (0) staff       (20)      955 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode.html
+-rw-r--r--   0 root         (0) staff       (20)       91 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode.tags
+-rw-r--r--   0 root         (0) staff       (20)      865 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode.text
+-rw-r--r--   0 root         (0) staff       (20)       97 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode_escape.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode_escape.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode_escape.tags
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/basic_safe_mode_escape.text
+-rw-r--r--   0 root         (0) staff       (20)      127 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote.html
+-rw-r--r--   0 root         (0) staff       (20)       43 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote.text
+-rw-r--r--   0 root         (0) staff       (20)       59 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote_containing_empty_lines.html
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote_containing_empty_lines.text
+-rw-r--r--   0 root         (0) staff       (20)       84 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote_two_in_a_row.html
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote_two_in_a_row.text
+-rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote_with_pre.html
+-rw-r--r--   0 root         (0) staff       (20)      154 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/blockquote_with_pre.text
+-rw-r--r--   0 root         (0) staff       (20)      205 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/break_on_newline.html
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/break_on_newline.opts
+-rw-r--r--   0 root         (0) staff       (20)      154 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/break_on_newline.text
+-rw-r--r--   0 root         (0) staff       (20)      993 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.html
+-rw-r--r--   0 root         (0) staff       (20)       32 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.opts
+-rw-r--r--   0 root         (0) staff       (20)      820 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.text
+-rw-r--r--   0 root         (0) staff       (20)      126 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_block_with_tabs.html
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_block_with_tabs.tags
+-rw-r--r--   0 root         (0) staff       (20)       74 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_block_with_tabs.text
+-rw-r--r--   0 root         (0) staff       (20)      144 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_blocks_leading_line.html
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_blocks_leading_line.text
+-rw-r--r--   0 root         (0) staff       (20)      142 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_safe_emphasis.html
+-rw-r--r--   0 root         (0) staff       (20)       30 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_safe_emphasis.opts
+-rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_safe_emphasis.tags
+-rw-r--r--   0 root         (0) staff       (20)      117 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/code_safe_emphasis.text
+-rw-r--r--   0 root         (0) staff       (20)      109 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codeblock.html
+-rw-r--r--   0 root         (0) staff       (20)       62 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codeblock.text
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans.html
+-rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans.text
+-rw-r--r--   0 root         (0) staff       (20)      131 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans_inside_link_text.html
+-rw-r--r--   0 root         (0) staff       (20)       72 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans_inside_link_text.text
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans_safe_mode.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans_safe_mode.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans_safe_mode.tags
+-rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/codespans_safe_mode.text
+-rw-r--r--   0 root         (0) staff       (20)      651 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/consecutive_image_links_issue498.html
+-rw-r--r--   0 root         (0) staff       (20)      535 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/consecutive_image_links_issue498.text
+-rw-r--r--   0 root         (0) staff       (20)      226 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_list_indented.html
+-rw-r--r--   0 root         (0) staff       (20)       30 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_list_indented.opts
+-rw-r--r--   0 root         (0) staff       (20)       36 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_list_indented.tags
+-rw-r--r--   0 root         (0) staff       (20)      146 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_list_indented.text
+-rw-r--r--   0 root         (0) staff       (20)      640 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_para_and_list.html
+-rw-r--r--   0 root         (0) staff       (20)       30 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_para_and_list.opts
+-rw-r--r--   0 root         (0) staff       (20)       36 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_para_and_list.tags
+-rw-r--r--   0 root         (0) staff       (20)      436 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_para_and_list.text
+-rw-r--r--   0 root         (0) staff       (20)      664 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_with_para.html
+-rw-r--r--   0 root         (0) staff       (20)      581 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/cuddled_with_para.text
+-rw-r--r--   0 root         (0) staff       (20)      175 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/demote_headers.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/demote_headers.opts
+-rw-r--r--   0 root         (0) staff       (20)      155 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/demote_headers.text
+-rw-r--r--   0 root         (0) staff       (20)      171 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_file_vars.html
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_file_vars.opts
+-rw-r--r--   0 root         (0) staff       (20)      147 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_file_vars.text
+-rw-r--r--   0 root         (0) staff       (20)       44 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_file_vars_with_metadata.html
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_file_vars_with_metadata.opts
+-rw-r--r--   0 root         (0) staff       (20)       53 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_file_vars_with_metadata.text
+-rw-r--r--   0 root         (0) staff       (20)      168 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_head_vars.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_head_vars.opts
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_head_vars.tags
+-rw-r--r--   0 root         (0) staff       (20)      161 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_head_vars.text
+-rw-r--r--   0 root         (0) staff       (20)      190 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_tail_vars.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_tail_vars.opts
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_tail_vars.tags
+-rw-r--r--   0 root         (0) staff       (20)      183 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emacs_tail_vars.text
+-rw-r--r--   0 root         (0) staff       (20)      130 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emphasis.html
+-rw-r--r--   0 root         (0) staff       (20)       85 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/emphasis.text
+-rw-r--r--   0 root         (0) staff       (20)      276 2023-04-10 22:55:50.000000 markdown2-2.4.9/test/tm-cases/empty_fenced_code_blocks.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-04-10 22:55:50.000000 markdown2-2.4.9/test/tm-cases/empty_fenced_code_blocks.opts
+-rw-r--r--   0 root         (0) staff       (20)      121 2023-04-10 22:55:50.000000 markdown2-2.4.9/test/tm-cases/empty_fenced_code_blocks.text
+-rw-r--r--   0 root         (0) staff       (20)     1648 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/escapes.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/escapes.tags
+-rw-r--r--   0 root         (0) staff       (20)     1331 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/escapes.text
+-rw-r--r--   0 root         (0) staff       (20)      353 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue113.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue113.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue113.tags
+-rw-r--r--   0 root         (0) staff       (20)      312 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue113.text
+-rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue127.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue127.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue127.tags
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue127.text
+-rw-r--r--   0 root         (0) staff       (20)       32 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue135.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue135.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue135.tags
+-rw-r--r--   0 root         (0) staff       (20)       15 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue135.text
+-rw-r--r--   0 root         (0) staff       (20)      277 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue161.html
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue161.opts
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue161.tags
+-rw-r--r--   0 root         (0) staff       (20)      197 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue161.text
+-rw-r--r--   0 root         (0) staff       (20)      270 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue327.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue327.opts
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue327.tags
+-rw-r--r--   0 root         (0) staff       (20)      203 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue327.text
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue355.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue355.opts
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue355.tags
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue355.text
+-rw-r--r--   0 root         (0) staff       (20)       31 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue396.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue396.opts
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue396.text
+-rw-r--r--   0 root         (0) staff       (20)     2553 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue426.html
+-rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue426.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue426.tags
+-rw-r--r--   0 root         (0) staff       (20)      891 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue426.text
+-rw-r--r--   0 root         (0) staff       (20)      205 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue462.html
+-rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue462.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue462.tags
+-rw-r--r--   0 root         (0) staff       (20)       65 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue462.text
+-rw-r--r--   0 root         (0) staff       (20)      190 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue86.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue86.opts
+-rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue86.tags
+-rw-r--r--   0 root         (0) staff       (20)      139 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue86.text
+-rw-r--r--   0 root         (0) staff       (20)      222 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_lang_space.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_lang_space.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_lang_space.tags
+-rw-r--r--   0 root         (0) staff       (20)       39 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_lang_space.text
+-rw-r--r--   0 root         (0) staff       (20)      144 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_line.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_line.opts
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_line.tags
+-rw-r--r--   0 root         (0) staff       (20)      114 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_line.text
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_paragraph.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_paragraph.opts
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_paragraph.tags
+-rw-r--r--   0 root         (0) staff       (20)       43 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_leading_paragraph.text
+-rw-r--r--   0 root         (0) staff       (20)      764 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight.html
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight.opts
+-rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight.tags
+-rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight.text
+-rw-r--r--   0 root         (0) staff       (20)      695 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight_old.html
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight_old.opts
+-rw-r--r--   0 root         (0) staff       (20)       48 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight_old.tags
+-rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight_old.text
+-rw-r--r--   0 root         (0) staff       (20)      277 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_simple.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_simple.opts
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_simple.tags
+-rw-r--r--   0 root         (0) staff       (20)      197 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_simple.text
+-rw-r--r--   0 root         (0) staff       (20)      764 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting.opts
+-rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting.tags
+-rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting.text
+-rw-r--r--   0 root         (0) staff       (20)      695 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.opts
+-rw-r--r--   0 root         (0) staff       (20)       48 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.tags
+-rw-r--r--   0 root         (0) staff       (20)      237 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.text
+-rw-r--r--   0 root         (0) staff       (20)      300 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_indentation.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_indentation.opts
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_indentation.tags
+-rw-r--r--   0 root         (0) staff       (20)       58 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_indentation.text
+-rw-r--r--   0 root         (0) staff       (20)     1196 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes.opts
+-rw-r--r--   0 root         (0) staff       (20)      378 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes.text
+-rw-r--r--   0 root         (0) staff       (20)     1184 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_custom.html
+-rw-r--r--   0 root         (0) staff       (20)       85 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_custom.opts
+-rw-r--r--   0 root         (0) staff       (20)      378 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_custom.text
+-rw-r--r--   0 root         (0) staff       (20)     1004 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_letters.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_letters.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_letters.tags
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_letters.text
+-rw-r--r--   0 root         (0) staff       (20)      802 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_markup.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_markup.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_markup.tags
+-rw-r--r--   0 root         (0) staff       (20)      301 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_markup.text
+-rw-r--r--   0 root         (0) staff       (20)      469 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_safe_mode_escape.html
+-rw-r--r--   0 root         (0) staff       (20)       49 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_safe_mode_escape.opts
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_safe_mode_escape.tags
+-rw-r--r--   0 root         (0) staff       (20)      185 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_safe_mode_escape.text
+-rw-r--r--   0 root         (0) staff       (20)      429 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_smarty-pants.html
+-rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_smarty-pants.opts
+-rw-r--r--   0 root         (0) staff       (20)      184 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_smarty-pants.text
+-rw-r--r--   0 root         (0) staff       (20)      788 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_underscores.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_underscores.opts
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_underscores.tags
+-rw-r--r--   0 root         (0) staff       (20)      130 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/footnotes_underscores.text
+-rw-r--r--   0 root         (0) staff       (20)       86 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/hash_html_blocks_issue_508.html
+-rw-r--r--   0 root         (0) staff       (20)       65 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/hash_html_blocks_issue_508.text
+-rw-r--r--   0 root         (0) staff       (20)      178 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hash_nested_html_blocks.html
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hash_nested_html_blocks.opts
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hash_nested_html_blocks.tags
+-rw-r--r--   0 root         (0) staff       (20)       50 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hash_nested_html_blocks.text
+-rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header.html
+-rw-r--r--   0 root         (0) staff       (20)       73 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header.text
+-rw-r--r--   0 root         (0) staff       (20)       31 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_atx_no_preceeding_space.html
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_atx_no_preceeding_space.text
+-rw-r--r--   0 root         (0) staff       (20)      185 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_1.html
+-rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_1.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_1.tags
+-rw-r--r--   0 root         (0) staff       (20)       81 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_1.text
+-rw-r--r--   0 root         (0) staff       (20)      193 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_2.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_2.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_2.tags
+-rw-r--r--   0 root         (0) staff       (20)       81 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_2.text
+-rw-r--r--   0 root         (0) staff       (20)      185 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_3.html
+-rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_3.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_3.tags
+-rw-r--r--   0 root         (0) staff       (20)      109 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_3.text
+-rw-r--r--   0 root         (0) staff       (20)      292 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_4.html
+-rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_4.opts
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_4.tags
+-rw-r--r--   0 root         (0) staff       (20)      151 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_4.text
+-rw-r--r--   0 root         (0) staff       (20)      238 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_5.html
+-rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_5.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_5.tags
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/header_ids_5.text
+-rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/headers_tag_friendly.html
+-rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/headers_tag_friendly.opts
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/headers_tag_friendly.tags
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/headers_tag_friendly.text
+-rw-r--r--   0 root         (0) staff       (20)      484 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/highlightjs_lang.html
+-rw-r--r--   0 root         (0) staff       (20)       55 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/highlightjs_lang.opts
+-rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/highlightjs_lang.tags
+-rw-r--r--   0 root         (0) staff       (20)      284 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/highlightjs_lang.text
+-rw-r--r--   0 root         (0) staff       (20)       77 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr.html
+-rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr.text
+-rw-r--r--   0 root         (0) staff       (20)      146 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr_length.html
+-rw-r--r--   0 root         (0) staff       (20)       88 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr_length.text
+-rw-r--r--   0 root         (0) staff       (20)      661 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr_spaces.html
+-rw-r--r--   0 root         (0) staff       (20)      630 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr_spaces.text
+-rw-r--r--   0 root         (0) staff       (20)      384 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr_uniform_characters.html
+-rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/hr_uniform_characters.text
+-rw-r--r--   0 root         (0) staff       (20)      173 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html5_block_tags.html
+-rw-r--r--   0 root         (0) staff       (20)        7 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html5_block_tags.tags
+-rw-r--r--   0 root         (0) staff       (20)      159 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html5_block_tags.text
+-rw-r--r--   0 root         (0) staff       (20)     1473 2023-02-21 04:51:16.000000 markdown2-2.4.9/test/tm-cases/html_classes.html
+-rw-r--r--   0 root         (0) staff       (20)      385 2023-02-21 04:51:16.000000 markdown2-2.4.9/test/tm-cases/html_classes.opts
+-rw-r--r--   0 root         (0) staff       (20)       32 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html_classes.tags
+-rw-r--r--   0 root         (0) staff       (20)      473 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html_classes.text
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html_classes_is_none.html
+-rw-r--r--   0 root         (0) staff       (20)       50 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html_classes_is_none.opts
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html_classes_is_none.tags
+-rw-r--r--   0 root         (0) staff       (20)       28 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/html_classes_is_none.text
+-rw-r--r--   0 root         (0) staff       (20)      319 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/img_in_link.html
+-rw-r--r--   0 root         (0) staff       (20)      235 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/img_in_link.text
+-rw-r--r--   0 root         (0) staff       (20)      310 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/incorrect_list_parse.html
+-rw-r--r--   0 root         (0) staff       (20)        9 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/incorrect_list_parse.tags
+-rw-r--r--   0 root         (0) staff       (20)      219 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/incorrect_list_parse.text
+-rw-r--r--   0 root         (0) staff       (20)      348 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/inline_code_pipe_within_table.html
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/inline_code_pipe_within_table.opts
+-rw-r--r--   0 root         (0) staff       (20)       12 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/inline_code_pipe_within_table.tags
+-rw-r--r--   0 root         (0) staff       (20)      176 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/inline_code_pipe_within_table.text
+-rw-r--r--   0 root         (0) staff       (20)      476 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/inline_links.html
+-rw-r--r--   0 root         (0) staff       (20)      278 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/inline_links.text
+-rw-r--r--   0 root         (0) staff       (20)      117 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue21_gt_escaping.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue21_gt_escaping.opts
+-rw-r--r--   0 root         (0) staff       (20)       15 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue21_gt_escaping.tags
+-rw-r--r--   0 root         (0) staff       (20)       74 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue21_gt_escaping.text
+-rw-r--r--   0 root         (0) staff       (20)      517 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue276_fenced_code_blocks_in_lists.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue276_fenced_code_blocks_in_lists.opts
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue276_fenced_code_blocks_in_lists.tags
+-rw-r--r--   0 root         (0) staff       (20)      314 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue276_fenced_code_blocks_in_lists.text
+-rw-r--r--   0 root         (0) staff       (20)      174 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue2_safe_mode_borks_markup.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue2_safe_mode_borks_markup.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue2_safe_mode_borks_markup.tags
+-rw-r--r--   0 root         (0) staff       (20)      120 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue2_safe_mode_borks_markup.text
+-rw-r--r--   0 root         (0) staff       (20)      294 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue341_xss.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue341_xss.opts
+-rw-r--r--   0 root         (0) staff       (20)      193 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue341_xss.text
+-rw-r--r--   0 root         (0) staff       (20)       70 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue348_incomplete_tag.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue348_incomplete_tag.opts
+-rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue348_incomplete_tag.text
+-rw-r--r--   0 root         (0) staff       (20)        5 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue52_hang.html
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue52_hang.tags
+-rw-r--r--   0 root         (0) staff       (20)      286 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue52_hang.text
+-rw-r--r--   0 root         (0) staff       (20)      535 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue54_escape_link_title.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue54_escape_link_title.tags
+-rw-r--r--   0 root         (0) staff       (20)      379 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/issue54_escape_link_title.text
+-rw-r--r--   0 root         (0) staff       (20)      408 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_defn_alt_title_delims.html
+-rw-r--r--   0 root         (0) staff       (20)      396 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_defn_alt_title_delims.text
+-rw-r--r--   0 root         (0) staff       (20)      301 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_defn_spaces_in_url.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_defn_spaces_in_url.tags
+-rw-r--r--   0 root         (0) staff       (20)      251 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_defn_spaces_in_url.text
+-rw-r--r--   0 root         (0) staff       (20)      798 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_nofollow.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_nofollow.opts
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_nofollow.tags
+-rw-r--r--   0 root         (0) staff       (20)      576 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_nofollow.text
+-rw-r--r--   0 root         (0) staff       (20)      259 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns.html
+-rw-r--r--   0 root         (0) staff       (20)      358 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns.opts
+-rw-r--r--   0 root         (0) staff       (20)       72 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns.text
+-rw-r--r--   0 root         (0) staff       (20)      186 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_double_hit.html
+-rw-r--r--   0 root         (0) staff       (20)      262 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_double_hit.opts
+-rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_double_hit.tags
+-rw-r--r--   0 root         (0) staff       (20)       55 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_double_hit.text
+-rw-r--r--   0 root         (0) staff       (20)      307 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_edge_cases.html
+-rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_edge_cases.opts
+-rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_edge_cases.tags
+-rw-r--r--   0 root         (0) staff       (20)      153 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_edge_cases.text
+-rw-r--r--   0 root         (0) staff       (20)      472 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_escape.html
+-rw-r--r--   0 root         (0) staff       (20)      358 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_escape.opts
+-rw-r--r--   0 root         (0) staff       (20)      461 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_escape.text
+-rw-r--r--   0 root         (0) staff       (20)      259 2023-04-11 03:44:46.000000 markdown2-2.4.9/test/tm-cases/link_patterns_hash_matching_issue287.html
+-rw-r--r--   0 root         (0) staff       (20)      289 2023-04-11 03:44:46.000000 markdown2-2.4.9/test/tm-cases/link_patterns_hash_matching_issue287.opts
+-rw-r--r--   0 root         (0) staff       (20)       89 2023-04-11 03:44:46.000000 markdown2-2.4.9/test/tm-cases/link_patterns_hash_matching_issue287.text
+-rw-r--r--   0 root         (0) staff       (20)      238 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_markdown_syntax.html
+-rw-r--r--   0 root         (0) staff       (20)      141 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_markdown_syntax.opts
+-rw-r--r--   0 root         (0) staff       (20)      126 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_patterns_markdown_syntax.text
+-rw-r--r--   0 root         (0) staff       (20)      288 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_safe_urls.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_safe_urls.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_safe_urls.tags
+-rw-r--r--   0 root         (0) staff       (20)      210 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_safe_urls.text
+-rw-r--r--   0 root         (0) staff       (20)      200 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank.html
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank.opts
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank.tags
+-rw-r--r--   0 root         (0) staff       (20)       84 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank.text
+-rw-r--r--   0 root         (0) staff       (20)      218 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank_nofollow.html
+-rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank_nofollow.opts
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank_nofollow.tags
+-rw-r--r--   0 root         (0) staff       (20)       84 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/link_with_blank_nofollow.text
+-rw-r--r--   0 root         (0) staff       (20)      145 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists.html
+-rw-r--r--   0 root         (0) staff       (20)       70 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists.text
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists2.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists2.tags
+-rw-r--r--   0 root         (0) staff       (20)       69 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists2.text
+-rw-r--r--   0 root         (0) staff       (20)     1626 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists3.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists3.tags
+-rw-r--r--   0 root         (0) staff       (20)     1188 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/lists3.text
+-rw-r--r--   0 root         (0) staff       (20)     1104 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/long_link.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/long_link.tags
+-rw-r--r--   0 root         (0) staff       (20)     1037 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/long_link.text
+-rw-r--r--   0 root         (0) staff       (20)      739 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html.html
+-rw-r--r--   0 root         (0) staff       (20)       40 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html.opts
+-rw-r--r--   0 root         (0) staff       (20)       27 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html.tags
+-rw-r--r--   0 root         (0) staff       (20)      549 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html.text
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html_in_lists.html
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html_in_lists.opts
+-rw-r--r--   0 root         (0) staff       (20)      262 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/markdown_in_html_in_lists.text
+-rw-r--r--   0 root         (0) staff       (20)      218 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mermaid.html
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mermaid.opts
+-rw-r--r--   0 root         (0) staff       (20)       15 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mermaid.tags
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mermaid.text
+-rw-r--r--   0 root         (0) staff       (20)      121 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata.opts
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata.tags
+-rw-r--r--   0 root         (0) staff       (20)      628 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata.text
+-rw-r--r--   0 root         (0) staff       (20)      121 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata2.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata2.opts
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata2.tags
+-rw-r--r--   0 root         (0) staff       (20)      327 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata2.text
+-rw-r--r--   0 root         (0) staff       (20)      107 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata3.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata3.opts
+-rw-r--r--   0 root         (0) staff       (20)      719 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/metadata3.text
+-rw-r--r--   0 root         (0) staff       (20)      650 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mismatched_footnotes.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mismatched_footnotes.opts
+-rw-r--r--   0 root         (0) staff       (20)      250 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mismatched_footnotes.text
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/missing_link_defn.html
+-rw-r--r--   0 root         (0) staff       (20)      111 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/missing_link_defn.text
+-rw-r--r--   0 root         (0) staff       (20)      261 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mix-ordered-and-unordered-lists.html
+-rw-r--r--   0 root         (0) staff       (20)      149 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/mix-ordered-and-unordered-lists.text
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_incomplete_tags_xss.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_incomplete_tags_xss.opts
+-rw-r--r--   0 root         (0) staff       (20)      156 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_incomplete_tags_xss.text
+-rw-r--r--   0 root         (0) staff       (20)      633 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/nested_list.html
+-rw-r--r--   0 root         (0) staff       (20)      386 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/nested_list.text
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_list_safe_mode.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_list_safe_mode.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_list_safe_mode.tags
+-rw-r--r--   0 root         (0) staff       (20)      106 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/nested_list_safe_mode.text
+-rw-r--r--   0 root         (0) staff       (20)      393 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/not_quite_a_list.html
+-rw-r--r--   0 root         (0) staff       (20)      282 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/not_quite_a_list.text
+-rw-r--r--   0 root         (0) staff       (20)     1270 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/numbering.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/numbering.opts
+-rw-r--r--   0 root         (0) staff       (20)     1269 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/numbering.text
+-rw-r--r--   0 root         (0) staff       (20)      429 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering.html
+-rw-r--r--   0 root         (0) staff       (20)      286 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering.text
+-rw-r--r--   0 root         (0) staff       (20)     2792 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering_issue471.html
+-rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering_issue471.opts
+-rw-r--r--   0 root         (0) staff       (20)     2539 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering_issue471.text
+-rw-r--r--   0 root         (0) staff       (20)       85 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/parens_in_url_4.html
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/parens_in_url_4.tags
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/parens_in_url_4.text
+-rw-r--r--   0 root         (0) staff       (20)      207 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pi_and_xinclude.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pi_and_xinclude.opts
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pi_and_xinclude.tags
+-rw-r--r--   0 root         (0) staff       (20)      203 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pi_and_xinclude.text
+-rw-r--r--   0 root         (0) staff       (20)      380 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell.opts
+-rw-r--r--   0 root         (0) staff       (20)      242 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell.text
+-rw-r--r--   0 root         (0) staff       (20)     1517 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell_and_fenced_code_blocks.html
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell_and_fenced_code_blocks.opts
+-rw-r--r--   0 root         (0) staff       (20)       42 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell_and_fenced_code_blocks.tags
+-rw-r--r--   0 root         (0) staff       (20)      280 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/pyshell_and_fenced_code_blocks.text
+-rw-r--r--   0 root         (0) staff       (20)      438 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.opts
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.tags
+-rw-r--r--   0 root         (0) staff       (20)      107 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.text
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/raw_html.html
+-rw-r--r--   0 root         (0) staff       (20)       86 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/raw_html.text
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ref_links.html
+-rw-r--r--   0 root         (0) staff       (20)       88 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/ref_links.text
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/relative_links_safe_mode.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/relative_links_safe_mode.opts
+-rw-r--r--   0 root         (0) staff       (20)      210 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/relative_links_safe_mode.text
+-rw-r--r--   0 root         (0) staff       (20)      119 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/seperated_list_items.html
+-rw-r--r--   0 root         (0) staff       (20)       52 2023-06-22 20:10:35.000000 markdown2-2.4.9/test/tm-cases/seperated_list_items.text
+-rw-r--r--   0 root         (0) staff       (20)     3807 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants.html
+-rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants.opts
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants.tags
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants.text
+-rw-r--r--   0 root         (0) staff       (20)      315 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants_image_links.html
+-rw-r--r--   0 root         (0) staff       (20)       29 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants_image_links.opts
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants_image_links.tags
+-rw-r--r--   0 root         (0) staff       (20)      222 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/smarty_pants_image_links.text
+-rw-r--r--   0 root         (0) staff       (20)      511 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/spoiler.html
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/spoiler.opts
+-rw-r--r--   0 root         (0) staff       (20)      225 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/spoiler.text
+-rw-r--r--   0 root         (0) staff       (20)       67 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/strike.html
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/strike.opts
+-rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/strike.tags
+-rw-r--r--   0 root         (0) staff       (20)       47 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/strike.text
+-rw-r--r--   0 root         (0) staff       (20)      403 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/sublist-ordered-para.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/sublist-ordered-para.tags
+-rw-r--r--   0 root         (0) staff       (20)      205 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/sublist-ordered-para.text
+-rw-r--r--   0 root         (0) staff       (20)      637 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/sublist-para.html
+-rw-r--r--   0 root         (0) staff       (20)       77 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/sublist-para.tags
+-rw-r--r--   0 root         (0) staff       (20)      531 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/sublist-para.text
+-rw-r--r--   0 root         (0) staff       (20)     4633 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tables.html
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tables.opts
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tables.tags
+-rw-r--r--   0 root         (0) staff       (20)     2318 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tables.text
+-rw-r--r--   0 root         (0) staff       (20)      267 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/task_list.html
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/task_list.opts
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/task_list.tags
+-rw-r--r--   0 root         (0) staff       (20)       39 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/task_list.text
+-rw-r--r--   0 root         (0) staff       (20)      242 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tg-spoiler.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tg-spoiler.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tg-spoiler.tags
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tg-spoiler.text
+-rw-r--r--   0 root         (0) staff       (20)      148 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_1.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_1.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_1.tags
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_1.text
+-rw-r--r--   0 root         (0) staff       (20)      377 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_2.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_2.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_2.tags
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_2.text
+-rw-r--r--   0 root         (0) staff       (20)      377 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_3.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_3.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_3.tags
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_3.text
+-rw-r--r--   0 root         (0) staff       (20)      217 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_4.html
+-rw-r--r--   0 root         (0) staff       (20)       20 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_4.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_4.tags
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_4.text
+-rw-r--r--   0 root         (0) staff       (20)      148 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_5.html
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_5.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_5.tags
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_5.text
+-rw-r--r--   0 root         (0) staff       (20)      377 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_depth.html
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_depth.opts
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_depth.tags
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/toc_depth.text
+-rw-r--r--   0 root         (0) staff       (20)      402 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tricky_anchors.html
+-rw-r--r--   0 root         (0) staff       (20)      268 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/tricky_anchors.text
+-rw-r--r--   0 root         (0) staff       (20)       86 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/two_comments.html
+-rw-r--r--   0 root         (0) staff       (20)       72 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/two_comments.text
+-rw-r--r--   0 root         (0) staff       (20)       43 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline.tags
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline.text
+-rw-r--r--   0 root         (0) staff       (20)      300 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline_html_comment.html
+-rw-r--r--   0 root         (0) staff       (20)       26 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline_html_comment.opts
+-rw-r--r--   0 root         (0) staff       (20)       17 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline_html_comment.tags
+-rw-r--r--   0 root         (0) staff       (20)      225 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline_html_comment.text
+-rw-r--r--   0 root         (0) staff       (20)      231 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline_in_autolink.html
+-rw-r--r--   0 root         (0) staff       (20)      148 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/underline_in_autolink.text
+-rw-r--r--   0 root         (0) staff       (20)    99243 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom.html
+-rw-r--r--   0 root         (0) staff       (20)       24 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom.opts
+-rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom.tags
+-rw-r--r--   0 root         (0) staff       (20)      710 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom.text
+-rwxr-xr-x   0 root         (0) staff       (20)      754 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom_no_embed.html
+-rw-r--r--   0 root         (0) staff       (20)       53 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom_no_embed.opts
+-rw-r--r--   0 root         (0) staff       (20)       14 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom_no_embed.tags
+-rw-r--r--   0 root         (0) staff       (20)      710 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wavedrom_no_embed.text
+-rw-r--r--   0 root         (0) staff       (20)     2456 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wiki_tables.html
+-rw-r--r--   0 root         (0) staff       (20)       28 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wiki_tables.opts
+-rw-r--r--   0 root         (0) staff       (20)       18 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wiki_tables.tags
+-rw-r--r--   0 root         (0) staff       (20)      691 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/wiki_tables.text
+-rw-r--r--   0 root         (0) staff       (20)       35 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/xss_issue_362.html
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/xss_issue_362.opts
+-rw-r--r--   0 root         (0) staff       (20)       25 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/xss_issue_362.text
+-rw-r--r--   0 root         (0) staff       (20)      124 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/xss_quotes.html
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/xss_quotes.tags
+-rw-r--r--   0 root         (0) staff       (20)       98 2023-02-12 22:32:18.000000 markdown2-2.4.9/test/tm-cases/xss_quotes.text
```

### Comparing `markdown2-2.4.8/CHANGES.md` & `markdown2-2.4.9/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # python-markdown2 Changelog
 
+## python-markdown2 2.4.9
+
+- [pull #500] Add `<thead>` tag to html-classes extra
+- [pull #501] Fix link patterns extra matching against internal hashes
+- [pull #502] Replace deprecated `optparse` with `argparse`
+- [pull #506] Fix `_uniform_outdent` failing with empty strings (issue #505)
+- [pull #509] Fix HTML elements not unhashing correctly (issue 508)
+- [pull #511] Remove deprecated `imp` module (issue #510)
+- [pull #512] Allow link patterns to be passed via extras dict
+- [pull #513] Fix relative links not working in safe mode (issue #254)
+
+
 ## python-markdown2 2.4.8
 
 - [pull #499] Fix images not being procesed correctly (#498)
 
 
 ## python-markdown2 2.4.7
```

### Comparing `markdown2-2.4.8/CONTRIBUTORS.txt` & `markdown2-2.4.9/CONTRIBUTORS.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,7 +54,8 @@
 Crozzers (github.com/Crozzers)
 Bastian Venthur (https://github.com/venthur), removed Python2 support
 gitbra (github.com/gitbra)
 Łukasz Langa (github.com/ambv)
 Max Omdal (github.com/momja)
 Kishore (github.com/jk6521)
 Ircama (github.com/Ircama)
+Ankit Mahato (github.com/animator)
```

### Comparing `markdown2-2.4.8/LICENSE.txt` & `markdown2-2.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/Makefile` & `markdown2-2.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/PKG-INFO` & `markdown2-2.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown2
-Version: 2.4.8
+Version: 2.4.9
 Summary: A fast and complete Python implementation of Markdown
 Home-page: https://github.com/trentm/python-markdown2
 Author: Trent Mick
 Author-email: trentm@gmail.com
 Maintainer: Trent Mick
 Maintainer-email: trentm@gmail.com
 License: MIT
@@ -32,10 +32,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.5, <4
-Provides-Extra: all
 Provides-Extra: wavedrom
+Provides-Extra: all
 Provides-Extra: code_syntax_highlighting
```

### Comparing `markdown2-2.4.8/README.md` & `markdown2-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/TODO.txt` & `markdown2-2.4.9/TODO.txt`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/lib/markdown2.egg-info/PKG-INFO` & `markdown2-2.4.9/lib/markdown2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown2
-Version: 2.4.8
+Version: 2.4.9
 Summary: A fast and complete Python implementation of Markdown
 Home-page: https://github.com/trentm/python-markdown2
 Author: Trent Mick
 Author-email: trentm@gmail.com
 Maintainer: Trent Mick
 Maintainer-email: trentm@gmail.com
 License: MIT
@@ -32,10 +32,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.5, <4
-Provides-Extra: all
 Provides-Extra: wavedrom
+Provides-Extra: all
 Provides-Extra: code_syntax_highlighting
```

### Comparing `markdown2-2.4.8/lib/markdown2.egg-info/SOURCES.txt` & `markdown2-2.4.9/lib/markdown2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,17 @@
 test/tm-cases/emacs_head_vars.text
 test/tm-cases/emacs_tail_vars.html
 test/tm-cases/emacs_tail_vars.opts
 test/tm-cases/emacs_tail_vars.tags
 test/tm-cases/emacs_tail_vars.text
 test/tm-cases/emphasis.html
 test/tm-cases/emphasis.text
+test/tm-cases/empty_fenced_code_blocks.html
+test/tm-cases/empty_fenced_code_blocks.opts
+test/tm-cases/empty_fenced_code_blocks.text
 test/tm-cases/escapes.html
 test/tm-cases/escapes.tags
 test/tm-cases/escapes.text
 test/tm-cases/fenced_code_blocks_issue113.html
 test/tm-cases/fenced_code_blocks_issue113.opts
 test/tm-cases/fenced_code_blocks_issue113.tags
 test/tm-cases/fenced_code_blocks_issue113.text
@@ -216,14 +219,16 @@
 test/tm-cases/footnotes_smarty-pants.html
 test/tm-cases/footnotes_smarty-pants.opts
 test/tm-cases/footnotes_smarty-pants.text
 test/tm-cases/footnotes_underscores.html
 test/tm-cases/footnotes_underscores.opts
 test/tm-cases/footnotes_underscores.tags
 test/tm-cases/footnotes_underscores.text
+test/tm-cases/hash_html_blocks_issue_508.html
+test/tm-cases/hash_html_blocks_issue_508.text
 test/tm-cases/hash_nested_html_blocks.html
 test/tm-cases/hash_nested_html_blocks.opts
 test/tm-cases/hash_nested_html_blocks.tags
 test/tm-cases/hash_nested_html_blocks.text
 test/tm-cases/header.html
 test/tm-cases/header.text
 test/tm-cases/header_atx_no_preceeding_space.html
@@ -329,14 +334,17 @@
 test/tm-cases/link_patterns_edge_cases.html
 test/tm-cases/link_patterns_edge_cases.opts
 test/tm-cases/link_patterns_edge_cases.tags
 test/tm-cases/link_patterns_edge_cases.text
 test/tm-cases/link_patterns_escape.html
 test/tm-cases/link_patterns_escape.opts
 test/tm-cases/link_patterns_escape.text
+test/tm-cases/link_patterns_hash_matching_issue287.html
+test/tm-cases/link_patterns_hash_matching_issue287.opts
+test/tm-cases/link_patterns_hash_matching_issue287.text
 test/tm-cases/link_patterns_markdown_syntax.html
 test/tm-cases/link_patterns_markdown_syntax.opts
 test/tm-cases/link_patterns_markdown_syntax.text
 test/tm-cases/link_safe_urls.html
 test/tm-cases/link_safe_urls.opts
 test/tm-cases/link_safe_urls.tags
 test/tm-cases/link_safe_urls.text
@@ -359,14 +367,17 @@
 test/tm-cases/long_link.html
 test/tm-cases/long_link.tags
 test/tm-cases/long_link.text
 test/tm-cases/markdown_in_html.html
 test/tm-cases/markdown_in_html.opts
 test/tm-cases/markdown_in_html.tags
 test/tm-cases/markdown_in_html.text
+test/tm-cases/markdown_in_html_in_lists.html
+test/tm-cases/markdown_in_html_in_lists.opts
+test/tm-cases/markdown_in_html_in_lists.text
 test/tm-cases/mermaid.html
 test/tm-cases/mermaid.opts
 test/tm-cases/mermaid.tags
 test/tm-cases/mermaid.text
 test/tm-cases/metadata.html
 test/tm-cases/metadata.opts
 test/tm-cases/metadata.tags
@@ -422,14 +433,19 @@
 test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.opts
 test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.tags
 test/tm-cases/quoted_fenced_code_blocks_whitespace_around_indented_lines.text
 test/tm-cases/raw_html.html
 test/tm-cases/raw_html.text
 test/tm-cases/ref_links.html
 test/tm-cases/ref_links.text
+test/tm-cases/relative_links_safe_mode.html
+test/tm-cases/relative_links_safe_mode.opts
+test/tm-cases/relative_links_safe_mode.text
+test/tm-cases/seperated_list_items.html
+test/tm-cases/seperated_list_items.text
 test/tm-cases/smarty_pants.html
 test/tm-cases/smarty_pants.opts
 test/tm-cases/smarty_pants.tags
 test/tm-cases/smarty_pants.text
 test/tm-cases/smarty_pants_image_links.html
 test/tm-cases/smarty_pants_image_links.opts
 test/tm-cases/smarty_pants_image_links.tags
```

### Comparing `markdown2-2.4.8/lib/markdown2.py` & `markdown2-2.4.9/lib/markdown2.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   implemented in other Markdown processors (tho not in Markdown.pl v1.0.1).
 * header-ids: Adds "id" attributes to headers. The id value is a slug of
   the header text.
 * highlightjs-lang: Allows specifying the language which used for syntax
   highlighting when using fenced-code-blocks and highlightjs.
 * html-classes: Takes a dict mapping html tag names (lowercase) to a
   string to use for a "class" tag attribute. Currently only supports "img",
-  "table", "pre", "code", "ul" and "ol" tags. Add an issue if you require
+  "table", "thead", "pre", "code", "ul" and "ol" tags. Add an issue if you require
   this for other tags.
 * link-patterns: Auto-link given regex patterns in text (e.g. bug number
   references, revision number references).
 * markdown-in-html: Allow the use of `markdown="1"` in a block HTML tag to
   have markdown processing be done on its contents. Similar to
   <http://michelf.com/projects/php-markdown/extra/#markdown-attr> but with
   some limitations.
@@ -95,26 +95,26 @@
 """
 
 # Dev Notes:
 # - Python's regex syntax doesn't have '\z', so I'm using '\Z'. I'm
 #   not yet sure if there implications with this. Compare 'pydoc sre'
 #   and 'perldoc perlre'.
 
-__version_info__ = (2, 4, 8)
+__version_info__ = (2, 4, 9)
 __version__ = '.'.join(map(str, __version_info__))
 __author__ = "Trent Mick"
 
-import sys
-import re
-import logging
-from hashlib import sha256
-import optparse
-from random import random, randint
+import argparse
 import codecs
+import logging
+import re
+import sys
 from collections import defaultdict
+from hashlib import sha256
+from random import randint, random
 
 # ---- globals
 
 DEBUG = False
 log = logging.getLogger("markdown")
 
 DEFAULT_TAB_WIDTH = 4
@@ -231,19 +231,22 @@
             if self.extras["toc"] is None:
                 self._toc_depth = 6
             else:
                 self._toc_depth = self.extras["toc"].get("depth", 6)
         self._instance_extras = self.extras.copy()
 
         if 'link-patterns' in self.extras:
+            # allow link patterns via extras dict without kwarg explicitly set
+            link_patterns = link_patterns or extras['link-patterns']
             if link_patterns is None:
                 # if you have specified that the link-patterns extra SHOULD
                 # be used (via self.extras) but you haven't provided anything
                 # via the link_patterns argument then an error is raised
                 raise MarkdownError("If the 'link-patterns' extra is used, an argument for 'link_patterns' is required")
+
         self.link_patterns = link_patterns
         self.footnote_title = footnote_title
         self.footnote_return_symbol = footnote_return_symbol
         self.use_file_vars = use_file_vars
         self._outdent_re = re.compile(r'^(\t|[ ]{1,%d})' % tab_width, re.M)
         self.cli = cli
 
@@ -356,14 +359,17 @@
 
         if self.safe_mode:
             text = self._hash_html_spans(text)
 
         # Turn block-level HTML blocks into hash entries
         text = self._hash_html_blocks(text, raw=True)
 
+        if 'markdown-in-html' in self.extras:
+            text = self._do_markdown_in_html(text)
+
         if "fenced-code-blocks" in self.extras and self.safe_mode:
             text = self._do_fenced_code_blocks(text)
 
         if 'admonitions' in self.extras:
             text = self._do_admonitions(text)
 
         # Because numbering references aren't links (yet?) then we can do everything associated with counters
@@ -871,47 +877,72 @@
             #
             #    <xi:include xmlns:xi="http://www.w3.org/2001/XInclude" href="chapter_1.md"/>
             _xml_oneliner_re = _xml_oneliner_re_from_tab_width(self.tab_width)
             text = _xml_oneliner_re.sub(hash_html_block_sub, text)
 
         return text
 
-    def _strict_tag_block_sub(self, text, html_tags_re, callback):
+    def _strict_tag_block_sub(self, text, html_tags_re, callback, allow_indent=False):
+        '''
+        Finds and substitutes HTML blocks within blocks of text
+
+        Args:
+            text: the text to search
+            html_tags_re: a regex pattern of HTML block tags to match against.
+                For example, `Markdown._block_tags_a`
+            callback: callback function that receives the found HTML text block
+            allow_indent: allow matching HTML blocks that are not completely outdented
+        '''
         tag_count = 0
         current_tag = html_tags_re
         block = ''
         result = ''
 
         for chunk in text.splitlines(True):
-            is_markup = re.match(r'^(?:</code>(?=</pre>))?(</?(%s)\b>?)' % current_tag, chunk)
+            is_markup = re.match(
+                r'^(\s{0,%s})(?:</code>(?=</pre>))?(</?(%s)\b>?)' % ('' if allow_indent else '0', current_tag), chunk
+            )
             block += chunk
 
             if is_markup:
-                if chunk.startswith('</'):
+                if chunk.startswith('%s</' % is_markup.group(1)):
                     tag_count -= 1
                 else:
                     # if close tag is in same line
-                    if '</%s>' % is_markup.group(2) in chunk[is_markup.end():]:
+                    if self._tag_is_closed(is_markup.group(3), chunk):
                         # we must ignore these
                         is_markup = None
                     else:
                         tag_count += 1
-                        current_tag = is_markup.group(2)
+                        current_tag = is_markup.group(3)
 
             if tag_count == 0:
                 if is_markup:
                     block = callback(block.rstrip('\n'))  # remove trailing newline
                 current_tag = html_tags_re
                 result += block
                 block = ''
 
         result += block
 
         return result
 
+    def _tag_is_closed(self, tag_name, text):
+        # super basic check if number of open tags == number of closing tags
+        return len(re.findall('<%s(?:.*?)>' % tag_name, text)) == len(re.findall('</%s>' % tag_name, text))
+
+    def _do_markdown_in_html(self, text):
+        def callback(block):
+            indent, block = self._uniform_outdent(block)
+            block = self._hash_html_block_sub(block)
+            block = self._uniform_indent(block, indent, include_empty_lines=True, indent_empty_lines=False)
+            return block
+
+        return self._strict_tag_block_sub(text, self._block_tags_a, callback, True)
+
     def _strip_link_definitions(self, text):
         # Strips link definitions from text, stores the URLs and titles in
         # hash references.
         less_than_tab = self.tab_width - 1
 
         # Link defs are in the form:
         #   [id]: url "optional title"
@@ -1135,15 +1166,15 @@
                 align_from_col_idx[col_idx] = ' style="text-align:center;"'
             elif col[0] == ':':
                 align_from_col_idx[col_idx] = ' style="text-align:left;"'
             elif col[-1] == ':':
                 align_from_col_idx[col_idx] = ' style="text-align:right;"'
 
         # thead
-        hlines = ['<table%s>' % self._html_class_str_from_tag('table'), '<thead>', '<tr>']
+        hlines = ['<table%s>' % self._html_class_str_from_tag('table'), '<thead%s>' % self._html_class_str_from_tag('thead'), '<tr>']
         cols = [re.sub(escape_bar_re, '|', cell.strip()) for cell in re.split(split_bar_re, re.sub(trim_bar_re, "", re.sub(trim_space_re, "", head)))]
         for col_idx, col in enumerate(cols):
             hlines.append('  <th%s>%s</th>' % (
                 align_from_col_idx.get(col_idx, ''),
                 self._run_span_gamut(col)
             ))
         hlines.append('</tr>')
@@ -1211,15 +1242,15 @@
 
         def format_cell(text):
             return self._run_span_gamut(re.sub(r"^\s*~", "", cell).strip(" "))
 
         add_hline('<table%s>' % self._html_class_str_from_tag('table'))
         # Check if first cell of first row is a header cell. If so, assume the whole row is a header row.
         if rows and rows[0] and re.match(r"^\s*~", rows[0][0]):
-            add_hline('<thead>', 1)
+            add_hline('<thead%s>' % self._html_class_str_from_tag('thead'), 1)
             add_hline('<tr>', 2)
             for cell in rows[0]:
                 add_hline("<th>{}</th>".format(format_cell(cell)), 3)
             add_hline('</tr>', 2)
             add_hline('</thead>', 1)
             # Only one header row allowed.
             rows = rows[1:]
@@ -1472,15 +1503,21 @@
         with it (eg: escaping "&" in URL parameters)
         '''
         url = _html_escape_url(url, safe_mode=self.safe_mode)
         key = _hash_text(url)
         self._escape_table[url] = key
         return key
 
-    _safe_protocols = re.compile(r'(https?|ftp):', re.I)
+    # _safe_href is copied from pagedown's Markdown.Sanitizer.js
+    # From: https://github.com/StackExchange/pagedown/blob/master/LICENSE.txt
+    # Original Showdown code copyright (c) 2007 John Fraser
+    # Modifications and bugfixes (c) 2009 Dana Robinson
+    # Modifications and bugfixes (c) 2009-2014 Stack Exchange Inc.
+    _safe_href = re.compile(r'^((https?|ftp):\/\/|\/|\.|#)[-A-Za-z0-9+&@#\/%?=~_|!:,.;\(\)*[\]$]*$', re.I)
+
     def _do_links(self, text):
         """Turn Markdown link shortcuts into XHTML <a> and <img> tags.
 
         This is a combination of Markdown.pl's _DoAnchors() and
         _DoImages(). They are done together because that simplified the
         approach. It was necessary to use a different approach than
         Markdown.pl because of the lack of atomic matching support in
@@ -1590,15 +1627,15 @@
                                self.empty_element_suffix)
                         if "smarty-pants" in self.extras:
                             result = result.replace('"', self._escape_table['"'])
                         curr_pos = start_idx + len(result)
                         anchor_allowed_pos = start_idx + len(result)
                         text = text[:start_idx] + result + text[url_end_idx:]
                     elif start_idx >= anchor_allowed_pos:
-                        safe_link = self._safe_protocols.match(url) or url.startswith('#')
+                        safe_link = self._safe_href.match(url)
                         if self.safe_mode and not safe_link:
                             result_head = '<a href="#"%s>' % (title_str)
                         else:
                             result_head = '<a href="%s"%s>' % (self._protect_url(url), title_str)
                         result = '%s%s</a>' % (result_head, link_text)
                         if "smarty-pants" in self.extras:
                             result = result.replace('"', self._escape_table['"'])
@@ -1646,15 +1683,15 @@
                                    img_class_str,
                                    self.empty_element_suffix)
                             if "smarty-pants" in self.extras:
                                 result = result.replace('"', self._escape_table['"'])
                             curr_pos = start_idx + len(result)
                             text = text[:start_idx] + result + text[match.end():]
                         elif start_idx >= anchor_allowed_pos:
-                            if self.safe_mode and not self._safe_protocols.match(url):
+                            if self.safe_mode and not self._safe_href.match(url):
                                 result_head = '<a href="#"%s>' % (title_str)
                             else:
                                 result_head = '<a href="%s"%s>' % (self._protect_url(url), title_str)
                             result = '%s%s</a>' % (result_head, link_text)
                             if "smarty-pants" in self.extras:
                                 result = result.replace('"', self._escape_table['"'])
                             # <img> allowed from curr_pos on, <a> from
@@ -1876,15 +1913,16 @@
                 return self._task_list_warpper_str % ('', item_text)
 
     _last_li_endswith_two_eols = False
     def _list_item_sub(self, match):
         item = match.group(4)
         leading_line = match.group(1)
         if leading_line or "\n\n" in item or self._last_li_endswith_two_eols:
-            item = self._run_block_gamut(self._outdent(item))
+            item = self._uniform_outdent(item, min_outdent=' ', max_outdent=self.tab)[1]
+            item = self._run_block_gamut(item)
         else:
             # Recursion for sub-lists:
             item = self._do_lists(self._uniform_outdent(item, min_outdent=' ')[1])
             if item.endswith('\n'):
                 item = item[:-1]
             item = self._run_span_gamut(item)
         self._last_li_endswith_two_eols = (len(match.group(5)) == 2)
@@ -2184,15 +2222,15 @@
                 pass
 
         # hash SVG to prevent <> chars being messed with
         self._escape_table[waves] = _hash_text(waves)
 
         return self._uniform_indent(
             '\n%s%s%s\n' % (open_tag, self._escape_table[waves], close_tag),
-            lead_indent, include_empty_lines=True
+            lead_indent, indent_empty_lines=True
         )
 
     def _do_wavedrom_blocks(self, text):
         return self._fenced_code_block_re.sub(self._wavedrom_block_sub, text)
 
     _admonitions = r'admonition|attention|caution|danger|error|hint|important|note|tip|warning'
     _admonitions_re = re.compile(r'''
@@ -2237,15 +2275,15 @@
         text = self._strike_re.sub(r"<s>\1</s>", text)
         return text
 
     _underline_re = re.compile(r"(?<!<!)--(?!>)(?=\S)(.+?)(?<=\S)(?<!<!)--(?!>)", re.S)
     def _do_underline(self, text):
         text = self._underline_re.sub(r"<u>\1</u>", text)
         return text
-    
+
     _tg_spoiler_re = re.compile(r"\|\|\s?(.+?)\s?\|\|", re.S)
     def _do_tg_spoiler(self, text):
         text = self._tg_spoiler_re.sub(r"<tg-spoiler>\1</tg-spoiler>", text)
         return text
 
     _strong_re = re.compile(r"(\*\*|__)(?=\S)(.+?[*_]*)(?<=\S)\1", re.S)
     _em_re = re.compile(r"(\*|_)(?=\S)(.+?)(?<=\S)\1", re.S)
@@ -2529,14 +2567,17 @@
 
     _basic_link_re = re.compile(r'!?\[.*?\]\(.*?\)')
     def _do_link_patterns(self, text):
         link_from_hash = {}
         for regex, repl in self.link_patterns:
             replacements = []
             for match in regex.finditer(text):
+                if any(self._match_overlaps_substr(text, match, h) for h in link_from_hash):
+                    continue
+
                 if hasattr(repl, "__call__"):
                     href = repl(match)
                 else:
                     href = match.expand(repl)
                 replacements.append((match.span(), href))
             for (start, end), href in reversed(replacements):
 
@@ -2592,33 +2633,41 @@
                 break
         return text
 
     def _outdent(self, text):
         # Remove one level of line-leading tabs or spaces
         return self._outdent_re.sub('', text)
 
-    def _uniform_outdent(self, text, min_outdent=None, max_outdent=None):
-        # Removes the smallest common leading indentation from each (non empty)
-        # line of `text` and returns said indent along with the outdented text.
-        # The `min_outdent` kwarg makes sure the smallest common whitespace
-        # must be at least this size
-        # The `max_outdent` sets the maximum amount a line can be
-        # outdented by
+    @staticmethod
+    def _uniform_outdent(text, min_outdent=None, max_outdent=None):
+        '''
+        Removes the smallest common leading indentation from each (non empty)
+        line of `text` and returns said indent along with the outdented text.
+
+        Args:
+            min_outdent: make sure the smallest common whitespace is at least this size
+            max_outdent: the maximum amount a line can be outdented by
+        '''
 
         # find the leading whitespace for every line
         whitespace = [
             re.findall(r'^[ \t]*', line)[0] if line else None
             for line in text.splitlines()
         ]
+        whitespace_not_empty = [i for i in whitespace if i is not None]
+
+        # if no whitespace detected (ie: no lines in code block, issue #505)
+        if not whitespace_not_empty:
+            return '', text
 
         # get minimum common whitespace
-        outdent = min(i for i in whitespace if i is not None)
+        outdent = min(whitespace_not_empty)
         # adjust min common ws to be within bounds
         if min_outdent is not None:
-            outdent = min([i for i in whitespace if i is not None and i >= min_outdent] or [min_outdent])
+            outdent = min([i for i in whitespace_not_empty if i >= min_outdent] or [min_outdent])
         if max_outdent is not None:
             outdent = min(outdent, max_outdent)
 
         outdented = []
         for line_ws, line in zip(whitespace, text.splitlines(True)):
             if line.startswith(outdent):
                 # if line starts with smallest common ws, dedent it
@@ -2627,19 +2676,47 @@
                 # if less indented than min common whitespace then outdent as much as possible
                 outdented.append(line.replace(line_ws, '', 1))
             else:
                 outdented.append(line)
 
         return outdent, ''.join(outdented)
 
-    def _uniform_indent(self, text, indent, include_empty_lines=False):
-        return ''.join(
-            (indent + line if line.strip() or include_empty_lines else '')
-            for line in text.splitlines(True)
-        )
+    @staticmethod
+    def _uniform_indent(text, indent, include_empty_lines=False, indent_empty_lines=False):
+        '''
+        Uniformly indent a block of text by a fixed amount
+
+        Args:
+            text: the text to indent
+            indent: a string containing the indent to apply
+            include_empty_lines: don't remove whitespace only lines
+            indent_empty_lines: indent whitespace only lines with the rest of the text
+        '''
+        blocks = []
+        for line in text.splitlines(True):
+            if line.strip() or indent_empty_lines:
+                blocks.append(indent + line)
+            elif include_empty_lines:
+                blocks.append(line)
+            else:
+                blocks.append('')
+        return ''.join(blocks)
+
+    @staticmethod
+    def _match_overlaps_substr(text, match, substr):
+        '''
+        Checks if a regex match overlaps with a substring in the given text.
+        '''
+        for instance in re.finditer(re.escape(substr), text):
+            start, end = instance.span()
+            if start <= match.start() <= end:
+                return True
+            if start <= match.end() <= end:
+                return True
+        return False
 
 
 class MarkdownWithExtras(Markdown):
     """A markdowner class that enables most extras:
 
     - footnotes
     - fenced-code-blocks (only highlights code if 'pygments' Python module on path)
@@ -2952,16 +3029,16 @@
         escaped = escaped.replace('+', ' ')
         escaped = escaped.replace("'", "&#39;")
     return escaped
 
 
 # ---- mainline
 
-class _NoReflowFormatter(optparse.IndentedHelpFormatter):
-    """An optparse formatter that does NOT reflow the description."""
+class _NoReflowFormatter(argparse.RawDescriptionHelpFormatter):
+    """An argparse formatter that does NOT reflow the description."""
     def format_description(self, description):
         return description or ""
 
 
 def _test():
     import doctest
     doctest.testmod()
@@ -2969,46 +3046,53 @@
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv
     if not logging.root.handlers:
         logging.basicConfig()
 
-    usage = "usage: %prog [PATHS...]"
-    version = "%prog "+__version__
-    parser = optparse.OptionParser(prog="markdown2", usage=usage,
-        version=version, description=cmdln_desc,
-        formatter=_NoReflowFormatter())
-    parser.add_option("-v", "--verbose", dest="log_level",
+    parser = argparse.ArgumentParser(
+        prog="markdown2", description=cmdln_desc, usage='%(prog)s [PATHS...]',
+        formatter_class=_NoReflowFormatter
+    )
+    parser.add_argument('--version', action='version',
+                        version='%(prog)s {version}'.format(version=__version__))
+    parser.add_argument('paths', nargs='*',
+                        help=(
+                            'optional list of files to convert.'
+                            'If none are given, stdin will be used'
+                        ))
+    parser.add_argument("-v", "--verbose", dest="log_level",
                       action="store_const", const=logging.DEBUG,
                       help="more verbose output")
-    parser.add_option("--encoding",
+    parser.add_argument("--encoding",
                       help="specify encoding of text content")
-    parser.add_option("--html4tags", action="store_true", default=False,
+    parser.add_argument("--html4tags", action="store_true", default=False,
                       help="use HTML 4 style for empty element tags")
-    parser.add_option("-s", "--safe", metavar="MODE", dest="safe_mode",
+    parser.add_argument("-s", "--safe", metavar="MODE", dest="safe_mode",
                       help="sanitize literal HTML: 'escape' escapes "
                            "HTML meta chars, 'replace' replaces with an "
                            "[HTML_REMOVED] note")
-    parser.add_option("-x", "--extras", action="append",
+    parser.add_argument("-x", "--extras", action="append",
                       help="Turn on specific extra features (not part of "
                            "the core Markdown spec). See above.")
-    parser.add_option("--use-file-vars",
+    parser.add_argument("--use-file-vars",
                       help="Look for and use Emacs-style 'markdown-extras' "
                            "file var to turn on extras. See "
                            "<https://github.com/trentm/python-markdown2/wiki/Extras>")
-    parser.add_option("--link-patterns-file",
+    parser.add_argument("--link-patterns-file",
                       help="path to a link pattern file")
-    parser.add_option("--self-test", action="store_true",
+    parser.add_argument("--self-test", action="store_true",
                       help="run internal self-tests (some doctests)")
-    parser.add_option("--compare", action="store_true",
+    parser.add_argument("--compare", action="store_true",
                       help="run against Markdown.pl as well (for testing)")
     parser.set_defaults(log_level=logging.INFO, compare=False,
                         encoding="utf-8", safe_mode=None, use_file_vars=False)
-    opts, paths = parser.parse_args()
+    opts = parser.parse_args()
+    paths = opts.paths
     log.setLevel(opts.log_level)
 
     if opts.self_test:
         return _test()
 
     if opts.extras:
         extras = {}
@@ -3042,28 +3126,28 @@
                 link_patterns.append(
                     (_regex_from_encoded_pattern(pat), href))
         finally:
             f.close()
     else:
         link_patterns = None
 
-    from os.path import join, dirname, abspath, exists
+    from os.path import abspath, dirname, exists, join
     markdown_pl = join(dirname(dirname(abspath(__file__))), "test",
                        "Markdown.pl")
     if not paths:
         paths = ['-']
     for path in paths:
         if path == '-':
             text = sys.stdin.read()
         else:
             fp = codecs.open(path, 'r', opts.encoding)
             text = fp.read()
             fp.close()
         if opts.compare:
-            from subprocess import Popen, PIPE
+            from subprocess import PIPE, Popen
             print("==== Markdown.pl ====")
             p = Popen('perl %s' % markdown_pl, shell=True, stdin=PIPE, stdout=PIPE, close_fds=True)
             p.stdin.write(text.encode('utf-8'))
             p.stdin.close()
             perl_html = p.stdout.read().decode('utf-8')
             sys.stdout.write(perl_html)
             print("==== markdown2.py ====")
```

### Comparing `markdown2-2.4.8/setup.py` & `markdown2-2.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/test.py` & `markdown2-2.4.9/test/test.py`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/test_markdown2.py` & `markdown2-2.4.9/test/test_markdown2.py`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/testall.py` & `markdown2-2.4.9/test/testall.py`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/testlib.py` & `markdown2-2.4.9/test/testlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 # - Make the quiet option actually quiet.
 
 __version_info__ = (0, 6, 6)
 __version__ = '.'.join(map(str, __version_info__))
 
 
 import os
-from os.path import join, basename, dirname, abspath, splitext, \
+from os.path import join, basename, abspath, splitext, \
                     isfile, isdir, normpath, exists
 import sys
 import getopt
 import glob
 import time
 import unittest
-import imp
+import importlib
 import logging
 import textwrap
 import traceback
 
 
 
 #---- globals and exceptions
@@ -230,21 +230,20 @@
     Modules are imported with 'testdir' first on sys.path.
     """
     testdir = normpath(testdir)
     for testmod_path in testmod_paths_from_testdir(testdir):
         testmod_name = splitext(basename(testmod_path))[0]
         log.debug("import test module '%s'", testmod_path)
         try:
-            iinfo = imp.find_module(testmod_name, [dirname(testmod_path)])
             testabsdir = abspath(testdir)
             sys.path.insert(0, testabsdir)
             old_dir = os.getcwd()
             os.chdir(testdir)
             try:
-                testmod = imp.load_module(testmod_name, *iinfo)
+                testmod = importlib.import_module(testmod_name)
             finally:
                 os.chdir(old_dir)
                 sys.path.remove(testabsdir)
         except TestSkipped:
             _, ex, _ = sys.exc_info()
             log.warning("'%s' module skipped: %s", testmod_name, ex)
         except Exception:
```

### Comparing `markdown2-2.4.8/test/tm-cases/admonitions.html` & `markdown2-2.4.9/test/tm-cases/admonitions.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/admonitions.text` & `markdown2-2.4.9/test/tm-cases/admonitions.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/admonitions_with_fenced_code_blocks.html` & `markdown2-2.4.9/test/tm-cases/admonitions_with_fenced_code_blocks.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/auto_link_email_with_underscore.html` & `markdown2-2.4.9/test/tm-cases/auto_link_email_with_underscore.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/backslash_escape_html_tags.html` & `markdown2-2.4.9/test/tm-cases/backslash_escape_html_tags.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/basic_safe_mode.html` & `markdown2-2.4.9/test/tm-cases/basic_safe_mode.html`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 <p>[HTML_REMOVED]yowzer![HTML_REMOVED]</p>
 
 <p>blah</p>
 
 <p>[HTML_REMOVED]alert(1)[HTML_REMOVED]</p>
 
-<p><a href="http://example.com&quot;onclick=&quot;alert(1)">link1</a></p>
+<p><a href="#">link1</a></p>
 
 <p><a href="http://example.com" title="title&quot;onclick=&quot;alert(1)">link2</a></p>
 
-<p><a href="http://example.com&gt;[HTML_REMOVED]alert(1)[HTML_REMOVED]">link3</a></p>
+<p><a href="#">link3</a></p>
 
-<p><a href="http://example.com&gt;[HTML_REMOVED]alert(1)[HTML_REMOVED]">link4 &gt;[HTML_REMOVED]alert(1)[HTML_REMOVED]</a></p>
+<p><a href="#">link4 &gt;[HTML_REMOVED]alert(1)[HTML_REMOVED]</a></p>
 
 <p><a href="#">link5</a></p>
 
 <p><a href="#">link6</a></p>
 
 <p><a href="#">link7</a></p>
```

### Comparing `markdown2-2.4.8/test/tm-cases/basic_safe_mode.text` & `markdown2-2.4.9/test/tm-cases/basic_safe_mode.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.html` & `markdown2-2.4.9/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.text` & `markdown2-2.4.9/test/tm-cases/break_on_newline_excessive_br_tags_in_ul.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/consecutive_image_links_issue498.html` & `markdown2-2.4.9/test/tm-cases/consecutive_image_links_issue498.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/consecutive_image_links_issue498.text` & `markdown2-2.4.9/test/tm-cases/consecutive_image_links_issue498.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/cuddled_para_and_list.html` & `markdown2-2.4.9/test/tm-cases/cuddled_para_and_list.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/cuddled_with_para.html` & `markdown2-2.4.9/test/tm-cases/cuddled_with_para.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/cuddled_with_para.text` & `markdown2-2.4.9/test/tm-cases/cuddled_with_para.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/escapes.html` & `markdown2-2.4.9/test/tm-cases/escapes.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/escapes.text` & `markdown2-2.4.9/test/tm-cases/escapes.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue426.html` & `markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue426.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/fenced_code_blocks_issue426.text` & `markdown2-2.4.9/test/tm-cases/fenced_code_blocks_issue426.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight.html` & `markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/fenced_code_blocks_safe_highlight_old.html` & `markdown2-2.4.9/test/tm-cases/fenced_code_blocks_safe_highlight_old.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting.html` & `markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.html` & `markdown2-2.4.9/test/tm-cases/fenced_code_blocks_syntax_highlighting_old.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/footnotes.html` & `markdown2-2.4.9/test/tm-cases/footnotes.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/footnotes_custom.html` & `markdown2-2.4.9/test/tm-cases/footnotes_custom.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/footnotes_letters.html` & `markdown2-2.4.9/test/tm-cases/footnotes_letters.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/footnotes_markup.html` & `markdown2-2.4.9/test/tm-cases/footnotes_markup.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/footnotes_underscores.html` & `markdown2-2.4.9/test/tm-cases/footnotes_underscores.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/hr_spaces.html` & `markdown2-2.4.9/test/tm-cases/hr_spaces.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/hr_spaces.text` & `markdown2-2.4.9/test/tm-cases/hr_spaces.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/html_classes.html` & `markdown2-2.4.9/test/tm-cases/html_classes.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <table class="table table-striped">
-<thead>
+<thead class="table-light">
 <tr>
   <th>Header 1</th>
   <th><em>Header</em> 2</th>
 </tr>
 </thead>
 <tbody>
 <tr>
@@ -14,15 +14,15 @@
   <td>Cell 3</td>
   <td><strong>Cell 4</strong></td>
 </tr>
 </tbody>
 </table>
 
 <table class="table table-striped">
-    <thead>
+    <thead class="table-light">
         <tr>
             <th>Year</th>
             <th>Temperature (low)</th>
             <th>Temperature (high)</th>
         </tr>
     </thead>
     <tbody>
```

### Comparing `markdown2-2.4.8/test/tm-cases/issue276_fenced_code_blocks_in_lists.html` & `markdown2-2.4.9/test/tm-cases/issue276_fenced_code_blocks_in_lists.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/issue54_escape_link_title.html` & `markdown2-2.4.9/test/tm-cases/issue54_escape_link_title.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/link_nofollow.html` & `markdown2-2.4.9/test/tm-cases/link_nofollow.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/link_nofollow.text` & `markdown2-2.4.9/test/tm-cases/link_nofollow.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/lists3.html` & `markdown2-2.4.9/test/tm-cases/lists3.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/lists3.text` & `markdown2-2.4.9/test/tm-cases/lists3.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/long_link.html` & `markdown2-2.4.9/test/tm-cases/long_link.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/long_link.text` & `markdown2-2.4.9/test/tm-cases/long_link.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/markdown_in_html.html` & `markdown2-2.4.9/test/tm-cases/markdown_in_html.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/markdown_in_html.text` & `markdown2-2.4.9/test/tm-cases/markdown_in_html.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/metadata.text` & `markdown2-2.4.9/test/tm-cases/metadata.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/metadata3.text` & `markdown2-2.4.9/test/tm-cases/metadata3.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/mismatched_footnotes.html` & `markdown2-2.4.9/test/tm-cases/mismatched_footnotes.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/numbering.html` & `markdown2-2.4.9/test/tm-cases/numbering.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/numbering.text` & `markdown2-2.4.9/test/tm-cases/numbering.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering_issue471.html` & `markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering_issue471.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/ordered_list_lazy_numbering_issue471.text` & `markdown2-2.4.9/test/tm-cases/ordered_list_lazy_numbering_issue471.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/pyshell_and_fenced_code_blocks.html` & `markdown2-2.4.9/test/tm-cases/pyshell_and_fenced_code_blocks.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/smarty_pants.html` & `markdown2-2.4.9/test/tm-cases/smarty_pants.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/smarty_pants.text` & `markdown2-2.4.9/test/tm-cases/smarty_pants.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/sublist-para.html` & `markdown2-2.4.9/test/tm-cases/sublist-para.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/sublist-para.text` & `markdown2-2.4.9/test/tm-cases/sublist-para.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/tables.html` & `markdown2-2.4.9/test/tm-cases/tables.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/tables.text` & `markdown2-2.4.9/test/tm-cases/tables.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/wavedrom.html` & `markdown2-2.4.9/test/tm-cases/wavedrom.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/wavedrom.text` & `markdown2-2.4.9/test/tm-cases/wavedrom.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/wavedrom_no_embed.html` & `markdown2-2.4.9/test/tm-cases/wavedrom_no_embed.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/wavedrom_no_embed.text` & `markdown2-2.4.9/test/tm-cases/wavedrom_no_embed.text`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/wiki_tables.html` & `markdown2-2.4.9/test/tm-cases/wiki_tables.html`

 * *Files identical despite different names*

### Comparing `markdown2-2.4.8/test/tm-cases/wiki_tables.text` & `markdown2-2.4.9/test/tm-cases/wiki_tables.text`

 * *Files identical despite different names*

