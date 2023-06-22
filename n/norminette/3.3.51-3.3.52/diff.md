# Comparing `tmp/norminette-3.3.51.tar.gz` & `tmp/norminette-3.3.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norminette-3.3.51.tar", last modified: Tue Nov  9 10:00:38 2021, max compression
+gzip compressed data, was "norminette-3.3.52.tar", max compression
```

## Comparing `norminette-3.3.51.tar` & `norminette-3.3.52.tar`

### file list

```diff
@@ -1,89 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 10:00:38.706806 norminette-3.3.51/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-11-09 10:00:24.000000 norminette-3.3.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2021-11-09 10:00:38.706806 norminette-3.3.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-11-09 10:00:24.000000 norminette-3.3.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 10:00:38.694806 norminette-3.3.51/norminette/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21262 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 10:00:38.694806 norminette-3.3.51/norminette/lexer/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/lexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/lexer/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)    17410 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/lexer/lexer.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/lexer/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     7071 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/norm_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 10:00:38.706806 norminette-3.3.51/norminette/rules/
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_assignation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_assignation_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_block_start.py
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_brace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_comment.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_comment_line_len.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_control_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_empty_line.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_enum_var_decl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_expression_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_func_arguments_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_func_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_func_spacing.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_functions_count.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_general_spacing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_global_naming.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_identifier_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_in_header.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_line_count.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_line_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_line_len.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_many_instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_nest_line_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_newline_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)    14947 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_operators_spacing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5482 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_preprocessor_define.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_preprocessor_include.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_preprocessor_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_preprocessor_protection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3452 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_prototype_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_spacing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_struct_naming.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_ternary.py
--rw-r--r--   0 runner    (1001) docker     (121)     6517 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_utype_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_variable_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4984 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/check_variable_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_ambiguous_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_assignation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_block_end.py
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_block_start.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_cast.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_comment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_control_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_empty_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_enum_var_decl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4734 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_expression_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     7858 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_func_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7456 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_func_prototype.py
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_function_call.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_preprocessor_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_ternary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_user_defined_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     7092 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/is_var_declaration.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/rules/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 10:00:38.706806 norminette-3.3.51/norminette/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-11-09 10:00:24.000000 norminette-3.3.51/norminette/tools/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 10:00:38.694806 norminette-3.3.51/norminette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2021-11-09 10:00:38.000000 norminette-3.3.51/norminette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2021-11-09 10:00:38.000000 norminette-3.3.51/norminette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-09 10:00:38.000000 norminette-3.3.51/norminette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-11-09 10:00:38.000000 norminette-3.3.51/norminette.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-09 10:00:38.000000 norminette-3.3.51/norminette.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-09 10:00:38.000000 norminette-3.3.51/norminette.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      939 2021-11-09 10:00:38.706806 norminette-3.3.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-11-09 10:00:24.000000 norminette-3.3.51/setup.py
+-rw-r--r--   0        0        0     1057 2023-06-22 11:35:35.699121 norminette-3.3.52/LICENSE
+-rw-r--r--   0        0        0     1384 2023-06-22 11:35:35.699121 norminette-3.3.52/README.md
+-rw-r--r--   0        0        0      100 2023-06-22 11:35:35.699121 norminette-3.3.52/norminette/__init__.py
+-rw-r--r--   0        0        0     4585 2023-06-22 11:35:35.699121 norminette-3.3.52/norminette/__main__.py
+-rw-r--r--   0        0        0    22189 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/context.py
+-rw-r--r--   0        0        0      191 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/exceptions.py
+-rw-r--r--   0        0        0      173 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/dictionary.py
+-rw-r--r--   0        0        0    18013 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/lexer.py
+-rw-r--r--   0        0        0      626 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/tokens.py
+-rw-r--r--   0        0        0     7072 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/norm_error.py
+-rw-r--r--   0        0        0     4064 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/registry.py
+-rw-r--r--   0        0        0     1041 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/__init__.py
+-rw-r--r--   0        0        0     3080 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_assignation.py
+-rw-r--r--   0        0        0     3234 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_assignation_indent.py
+-rw-r--r--   0        0        0     1609 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_block_start.py
+-rw-r--r--   0        0        0     1894 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_brace.py
+-rw-r--r--   0        0        0     1159 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_comment.py
+-rw-r--r--   0        0        0      664 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_comment_line_len.py
+-rw-r--r--   0        0        0     2572 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_control_statement.py
+-rw-r--r--   0        0        0      541 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_declaration.py
+-rw-r--r--   0        0        0     2521 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_empty_line.py
+-rw-r--r--   0        0        0      834 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_enum_var_decl.py
+-rw-r--r--   0        0        0     2497 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_expression_statement.py
+-rw-r--r--   0        0        0     4684 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_func_arguments_name.py
+-rw-r--r--   0        0        0     2786 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_func_declaration.py
+-rw-r--r--   0        0        0     1682 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_func_spacing.py
+-rw-r--r--   0        0        0      496 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_functions_count.py
+-rw-r--r--   0        0        0      885 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_general_spacing.py
+-rw-r--r--   0        0        0     1182 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_global_naming.py
+-rw-r--r--   0        0        0     2273 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_header.py
+-rw-r--r--   0        0        0     1418 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_identifier_name.py
+-rw-r--r--   0        0        0     1540 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_in_header.py
+-rw-r--r--   0        0        0      562 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_label.py
+-rw-r--r--   0        0        0     1104 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_line_count.py
+-rw-r--r--   0        0        0     2045 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_line_indent.py
+-rw-r--r--   0        0        0      558 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_line_len.py
+-rw-r--r--   0        0        0     1100 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_many_instructions.py
+-rw-r--r--   0        0        0     2938 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_nest_line_indent.py
+-rw-r--r--   0        0        0     1030 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_newline_indent.py
+-rw-r--r--   0        0        0    16112 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_operators_spacing.py
+-rw-r--r--   0        0        0     5546 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_define.py
+-rw-r--r--   0        0        0     2042 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_include.py
+-rw-r--r--   0        0        0     1922 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_indent.py
+-rw-r--r--   0        0        0     2145 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_protection.py
+-rw-r--r--   0        0        0     3452 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_prototype_indent.py
+-rw-r--r--   0        0        0     2394 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_spacing.py
+-rw-r--r--   0        0        0     1218 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_struct_naming.py
+-rw-r--r--   0        0        0      438 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_ternary.py
+-rw-r--r--   0        0        0     6726 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_utype_declaration.py
+-rw-r--r--   0        0        0     2996 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_variable_declaration.py
+-rw-r--r--   0        0        0     5223 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_variable_indent.py
+-rw-r--r--   0        0        0      705 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_ambiguous_declaration.py
+-rw-r--r--   0        0        0     2935 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_assignation.py
+-rw-r--r--   0        0        0     2302 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_block_end.py
+-rw-r--r--   0        0        0     1897 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_block_start.py
+-rw-r--r--   0        0        0     1211 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_cast.py
+-rw-r--r--   0        0        0      464 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_comment.py
+-rw-r--r--   0        0        0     3644 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_control_statement.py
+-rw-r--r--   0        0        0      941 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_declaration.py
+-rw-r--r--   0        0        0      687 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_empty_line.py
+-rw-r--r--   0        0        0     3298 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_enum_var_decl.py
+-rw-r--r--   0        0        0     4819 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_expression_statement.py
+-rw-r--r--   0        0        0     8095 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_func_declaration.py
+-rw-r--r--   0        0        0     7656 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_func_prototype.py
+-rw-r--r--   0        0        0     3286 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_function_call.py
+-rw-r--r--   0        0        0      652 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_label.py
+-rw-r--r--   0        0        0     1180 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_preprocessor_statement.py
+-rw-r--r--   0        0        0      730 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_ternary.py
+-rw-r--r--   0        0        0     2798 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_user_defined_type.py
+-rw-r--r--   0        0        0     7392 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_var_declaration.py
+-rw-r--r--   0        0        0      821 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/rule.py
+-rwxr-xr-x   0        0        0      288 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/run_test.sh
+-rw-r--r--   0        0        0     3382 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/scope.py
+-rw-r--r--   0        0        0      949 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/tools/colors.py
+-rw-r--r--   0        0        0      914 2023-06-22 11:35:35.743118 norminette-3.3.52/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 norminette-3.3.52/PKG-INFO
```

### Comparing `norminette-3.3.51/LICENSE` & `norminette-3.3.52/LICENSE`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/PKG-INFO` & `norminette-3.3.52/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 Metadata-Version: 2.1
 Name: norminette
-Version: 3.3.51
-Summary: Open source norminette to apply 42's norme to C files
+Version: 3.3.52
+Summary: Open source C files linter for 42 Network campuses
 Home-page: https://github.com/42School/norminette
+License: MIT Licence
+Keywords: 42,norminette
 Author: 42
 Author-email: pedago@42.fr
-License: MIT License
-Keywords: 42,norminette
-Platform: UNKNOWN
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Project-URL: Repository, https://github.com/42School/norminette
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # norminette for 42 schools
 
-## Install:
+## Install
 
-Requires python3.7+ (3.7, 3.8, 3.9)
+Requires python3.8+ (3.8, 3.9, 3.10, 3.11)
 
 ### Directly inside your global commands
 
 Install using pip.
 ```shell
 python3 -m pip install --upgrade pip setuptools
 python3 -m pip install norminette
 ```
 
 To upgrade an existing install, use
 ```shell
 python3 -m pip install --upgrade norminette
 ```
 
-### Inside a virtual environment
-
-Using a virtual environment will avoid version conflicts with already globally installed packages.
-
-```shell
-python3 -m venv venv
-source venv/bin/activate
-pip install norminette
-```
-
 ## Usage
 
+- Runs on the current folder and any subfolder:
+
 ```
 norminette
 ```
-Runs on the current folder and any subfolder
+
+- Runs on the given filename(s):
 
 ```
 norminette filename.[c/h]
 ```
-Runs on the given filename(s)
+
+- Prevents stopping on various blocking errors:
 
 ```
 norminette -d
 ```
-Prevents stopping on various blocking errors
+
+- Outputs all the debug logging:
 
 ```
 norminette -dd
 ```
-Outputs all the debug logging
 
 ## Docker usage
 
 ```
 docker build -t norminette .
 cd ~/42/ft_printf
 docker run -v $PWD:/code norminette /code
@@ -84,8 +80,27 @@
  - Post a message on the dedicated slack channel (#norminette-v3-beta)
     
 
 Please try to include as much information as possible (the file on which it crashed, etc)
 
 Feel free to do pull requests if you want to help as well. Make sure that run_test.sh properly runs after your modifications.
 
+## Run for development
+
+This new version uses poetry as a dependency manager.
+
+If you want to contribute:
+
+```shell
+poetry install
+
+# Run dev norminette
+poetry run norminette
+
+# Or... with virtual env
+source .venv/bin/activate
+norminette
+
+# Run tests
+poetry run pytest
+```
```

### Comparing `norminette-3.3.51/norminette/__main__.py` & `norminette-3.3.52/norminette/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import glob
 import os
 import sys
+from importlib.metadata import version
 
 import argparse
 from norminette.lexer import Lexer, TokenError
 from norminette.exceptions import CParsingError
 from norminette.registry import Registry
 from norminette.context import Context
 from norminette.tools.colors import colors
-from norminette import __version__
+
+from pathlib import Path
 
 import _thread
 from threading import Event
 import time
 
 
 has_err = False
@@ -34,25 +36,30 @@
         action="append",
         nargs="*",
     )
     parser.add_argument(
         "-d",
         "--debug",
         action="count",
-        help="Debug output (multiple values available)",
+        help="Debug output (-dd outputs the whole tokenization and such, used for developping)",
         default=0,
     )
     parser.add_argument(
         "-o",
         "--only-filename",
         action="store_true",
         help="By default norminette displays the full path to the file, this allows to show only filename",
         default=False,
     )
-    parser.add_argument("-v", "--version", action="version", version="norminette " + str(__version__))
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version="norminette " + version("norminette"),
+    )
     parser.add_argument(
         "--cfile",
         action="store",
         help="Store C file content directly instead of filename",
     )
     parser.add_argument(
         "--hfile",
@@ -68,19 +75,19 @@
     args = parser.parse_args()
     registry = Registry()
     targets = []
     has_err = None
     content = None
 
     debug = args.debug
-    if args.cfile != None or args.hfile != None:
+    if args.cfile is not None or args.hfile is not None:
         if args.filename:
-            targets = [ args.filename ]
+            targets = [args.filename]
         else:
-            targets = [ "file.c" ] if args.cfile else ["file.h"]
+            targets = ["file.c"] if args.cfile else ["file.h"]
         content = args.cfile if args.cfile else args.hfile
     else:
         args.file = args.file[0]
         if args.file == [[]] or args.file == []:
             targets = glob.glob("**/*.[ch]", recursive=True)
         else:
             for arg in args.file:
@@ -95,30 +102,30 @@
     event = []
     for target in targets:
         if target[-2:] not in [".c", ".h"]:
             print(f"Error: {target} is not valid C or C header file")
         else:
             try:
                 event.append(Event())
-                if content == None:
+                if content is None:
                     with open(target) as f:
                         try:
                             source = f.read()
                         except Exception as e:
-                            print ("Error: File could not be read: ", e)
+                            print("Error: File could not be read: ", e)
                             sys.exit(0)
                 else:
                     source = content
                 try:
                     lexer = Lexer(source)
                     tokens = lexer.get_tokens()
                 except KeyError as e:
-                    print ("Error while parsing file:", e)
+                    print("Error while parsing file:", e)
                     sys.exit(0)
-                if args.only_filename == True:
+                if args.only_filename is True:
                     # target = target.split("/")[-1]
                     target = Path(target).name
                 context = Context(target, tokens, debug, args.R)
                 registry.run(context, source)
                 event[-1].set()
                 if context.errors:
                     has_err = True
@@ -126,15 +133,15 @@
                 has_err = True
                 print(target + f": Error!\n\t{colors(e.msg, 'red')}")
                 event[-1].set()
             except CParsingError as e:
                 has_err = True
                 print(target + f": Error!\n\t{colors(e.msg, 'red')}")
                 event[-1].set()
-            except KeyboardInterrupt as e:
+            except KeyboardInterrupt:
                 event[-1].set()
                 sys.exit(1)
     sys.exit(1 if has_err else 0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `norminette-3.3.51/norminette/context.py` & `norminette-3.3.52/norminette/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from norminette.exceptions import CParsingError
-from norminette.lexer.dictionary import operators
 from norminette.norm_error import NormError, NormWarning
 from norminette.scope import GlobalScope, ControlStructure
 from norminette.tools.colors import colors
+
 types = [
     "CHAR",
     "DOUBLE",
     "ENUM",
     "FLOAT",
     "INT",
     "UNION",
@@ -133,19 +133,18 @@
 
 sign_specifiers = ["SIGNED", "UNSIGNED"]
 
 whitespaces = ["SPACE", "TAB", "ESCAPED_NEWLINE", "NEWLINE"]
 
 arg_separator = ["COMMA", "CLOSING_PARENTHESIS"]
 
-import pdb
 
 class Context:
     def __init__(self, filename, tokens, debug=0, added_value=[]):
-        #Header relative informations
+        # Header relative informations
         self.header_started = False
         self.header_parsed = False
         self.header = ""
         # File relative informations
         self.filename = filename
         self.filetype = filename.split(".")[-1]  # ?
         self.tokens = tokens
@@ -162,15 +161,17 @@
         self.func_alignment = 0
         self.sub = None
         self.fname_pos = 0
         self.arg_pos = [0, 0]
 
         # Preprocessor handling
         self.preproc_scope_indent = 0
-        self.skip_define_error = True if added_value is not None and "CheckDefine" in added_value else False
+        self.skip_define_error = (
+            True if added_value is not None and "CheckDefine" in added_value else False
+        )
 
     def peek_token(self, pos):
         return self.tokens[pos] if pos < len(self.tokens) else None
 
     def pop_tokens(self, stop):
         self.tokens = self.tokens[stop:]
 
@@ -192,15 +193,17 @@
         nests = 0
         for i in range(0, self.tkn_scope):
             tkn = self.peek_token(i)
             if self.check_token(i, ["LBRACKET", "LPARENTHESIS", "LBRACE"]) is True:
                 nests += 1
             if self.check_token(i, ["RBRACKET", "RPARENTHESIS", "RBRACE"]) is True:
                 nests -= 1
-            if tkn.type == value and (nested == True or (nests == 0 and nested == False)):
+            if tkn.type == value and (
+                nested is True or (nests == 0 and nested is False)
+            ):
                 return i
         return -1
 
     def new_error(self, errno, tkn):
         self.errors.append(NormError(errno, tkn.pos[0], tkn.pos[1]))
 
     def new_warning(self, errno, tkn):
@@ -221,15 +224,19 @@
             or self.history[-1] == "IsComment"
             or self.history[-1] == "IsPreprocessorStatement"
         ):
             return
         if self.sub is not None:
             self.scope = self.sub
             self.sub = None
-        if type(self.scope) is ControlStructure and self.scope.multiline is False and self.scope.instructions > 0:
+        if (
+            type(self.scope) is ControlStructure
+            and self.scope.multiline is False
+            and self.scope.instructions > 0
+        ):
             self.scope = self.scope.outer()
             self.sub = None
             self.update()
         self.arg_pos = [0, 0]
 
     def dprint(self, rule, pos):
         """Debug printing, shows the primary rules that succeed in matching
@@ -251,30 +258,30 @@
                 i = 0
             else:
                 print(t, end=" ")
                 i += 1
         if pos - 1 < len(self.tokens) and self.tokens[pos - 1].type != "NEWLINE":
             print("")
         elif len(self.tokens) == 1 and self.tokens[-1].type != "NEWLINE":
-            print ("")
+            print("")
 
     def eol(self, pos):
         """Skips white space characters (tab, space) until end of line
         (included) or any other token (excluded)
         """
         while self.check_token(pos, ["TAB", "SPACE", "NEWLINE"]) is True:
             if self.check_token(pos, "NEWLINE"):
                 pos += 1
                 break
             pos += 1
         return pos
 
     def skip_ws(self, pos, nl=False):
         ws = whitespaces[:]
-        if nl == False:
+        if nl is False:
             ws.remove("NEWLINE")
         while self.check_token(pos, ws):
             pos += 1
         return pos
 
     def skip_nest_reverse(self, pos):
         """Skips anything between two brackets, parentheses or braces starting
@@ -310,18 +317,18 @@
     def skip_nest(self, pos):
         """Skips anything between two brackets, parentheses or braces starting
         at 'pos', if the brackets, parentheses or braces are not closed or
         are closed in the wrong order an error shall be raised
         """
         lbrackets = ["LBRACKET", "LBRACE", "LPARENTHESIS"]
         rbrackets = ["RBRACKET", "RBRACE", "RPARENTHESIS"]
-        try:
-            c = self.peek_token(pos).type
-        except:
-            raise CParsingError(f"Error: Code ended unexpectedly.")
+        # try:
+        c = self.peek_token(pos).type
+        # except:
+        # raise CParsingError(f"Error: Code ended unexpectedly.")
         if c not in lbrackets:
             return pos
         c = rbrackets[lbrackets.index(c)]
         i = pos + 1
         while self.peek_token(i) is not None:
             if self.check_token(i, lbrackets) is True:
                 i = self.skip_nest(i)
@@ -403,17 +410,19 @@
                 if self.check_token(i, "IDENTIFIER") is True:
                     i += 1
                     return True, i
             if self.check_token(i, types + ["IDENTIFIER"]) is False:
                 return False, 0
             if self.check_token(i, "IDENTIFIER") is True:
                 i += 1
-                #i = self.skip_ws(i)
+                # i = self.skip_ws(i)
                 return True, i + 1
-            while self.check_token(i, types + whitespaces + ["MULT", "BWISE_AND"]) is True:
+            while (
+                self.check_token(i, types + whitespaces + ["MULT", "BWISE_AND"]) is True
+            ):
                 i += 1
             tmp = self.skip_misc_specifier(i, nl=nl)
             if tmp == i:
                 return True, i - 1
             else:
                 return True, tmp
 
@@ -458,32 +467,37 @@
                 ["PLUS", "MINUS", "BWISE_OR", "BWISE_AND", "BWISE_NOT", "BWISE_XOR"],
             )
             is False
         ):
             return False
         pos += 1
         pos = self.skip_ws(pos, nl=False)
-        if self.check_token(pos, ["IDENTIFIER", "CONSTANT", "MULT", "BWISE_AND"]) is False:
+        if (
+            self.check_token(pos, ["IDENTIFIER", "CONSTANT", "MULT", "BWISE_AND"])
+            is False
+        ):
             return False
         pos = start - 1
         while (self.check_token(pos, ["SPACE", "TAB"])) is True:
             pos -= 1
         if self.check_token(pos, glued) is True:
             return True
         return False
 
     def is_operator(self, pos):
         """
         Returns True if the given operator (among '*&') is an actual operator,
         and returns False if said operator is a pointer/adress indicator
         """
-        i = 0
         start = pos + 1
         pos -= 1
-        if self.history[-1] == "IsFuncPrototype" or self.history[-1] == "IsFuncDeclaration":
+        if (
+            self.history[-1] == "IsFuncPrototype"
+            or self.history[-1] == "IsFuncDeclaration"
+        ):
             return False
         if self.check_token(start, ["RPARENTHESIS", "MULT"]) is True:
             return False
         start = self.skip_ws(start, nl=False)
         if self.check_token(start, ["SIZEOF"]) is True:
             return True
         if self.history[-1] == "IsVarDeclaration":
@@ -494,37 +508,61 @@
                 if self.check_token(tmp, ["RBRACKET", "RPARENTHESIS"]) is True:
                     tmp = self.skip_nest_reverse(tmp) - 1
                 if self.check_token(tmp, ["ASSIGN"]) is True:
                     right_side = True
                 if self.check_token(tmp, "LBRACKET") is True:
                     bracketed = True
                 tmp -= 1
-            if right_side == False and bracketed == False:
+            if right_side is False and bracketed is False:
                 return False
         skip = 0
         value_before = False
         while pos > 0:
             if self.check_token(pos, ["RBRACKET", "RPARENTHESIS"]) is True:
                 value_before = True
                 pos = self.skip_nest_reverse(pos) - 1
-                if self.check_token(pos + 1, "LPARENTHESIS") is True and self.parenthesis_contain(pos + 1)[0] == "variable":
+                if (
+                    self.check_token(pos + 1, "LPARENTHESIS") is True
+                    and self.parenthesis_contain(pos + 1)[0] == "variable"
+                ):
                     return True
-                if self.check_token(pos + 1, "LPARENTHESIS") is True and self.parenthesis_contain(pos + 1)[0] == "cast":
+                if (
+                    self.check_token(pos + 1, "LPARENTHESIS") is True
+                    and self.parenthesis_contain(pos + 1)[0] == "cast"
+                ):
                     return False
                 skip = 1
-            if self.check_token(pos, ["IDENTIFIER", "CONSTANT", "SIZEOF", "CHAR_CONST"]) is True:
-                if self.check_token(pos, "IDENTIFIER") is True and self.check_token(pos + 1, "TAB") is True:
+            if (
+                self.check_token(
+                    pos, ["IDENTIFIER", "CONSTANT", "SIZEOF", "CHAR_CONST"]
+                )
+                is True
+            ):
+                if (
+                    self.check_token(pos, "IDENTIFIER") is True
+                    and self.check_token(pos + 1, "TAB") is True
+                ):
                     return False
                 return True
-            if self.check_token(pos, ["COMMA", "LPARENTHESIS", "LBRACKET"] + operators) is True and skip == 1 and self.parenthesis_contain(pos + 1)[0] != "cast":
+            if (
+                self.check_token(pos, ["COMMA", "LPARENTHESIS", "LBRACKET"] + operators)
+                is True
+                and skip == 1
+                and self.parenthesis_contain(pos + 1)[0] != "cast"
+            ):
                 return True
-            if self.check_token(pos, ["LBRACKET", "LPARENTHESIS", "MULT", "BWISE_AND", "COMMA"] + operators + types):
+            if self.check_token(
+                pos,
+                ["LBRACKET", "LPARENTHESIS", "MULT", "BWISE_AND", "COMMA"]
+                + operators
+                + types,
+            ):
                 return False
             pos -= 1
-        if value_before == True:
+        if value_before is True:
             return True
         else:
             return False
 
     def parenthesis_contain(self, i, ret_store=None):
         """
         Explore parenthesis to return its content
@@ -542,79 +580,97 @@
         pointer = None
         sizeof = False
         id_only = True
         if self.check_token(start - 1, "SIZEOF") is True:
             sizeof = True
         i = self.skip_ws(i)
         while deep > 0 and self.peek_token(i) is not None:
-            #print (self.peek_token(i), deep, identifier, self.check_token(i, "NULL"))
+            # print (self.peek_token(i), deep, identifier, self.check_token(i, "NULL"))
             if self.check_token(i, "RPARENTHESIS"):
                 deep -= 1
             elif self.check_token(i, "LPARENTHESIS"):
                 deep += 1
-                #if identifier is not None and deep >= 0:
-                    #return "pointer", self.skip_nest(start)
-            elif deep > 1 and identifier == True and self.check_token(i, ["NULL", "IDENTIFIER"]):
+                # if identifier is not None and deep >= 0:
+                # return "pointer", self.skip_nest(start)
+            elif (
+                deep > 1
+                and identifier is True
+                and self.check_token(i, ["NULL", "IDENTIFIER"])
+            ):
                 return "fct_call", self.skip_nest(start)
-            elif self.check_token(i, "COMMA") and nested_id == True:
+            elif self.check_token(i, "COMMA") and nested_id is True:
                 return "function", self.skip_nest(start)
             elif self.check_token(i, assigns) and deep == 1:
                 return "assign", self.skip_nest(start)
             elif self.check_token(i, "PTR") and deep == 1:
                 return "variable", self.skip_nest(start)
             elif self.check_token(i, "COMMA"):
                 return None, self.skip_nest(start)
             elif self.check_token(i, ws):
                 pass
             elif self.check_token(i, types):
                 tmp = start - 1
-                while self.check_token(tmp, ["SPACE", "TAB"]) == True:
+                while self.check_token(tmp, ["SPACE", "TAB"]) is True:
                     tmp -= 1
-                if self.check_token(tmp, "SIZEOF") == True:
+                if self.check_token(tmp, "SIZEOF") is True:
                     return None, self.skip_nest(start)
                 tmp = start + 1
                 while self.check_token(tmp, "RPARENTHESIS") is False:
                     if self.check_token(tmp, ["LPARENTHESIS", "IDENTIFIER"]) is True:
                         return None, self.skip_nest(start)
                     tmp += 1
                 if deep == 1:
                     return "cast", self.skip_nest(start)
             elif self.check_token(i, "IDENTIFIER"):
                 tmp = i + 1
-                if (identifier is not True and pointer == True) or ret_store is not None:
+                if (
+                    identifier is not True and pointer is True
+                ) or ret_store is not None:
                     nested_id = True
-                if identifier is not True and self.check_token(tmp, "RPARENTHESIS") and self.scope.name == "Function" and deep == 1 and pointer == None and sizeof == False:
+                if (
+                    identifier is not True
+                    and self.check_token(tmp, "RPARENTHESIS")
+                    and self.scope.name == "Function"
+                    and deep == 1
+                    and pointer is None
+                    and sizeof is False
+                ):
                     tmp = self.skip_nest(start) + 1
                     tmp = self.skip_ws(tmp)
-                    if self.check_token(tmp, ["IDENTIFIER", "CONSTANT", "MINUS", "PLUS"]) is False:
+                    if (
+                        self.check_token(
+                            tmp, ["IDENTIFIER", "CONSTANT", "MINUS", "PLUS"]
+                        )
+                        is False
+                    ):
                         return None, self.skip_nest(start)
                     return "cast", self.skip_nest(start)
                 identifier = True
                 tmp = self.skip_ws(tmp)
-                if pointer == True:
+                if pointer is True:
                     if self.check_token(tmp, "LBRACKET"):
                         tmp = self.skip_nest(tmp)
                         tmp += 1
                     while self.check_token(tmp, "RPARENTHESIS"):
                         tmp += 1
                         # start = tmp
                     tmp = self.skip_ws(tmp)
                     if self.check_token(tmp, "LPARENTHESIS"):
                         return "pointer", self.skip_nest(start)
                     elif self.check_token(tmp, "RPARENTHESIS"):
                         return None, self.skip_nest(start)
             elif self.check_token(i, ["MULT", "BWISE_AND"]):
                 tmp = i + 1
                 pointer = True
-                if identifier != None:
+                if identifier is not None:
                     tmp = start - 1
-                    while self.check_token(tmp, ["SPACE", "TAB"]) == True:
+                    while self.check_token(tmp, ["SPACE", "TAB"]) is True:
                         tmp -= 1
-                    if self.check_token(tmp, "SIZEOF") == True:
+                    if self.check_token(tmp, "SIZEOF") is True:
                         return None, self.skip_nest(start)
                     tmp = self.skip_ws(i + 1)
                     if self.check_token(tmp, "RPARENTHESIS") is True:
                         return "cast", self.skip_nest(start)
             i += 1
-        if identifier == True and id_only == True:
+        if identifier is True and id_only is True:
             return "var", self.skip_nest(start)
         return None, self.skip_nest(start)
```

### Comparing `norminette-3.3.51/norminette/lexer/dictionary.py` & `norminette-3.3.52/norminette/lexer/dictionary.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/lexer/lexer.py` & `norminette-3.3.52/norminette/lexer/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import string
-import pdb
 
 from norminette.lexer.dictionary import brackets
 from norminette.lexer.dictionary import keywords
 from norminette.lexer.dictionary import operators
 from norminette.lexer.dictionary import preproc_keywords
 from norminette.lexer.tokens import Token
 
@@ -53,15 +52,17 @@
         """Pop a character that's been read by increasing self.__pos,
         for escaped characters self.__pos will be increased twice
         """
         if self.peek_char() == "\t":
             # this calculates the 'visual offset' of a tab based on it's
             # position on the line, if there's an easier way to calculate this
             # you're welcome
-            self.__line_pos = int((self.__line_pos + 4 - (self.__line_pos - 1) % 4) * 5 / 5)
+            self.__line_pos = int(
+                (self.__line_pos + 4 - (self.__line_pos - 1) % 4) * 5 / 5
+            )
         else:
             self.__line_pos += 1
         if self.__pos < self.len and self.src[self.__pos] == "\\":
             self.__pos += 1
         self.__pos += 1
         return self.peek_char()
 
@@ -135,15 +136,15 @@
             tkn_value += self.peek_char()
             if self.peek_char() == "\n":
                 self.pop_char()
                 self.tokens.append(Token("TKN_ERROR", pos))
                 return
             if self.peek_char() == "'":
                 for i in tkn_value:
-                    if i == '\\':
+                    if i == "\\":
                         self.__line_pos += 1
                 self.pop_char()
                 self.tokens.append(Token("CHAR_CONST", pos, tkn_value))
                 return
             self.pop_char()
         raise TokenError(pos)
 
@@ -164,35 +165,45 @@
         Plus/minus operators ('+'/'-') can prefix any of those tokens
 
         a numeric constant could start with a '.' (dot character)
         """
         pos = self.line_pos()
         tkn_value = ""
         bucket = ".0123456789aAbBcCdDeEfFlLuUxX-+"
-        while self.peek_char() and (self.peek_char() in bucket or self.peek_char() == "\\\n"):
+        while self.peek_char() and (
+            self.peek_char() in bucket or self.peek_char() == "\\\n"
+        ):
             if self.peek_char() in "xX":
                 if tkn_value.startswith("0") is False or len(tkn_value) > 1:
                     raise TokenError(pos)
                 for c in "xX":
                     if c in tkn_value:
                         raise TokenError(pos)
 
             elif self.peek_char() in "bB":
-                if tkn_value != "0" and tkn_value.startswith("0x") is False and tkn_value.startswith("0X") is False:
+                if (
+                    tkn_value != "0"
+                    and tkn_value.startswith("0x") is False
+                    and tkn_value.startswith("0X") is False
+                ):
                     raise TokenError(pos)
 
             elif self.peek_char() in "+-":
                 if (
                     tkn_value.endswith("e") is False
                     and tkn_value.endswith("E") is False
                     or self.peek_sub_string(2) in ["++", "--"]
                 ):
                     break
 
-            elif self.peek_char() in "eE" and "0x" not in tkn_value and "0X" not in tkn_value:
+            elif (
+                self.peek_char() in "eE"
+                and "0x" not in tkn_value
+                and "0X" not in tkn_value
+            ):
                 if (
                     "e" in tkn_value
                     or "E" in tkn_value
                     or "f" in tkn_value
                     or "F" in tkn_value
                     or "u" in tkn_value
                     or "U" in tkn_value
@@ -207,33 +218,44 @@
                     lcount > 1
                     or (lcount == 1 and tkn_value[-1] not in "lL")
                     or ("f" in tkn_value or "F" in tkn_value)
                     and "0x" not in tkn_value
                     and "0X" not in tkn_value
                 ):
                     raise TokenError(pos)
-                elif self.peek_char() == "l" and "L" in tkn_value or self.peek_char() == "L" and "l" in tkn_value:
+                elif (
+                    self.peek_char() == "l"
+                    and "L" in tkn_value
+                    or self.peek_char() == "L"
+                    and "l" in tkn_value
+                ):
                     raise TokenError(pos)
 
             elif self.peek_char() in "uU":
                 if (
                     "u" in tkn_value
                     or "U" in tkn_value
                     or (
-                        ("e" in tkn_value or "E" in tkn_value or "f" in tkn_value or "F" in tkn_value)
+                        (
+                            "e" in tkn_value
+                            or "E" in tkn_value
+                            or "f" in tkn_value
+                            or "F" in tkn_value
+                        )
                         and ("0x" not in tkn_value and "0X" not in tkn_value)
                     )
                 ):
                     raise TokenError(pos)
 
             elif self.peek_char() in "Ff":
                 if (
                     tkn_value.startswith("0x") is False
                     and tkn_value.startswith("0X") is False
                     and ("." not in tkn_value or "f" in tkn_value or "F" in tkn_value)
+                    and "e" not in tkn_value
                     or "u" in tkn_value
                     or "U" in tkn_value
                     or "l" in tkn_value
                     or "L" in tkn_value
                 ):
                     raise TokenError(pos)
 
@@ -258,15 +280,19 @@
                 raise TokenError(pos)
 
             elif self.peek_char() == "." and "." in tkn_value:
                 raise TokenError(pos)
 
             tkn_value += self.peek_char()
             self.pop_char()
-        if tkn_value[-1] in "eE" and tkn_value.startswith("0x") is False or tkn_value[-1] in "xX":
+        if (
+            tkn_value[-1] in "eE"
+            and tkn_value.startswith("0x") is False
+            or tkn_value[-1] in "xX"
+        ):
             raise TokenError(pos)
         else:
             self.tokens.append(Token("CONSTANT", pos, tkn_value))
 
     def mult_comment(self):
         pos = self.line_pos()
         self.pop_char(), self.pop_char()
@@ -295,27 +321,28 @@
         self.pop_char(), self.pop_char()
         while self.peek_char() is not None:
             if self.peek_char() == "\n":
                 self.tokens.append(Token("COMMENT", pos, tkn_value))
                 return
             tkn_value += self.peek_char()
             self.pop_char()
-        if (self.__pos == self.len):
+        if self.__pos == self.len:
             self.tokens.append(Token("COMMENT", pos, tkn_value))
             return
         raise TokenError(pos)
 
     def identifier(self):
         """Identifiers can start with any letter [a-z][A-Z] or an underscore
         and contain any letters [a-z][A-Z] digits [0-9] or underscores
         """
         pos = self.line_pos()
         tkn_value = ""
         while self.peek_char() and (
-            self.peek_char() in string.ascii_letters + "0123456789_" or self.peek_char() == "\\\n"
+            self.peek_char() in string.ascii_letters + "0123456789_"
+            or self.peek_char() == "\\\n"
         ):
             if self.peek_char() == "\\\n":
                 self.pop_char()
                 continue
             tkn_value += self.peek_char()
             self.pop_char()
         if tkn_value in keywords:
@@ -328,15 +355,14 @@
         """Operators can be made of one or more sign, so the longest operators
         need to be looked up for first in order to avoid false positives
         eg: '>>' being understood as two 'MORE_THAN' operators instead of
             one 'RIGHT_SHIFT' operator
         """
         pos = self.line_pos()
         if self.peek_char() in ".+-*/%<>^&|!=":
-
             if self.peek_sub_string(3) in [">>=", "<<=", "..."]:
                 self.tokens.append(Token(operators[self.peek_sub_string(3)], pos))
                 self.pop_char(), self.pop_char(), self.pop_char()
 
             elif self.peek_sub_string(2) in [">>", "<<", "->"]:
                 self.tokens.append(Token(operators[self.peek_sub_string(2)], pos))
                 self.pop_char(), self.pop_char()
@@ -377,28 +403,33 @@
                 break
         if len(tkn_value) <= 1:
             raise TokenError(self.line_pos())
         tkn_key = tkn_value[1:].split()[0]
         if tkn_key not in preproc_keywords and tkn_key[: len("include")] != "include":
             raise TokenError(self.line_pos())
         else:
-            if tkn_key not in preproc_keywords and tkn_key[: len("include")] == "include":
+            if (
+                tkn_key not in preproc_keywords
+                and tkn_key[: len("include")] == "include"
+            ):
                 tkn_key = "include"
             self.tokens.append(Token(preproc_keywords.get(tkn_key), pos, tkn_value))
 
     def get_next_token(self):
         """Peeks one character and tries to match it to a token type,
         if it doesn't match any of the token types, an error will be raised
         and current file's parsing will stop
         """
         while self.peek_char() is not None:
             if self.is_string():
                 self.string()
 
-            elif (self.peek_char().isalpha() and self.peek_char().isascii()) or self.peek_char() == "_":
+            elif (
+                self.peek_char().isalpha() and self.peek_char().isascii()
+            ) or self.peek_char() == "_":
                 self.identifier()
 
             elif self.is_constant():
                 self.constant()
 
             elif self.is_char_constant():
                 self.char_constant()
```

### Comparing `norminette-3.3.51/norminette/lexer/tokens.py` & `norminette-3.3.52/norminette/lexer/tokens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-from norminette.lexer.dictionary import brackets
-from norminette.lexer.dictionary import keywords
-from norminette.lexer.dictionary import operators
-from norminette.lexer.dictionary import preproc_keywords
-
-
 class Token:
     def __init__(self, tkn_type, pos, tkn_value=None):
         self.type = str(tkn_type)
         self.pos = pos
         if tkn_value is not None:
             self.value = str(tkn_value)
             self.length = len(tkn_value)
```

### Comparing `norminette-3.3.51/norminette/norm_error.py` & `norminette-3.3.52/norminette/norm_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             self.error_pos = f"(line: {(str(self.line)).rjust(3)}):\t "
         self.prefix = f"Error: {self.errno:<20} {self.error_pos:>21}"
         self.error_msg = f"{errors.get(self.errno, 'ERROR NOT FOUND')}"
 
     def __str__(self):
         return self.prefix + self.error_msg
 
+
 class NormWarning:
     def __init__(self, errno, line, col=None):
         self.errno = errno
         self.line = line
         self.col = col
         if col is not None:
             self.error_pos = f"(line: {(str(self.line)).rjust(3)}, col: {(str(self.col)).rjust(3)}):\t"
```

### Comparing `norminette-3.3.51/norminette/registry.py` & `norminette-3.3.52/norminette/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 if type(context.scope) not in rule.scope and rule.scope != []:
                     continue
                 ret, jump = self.run_rules(context, rule)
                 if ret is True:
                     if unrecognized_tkns != []:
                         if context.debug == 0:
                             raise CParsingError(
-                                f"Error: Unrecognized line {unrecognized_tkns[0].pos} while parsing line {unrecognized_tkns}"
+                                f"Error: Unrecognized line {unrecognized_tkns[0].pos} while parsing line {unrecognized_tkns}"  # noqa: E501
                             )
                         print("uncaught -> ", context.filename)
                         print("uncaught -> ", unrecognized_tkns)
                         unrecognized_tkns = []
                     context.dprint(rule.name, jump)
                     context.update()
                     context.pop_tokens(jump)
@@ -86,13 +86,15 @@
             print(context.debug)
             if context.debug > 0:
                 print("uncaught ->", unrecognized_tkns)
         if context.errors == []:
             print(context.filename + ": OK!")
         else:
             print(context.filename + ": Error!")
-            context.errors = sorted(context.errors + context.warnings, key=cmp_to_key(sort_errs))
+            context.errors = sorted(
+                context.errors + context.warnings, key=cmp_to_key(sort_errs)
+            )
             for err in context.errors:
                 print(err)
             # context.warnings = sorted(context.warnings, key=cmp_to_key(sort_errs))
             # for warn in context.warnings:
-            #     print (warn)
+            #     print (warn)
```

### Comparing `norminette-3.3.51/norminette/rules/__init__.py` & `norminette-3.3.52/norminette/rules/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,9 +26,11 @@
     mod_name = f.split(os.path.sep)[-1].split(".")[0]
     class_name = "".join([s.capitalize() for s in mod_name.split("_")])
     module = importlib.import_module("norminette.rules." + mod_name)
     rule = getattr(module, class_name)
     primary_rules[class_name] = rule()
 
 
-primary_rules = [v for k, v in sorted(primary_rules.items(), key=lambda item: -item[1].priority)]
-__all__ = ["rules", "primary_rules"]
+primary_rules = [
+    v for k, v in sorted(primary_rules.items(), key=lambda item: -item[1].priority)
+]
+__all__ = ["rules", "primary_rules", "Rule", "PrimaryRule"]
```

### Comparing `norminette-3.3.51/norminette/rules/check_assignation.py` & `norminette-3.3.52/norminette/rules/check_assignation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from norminette.rules import Rule
-import pdb
 
 assigns = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
     "ADD_ASSIGN",
     "SUB_ASSIGN",
     "MUL_ASSIGN",
@@ -11,18 +10,15 @@
     "MOD_ASSIGN",
     "AND_ASSIGN",
     "XOR_ASSIGN",
     "OR_ASSIGN",
     "ASSIGN",
 ]
 
-special_assigns = [
-    "INC",
-    "DEC"
-]
+special_assigns = ["INC", "DEC"]
 
 
 class CheckAssignation(Rule):
     def __init__(self):
         super().__init__()
         self.depends_on = ["IsAssignation"]
 
@@ -32,55 +28,63 @@
         while context.check_token(i, "RBRACE") is False and deep > 0:
             i += 1
         return True, i
 
     def check_assign_right(self, context, i, mini_assign=False):
         tmp_typ = None
         start = 0
-        full_assign = False
         while context.check_token(i, "SEMI_COLON") is False:
             typ = None
             if context.check_token(i, "LBRACE"):
                 ret, i = self.check_brace_assign(context, i)
-                if ret == False:
+                if ret is False:
                     return True, i
                 break
             if context.check_token(i, "LPARENTHESIS") is True:
                 start = i
                 tmp_typ, i = context.parenthesis_contain(i)
-                if tmp_typ != None:
+                if tmp_typ is not None:
                     typ = tmp_typ
                 if tmp_typ == "assign":
                     context.new_error("MULT_ASSIGN_LINE", context.peek_token(start))
                 if tmp_typ is None:
                     tmp = start + 1
-                    while context.peek_token(tmp) and context.check_token(tmp, "RPARENTHESIS") is False:
-                        if context.check_token(tmp, "COMMA") is True and typ is not None:
+                    while (
+                        context.peek_token(tmp)
+                        and context.check_token(tmp, "RPARENTHESIS") is False
+                    ):
+                        if (
+                            context.check_token(tmp, "COMMA") is True
+                            and typ is not None
+                        ):
                             context.new_error("TOO_MANY_INSTR", context.peek_token(tmp))
                         tmp += 1
             if context.check_token(i, assigns) is True:
-                if mini_assign == True:
+                if mini_assign is True:
                     mini_assign = False
                 else:
                     context.new_error("MULT_ASSIGN_LINE", context.peek_token(i))
             if context.check_token(i, special_assigns) is True:
-                if mini_assign == True:
+                if mini_assign is True:
                     context.new_error("MULT_ASSIGN_LINE", context.peek_token(i))
             i += 1
         return False, 0
 
     def run(self, context):
         """
         Only one assignation at a time
         Unless the variable is static (or global), you cannot assign its value when you declare it.
         """
         i = 0
         assign_present = False
         mini_assign = False
         while context.check_token(i, "SEMI_COLON") is False:
-            if context.check_token(i, assigns + special_assigns) is True and assign_present == False:
+            if (
+                context.check_token(i, assigns + special_assigns) is True
+                and assign_present is False
+            ):
                 assign_present = True
                 if context.check_token(i, special_assigns):
                     mini_assign = True
                 return self.check_assign_right(context, i + 1, mini_assign)
             i += 1
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_assignation_indent.py` & `norminette-3.3.52/norminette/rules/check_assignation_indent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pdb
-
 from norminette.rules import Rule
 from norminette.exceptions import CParsingError
 
 
 operators = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
@@ -43,15 +41,20 @@
 
 nest_kw = ["RPARENTHESIS", "LPARENTHESIS", "NEWLINE"]
 
 
 class CheckAssignationIndent(Rule):
     def __init__(self):
         super().__init__()
-        self.depends_on = ["IsAssignation", "IsFuncPrototype", "IsFunctionCall", "IsVarDeclaration"]
+        self.depends_on = [
+            "IsAssignation",
+            "IsFuncPrototype",
+            "IsFunctionCall",
+            "IsVarDeclaration",
+        ]
 
     def run(self, context):
         """
         Declared variables must be aligned using tabs with other variables on the same scope
         """
         i = 0
         expected = context.scope.indent
@@ -69,22 +72,34 @@
                 if context.check_token(tmp, "COMMA"):
                     context.new_error("COMMA_START_LINE", context.peek_token(i))
                 got = 0
                 i += 1
                 while context.check_token(i + got, "TAB") is True:
                     got += 1
                 if context.peek_token(i + got) is None:
-                    raise CParsingError(f"Error: Unexpected EOF l.{context.peek_token(i - 1).pos[0]}")
-                if context.check_token(i + got, ["LBRACKET", "RBRACKET", "LBRACE", "RBRACE"]):
+                    raise CParsingError(
+                        f"Error: Unexpected EOF l.{context.peek_token(i - 1).pos[0]}"
+                    )
+                if context.check_token(
+                    i + got, ["LBRACKET", "RBRACKET", "LBRACE", "RBRACE"]
+                ):
                     nest -= 1
-                if got > nest or (got > nest + 1 and context.history[-1] in ["IsAssignation", "IsVarDeclaration"]):
+                if got > nest or (
+                    got > nest + 1
+                    and context.history[-1] in ["IsAssignation", "IsVarDeclaration"]
+                ):
                     context.new_error("TOO_MANY_TAB", context.peek_token(i))
-                elif got < nest or (got < nest - 1 and context.history[-1] in ["IsAssignation", "IsVarDeclaration"]):
+                elif got < nest or (
+                    got < nest - 1
+                    and context.history[-1] in ["IsAssignation", "IsVarDeclaration"]
+                ):
                     context.new_error("TOO_FEW_TAB", context.peek_token(i))
-                if context.check_token(i + got, ["LBRACKET", "RBRACKET", "LBRACE", "RBRACE"]):
+                if context.check_token(
+                    i + got, ["LBRACKET", "RBRACKET", "LBRACE", "RBRACE"]
+                ):
                     nest += 1
             if context.check_token(i, "LPARENTHESIS") is True:
                 nest += 1
             if context.check_token(i, "RPARENTHESIS") is True:
                 nest -= 1
             i += 1
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_block_start.py` & `norminette-3.3.52/norminette/rules/check_block_start.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,11 +30,15 @@
                 and hist_1 == "IsFuncDeclaration"
                 and hist_2 == "IsPreprocessorStatement"
             ):
                 context.scope.functions -= 1
                 context.scope = context.tmp_scope
                 context.scope.multiline = True
                 context.tmp_scope = None
-        if type(context.scope) == ControlStructure and outer is not None and type(outer) == ControlStructure:
-            if outer.multiline == False:
+        if (
+            type(context.scope) == ControlStructure
+            and outer is not None
+            and type(outer) == ControlStructure
+        ):
+            if outer.multiline is False:
                 context.new_error("MULT_IN_SINGLE_INSTR", context.peek_token(0))
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_brace.py` & `norminette-3.3.52/norminette/rules/check_brace.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         # if context.check_token(i, ["RBRACE", "LBRACE"]) is False and context.scope.type != "GlobalScope":
         #    context.new_error("BRACE_EMPTY_LINE")
         if context.check_token(i, ["RBRACE", "LBRACE"]) is False:
             context.new_error("EXPECTED_BRACE", context.peek_token(i))
             return False, 0
         i += 1
         i = context.skip_ws(i, nl=False)
+        if context.check_token(i, "NEWLINE") is True and context.check_token(i - 1, ["SPACE", "TAB"]):
+            context.new_error("SPC_BEFORE_NL", context.peek_token(i - 1))
         if context.check_token(i, "NEWLINE") is False or context.check_token(i, "NEWLINE") is None:
             if context.scope.name == "UserDefinedType" or context.scope.name == "UserDefinedEnum":
                 i = context.skip_ws(i, nl=False)
                 if context.check_token(i, "SEMI_COLON") is True:
                     return False, 0
                 if context.check_token(i, "IDENTIFIER") is False:
                     context.new_error("BRACE_SHOULD_EOL", context.peek_token(i - 1))
```

### Comparing `norminette-3.3.51/norminette/rules/check_comment.py` & `norminette-3.3.52/norminette/rules/check_comment.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 
     def run(self, context):
         """
         Comments are only allowed in GlobalScope.
         """
         i = context.skip_ws(0)
         has_comment = False
-        while context.peek_token(i) is not None and context.check_token(i, "NEWLINE") is False:
+        while (
+            context.peek_token(i) is not None
+            and context.check_token(i, "NEWLINE") is False
+        ):
             if context.check_token(i, allowed_on_comment) is False:
-                if has_comment == True:
+                if has_comment is True:
                     context.new_error("COMMENT_ON_INSTR", context.peek_token(i))
                     return True, i
             elif context.check_token(i, ["COMMENT", "MULT_COMMENT"]) is True:
-                if context.scope.name != "GlobalScope" or context.history[-1] == "IsFuncDeclaration":
+                if (
+                    context.scope.name != "GlobalScope"
+                    or context.history[-1] == "IsFuncDeclaration"
+                ):
                     context.new_error("WRONG_SCOPE_COMMENT", context.peek_token(i))
                 has_comment = True
             i += 1
         i = context.skip_ws(0)
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_comment_line_len.py` & `norminette-3.3.52/norminette/rules/check_comment_line_len.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_control_statement.py` & `norminette-3.3.52/norminette/rules/check_control_statement.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_declaration.py` & `norminette-3.3.52/norminette/rules/check_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_empty_line.py` & `norminette-3.3.52/norminette/rules/check_empty_line.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,30 +14,48 @@
         No other empty lines are allowed in functions
         You must have an empty between two functions
         """
         i = 0
         if len(context.history) == 1 and context.history[-1] == "IsEmptyLine":
             context.new_error("EMPTY_LINE_FILE_START", context.peek_token(i))
             return False, 0
-        if context.scope.name != "GlobalScope" and context.history[-1] != "IsBlockStart":
-            if context.history[-1] != "IsVarDeclaration" and context.scope.vdeclarations_allowed == True:
+        if (
+            context.scope.name != "GlobalScope"
+            and context.history[-1] != "IsBlockStart"
+        ):
+            if (
+                context.history[-1] != "IsVarDeclaration"
+                and context.scope.vdeclarations_allowed is True
+            ):
                 context.scope.vdeclarations_allowed = False
                 if context.history[-1] not in ["IsEmptyLine", "IsComment"]:
-                    if context.history[-1] == "IsBlockEnd" and context.scope.name == "Function":
+                    if (
+                        context.history[-1] == "IsBlockEnd"
+                        and context.scope.name == "Function"
+                    ):
                         pass
                     else:
                         context.new_error("NL_AFTER_VAR_DECL", context.peek_token(i))
                         return True, i
-        if len(context.history) > 1 and context.history[-2] == "IsPreprocessorStatement" and context.history[-1] != "IsPreprocessorStatement" and context.history[-1] != "IsEmptyLine" and context.history[-1] != "IsComment":
+        if (
+            len(context.history) > 1
+            and context.history[-2] == "IsPreprocessorStatement"
+            and context.history[-1] != "IsPreprocessorStatement"
+            and context.history[-1] != "IsEmptyLine"
+            and context.history[-1] != "IsComment"
+        ):
             context.new_error("NL_AFTER_PREPROC", context.peek_token(i))
         if context.history[-1] != "IsEmptyLine":
             return False, 0
         if context.check_token(i, "NEWLINE") is False:
             context.new_error("SPACE_EMPTY_LINE", context.peek_token(i))
         if context.history[-2] == "IsEmptyLine":
             context.new_error("CONSECUTIVE_NEWLINES", context.peek_token(i))
-        if context.history[-2] != "IsVarDeclaration" and context.scope.name != "GlobalScope":
-            context.new_error("EMPTY_LINE_FUNCTION", context.peek_token(i))
-        if context.peek_token(i + 1) is None:
+        if (
+            context.history[-2] != "IsVarDeclaration"
+            and context.scope.name != "GlobalScope"
+        ):
+            context.new_error("EMPTY_LINE_FUNCTION", context.peek_token(0))
+        if context.check_token(i, "NEWLINE") and context.peek_token(i + 1) is None:
             context.new_error("EMPTY_LINE_EOF", context.peek_token(i))
 
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_enum_var_decl.py` & `norminette-3.3.52/norminette/rules/check_enum_var_decl.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_expression_statement.py` & `norminette-3.3.52/norminette/rules/check_expression_statement.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,28 +40,33 @@
     def __init__(self):
         super().__init__()
         self.depends_on = [
             "IsExpressionStatement",
             "IsControlStatement",
             "IsFunctionCall",
             "IsAssignation",
-            "IsCast"
+            "IsCast",
         ]
 
     def run(self, context):
         """
         C keywords (return, break, continue...) must be followed by a space, with the
         exception of sizeof
         Return values in a function must be contained in parenthesis
         """
         i = 0
-        parenthesis = False
         while context.check_token(i, ["SEMI_COLON", "NEWLINE"]) is False:
             if context.check_token(i, kw) is True:
-                if context.check_token(i + 1, ["SPACE", "NEWLINE", "RPARENTHESIS", "COMMENT", "MULT_COMMENT"]) is False:
+                if (
+                    context.check_token(
+                        i + 1,
+                        ["SPACE", "NEWLINE", "RPARENTHESIS", "COMMENT", "MULT_COMMENT"],
+                    )
+                    is False
+                ):
                     context.new_error("SPACE_AFTER_KW", context.peek_token(i))
             if context.check_token(i, ["MULT", "BWISE_AND"]) is True and i > 0:
                 if context.check_token(i - 1, "IDENTIFIER") is True:
                     context.new_error("SPACE_AFTER_KW", context.peek_token(i - 1))
             if context.check_token(i, "RETURN") is True:
                 tmp = i + 1
                 tmp = context.skip_ws(tmp)
```

### Comparing `norminette-3.3.51/norminette/rules/check_func_arguments_name.py` & `norminette-3.3.52/norminette/rules/check_func_arguments_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from norminette.lexer import Token
 from norminette.rules import Rule
 
-import pdb
-
 type_specifiers = ["CHAR", "DOUBLE", "ENUM", "FLOAT", "INT", "UNION", "VOID", "SHORT"]
 
 misc_specifiers = ["CONST", "REGISTER", "STATIC", "STRUCT", "VOLATILE"]
 
 size_specifiers = ["LONG", "SHORT"]
 
 sign_specifiers = ["SIGNED", "UNSIGNED"]
@@ -41,23 +38,25 @@
             i += 1
             if context.peek_token(i).type in stop:
                 i += 1
             return i
         ret, i = context.check_type_specifier(i)
         has_tab = False
         while context.check_token(i, ["SPACE", "TAB"]):
-            if context.check_token(i, "TAB") is True and has_tab == False:
+            if context.check_token(i, "TAB") is True and has_tab is False:
                 context.new_error("TAB_INSTEAD_SPC", context.peek_token(i))
                 has_tab = True
             i += 1
 
-        if ret == False:
+        if ret is False:
             context.new_error("ARG_TYPE_UKN", context.peek_token(i))
             return -1
-        while context.peek_token(i) is not None and context.check_token(i, ["LPARENTHESIS"] + whitespaces):
+        while context.peek_token(i) is not None and context.check_token(
+            i, ["LPARENTHESIS"] + whitespaces
+        ):
             if context.check_token(i, "LPARENTHESIS") is True:
                 p += 1
             if context.check_token(i, "RPARENTHESIS") is True:
                 p -= 1
             i += 1
 
         if ret is True:
@@ -67,25 +66,27 @@
                 context.new_error("MISSING_IDENTIFIER", context.peek_token(i - 1))
             else:
                 i += 1
                 i = context.skip_ws(i)
             while context.peek_token(i) is not None and i < context.arg_pos[1]:
                 if context.check_token(i, stop) is True:
                     if context.check_token(i, "RPARENTHESIS") is True and p > 0:
-
                         p -= 1
                     else:
                         break
                 if context.check_token(i, "LPARENTHESIS"):
                     i = context.skip_nest(i)
                 i += 1
             i += 1
 
         else:
-            while context.peek_token(i) is not None and context.peek_token(i).type not in stop:
+            while (
+                context.peek_token(i) is not None
+                and context.peek_token(i).type not in stop
+            ):
                 i += 1
             i += 1
         return i
 
     def no_arg_func(self, context, pos):
         i = context.skip_ws(pos)
         if context.check_token(i, "VOID"):
```

### Comparing `norminette-3.3.51/norminette/rules/check_func_declaration.py` & `norminette-3.3.52/norminette/rules/check_func_declaration.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,49 +9,53 @@
         self.depends_on = ["IsFuncDeclaration", "IsFuncPrototype"]
 
     def run(self, context):
         """
         Maximum 4 arguments in a function
         Function declaration must be preceded by a newline
         """
+        # pdb.set_trace()
         i = 0
         tmp = 0
         start = 0
         arg = 1
         while context.check_token(tmp, ["SEMI_COLON", "NEWLINE"]) is False:
             if context.check_token(tmp, "LBRACE") is True:
                 context.new_error("BRACE_NEWLINE", context.peek_token(tmp))
             tmp += 1
         # if tmp < context.tkn_scope - 2:
         # context.new_error("NEWLINE_IN_DECL", context.peek_token(tmp))
         # this is a func declaration
-        if context.history[-1] == 'IsFuncDeclaration':
-#        if context.check_token(tmp, "SEMI_COLON") is False:
+        if context.history[-1] == "IsFuncDeclaration":
+            #        if context.check_token(tmp, "SEMI_COLON") is False:
             i = 2
             length = len(context.history)
-            while length - i >= 0 and (context.history[-i] == "IsPreprocessorStatement"
+            while length - i >= 0 and (
+                context.history[-i] == "IsPreprocessorStatement"
                 or context.history[-i] == "IsComment"
                 or context.history[-i] == "IsFuncDeclaration"
             ):
                 i += 1
             if length - i > 0 and context.history[-i] != "IsEmptyLine":
                 context.new_error("NEWLINE_PRECEDES_FUNC", context.peek_token(start))
         i = context.fname_pos + 1
-        while (context.check_token(i, ["RPARENTHESIS"])) is True: #, "SPACE", "TAB"])) is True:
+        while (
+            context.check_token(i, ["RPARENTHESIS"])
+        ) is True:  # , "SPACE", "TAB"])) is True:
             i += 1
         if context.check_token(i, "LPARENTHESIS") is False:
             context.new_error("EXP_PARENTHESIS", context.peek_token(i))
         i += 1
         deep = 1
         while deep > 0:
             if context.check_token(i, "LPARENTHESIS"):
                 i = context.skip_nest(i)
-            if context.check_token(i, "RPARENTHESIS"):
+            elif context.check_token(i, "RPARENTHESIS"):
                 deep -= 1
-            if context.check_token(i, "COMMA"):
+            elif context.check_token(i, "COMMA"):
                 arg += 1
             i += 1
         if context.check_token(i - 1, ["SPACE", "TAB"]) is True:
             tmp = i - 1
             while context.check_token(tmp, ["SPACE", "TAB"]) is True:
                 tmp -= 1
             if context.check_token(tmp, "NEWLINE") is False:
```

### Comparing `norminette-3.3.51/norminette/rules/check_func_spacing.py` & `norminette-3.3.52/norminette/rules/check_func_spacing.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_general_spacing.py` & `norminette-3.3.52/norminette/rules/check_general_spacing.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_global_naming.py` & `norminette-3.3.52/norminette/rules/check_global_naming.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,20 +28,22 @@
         self.depends_on = ["IsVarDeclaration"]
 
     def run(self, context):
         """
         Global variable names must be preceded by g_
         """
         i = 0
-        last_id = ""
         if context.scope.name != "GlobalScope":
             return False, 0
         i = context.skip_ws(i)
         _, i = context.check_type_specifier(i)
         i = context.skip_ws(i)
         while context.check_token(i, "IDENTIFIER") is False:
             i += 1
-        if context.peek_token(i) is not None and context.peek_token(i).value != "environ":
+        if (
+            context.peek_token(i) is not None
+            and context.peek_token(i).value != "environ"
+        ):
             context.new_warning("GLOBAL_VAR_DETECTED", context.peek_token(0))
             if context.peek_token(i).value.startswith("g_") is False:
                 context.new_error("GLOBAL_VAR_NAMING", context.peek_token(i))
         return False, i
```

### Comparing `norminette-3.3.51/norminette/rules/check_header.py` & `norminette-3.3.52/norminette/rules/check_line_indent.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 from norminette.rules import Rule
-import re
+from norminette.scope import GlobalScope
 
-class CheckHeader(Rule):
+
+class CheckLineIndent(Rule):
     def __init__(self):
         super().__init__()
         self.depends_on = []
 
-    def parse_header(self, context):
-        if context.check_token(0, "MULT_COMMENT") is False:
-            # print ("Missing or invalid header. Header are being reintroduced as a mandatory part of your files. This is not yet an error.")
-            context.new_error("INVALID_HEADER", context.peek_token(0))
-            context.header_parsed = True
-            return
-        context.header += context.peek_token(0).value + '\n'
-
-    def check_header(self, context):
-        #val = r"\/\* \*{74} \*\/\n\/\*.*\*\/\n\/\*.*\*\/\n\/\*.{3}([^ ]*).*\*\/\n\/\*.*\*\/\n\/\*   By: ([^ ]*).*\*\/\n\/\*.*\*\/\n\/\*   Created: ([^ ]* [^ ]*) by ([^ ]*).*\*\/\n\/\*   Updated: ([^ ]* [^ ]*) by ([^ ]*).*\*\/\n\/\*.*\*\/\n\/\* \*{74} \*\/\n"
-        val_no_check_nl = r"\/\* \*{74} \*\/.\/\*.*\*\/.\/\*.*\*\/.\/\*.{3}([^ ]*).*\*\/.\/\*.*\*\/.\/\*   By: ([^ ]*).*\*\/.\/\*.*\*\/.\/\*   Created: ([^ ]* [^ ]*) by ([^ ]*).*\*\/.\/\*   Updated: ([^ ]* [^ ]*) by ([^ ]*).*\*\/.\/\*.*\*\/.\/\* \*{74} \*\/."
-
-        #correct_header = re.match(val, context.header)
-        regex = re.compile(val_no_check_nl, re.DOTALL)
-        #correct_header_no_nl = re.match(val_no_check_nl, context.header)
-        correct_header_no_nl = regex.search(context.header)
-        if correct_header_no_nl is None:
-            # print ("Missing or invalid header. Header are being reintroduced as a mandatory part of your files. This is not yet an error.")
-            context.new_error("INVALID_HEADER", context.peek_token(0))
-        #else:
-        #    print (correct_header.group(1,2,3,4,5,6))
-
     def run(self, context):
         """
-            Header checking. Just a warning for now. Does not trigger moulinette error
+        Each new scope (function, control structure, struct/enum type declaration) adds a tab to the general indentation
         """
-        if context.header_parsed == True:
+        expected = context.scope.indent
+        if context.history[-1] in [
+            "IsEmptyLine",
+            "IsComment",
+            "IsPreprocessorStatement",
+            "IsVariableDeclaration",
+        ]:
             return False, 0
-        elif context.history[-1] == "IsComment" and context.header_parsed == False:
-            self.parse_header(context)
-            context.header_started = True
-        elif context.history[-1] != "IsComment" and context.header_started == True:
-            self.check_header(context)
-            context.header_parsed = True
-        elif context.header_started == False and context.header_parsed == False and context.history[-1] != "IsComment":
-            context.new_error("INVALID_HEADER", context.peek_token(0))
-            # print ("Missing or invalid header. Header are being reintroduced as a mandatory part of your files. This is not yet an error.")
-            context.header_parsed = True
+        if (
+            context.history[-1] != "IsPreprocessorStatement"
+            and type(context.scope) is GlobalScope
+            and context.scope.include_allowed is True
+        ):
+            context.scope.include_allowed = False
+        got = 0
+        while context.check_token(got, "TAB"):
+            got += 1
+        if context.check_token(got, ["LBRACE", "RBRACE"]) and expected > 0:
+            if context.check_token(got, "RBRACE") is True:
+                expected -= 1
+            else:
+                hist = context.history[: len(context.history) - 1]
+                for item in hist[::-1]:
+                    if (
+                        item == "IsEmptyLine"
+                        or item == "IsComment"
+                        or item == "IsPreprocessorStatement"
+                    ):
+                        continue
+                    if item not in [
+                        "IsControlStatement",
+                        "IsFuncDeclaration",
+                        "IsUserDefinedType",
+                    ]:
+                        break
+                    else:
+                        expected -= 1
+                    break
+        if expected > got:
+            context.new_error("TOO_FEW_TAB", context.peek_token(0))
+            return False, got
+        elif got > expected:
+            context.new_error("TOO_MANY_TAB", context.peek_token(0))
+            return False, got
+        return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_identifier_name.py` & `norminette-3.3.52/norminette/rules/check_preprocessor_indent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import string
-
 from norminette.rules import Rule
-from norminette.scope import GlobalScope, UserDefinedType
-
 
-assigns = ["ASSIGN"]
+ALLOWED_PREPROC = [
+    "DEFINE",
+    "IFNDEF",
+    "IFDEF",
+    "#IF",
+    "ELIF",
+    "#ELSE",
+    "ENDIF",
+    "INCLUDE",
+    "WARNING",
+    "UNDEF",
+    "ERROR",
+]
+TOO_MUCH_INDENT = ["IFNDEF", "IFDEF", "ELIF", "#IF", "#ELSE"]
 
 
-class CheckIdentifierName(Rule):
+class CheckPreprocessorIndent(Rule):
     def __init__(self):
         super().__init__()
-        self.depends_on = []
+        self.depends_on = ["IsPreprocessorStatement"]
+
+    def get_space_number(self, val):
+        val = val[1:]
+        spaces = 0
+        for i in val:
+            if i == " ":
+                spaces += 1
+            else:
+                return spaces
 
     def run(self, context):
         """
-        Function can only be declared in the global scope
-        User defined identifiers can only contain lowercase characters, '_' or digits
+        Preprocessor statements must be indented by an additionnal space for each #ifdef/#ifndef/#if
+        statement.
+        Structure is `#{indentation}preproc_statement`
+        Preprocessor must always be at the start of the line
         """
         i = 0
-        legal_characters = string.ascii_lowercase + string.digits + "_"
-        legal_cap_characters = string.ascii_uppercase + string.digits + "_"
-        if context.history[-1] == "IsFuncDeclaration":
-            sc = context.scope
-            if type(sc) is not GlobalScope and type(sc) is not UserDefinedType:
-                context.new_error("WRONG_SCOPE_FCT", context.peek_token(0))
-            while type(sc) != GlobalScope:
-                sc = sc.outer()
-            for c in sc.fnames[-1]:
-                if c not in legal_characters:
-                    context.new_error("FORBIDDEN_CHAR_NAME", context.peek_token(context.fname_pos))
-        if len(context.scope.vars_name) > 0:
-            for val in context.scope.vars_name[::]:
-                for c in val.value:
-                    if c not in legal_characters:
-                        context.new_error("FORBIDDEN_CHAR_NAME", val)
-                        break
-                context.scope.vars_name.remove(val)
-        # passed_assign = False
-        # err = None
-        # hist = context.history[-1]
-        # while i < context.tkn_scope and context.peek_token(i) is not None:
-        # if context.check_token(i, assigns) is True:
-        # passed_assign = True
-        #        if context.check_token(i, "IDENTIFIER") and hist in ['IsVarDeclaration']:
-        # for c in context.peek_token(i).value:
-        # if c not in legal_characters:
-        # err = ("FORBIDDEN_CHAR_NAME", context.peek_token(i))
-        # break
-        # if err is not None and hist not in ['IsFuncDeclaration', 'IsFuncPrototype'] or (hist == 'IsVariable' and passed_assign == True):
-        # for c in context.peek_token(i).value:
-        # if c not in legal_cap_characters:
-        # err = ("FORBIDDEN_CHAR_NAME", context.peek_token(i))
-        # break
-        # else:
-        # err = None
-        # if err is not None:
-        # context.new_error(err[0], err[1])
-        # break
-        # i += 1
+        i = context.skip_ws(i)
+        tken = context.peek_token(i)
+        current_indent = context.preproc_scope_indent
+        if context.peek_token(i).pos[1] != 1:
+            context.new_error("PREPROC_START_LINE", context.peek_token(0))
+        tken = context.peek_token(i)
+        if context.check_token(i, ALLOWED_PREPROC) is False:
+            context.new_error("PREPROC_UKN_STATEMENT", context.peek_token(i))
+        if context.check_token(i, TOO_MUCH_INDENT) is True:
+            current_indent -= 1
+        if current_indent < 0:
+            current_indent = 0
+        spaces = self.get_space_number(tken.value if tken.value else tken.type)
+        if current_indent != spaces:
+            context.new_error("PREPROC_BAD_INDENT", context.peek_token(i))
+
+        i += 1
+        tken = context.peek_token(i)
+        if tken is not None and tken.type not in ["NEWLINE", "COMMENT", "MULT_COMMENT"]:
+            context.new_error("PREPROC_EXPECTED_EOL", context.peek_token(i))
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_in_header.py` & `norminette-3.3.52/norminette/rules/check_in_header.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_label.py` & `norminette-3.3.52/norminette/rules/check_label.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_line_count.py` & `norminette-3.3.52/norminette/rules/check_line_count.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_line_indent.py` & `norminette-3.3.52/norminette/rules/is_block_start.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-import pdb
+from norminette.context import ControlStructure
+from norminette.rules import PrimaryRule
+from norminette.scope import GlobalScope, UserDefinedEnum, Function, UserDefinedType, VariableAssignation
 
-from norminette.rules import Rule
-from norminette.scope import GlobalScope
 
-
-class CheckLineIndent(Rule):
+class IsBlockStart(PrimaryRule):
     def __init__(self):
         super().__init__()
-        self.depends_on = []
+        self.priority = 55
+        self.scope = [
+            Function,
+            UserDefinedType,
+            VariableAssignation,
+            ControlStructure,
+            UserDefinedEnum,
+            GlobalScope,
+        ]
 
     def run(self, context):
         """
-        Each new scope (function, control structure, struct/enum type declaration) adds a tab to the general indentation
+        Catches LBRACE tokens
+        Creates new scope based on previous instruction or set it to multiline if it
+        is a control statement
         """
-        expected = context.scope.indent 
-        if context.history[-1] in ["IsEmptyLine", 'IsComment', "IsPreprocessorStatement", "IsVariableDeclaration", "IsAssignation"]:
+        i = context.skip_ws(0, nl=False)
+        if context.check_token(i, "LBRACE") is False:
             return False, 0
-        if (
-            context.history[-1] != "IsPreprocessorStatement"
-            and type(context.scope) is GlobalScope
-            and context.scope.include_allowed == True
-        ):
-            context.scope.include_allowed = False
-        got = 0
-        while context.check_token(got, "TAB"):
-            got += 1
-        if context.check_token(got, ["LBRACE", "RBRACE"]) and expected > 0:
-            if context.check_token(got, "RBRACE") is True:
-                expected -= 1
+        i += 1
+        hist = context.history
+        lines = context.scope.lines
+        for item in hist[::-1]:
+            if item == "IsEmptyLine" or item == "IsComment" or item == "IsPreprocessorStatement":
+                lines -= 1
+                continue
+            if (
+                item
+                not in [
+                    "IsControlStatement",
+                    "IsFuncDeclaration",
+                    "IsUserDefinedType",
+                ]
+                or (item in ["IsControlStatement", "IsFuncDeclaration", "IsUserDefinedType"] and lines >= 1)
+            ):
+                context.sub = context.scope.inner(ControlStructure)
+                context.sub.multiline = True
+                break
             else:
-                hist = context.history[: len(context.history) - 1]
-                for item in hist[::-1]:
-                    if item == "IsEmptyLine" or item == "IsComment" or item == "IsPreprocessorStatement":
-                        continue
-                    if item not in [
-                        "IsControlStatement",
-                        "IsFuncDeclaration",
-                        "IsUserDefinedType",
-                    ]:
-                        break
-                    else:
-                        expected -= 1
-                    break
-        if expected > got:
-            context.new_error("TOO_FEW_TAB", context.peek_token(0))
-            return False, got
-        elif got > expected:
-            context.new_error("TOO_MANY_TAB", context.peek_token(0))
-            return False, got
-        return False, 0
+                context.scope.multiline = True
+            break
+
+        tmp = i
+        # while context.peek_token(tmp) and (context.check_token(tmp, ["NEWLINE"])) is False:
+        #    tmp += 1
+        tmp = context.eol(tmp)
+        if context.peek_token(tmp) is not None:
+            i = tmp
+        return True, i
```

### Comparing `norminette-3.3.51/norminette/rules/check_line_len.py` & `norminette-3.3.52/norminette/rules/check_line_len.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_many_instructions.py` & `norminette-3.3.52/norminette/rules/check_many_instructions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from norminette.rules import Rule
 
+
 class CheckManyInstructions(Rule):
     def __init__(self):
         super().__init__()
         self.depends_on = [
             "IsAssignation",
             "IsBlockEnd",
             "IsControlStatement",
```

### Comparing `norminette-3.3.51/norminette/rules/check_nest_line_indent.py` & `norminette-3.3.52/norminette/rules/check_nest_line_indent.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,19 @@
 ]
 nest_kw = ["RPARENTHESIS", "LPARENTHESIS", "NEWLINE"]
 
 
 class CheckNestLineIndent(Rule):
     def __init__(self):
         super().__init__()
-        self.depends_on = ["IsControlStatement", "IsExpressionStatement", "IsDeclaration"]
+        self.depends_on = [
+            "IsControlStatement",
+            "IsExpressionStatement",
+            "IsDeclaration",
+        ]
 
     def find_nest_content(self, context, nest, i):
         expected = context.scope.indent + nest
         while context.peek_token(i) is not None:
             if context.check_token(i, ["LPARENTHESIS", "LBRACE", "LBRACKET"]) is True:
                 i += 1
                 i = self.find_nest_content(context, nest + 1, i) + 1
@@ -75,19 +79,21 @@
         return i
 
     def run(self, context):
         """
         Each nest (parenthesis, brackets, braces) adds a tab to the general indentation
         """
         i = 0
-        expected = context.scope.indent
         nest = 0
         if context.history[-1] == "IsEmptyLine":
             return False, 0
-        while context.peek_token(i) and context.check_token(i, ["LPARENTHESIS", "NEWLINE"]) is False:
+        while (
+            context.peek_token(i)
+            and context.check_token(i, ["LPARENTHESIS", "NEWLINE"]) is False
+        ):
             i += 1
         if context.check_token(i, "NEWLINE") is True:
             return False, 0
         if context.check_token(i, "LPARENTHESIS") is True:
             nest += 1
             i += 1
             self.find_nest_content(context, nest, i)
```

### Comparing `norminette-3.3.51/norminette/rules/check_operators_spacing.py` & `norminette-3.3.52/norminette/rules/check_operators_spacing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from norminette.rules import Rule
-import pdb
+
 operators = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
     "ADD_ASSIGN",
     "SUB_ASSIGN",
     "MUL_ASSIGN",
     "DIV_ASSIGN",
@@ -92,17 +92,16 @@
     # operators that should only be prefixed by a space
     "ELLIPSIS"  # ...
 ]
 
 s_operators = [
     # operators that should only be suffixed by a space
     "COMMA",  # ,
-    #Where do i put that shit
-    #"COLON",  # :
-
+    # Where do i put that shit
+    # "COLON",  # :
 ]
 
 son_operators = [
     # operators that should only be suffixed by a space or newline
     "SEMI_COLON"  # ;
 ]
 
@@ -112,26 +111,19 @@
     "MINUS",
     "BWISE_XOR",  # ^
     "BWISE_OR",  # |
     "BWISE_AND",  # &
     "BWISE_NOT",  # ~
 ]
 
-glued_operators = [
-    "MULT",
-    "PLUS",
-    "MINUS",
-    "DIV",
-    "NOT",
-    "BWISE_NOT"
-]
+glued_operators = ["MULT", "PLUS", "MINUS", "DIV", "NOT", "BWISE_NOT"]
 
 spec_operators = [
     "NOT",
-    "BWISE_NOT", 
+    "BWISE_NOT",
     "DIV",
 ]
 
 rnests = ["RPARENTHESIS", "RBRACE", "RBRACKET"]
 
 lnests = [
     "LBRACE",
@@ -158,32 +150,47 @@
             "IsVarDeclaration",
             "IsFunctionCall",
             "IsDeclaration",
         ]
         self.last_seen_tkn = None
 
     def check_prefix(self, context, pos):
-        tmp = -1
-
         if pos > 0 and context.check_token(pos, ["TAB", "SPACE"]):
             context.new_error("", context.peek_token(pos))
-        if pos + 1 < len(context.tokens[: context.tkn_scope]) and context.peek_token(pos + 1).type == "SPACE":
+        if (
+            pos + 1 < len(context.tokens[: context.tkn_scope])
+            and context.peek_token(pos + 1).type == "SPACE"
+        ):
             context.new_error("NO_SPC_AFR_OPR", context.peek_token(pos))
 
     def check_lnest(self, context, pos):
-        if context.history[-1] == "IsFuncDeclaration" or context.history[-1] == "IsFuncPrototype":
+        if (
+            context.history[-1] == "IsFuncDeclaration"
+            or context.history[-1] == "IsFuncPrototype"
+        ):
             return False
         tmp = pos + 1
         # Here is `(_`
-        while context.peek_token(tmp) and context.check_token(tmp, ["SPACE", "TAB"]) is True:
+        while (
+            context.peek_token(tmp)
+            and context.check_token(tmp, ["SPACE", "TAB"]) is True
+        ):
             tmp += 1
         if context.check_token(tmp, "NEWLINE") is False:
-            if context.check_token(tmp, lnests + rnests + ["SEMI_COLON", "PTR", "DOT"]) is True and tmp != pos + 1:
+            if (
+                context.check_token(tmp, lnests + rnests + ["SEMI_COLON", "PTR", "DOT"])
+                is True
+                and tmp != pos + 1
+            ):
                 context.new_error("SPC_AFTER_PAR", context.peek_token(pos))
-            elif context.check_token(tmp, lnests + rnests + ["SEMI_COLON", "PTR", "DOT"]) is False and tmp != pos + 1:
+            elif (
+                context.check_token(tmp, lnests + rnests + ["SEMI_COLON", "PTR", "DOT"])
+                is False
+                and tmp != pos + 1
+            ):
                 context.new_error("NO_SPC_AFR_PAR", context.peek_token(pos))
         tmp = pos - 1
         # Here is `_(`
         while tmp >= 0 and context.check_token(tmp, ["SPACE", "TAB"]) is True:
             tmp -= 1
         if context.check_token(tmp, "NEWLINE") is False:
             if (
@@ -202,15 +209,18 @@
                         "IDENTIFIER",
                         "SIZEOF",
                     ],
                 )
                 is True
                 and tmp != pos - 1
             ):
-                if context.check_token(tmp, ["MULT", "BWISE_AND"]) is True and context.is_operator == False:
+                if (
+                    context.check_token(tmp, ["MULT", "BWISE_AND"]) is True
+                    and context.is_operator is False
+                ):
                     context.new_error("NO_SPC_BFR_PAR", context.peek_token(pos))
             elif (
                 context.check_token(
                     tmp,
                     lnests
                     + rnests
                     + [
@@ -227,33 +237,42 @@
                         "IDENTIFIER",
                         "SIZEOF",
                         "NOT",
                         "MINUS",
                         "PLUS",
                         "CONSTANT",
                         "CHAR_CONSTANT",
-                        "STRING"
+                        "STRING",
                     ],
                 )
                 is False
                 and tmp == pos - 1
             ):
                 context.new_error("SPC_BFR_PAR", context.peek_token(pos))
         return False
 
     def check_rnest(self, context, pos):
-        if context.history[-1] == "IsFuncDeclaration" or context.history[-1] == "IsFuncPrototype":
+        if (
+            context.history[-1] == "IsFuncDeclaration"
+            or context.history[-1] == "IsFuncPrototype"
+        ):
             return False
         tmp = pos + 1
         # Here is `)_`
-        while context.peek_token(tmp) and context.check_token(tmp, ["SPACE", "TAB"]) is True:
+        while (
+            context.peek_token(tmp)
+            and context.check_token(tmp, ["SPACE", "TAB"]) is True
+        ):
             tmp += 1
         if context.check_token(tmp, "NEWLINE") is False:
             if (
-                context.check_token(tmp, lnests + rnests + ["SEMI_COLON", "PTR", "DOT", "INC", "DEC"]) is True
+                context.check_token(
+                    tmp, lnests + rnests + ["SEMI_COLON", "PTR", "DOT", "INC", "DEC"]
+                )
+                is True
                 and tmp != pos + 1
             ):
                 context.new_error("NO_SPC_AFR_PAR", context.peek_token(pos))
             elif (
                 context.check_token(
                     tmp,
                     lnests
@@ -267,15 +286,15 @@
                         "MINUS",
                         "MULT",
                         "BWISE_AND",
                         "IDENTIFIER",
                         "COMMA",
                         "STRING",
                         "CONSTANT",
-                        "PLUS"
+                        "PLUS",
                     ],
                 )
                 is False
                 and tmp == pos + 1
             ):
                 context.new_error("SPC_AFTER_PAR", context.peek_token(pos))
         tmp = pos - 1
@@ -303,68 +322,115 @@
                 is True
                 and tmp != pos - 1
             ):
                 context.new_error("NO_SPC_BFR_PAR", context.peek_token(pos))
         return False
 
     def check_suffix(self, context, pos):
-        if pos + 1 < len(context.tokens[: context.tkn_scope]) and not context.check_token(
+        if pos + 1 < len(
+            context.tokens[: context.tkn_scope]
+        ) and not context.check_token(
             pos + 1, ["SPACE", "NEWLINE", "TAB"] + glued_operators + rnests
         ):
             context.new_error("SPC_AFTER_OPERATOR", context.peek_token(pos))
         if pos > 0 and context.peek_token(pos - 1).type == "SPACE":
             context.new_error("NO_SPC_BFR_OPR", context.peek_token(pos))
 
     def check_glued_prefix_and_suffix(self, context, pos):
         if pos > 0 and context.peek_token(pos - 1).type != "SPACE":
             if context.check_token(pos - 1, "TAB") is True:
                 tmp = -1
                 while context.check_token(pos + tmp, "TAB") is True:
                     tmp -= 1
-                if context.check_token(pos + tmp, ["NEWLINE", "ESCAPED_NEWLINE"] + glued_operators) is True:
+                if (
+                    context.check_token(
+                        pos + tmp, ["NEWLINE", "ESCAPED_NEWLINE"] + glued_operators
+                    )
+                    is True
+                ):
                     return False, 0
             context.new_error("SPC_BFR_OPERATOR", context.peek_token(pos))
         if (
             pos + 1 < len(context.tokens[: context.tkn_scope])
-            and context.check_token(pos + 1, ["SPACE", "LPARENTHESIS", "LBRACKET", "LBRACE", "NEWLINE"] + glued_operators) is False
+            and context.check_token(
+                pos + 1,
+                ["SPACE", "LPARENTHESIS", "LBRACKET", "LBRACE", "NEWLINE"]
+                + glued_operators,
+            )
+            is False
         ):
             context.new_error("SPC_AFTER_OPERATOR", context.peek_token(pos))
 
     def check_prefix_and_suffix(self, context, pos):
-        if pos > 0 and context.check_token(pos - 1, ["SPACE", "LPARENTHESIS", "LBRACKET"] + glued_operators) is False:
+        if (
+            pos > 0
+            and context.check_token(
+                pos - 1, ["SPACE", "LPARENTHESIS", "LBRACKET"] + glued_operators
+            )
+            is False
+        ):
             if context.check_token(pos - 1, "TAB") is True:
                 tmp = -1
                 while context.check_token(pos + tmp, "TAB") is True:
                     tmp -= 1
-                if context.check_token(pos + tmp, ["NEWLINE", "ESCAPED_NEWLINE"]) is True:
+                if (
+                    context.check_token(pos + tmp, ["NEWLINE", "ESCAPED_NEWLINE"])
+                    is True
+                ):
                     return False, 0
-            if context.check_token(pos - 1, "RPARENTHESIS") and context.parenthesis_contain(context.skip_nest_reverse(pos - 1))[0] == "cast":
+            if (
+                context.check_token(pos - 1, "RPARENTHESIS")
+                and context.parenthesis_contain(context.skip_nest_reverse(pos - 1))[0]
+                == "cast"
+            ):
                 return False, 0
             context.new_error("SPC_BFR_OPERATOR", context.peek_token(pos))
-        if (pos + 1 < len(context.tokens[: context.tkn_scope]) and context.check_token(pos + 1, ["SPACE", "LPARENTHESIS", "RPARENTHESIS", "LBRACKET", "RBRACKET", "NEWLINE", "COMMA"] + spec_operators) is False):
+        if (
+            pos + 1 < len(context.tokens[: context.tkn_scope])
+            and context.check_token(
+                pos + 1,
+                [
+                    "SPACE",
+                    "LPARENTHESIS",
+                    "RPARENTHESIS",
+                    "LBRACKET",
+                    "RBRACKET",
+                    "NEWLINE",
+                    "COMMA",
+                ]
+                + spec_operators,
+            )
+            is False
+        ):
             tmp = pos - 1
-            while context.check_token(tmp, ['SPACE', 'TAB']):
+            while context.check_token(tmp, ["SPACE", "TAB"]):
                 tmp -= 1
             if context.check_token(tmp, "RPARENTHESIS"):
                 tmp = context.skip_nest_reverse(tmp)
                 if context.parenthesis_contain(tmp)[0] != "cast":
                     context.new_error("SPC_AFTER_OPERATOR", context.peek_token(pos))
-            elif context.check_token(tmp, glued_operators) is False and not (context.check_token(pos, ["PLUS", "MINUS"]) and context.check_token(pos + 1, "CONSTANT")):
+            elif context.check_token(tmp, glued_operators) is False and not (
+                context.check_token(pos, ["PLUS", "MINUS"])
+                and context.check_token(pos + 1, "CONSTANT")
+            ):
                 context.new_error("SPC_AFTER_OPERATOR", context.peek_token(pos))
 
     def check_glued_operator(self, context, pos):
         glued = [
             "LPARENTHESIS",
             "LBRACKET",
             "LBRACE",
         ]
         if context.check_token(pos + 1, ["SPACE", "TAB"]) is True:
             context.new_error("SPC_AFTER_OPERATOR", context.peek_token(pos))
         pos -= 1
-        if context.check_token(pos, glued + ["SPACE", "TAB"] + glued_operators) is False:
+        if (
+            context.check_token(pos, glued + ["SPACE", "TAB"] + glued_operators)
+            is False
+        ):
             context.new_error("SPC_BFR_OPERATOR", context.peek_token(pos))
         while pos >= 0 and context.check_token(pos, ["SPACE", "TAB"]) is True:
             pos -= 1
             if pos >= 0 and context.check_token(pos, glued) is True:
                 context.new_error("NO_SPC_BFR_OPR", context.peek_token(pos))
 
     def check_combined_op(self, context, pos):
@@ -379,20 +445,21 @@
             "RBRACKET",
             "RBRACE",
             "MINUS",
             "PLUS",
             "BWISE_NOT",
             "BWISE_OR",
             "BWISE_AND",
-           "BWISE_XOR",
+            "BWISE_XOR",
         ]
-        lsign = operators + ["LBRACKET"]
         i = 0
         if context.peek_token(pos).type == "MULT":
-            if context.check_token(pos - 1, lpointer) == False and (context.is_glued_operator(pos - 1) is True):# or context.check_token(pos - 1, c_operators) is False):
+            if context.check_token(pos - 1, lpointer) is False and (
+                context.is_glued_operator(pos - 1) is True
+            ):  # or context.check_token(pos - 1, c_operators) is False):
                 context.new_error("SPC_BFR_POINTER", context.peek_token(pos))
             if context.check_token(pos + 1, ["SPACE", "TAB"]):
                 context.new_error("SPC_AFTER_POINTER", context.peek_token(pos))
             i = 1
             while context.peek_token(pos + i).type in ["MULT", "LPARENTHESIS"]:
                 i += 1
                 if context.peek_token(pos + i).type == "SPACE":
@@ -426,15 +493,18 @@
                 self.check_rnest(context, i)
             elif context.check_token(i, ps_operators) is True:
                 self.check_prefix_and_suffix(context, i)
             elif context.check_token(i, gps_operators) is True:
                 self.check_glued_prefix_and_suffix(context, i)
             elif context.check_token(i, s_operators) is True:
                 self.check_suffix(context, i)
-            elif context.check_token(i, son_operators) is True and context.check_token(i + 1, "NEWLINE") is False:
+            elif (
+                context.check_token(i, son_operators) is True
+                and context.check_token(i + 1, "NEWLINE") is False
+            ):
                 self.check_suffix(context, i)
             elif context.check_token(i, p_operators) is True:
                 self.check_prefix(context, i)
             if context.check_token(i, whitespaces) is False:
                 self.last_seen_tkn = context.peek_token(i)
             i += 1
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_preprocessor_define.py` & `norminette-3.3.52/norminette/rules/check_preprocessor_define.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 
 from norminette.lexer import Lexer
 from norminette.rules import Rule
 from norminette.scope import GlobalScope, Function
 
-import pdb
 
 class CheckPreprocessorDefine(Rule):
     def __init__(self):
         super().__init__()
         self.depends_on = ["IsPreprocessorStatement"]
 
     def skip_define_nest(self, i, tkns):
@@ -36,15 +35,15 @@
         Define cannot contain newlines
         Define can only contain constant values, such as integers and strings
         """
         i = context.skip_ws(0)
         if len(context.history) > 1 and context.history[-2] == "IsFuncDeclaration":
             self.check_function_declaration(context)
         if type(context.scope) is not GlobalScope:
-            if type(context.scope) == Function and context.scope.multiline == False:
+            if type(context.scope) == Function and context.scope.multiline is False:
                 pass
             else:
                 context.new_error("PREPROC_GLOBAL", context.peek_token(0))
         if context.check_token(i, "DEFINE") is True:
             val = context.peek_token(i).value.split("define", 1)[1]
         elif context.check_token(i, "IFNDEF") is True:
             val = context.peek_token(i).value.split("ifndef", 1)[1]
@@ -60,16 +59,18 @@
             if tkn.type == "ESCAPED_NEWLINE":
                 context.new_error("NEWLINE_DEFINE", tkn)
             elif tkn.type in ["TAB", "SPACE"]:
                 if tkn.type == "TAB" and len(identifiers) == 0:
                     context.new_error("TAB_INSTEAD_SPC", tkn)
                 i += 1
                 continue
-            elif tkn.type == "IDENTIFIER" and len(identifiers) == 0:
-                if tkn.value.isupper() is False:
+            elif (tkn.type == "IDENTIFIER" or tkn.type == "NULL") and len(
+                identifiers
+            ) == 0:
+                if tkn.type != "NULL" and tkn.value.isupper() is False:
                     context.new_error("MACRO_NAME_CAPITAL", tkn)
                 identifiers.append(tkn)
                 tmp = i
                 while tmp < len(tkns) - 1 and tkns[tmp].type in [
                     "SPACE",
                     "TAB",
                     "IDENTIFIER",
@@ -81,48 +82,48 @@
                     if context.scope.header_protection == 0:
                         if identifiers[0].value == protection:
                             context.scope.header_protection = 1
                         elif identifiers[0].value != protection:
                             context.new_error("HEADER_PROT_NAME", tkns[1])
                 elif (
                     context.filetype == "c"
-                    and context.scope.include_allowed == True
+                    and context.scope.include_allowed is True
                     and (
                         len(tkns) > tmp + 1
                         or (
                             len(tkns) == tmp + 1
                             and identifiers[0].value != protection
                             and context.scope.header_protection == -1
                         )
                     )
                 ):
                     context.scope.include_allowed = False
             elif tkn.type in ["IDENTIFIER", "STRING", "CONSTANT"]:
-                if context.skip_define_error == True:
+                if context.skip_define_error is True:
                     continue
                 if len(identifiers) == 1:
                     if tkn.type == "IDENTIFIER" and tkn.value.isupper() is False:
                         context.new_error("PREPROC_CONSTANT", tkn)
                     identifiers.append(tkn)
                 elif len(identifiers) == 0:
                     context.new_error("INCORRECT_DEFINE", tkn)
                 else:
                     context.new_error("TOO_MANY_VALS", tkn)
             elif tkn.type == "LPARENTHESIS":
-                if context.skip_define_error == True:
+                if context.skip_define_error is True:
                     continue
                 if len(identifiers) == 0:
                     continue
                 elif len(identifiers) == 1 and tkns[i - 1].type in ["SPACE", "TAB"]:
                     if tkn.type == "TAB":
                         context.new_error("TAB_INSTEAD_SPC", tkn)
                     continue
                 else:
                     context.new_error("PREPROC_CONSTANT", tkn)
             elif tkn.type in ["LBRACKET", "LBRACE"]:
-                if context.skip_define_error == True:
+                if context.skip_define_error is True:
                     continue
                 context.new_error("PREPROC_CONSTANT", tkn)
             i += 1
         if context.filetype == "h" and context.scope.header_protection != 1:
-            context.new_error("HEADER_PROT_ALL_2", context.peek_token(i))
+            context.new_error("HEADER_PROT_ALL", context.peek_token(0))
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_preprocessor_include.py` & `norminette-3.3.52/norminette/rules/check_preprocessor_include.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         Includes must be at the start of the file
         You cannot include anything that isn't an header file
         """
         i = 0
         filetype = ""
         if context.check_token(i, "INCLUDE") is False:
             return False, 0
-        if type(context.scope) is not GlobalScope or context.scope.include_allowed == False:
+        if (
+            type(context.scope) is not GlobalScope
+            or context.scope.include_allowed is False
+        ):
             context.new_error("INCLUDE_START_FILE", context.peek_token(i))
             return True, i
         val = context.peek_token(i).value.split("include", 1)[1]
         content = Lexer(val, context.peek_token(i).pos[0])
         tkns = content.get_tokens()
         i = 1
         while i < len(tkns) and tkns[i].type in ["TAB", "SPACE"]:
@@ -37,10 +40,16 @@
                     break
                 i -= 1
         elif i < len(tkns) and tkns[i].type == "STRING":
             try:
                 filetype = tkns[i].value.split(".")[-1][0]
             except:
                 filetype = ""
+        while tkns[i].type != "NEWLINE" and i < len(tkns) - 1:
+            i += 1
+        if (tkns[i].type == "NEWLINE" and tkns[i - 1].type in ["SPACE", "TAB"]) or tkns[
+            i
+        ].type in ["SPACE", "TAB"]:
+            context.new_error("SPC_BEFORE_NL", context.peek_token(0))
         if filetype and filetype != "h":
             context.new_error("INCLUDE_HEADER_ONLY", context.peek_token(0))
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_preprocessor_protection.py` & `norminette-3.3.52/norminette/rules/check_preprocessor_protection.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_prototype_indent.py` & `norminette-3.3.52/norminette/rules/check_prototype_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_spacing.py` & `norminette-3.3.52/norminette/rules/check_spacing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from norminette.rules import Rule
 
-import pdb
 
 class CheckSpacing(Rule):
     def __init__(self):
         super().__init__()
         self.depends_on = []
 
     def run(self, context):
@@ -16,37 +15,35 @@
         if context.history[-1] == "IsEmptyLine":
             return False, 0
         space_tab_error = False
         space_error = False
         while i in range(len(context.tokens[: context.tkn_scope])):
             if context.check_token(i, "SPACE"):
                 if context.check_token(i - 1 if i > 0 else 0, "TAB"):
-                    if space_tab_error == False:
+                    if space_tab_error is False:
                         context.new_error("MIXED_SPACE_TAB", context.peek_token(i - 1))
                         space_tab_error = True
                 if context.peek_token(i).pos[1] == 1:
                     while i < context.tkn_scope and context.check_token(i, "SPACE"):
                         i += 1
                     if context.check_token(i + 1, "NEWLINE"):
                         context.new_error("SPACE_EMPTY_LINE", context.peek_token(i))
                         i += 1
                         continue
                     context.new_error("SPACE_REPLACE_TAB", context.peek_token(i))
                     continue
                 i += 1
                 if context.check_token(i, "SPACE"):
-                    if space_error == False:
+                    if space_error is False:
                         context.new_error("CONSECUTIVE_SPC", context.peek_token(i - 1))
                         space_error = True
                     while i < context.tkn_scope and context.check_token(i, "SPACE"):
                         i += 1
-                if context.check_token(i, "NEWLINE"):
-                    context.new_error("SPC_BEFORE_NL", context.peek_token(i - 1))
                 if context.check_token(i, "TAB"):
-                    if space_tab_error == False:
+                    if space_tab_error is False:
                         context.new_error("MIXED_SPACE_TAB", context.peek_token(i - 1))
                         space_tab_error = True
             elif context.check_token(i, "TAB"):
                 if context.peek_token(i).pos[1] == 1:
                     while context.check_token(i, "TAB"):
                         i += 1
                     if context.check_token(i, "NEWLINE"):
```

### Comparing `norminette-3.3.51/norminette/rules/check_struct_naming.py` & `norminette-3.3.52/norminette/rules/check_struct_naming.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/check_utype_declaration.py` & `norminette-3.3.52/norminette/rules/check_utype_declaration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from norminette.exceptions import CParsingError
 from norminette.rules import Rule
-import pdb
 
 types = [
     "STRUCT",
     "ENUM",
     "UNION",
     "INT",
     "VOID",
@@ -34,68 +33,74 @@
             - Struct names start with s_
             - Enum names start with e_
             - Union names start with u_
             - Typedef names start with t_
         """
         i = 0
         i = context.skip_ws(i)
-        tkns = context.tokens
         is_td = False
         on_newline = False
         utype = None
         contain_full_def = False
         ids = []
-        while context.check_token(i, ["SEMI_COLON"]) is False and i < len(context.tokens):
+        while context.check_token(i, ["SEMI_COLON"]) is False and i < len(
+            context.tokens
+        ):
             if context.check_token(i, ["SPACE", "TAB"]):
                 pass
             if context.check_token(i, ["LPARENTHESIS"]) is True:
                 val, tmp = context.parenthesis_contain(i)
-                if val == None or val == "cast" or val == "var":
+                if val is None or val == "cast" or val == "var":
                     i = tmp
             if context.check_token(i, utypes) is True:
                 utype = context.peek_token(i)
             if context.check_token(i, "TYPEDEF") is True:
                 is_td = True
             if context.check_token(i, "LBRACKET") is True:
                 i = context.skip_nest(i)
             if context.check_token(i, "IDENTIFIER") is True:
                 if context.peek_token(i).value == "__attribute__":
                     i += 1
                     i = context.skip_ws(i)
                     i = context.skip_nest(i)
                     continue
-                if context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"]) is True:
+                if (
+                    context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"])
+                    is True
+                ):
                     tmp = i - 1
-                    while context.check_token(tmp - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"]) is True and context.is_operator(tmp) == False:
+                    while (
+                        context.check_token(
+                            tmp - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"]
+                        )
+                        is True
+                        and context.is_operator(tmp) is False
+                    ):
                         tmp -= 1
-                    # if context.check_token(tmp, "LPARENTHESIS") is True:
-                    #     tmp = tmp - 1
-                    #     while context.check_token(tmp, ["LPARENTHESIS"]) is True and context.is_operator(tmp) == False:
-                    #         tmp -= 1
                     ids.append((context.peek_token(i), tmp))
                 else:
                     ids.append((context.peek_token(i), i))
             if context.check_token(i, "LBRACE") is True:
                 contain_full_def = True
                 i = context.skip_nest(i)
             i += 1
         check = -1
-#        print (ids, utype, contain_full_def)
-        if is_td == True and len(ids) < 2 and utype != None:
+        #        print (ids, utype, contain_full_def)
+        if is_td is True and len(ids) < 2 and utype is not None:
             context.new_error("MISSING_TYPEDEF_ID", context.peek_token(0))
             return False, 0
-        if contain_full_def == False and is_td == False and len(ids) > 1:
+        if contain_full_def is False and is_td is False and len(ids) > 1:
             check = -2
         else:
             check = -1
         if len(ids) == 0:
             return False, 0
         name = ids[0][0]
         loc = ids[check][1]
-        if is_td == True:
+        if is_td is True:
             if ids[check][0].value.startswith("t_") is False:
                 context.new_error("USER_DEFINED_TYPEDEF", context.peek_token(loc))
             if utype is not None:
                 if len(ids) > 1:
                     name = ids[0][0]
                 else:
                     if context.debug >= 1:
@@ -103,53 +108,71 @@
                     elif context.debug == 0:
                         raise CParsingError(
                             f"Error: {context.filename}: Could not parse structure line {context.peek_token(0).pos[0]}"
                         )
             loc = ids[0][1]
         else:
             loc = ids[0][1]
-        if is_td == False:
-            if utype is not None and utype.type == "STRUCT" and name.value.startswith("s_") is False:
+        if is_td is False:
+            if (
+                utype is not None
+                and utype.type == "STRUCT"
+                and name.value.startswith("s_") is False
+            ):
                 context.new_error("STRUCT_TYPE_NAMING", context.peek_token(loc))
-            if utype is not None and utype.type == "UNION" and name.value.startswith("u_") is False:
+            if (
+                utype is not None
+                and utype.type == "UNION"
+                and name.value.startswith("u_") is False
+            ):
                 context.new_error("UNION_TYPE_NAMING", context.peek_token(loc))
-            if utype is not None and utype.type == "ENUM" and name.value.startswith("e_") is False:
+            if (
+                utype is not None
+                and utype.type == "ENUM"
+                and name.value.startswith("e_") is False
+            ):
                 context.new_error("ENUM_TYPE_NAMING", context.peek_token(loc))
-        if is_td or (is_td == False and contain_full_def == False):
+        if is_td or (is_td is False and contain_full_def is False):
             tmp = ids[-1][1] - 1
             tabs = 0
             while (context.check_token(tmp, "TAB")) is True and tmp > 0:
                 tabs += 1
                 tmp -= 1
-            #if tabs > 1:
-                #context.new_error("TOO_MANY_TABS_TD", context.peek_token(tmp))
+            # if tabs > 1:
+            # context.new_error("TOO_MANY_TABS_TD", context.peek_token(tmp))
             if context.check_token(tmp, "SPACE") is True:
                 context.new_error("SPACE_REPLACE_TAB", context.peek_token(tmp))
             tab_error = False
             can_nl_error = False
             while tmp > 0:
                 if context.check_token(tmp, "RBRACE") is True:
                     can_nl_error = True
                     tmp = context.skip_nest_reverse(tmp)
-                if context.check_token(tmp, "TAB") is True and on_newline == False:
+                if context.check_token(tmp, "TAB") is True and on_newline is False:
                     tab_error = True
-                if context.check_token(tmp, "NEWLINE") is True and can_nl_error == False:
+                if (
+                    context.check_token(tmp, "NEWLINE") is True
+                    and can_nl_error is False
+                ):
                     context.new_error("NEWLINE_IN_DECL", context.peek_token(ids[-1][1]))
                     can_nl_error = True
                 tmp -= 1
             if tab_error:
                 context.new_error("TAB_REPLACE_SPACE", context.peek_token(tmp))
-        if contain_full_def == False:
+        if contain_full_def is False:
             i = 0
-            identifier = ids[-1][0]
             i = ids[-1][1]
-            if context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"]) is True:
+            if (
+                context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"])
+                is True
+            ):
                 i -= 1
                 while (
-                    context.check_token(i, ["MULT", "BWISE_AND", "LPARENTHESIS"]) is True
+                    context.check_token(i, ["MULT", "BWISE_AND", "LPARENTHESIS"])
+                    is True
                     and context.is_operator(i) is False
                 ):
                     i -= 1
             current_indent = context.peek_token(i).pos[1]
             if context.scope.vars_alignment == 0:
                 context.scope.vars_alignment = current_indent
             elif context.scope.vars_alignment != current_indent:
```

### Comparing `norminette-3.3.51/norminette/rules/check_variable_declaration.py` & `norminette-3.3.52/norminette/rules/check_variable_declaration.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,45 +29,51 @@
         i = 0
         static_or_const = False
         passed_assign = False
         if context.scope.name == "Function":
             context.scope.vars += 1
             if context.scope.vars > 5:
                 context.new_error("TOO_MANY_VARS_FUNC", context.peek_token(i))
-            if context.history[-2] != "IsBlockStart" and context.history[-2] != "IsVarDeclaration":
+            if (
+                context.history[-2] != "IsBlockStart"
+                and context.history[-2] != "IsVarDeclaration"
+            ):
                 context.new_error("VAR_DECL_START_FUNC", context.peek_token(i))
-            elif context.scope.vdeclarations_allowed == False:
+            elif context.scope.vdeclarations_allowed is False:
                 context.new_error("VAR_DECL_START_FUNC", context.peek_token(i))
-            elif context.scope.vdeclarations_allowed == None:
+            elif context.scope.vdeclarations_allowed is None:
                 context.scope.vdeclarations_allowed = True
-        elif context.scope.name == "GlobalScope" or context.scope.name == "UserDefinedType":
+        elif (
+            context.scope.name == "GlobalScope"
+            or context.scope.name == "UserDefinedType"
+        ):
             pass
         else:
             context.new_error("WRONG_SCOPE_VAR", context.peek_token(i))
         tmp = 0
         ret, tmp = context.check_type_specifier(tmp)
         tmp = context.skip_ws(tmp)
         tmp -= 1
         identifier = False
         while context.check_token(tmp, ["SEMI_COLON"] + assigns) is False:
             if context.check_token(tmp, "IDENTIFIER"):
                 identifier = True
             tmp += 1
-        if identifier == False:
+        if identifier is False:
             context.new_error("IMPLICIT_VAR_TYPE", context.peek_token(0))
             return False
         while context.peek_token(i) and context.check_token(i, "SEMI_COLON") is False:
             if context.check_token(i, "LPARENTHESIS") is True:
                 i = context.skip_nest(i)
             if context.check_token(i, "ASSIGN") is True:
                 passed_assign = True
             if context.check_token(i, ["STATIC", "CONST"]) is True:
                 static_or_const = True
-            if context.check_token(i, assigns) is True and static_or_const == False:
+            if context.check_token(i, assigns) is True and static_or_const is False:
                 if context.scope.name == "GlobalScope":
                     i += 1
                     continue
                 context.new_error("DECL_ASSIGN_LINE", context.peek_token(i))
-            if context.check_token(i, "COMMA") is True and passed_assign == False:
+            if context.check_token(i, "COMMA") is True and passed_assign is False:
                 context.new_error("MULT_DECL_LINE", context.peek_token(i))
             i += 1
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/check_variable_indent.py` & `norminette-3.3.52/norminette/rules/check_variable_indent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import math
 import string
 
 from norminette.rules import Rule
-import pdb
 
 
 keywords = [
     # C reserved keywords #
     "AUTO",
     "BREAK",
     "CASE",
@@ -71,29 +70,35 @@
         has_tab = False
         line_start = True
         id_length = 0
         buffer_len = 0
         while context.check_token(i, assigns_or_eol) is False:
             if context.check_token(i, keywords) is True:
                 type_identifier_nb += 1
-            if context.check_token(i, ["LPARENTHESIS", "LBRACE", "LBRACKET"]) and type_identifier_nb > 0 and context.parenthesis_contain(i)[0] != "pointer":
+            if (
+                context.check_token(i, ["LPARENTHESIS", "LBRACE", "LBRACKET"])
+                and type_identifier_nb > 0
+                and context.parenthesis_contain(i)[0] != "pointer"
+            ):
                 i = context.skip_nest(i)
             i += 1
         i = 0
         while context.check_token(i, assigns_or_eol) is False:
             if context.check_token(i, "LBRACKET") is True:
                 while context.check_token(i, "RBRACKET") is False:
                     if context.check_token(i, "SIZEOF") is True:
                         i += 1
                         i = context.skip_nest(i)
                         continue
                     elif context.check_token(i, "IDENTIFIER") is True:
                         for c in context.peek_token(i).value:
                             if c in string.ascii_lowercase:
-                                context.new_error("VLA_FORBIDDEN", context.peek_token(i))
+                                context.new_error(
+                                    "VLA_FORBIDDEN", context.peek_token(i)
+                                )
                                 break
                         return True, i
                     i += 1
             if context.check_token(i, keywords) is True and type_identifier_nb > 0:
                 line_start = False
                 type_identifier_nb -= 1
                 if context.peek_token(i).length == 0:
@@ -107,44 +112,52 @@
             elif context.check_token(i, "TAB") is False and type_identifier_nb == 0:
                 context.new_error("SPACE_REPLACE_TAB", context.peek_token(i))
                 return True, i
             elif context.check_token(i, "TAB") is True and type_identifier_nb == 0:
                 has_tab += 1
                 current_indent += 1
                 type_identifier_nb -= 1
-            elif context.check_token(i, "TAB") and type_identifier_nb > 0 and line_start == False:
+            elif (
+                context.check_token(i, "TAB")
+                and type_identifier_nb > 0
+                and line_start is False
+            ):
                 context.new_error("TAB_REPLACE_SPACE", context.peek_token(i))
             i += 1
         return False, 0
 
     def run(self, context):
         """
         Each variable must be indented at the same level for its scope
         """
         i = 0
         identifier = None
         ident = [0, 0]
         ret = None
         self.check_tabs(context)
-        while context.peek_token(i) and context.check_token(i, ["SEMI_COLON", "COMMA", "ASSIGN"]) is False:
+        while (
+            context.peek_token(i)
+            and context.check_token(i, ["SEMI_COLON", "COMMA", "ASSIGN"]) is False
+        ):
             if context.check_token(i, ["LBRACKET", "LBRACE"]) is True:
                 i = context.skip_nest(i)
             if context.check_token(i, "LPARENTHESIS") is True:
                 ret, _ = context.parenthesis_contain(i)
             if context.check_token(i, "IDENTIFIER") is True:
                 ident = (context.peek_token(i), i)
                 if ret == "pointer":
                     break
             i += 1
         i = ident[1]
         identifier = ident[0]
         if context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"]) is True:
             i -= 1
             while (
-                context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"]) is True
+                context.check_token(i - 1, ["MULT", "BWISE_AND", "LPARENTHESIS"])
+                is True
                 and context.is_operator(i) is False
             ):
                 i -= 1
             identifier = context.peek_token(i)
         if context.scope.vars_alignment == 0:
             context.scope.vars_alignment = identifier.pos[1]
         elif context.scope.vars_alignment != identifier.pos[1]:
```

### Comparing `norminette-3.3.51/norminette/rules/is_ambiguous_declaration.py` & `norminette-3.3.52/norminette/rules/is_ambiguous_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/is_assignation.py` & `norminette-3.3.52/norminette/rules/is_assignation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from norminette.rules import PrimaryRule
-import pdb
 
 assign_ops = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
     "ADD_ASSIGN",
     "SUB_ASSIGN",
     "MUL_ASSIGN",
@@ -15,17 +14,17 @@
     "ASSIGN",
     "INC",
     "DEC",
 ]
 
 SEPARATORS = [
     "COMMA",
-    "AND",
-    "OR",
-    "SEMI_COLON"
+    # "AND",
+    # "OR",
+    "SEMI_COLON",
 ]
 
 types = [
     "CHAR",
     "DOUBLE",
     "ENUM",
     "FLOAT",
@@ -64,23 +63,19 @@
 class IsAssignation(PrimaryRule):
     def __init__(self):
         super().__init__()
         self.primary = True
         self.priority = 20
         self.scope = []
 
-    def skip_ptr(self, context, pos):
-        i = context.skip_ws(pos)
-        while context.check_token(i, operators + ws + ["IDENTIFIER"]) is True:
-            i += 1
-        return i
-
     def check_identifier(self, context, pos):
         i = pos
-        while context.check_token(i, types + ws + op + ["IDENTIFIER", "CONSTANT", "INC", "DEC"]):
+        while context.check_token(
+            i, types + ws + op + ["IDENTIFIER", "CONSTANT", "INC", "DEC"]
+        ):
             if context.check_token(i, "LBRACKET"):
                 i = context.skip_nest(i)
             i += 1
         if "IDENTIFIER" in [t.type for t in context.tokens[: i + 1]]:
             return True, i
         else:
             return False, 0
@@ -88,37 +83,41 @@
     def parse_assign_right_side(self, context, i):
         while context.check_token(i, SEPARATORS) is False:
             if context.check_token(i, ["LBRACE", "LPARENTHESIS", "LBRACKET"]):
                 i = context.skip_nest(i)
             i += 1
         return i
 
-
     def run(self, context):
         """
         Catches all assignation instructions
         Requires assign token
         """
+        # pdb.set_trace()
         ret, i = self.check_identifier(context, 0)
         if ret is False:
             return False, 0
         tmp = 0
         while context.check_token(tmp, assign_ops) is False and tmp <= i:
             tmp += 1
         if context.check_token(tmp, assign_ops) is False:
             return False, 0
         i = tmp + 1
-        #i += 1
+        # i += 1
         i = context.skip_ws(i)
         # if context.check_token(i, "LBRACE") is True:
         # i += 1
         # context.sub = context.scope.inner(VariableAssignation)
         # return True, i
         if context.scope.name == "UserDefinedEnum":
-            while context.peek_token(i) and (context.check_token(i, ["COMMA", "SEMI_COLON", "NEWLINE"])) is False:
+            while (
+                context.peek_token(i)
+                and (context.check_token(i, ["COMMA", "SEMI_COLON", "NEWLINE"]))
+                is False
+            ):
                 i += 1
             i = context.eol(i)
             return True, i
         i = self.parse_assign_right_side(context, i)
         # while context.check_token(i, SEPARATORS) is False:
         #     i += 1
         #     if context.peek_token(i) is None:
```

### Comparing `norminette-3.3.51/norminette/rules/is_block_end.py` & `norminette-3.3.52/norminette/rules/is_block_end.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/is_cast.py` & `norminette-3.3.52/norminette/rules/is_cast.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/is_control_statement.py` & `norminette-3.3.52/norminette/rules/is_control_statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 whitespaces = ["TAB", "SPACE", "NEWLINE"]
 
 
 class IsControlStatement(PrimaryRule):
     def __init__(self):
         super().__init__()
-        self.priority = 70
+        self.priority = 65
         self.scope = [Function, ControlStructure, GlobalScope]
 
     def run(self, context):
         """
         Catches control statements, including for/switch
         Includes the condition, even if over multiple lines
         """
@@ -78,24 +78,24 @@
                 return True, i
             else:
                 context.sub = context.scope.inner(ControlStructure)
                 context.sub.multiline = False
                 i = context.eol(i)
                 return True, i
         i += 1
-        if id_instead_cs == True:
+        if id_instead_cs is True:
             return False, 0
         i = context.skip_ws(i, nl=False)
         if context.check_token(i, "LPARENTHESIS") is False:
             return False, 0
         i = context.skip_nest(i)
         i += 1
         tmp = context.skip_ws(i, nl=True)
         if context.check_token(tmp, "SEMI_COLON") is True:
-            if is_id == True:
+            if is_id is True:
                 return False, 0
             tmp += 1
             tmp = context.eol(tmp)
             return True, tmp
         i = context.skip_ws(i, nl=False)
         context.sub = context.scope.inner(ControlStructure)
         context.sub.multiline = False
```

### Comparing `norminette-3.3.51/norminette/rules/is_declaration.py` & `norminette-3.3.52/norminette/rules/is_declaration.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,25 @@
         self.scope = []
 
     def run(self, context):
         # return False, 0
         i = context.skip_ws(0, nl=False)
         p = 0
         ident = None
-        while context.peek_token(i) is not None and context.check_token(i, "SEMI_COLON") is False:
+        while (
+            context.peek_token(i) is not None
+            and context.check_token(i, "SEMI_COLON") is False
+        ):
             if context.check_token(i, "LPARENTHESIS"):
                 p += 1
             if context.check_token(i, "RPARENTHESIS"):
                 p -= 1
             if context.check_token(i, ["IDENTIFIER", "NULL"]):
                 ident = context.peek_token(i)
             i += 1
         i += 1
         i = context.skip_ws(i, nl=False)
         if context.check_token(i, "NEWLINE"):
             i += 1
-        if p == 0 and ident != None:
+        if p == 0 and ident is not None:
             return True, i
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/is_empty_line.py` & `norminette-3.3.52/norminette/rules/is_ternary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from norminette.rules import PrimaryRule
+from norminette.rules import Rule
 
 
-cs_keywords = ["DO", "WHILE", "FOR", "IF", "ELSE", "SWITCH"]
-whitespaces = ["TAB", "SPACE", "NEWLINE"]
-
-
-class IsEmptyLine(PrimaryRule):
+class IsTernary(Rule):
     def __init__(self):
         super().__init__()
-        self.priority = 65
+        self.priority = 53
         self.scope = []
 
     def run(self, context):
         """
-        Catches empty line
-        BUG: Catches end of line token on unrecognized line
+        Catches ternaries and raises an error
         """
         i = 0
-        while context.check_token(i, ["SPACE", "TAB"]) is True:
+        while context.peek_token(i) is not None and context.check_token(i, ["SEMI_COLON", "NEWLINE"]) is False:
+            if context.check_token(i, "TERN_CONDITION") is True:
+                while context.peek_token(i) is not None and context.check_token(i, ["SEMI_COLON", "NEWLINE"]) is False:
+                    i += 1
+                i += 1
+                i = context.eol(i)
+                return True, i
             i += 1
-        if context.check_token(i, "NEWLINE") is True:
-            i = context.eol(i)
-            return True, i
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/is_enum_var_decl.py` & `norminette-3.3.52/norminette/rules/is_enum_var_decl.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,29 @@
         while context.peek_token(i) and context.check_token(i, sep) is False:
             if context.check_token(i, lbrackets) is True:
                 i = context.skip_nest(i)
             i += 1
         return True, i
 
     def var_declaration(self, context, pos):
-        pclose = ["RPARENTHESIS", "NEWLINE", "SPACE", "TAB"]
         brackets = 0
         parenthesis = 0
         braces = 0
         i = pos
         identifier = False
-        while context.peek_token(i) is not None and context.check_token(i, ["COMMA", "RBRACE", "NEWLINE"]) is False:
-            if context.check_token(i, "IDENTIFIER") is True and braces == 0 and brackets == 0 and parenthesis == 0:
+        while (
+            context.peek_token(i) is not None
+            and context.check_token(i, ["COMMA", "RBRACE", "NEWLINE"]) is False
+        ):
+            if (
+                context.check_token(i, "IDENTIFIER") is True
+                and braces == 0
+                and brackets == 0
+                and parenthesis == 0
+            ):
                 identifier = True
             elif context.check_token(i, lbrackets) is True:
                 if context.check_token(i, "LBRACE") is True:
                     braces += 1
                 if context.check_token(i, "LBRACKET") is True:
                     brackets += 1
                 if context.check_token(i, "LPARENTHESIS") is True:
@@ -42,26 +49,28 @@
                 if context.check_token(i, "RBRACE") is True:
                     braces -= 1
                 if context.check_token(i, "RBRACKET") is True:
                     brackets -= 1
                 if context.check_token(i, "RPARENTHESIS") is True:
                     parenthesis -= 1
             elif context.check_token(i, "ASSIGN") is True:
-                if identifier == False:
+                if identifier is False:
                     return False, pos
                 ret, i = self.assignment_right_side(context, i + 1)
                 i -= 1
                 if ret is False:
                     return False, pos
-            elif context.check_token(i, ["SPACE", "TAB", "MULT", "BWISE_AND", "NEWLINE"]):
+            elif context.check_token(
+                i, ["SPACE", "TAB", "MULT", "BWISE_AND", "NEWLINE"]
+            ):
                 pass
             elif parenthesis == 0 and brackets == 0 and braces == 0:
                 return False, 0
             i += 1
-        if identifier == False:
+        if identifier is False:
             return False, pos
         if context.check_token(i, ["NEWLINE", "COMMA"]) is True:
             return True, i
         return False, pos
 
     def run(self, context):
         """
```

### Comparing `norminette-3.3.51/norminette/rules/is_expression_statement.py` & `norminette-3.3.52/norminette/rules/is_expression_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from norminette.context import ControlStructure
 from norminette.scope import Function
 from norminette.exceptions import CParsingError
 from norminette.rules import PrimaryRule
-import pdb
+
 keywords = ["BREAK", "CONTINUE", "GOTO", "RETURN"]
 
 operators = [
     "MULT",
     "LPARENTHESIS",
     "RPARENTHESIS",
     "LBRACKET",
@@ -32,22 +32,27 @@
             while context.check_token(i, "SEMI_COLON") is False:
                 i += 1
             i += 1
             return True, i
         elif context.check_token(pos, "GOTO"):
             i = pos + 1
             i = context.skip_ws(i)
-            while context.check_token(i, ["MULT", "BWISE_AND"]) is True and context.is_operator(i) is False:
+            while (
+                context.check_token(i, ["MULT", "BWISE_AND"]) is True
+                and context.is_operator(i) is False
+            ):
                 i += 1
             if context.check_token(i, "IDENTIFIER") is False:
                 if context.check_token(i, "LPARENTHESIS") is True:
                     # parse label value here
                     i = context.skip_nest(i)
                 elif context.debug == 0:
-                    raise CParsingError("Error: Goto statement should be followed by a label")
+                    raise CParsingError(
+                        "Error: Goto statement should be followed by a label"
+                    )
             i += 1
             i = context.skip_ws(i)
             i += 1
             return True, i
         else:
             i = pos + 1
             i = context.skip_ws(i)
@@ -133,15 +138,15 @@
         """
         Catches expression statement by elimination
         """
         i = context.skip_ws(0)
         ret, i = self.check_instruction(context, i)
         if ret is False:
             ret, i = self.check_reserved_keywords(context, i)
-            #if ret is False:
+            # if ret is False:
             #    ret, i = self.check_inc_dec(context, i)
             if ret is False:
                 ret, i = self.void_identifier(context, i)
                 if ret is False:
                     return False, 0
         i = context.eol(i)
         return True, i
```

### Comparing `norminette-3.3.51/norminette/rules/is_func_declaration.py` & `norminette-3.3.52/norminette/rules/is_func_prototype.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-from norminette.scope import Function
 from norminette.context import GlobalScope
+from norminette.scope import UserDefinedType
 from norminette.rules import PrimaryRule
 
-import pdb
-
 whitespaces = ["SPACE", "TAB"]
-
-SEPARATORS = [
-    "COMMA",
-    "AND",
-    "OR",
-    "SEMI_COLON"
-]
 preproc = [
     "DEFINE",
     "ERROR",
     "ENDIF",
     "ELIF",
     "IFDEF",
     "IFNDEF",
@@ -62,22 +53,22 @@
     "UNION",
     "VOID",
     "LONG",
     "SHORT",
 ]
 
 
-class IsFuncDeclaration(PrimaryRule):
+class IsFuncPrototype(PrimaryRule):
     def __init__(self):
         super().__init__()
-        self.priority = 81
+        self.priority = 82
         self.scope = [GlobalScope]
 
     def check_args(self, context, pos):
-        i = context.skip_ws(pos, nl=True)
+        i = context.skip_ws(pos)
         while context.check_token(i, whitespaces + ["RPARENTHESIS"]):
             i += 1
         if context.check_token(i, "LPARENTHESIS") is False:
             return False, pos
         p = 1
         i += 1
         while p:
@@ -87,157 +78,157 @@
                 p -= 1
             elif context.peek_token(i) is None:
                 return False, 0
             i += 1
         return True, i
 
     def check_func_identifier(self, context, pos):
-        i = context.skip_ws(pos, nl=True)
+        i = context.skip_ws(pos)
         pp = 0  # Pointer operator's position
         lp = 0  # Left parenthesis counter (nesting level)
-
         if context.check_token(i, "IDENTIFIER"):
             i += 1
             return True, i, False
 
         d = ["LPARENTHESIS", "MULT"] + whitespaces
         while context.check_token(i, d):
             if context.check_token(i, "MULT") and not pp:
                 pp = i
             elif pp and context.check_token(i, "LPARENTHESIS"):
                 lp += 1
             i += 1
-        i = context.skip_misc_specifier(i, nl=True)
+        i = context.skip_misc_specifier(i)
         if context.check_token(i, "IDENTIFIER") is False:
             return False, pos, False
 
         i += 1
         while context.check_token(i, ["RPARENTHESIS"] + whitespaces):
             if context.check_token(i, "RPARENTHESIS"):
                 lp -= 1
             i += 1
-        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS"):
+        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS") is False:
             return False, pos, False
-
         return True, i, (True if pp else False)
 
     def check_func_format(self, context):
         i = context.skip_ws(0, nl=False)
         type_id = []
         misc_id = []
-        identifier = None
+        arg_start = 0
+        arg_end = 0
         args = False
+        identifier = None
         if context.check_token(i, "NEWLINE") is True:
             return False, 0
-        while context.peek_token(i):
-            while context.check_token(i, "IDENTIFIER") is True and context.peek_token(i).value == "__attribute__":
+        while context.peek_token(i):  # and context.check_token(i, "NEWLINE") is False:
+            while (
+                context.check_token(i, "IDENTIFIER") is True
+                and context.peek_token(i).value == "__attribute__"
+            ):
                 i += 1
                 i = context.skip_ws(i)
-                i = context.skip_nest(i)
+                i = context.skip_nest(i) + 1
                 i = context.skip_ws(i)
-            if context.check_token(i, "NEWLINE") is True and identifier == False and misc_id == [] and type_id == []:
-                return False, 0
             if context.check_token(i, misc_identifier) is True:
                 misc_id.append(context.peek_token(i))
             elif context.check_token(i, type_identifier) is True:
                 type_id.append(context.peek_token(i))
-            if context.check_token(i, assigns + ["TYPEDEF", "COMMA", "LBRACE"] + preproc) is True:
+            if (
+                context.check_token(
+                    i, assigns + ["TYPEDEF", "COMMA", "LBRACE", "RBRACE"] + preproc
+                )
+                is True
+            ):
                 return False, 0
             if context.check_token(i, "SEMI_COLON") is True:
-                return False, 0
+                break
             elif context.check_token(i, "IDENTIFIER") is True:
                 if identifier is not None:
                     type_id.append(identifier[0])
                 identifier = (context.peek_token(i), i)
-            if context.check_token(i, "NEWLINE") is True:
-                if args == False:
-                    i += 1
-                    continue
-                else:
-                    break
             if context.check_token(i, "LPARENTHESIS") is True:
                 par = context.parenthesis_contain(i)
                 if par[0] == "function":
                     if identifier is not None:
                         type_id.append(identifier[0])
                     while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
                         i += 1
                     identifier = (context.peek_token(i), i)
                     i = context.skip_nest(i)
-                elif identifier is not None:
+                elif par[0] == "pointer":
+                    if identifier is not None:
+                        type_id.append(identifier[0])
+                    while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
+                        i += 1
+                    identifier = (context.peek_token(i), i)
+                    nxt = par[1] + 1
+                    if context.check_token(nxt, ["LPARENTHESIS"]) is False:
+                        return False, 0
+                    i = context.skip_nest(i)
+                else:
                     args = True
                     arg_start = i
                     i = context.skip_nest(i)
                     arg_end = i
-                    while (context.check_token(i, "RPARENTHESIS")) is True:
-                        i += 1
-                    i = context.skip_ws(i)
-                    if context.check_token(i, "LPARENTHESIS") is True:
-                        arg_start = i
-                        i = context.skip_nest(i)
-                        arg_end = i
                     break
-                else:
-                    i += 1
             else:
                 i += 1
-        if len(type_id) > 0 and args == True and identifier != None:
+        if len(type_id) > 0 and args is True and identifier is not None:
             i = identifier[1]
-            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]) is True:
                 i += 1
             sc = context.scope
             while type(sc) != GlobalScope:
                 sc = sc.outer()
             sc.fnames.append(context.peek_token(i).value)
+            if context.func_alignment == 0:
+                tmp = i
+                while context.check_token(
+                    tmp - 1, ["LPARENTHESIS", "MULT", "BWISE_AND"]
+                ):
+                    tmp -= 1
+                context.func_alignment = int(context.peek_token(tmp).pos[1] / 4)
             context.fname_pos = i
             context.arg_pos = [arg_start, arg_end]
             i = arg_end
-            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["RPARENTHESIS"]) is True:
                 i += 1
-            i = context.skip_ws(i, nl=True)
-            if context.check_token(i, "LPARENTHESIS") is True:
-                i = context.skip_nest(i)
+            i = context.skip_nest(i)
+            while context.check_token(i, ["RPARENTHESIS"]) is True:
                 i += 1
             i = context.skip_ws(i, nl=True)
-            while context.check_token(i, "LBRACKET"):
-                i = context.skip_nest(i)
-                i += 1
-                i = context.skip_ws(i, nl=True)
-            while context.check_token(i, "IDENTIFIER") is True and context.peek_token(i).value == "__attribute__":
-                i += 1
-                i = context.skip_ws(i)
-                i = context.skip_nest(i) + 1
-                i = context.skip_ws(i)
             return True, i
         return False, 0
 
     def run(self, context):
         """
-        Catches function declaration
+        Catches function prototypes
         Allows newline inside it
-        Creates context variable for function name, arg_start, arg_end
+        End condition is SEMI_COLON token, otherwise line will be considered as
+        function declaration
         """
-        if type(context.scope) is not GlobalScope:
+        if (
+            type(context.scope) is not GlobalScope
+            and type(context.scope) is not UserDefinedType
+        ):
             return False, 0
         ret, read = self.check_func_format(context)
         if ret is False:
             return False, 0
+        if context.check_token(read, "IDENTIFIER") is True:
+            while context.peek_token(read).value == "__attribute__":
+                read += 1
+                read = context.skip_ws(read)
+                read = context.skip_nest(read) + 1
+                read = context.skip_ws(read, nl=True)
         while context.check_token(read, ["COMMENT", "MULT_COMMENT"]) is True:
             read += 1
         read = context.skip_ws(read, nl=False)
-        if context.check_token(read, ["NEWLINE", "LBRACE"] + preproc):
-            if context.check_token(read, ["LBRACE"] + preproc) is True:
-                read -= 1
-            context.scope.functions += 1
-            read += 1
-            context.sub = context.scope.inner(Function)
-            read = context.eol(read)
-            return True, read
+        if context.check_token(read, "NEWLINE"):
+            return False, 0
 
-        elif context.check_token(read, SEPARATORS):
+        elif context.check_token(read, "SEMI_COLON"):
             read += 1
             read = context.eol(read)
-            return False, 0
+            return True, read
 
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/is_func_prototype.py` & `norminette-3.3.52/norminette/rules/is_func_declaration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from norminette.scope import Function
 from norminette.context import GlobalScope
-from norminette.scope import UserDefinedType
 from norminette.rules import PrimaryRule
 
-import pdb
 
 whitespaces = ["SPACE", "TAB"]
+
+SEPARATORS = ["COMMA", "AND", "OR", "SEMI_COLON"]
 preproc = [
     "DEFINE",
     "ERROR",
     "ENDIF",
     "ELIF",
     "IFDEF",
     "IFNDEF",
@@ -55,22 +56,22 @@
     "UNION",
     "VOID",
     "LONG",
     "SHORT",
 ]
 
 
-class IsFuncPrototype(PrimaryRule):
+class IsFuncDeclaration(PrimaryRule):
     def __init__(self):
         super().__init__()
-        self.priority = 82
+        self.priority = 81
         self.scope = [GlobalScope]
 
     def check_args(self, context, pos):
-        i = context.skip_ws(pos)
+        i = context.skip_ws(pos, nl=True)
         while context.check_token(i, whitespaces + ["RPARENTHESIS"]):
             i += 1
         if context.check_token(i, "LPARENTHESIS") is False:
             return False, pos
         p = 1
         i += 1
         while p:
@@ -80,144 +81,173 @@
                 p -= 1
             elif context.peek_token(i) is None:
                 return False, 0
             i += 1
         return True, i
 
     def check_func_identifier(self, context, pos):
-        i = context.skip_ws(pos)
+        i = context.skip_ws(pos, nl=True)
         pp = 0  # Pointer operator's position
         lp = 0  # Left parenthesis counter (nesting level)
+
         if context.check_token(i, "IDENTIFIER"):
             i += 1
             return True, i, False
 
         d = ["LPARENTHESIS", "MULT"] + whitespaces
         while context.check_token(i, d):
             if context.check_token(i, "MULT") and not pp:
                 pp = i
             elif pp and context.check_token(i, "LPARENTHESIS"):
                 lp += 1
             i += 1
-        i = context.skip_misc_specifier(i)
+        i = context.skip_misc_specifier(i, nl=True)
         if context.check_token(i, "IDENTIFIER") is False:
             return False, pos, False
 
         i += 1
         while context.check_token(i, ["RPARENTHESIS"] + whitespaces):
             if context.check_token(i, "RPARENTHESIS"):
                 lp -= 1
             i += 1
-        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS") is False:
+        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS"):
             return False, pos, False
+
         return True, i, (True if pp else False)
 
     def check_func_format(self, context):
         i = context.skip_ws(0, nl=False)
         type_id = []
         misc_id = []
-        arg_start = 0
-        arg_end = 0
-        args = False
         identifier = None
+        args = False
         if context.check_token(i, "NEWLINE") is True:
             return False, 0
-        while context.peek_token(i):  # and context.check_token(i, "NEWLINE") is False:
-            while context.check_token(i, "IDENTIFIER") is True and context.peek_token(i).value == "__attribute__":
+        while context.peek_token(i):
+            while (
+                context.check_token(i, "IDENTIFIER") is True
+                and context.peek_token(i).value == "__attribute__"
+            ):
                 i += 1
                 i = context.skip_ws(i)
-                i = context.skip_nest(i) + 1
+                i = context.skip_nest(i)
                 i = context.skip_ws(i)
+            if (
+                context.check_token(i, "NEWLINE") is True
+                and identifier is False
+                and misc_id == []
+                and type_id == []
+            ):
+                return False, 0
             if context.check_token(i, misc_identifier) is True:
                 misc_id.append(context.peek_token(i))
             elif context.check_token(i, type_identifier) is True:
                 type_id.append(context.peek_token(i))
-            if context.check_token(i, assigns + ["TYPEDEF", "COMMA", "LBRACE", "RBRACE"] + preproc) is True:
+            if (
+                context.check_token(
+                    i, assigns + ["TYPEDEF", "COMMA", "LBRACE"] + preproc
+                )
+                is True
+            ):
                 return False, 0
             if context.check_token(i, "SEMI_COLON") is True:
-                break
+                return False, 0
             elif context.check_token(i, "IDENTIFIER") is True:
                 if identifier is not None:
                     type_id.append(identifier[0])
                 identifier = (context.peek_token(i), i)
+            if context.check_token(i, "NEWLINE") is True:
+                if args is False:
+                    i += 1
+                    continue
+                else:
+                    break
             if context.check_token(i, "LPARENTHESIS") is True:
                 par = context.parenthesis_contain(i)
                 if par[0] == "function":
                     if identifier is not None:
                         type_id.append(identifier[0])
                     while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
                         i += 1
                     identifier = (context.peek_token(i), i)
                     i = context.skip_nest(i)
-                elif par[0] == "pointer":
-                    if identifier is not None:
-                        type_id.append(identifier[0])
-                    while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
-                        i += 1
-                    identifier = (context.peek_token(i), i)
-                    nxt = par[1] + 1
-                    if context.check_token(nxt, ["LPARENTHESIS"]) is False:
-                        return False, 0
-                    i = context.skip_nest(i)
-                else:
+                elif identifier is not None:
                     args = True
                     arg_start = i
                     i = context.skip_nest(i)
                     arg_end = i
+                    while (context.check_token(i, "RPARENTHESIS")) is True:
+                        i += 1
+                    i = context.skip_ws(i)
+                    if context.check_token(i, "LPARENTHESIS") is True:
+                        arg_start = i
+                        i = context.skip_nest(i)
+                        arg_end = i
                     break
+                else:
+                    i += 1
             else:
                 i += 1
-        if len(type_id) > 0 and args == True and identifier != None:
+        if len(type_id) > 0 and args is True and identifier is not None:
             i = identifier[1]
+            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]) is True:
                 i += 1
             sc = context.scope
             while type(sc) != GlobalScope:
                 sc = sc.outer()
             sc.fnames.append(context.peek_token(i).value)
-            if context.func_alignment == 0:
-                tmp = i
-                while context.check_token(tmp - 1, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
-                    tmp -= 1
-                context.func_alignment = int(context.peek_token(tmp).pos[1] / 4)
             context.fname_pos = i
             context.arg_pos = [arg_start, arg_end]
             i = arg_end
+            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["RPARENTHESIS"]) is True:
                 i += 1
-            i = context.skip_nest(i)
-            while context.check_token(i, ["RPARENTHESIS"]) is True:
+            i = context.skip_ws(i, nl=True)
+            if context.check_token(i, "LPARENTHESIS") is True:
+                i = context.skip_nest(i)
                 i += 1
             i = context.skip_ws(i, nl=True)
+            while context.check_token(i, "LBRACKET"):
+                i = context.skip_nest(i)
+                i += 1
+                i = context.skip_ws(i, nl=True)
+            while (
+                context.check_token(i, "IDENTIFIER") is True
+                and context.peek_token(i).value == "__attribute__"
+            ):
+                i += 1
+                i = context.skip_ws(i)
+                i = context.skip_nest(i) + 1
+                i = context.skip_ws(i)
             return True, i
         return False, 0
 
     def run(self, context):
         """
-        Catches function prototypes
+        Catches function declaration
         Allows newline inside it
-        End condition is SEMI_COLON token, otherwise line will be considered as
-        function declaration
+        Creates context variable for function name, arg_start, arg_end
         """
-        if type(context.scope) is not GlobalScope and type(context.scope) is not UserDefinedType:
+        if type(context.scope) is not GlobalScope:
             return False, 0
         ret, read = self.check_func_format(context)
         if ret is False:
             return False, 0
-        if context.check_token(read, "IDENTIFIER") is True:
-            while context.peek_token(read).value == "__attribute__":
-                read += 1
-                read = context.skip_ws(read)
-                read = context.skip_nest(read) + 1
-                read = context.skip_ws(read, nl=True)
         while context.check_token(read, ["COMMENT", "MULT_COMMENT"]) is True:
             read += 1
         read = context.skip_ws(read, nl=False)
-        if context.check_token(read, "NEWLINE"):
-            return False, 0
-
-        elif context.check_token(read, "SEMI_COLON"):
+        if context.check_token(read, ["NEWLINE", "LBRACE"] + preproc):
+            if context.check_token(read, ["LBRACE"] + preproc) is True:
+                read -= 1
+            context.scope.functions += 1
             read += 1
+            context.sub = context.scope.inner(Function)
             read = context.eol(read)
             return True, read
 
+        elif context.check_token(read, SEPARATORS):
+            read += 1
+            read = context.eol(read)
+            return False, 0
+
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/is_function_call.py` & `norminette-3.3.52/norminette/rules/is_function_call.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,20 +22,15 @@
     "MULT",
     "DIV",
     "MODULO",
     "LESS_THAN",
     "MORE_THAN",
 ]
 
-SEPARATORS = [
-    "COMMA",
-    "AND",
-    "OR",
-    "SEMI_COLON"
-]
+SEPARATORS = ["COMMA", "AND", "OR", "SEMI_COLON"]
 
 assign_ops = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
     "ADD_ASSIGN",
     "SUB_ASSIGN",
     "MUL_ASSIGN",
@@ -96,20 +91,22 @@
     def run(self, context):
         """
         Catches function calls when it's in an assignation
         """
         i = context.skip_ws(0, nl=False)
         types = []
         while context.check_token(i, "LPARENTHESIS") is True:
-            start = i
             typ, i = context.parenthesis_contain(i)
             types.append(typ)
-            if typ == None or typ == "pointer":
+            if typ is None or typ == "pointer":
                 i = context.skip_ws(i + 1)
-                if context.peek_token(i) is None or context.check_token(i, "NEWLINE") is True:
+                if (
+                    context.peek_token(i) is None
+                    or context.check_token(i, "NEWLINE") is True
+                ):
                     return False, 0
                 # i += 1
                 if len(types) > 1:
                     i = context.skip_ws(i, nl=False)
                     if context.check_token(i, SEPARATORS) is True:
                         i += 1
                         i = context.eol(i)
@@ -120,19 +117,27 @@
                 i += 1
                 i = context.skip_ws(i)
         while context.check_token(i, ["MULT", "BWISE_AND"]):
             i += 1
         if context.check_token(i, "IDENTIFIER") is True:
             i += 1
             i = context.skip_ws(i)
-            if context.check_token(i, "LPARENTHESIS") is True:
-                i = context.skip_nest(i)
-                while context.peek_token(i) is not None and context.check_token(i, SEPARATORS) is False:
+            if context.check_token(i, "LPARENTHESIS"):
+                while context.check_token(i, "LPARENTHESIS") is True:
+                    i = context.skip_nest(i) + 1
+                while (
+                    context.peek_token(i) is not None
+                    and context.check_token(i, SEPARATORS) is False
+                ):
                     i += 1
                 i += 1
                 i = context.eol(i)
                 return True, i
-        elif len(types) > 1 and typ == "cast" and (types[-2] == "function" or types[-2] == "pointer"):
+        elif (
+            len(types) > 1
+            and typ == "cast"
+            and (types[-2] == "function" or types[-2] == "pointer")
+        ):
             i += 1
             i = context.eol(i)
             return True, i
         return False, 0
```

### Comparing `norminette-3.3.51/norminette/rules/is_label.py` & `norminette-3.3.52/norminette/rules/is_label.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/is_preprocessor_statement.py` & `norminette-3.3.52/norminette/rules/is_preprocessor_statement.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/rules/is_user_defined_type.py` & `norminette-3.3.52/norminette/rules/is_user_defined_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from norminette.rules import PrimaryRule
 from norminette.scope import UserDefinedType, GlobalScope, UserDefinedEnum
-import pdb
 
 utypes = ["TYPEDEF", "UNION", "STRUCT", "ENUM"]
 
 
 class IsUserDefinedType(PrimaryRule):
     def __init__(self):
         super().__init__()
@@ -25,16 +24,14 @@
         return True, i
 
     def utype_definition(self, context, pos):
         utypes = ["STRUCT", "ENUM", "UNION"]
         if not [tkn for tkn in context.tokens[:pos] if tkn.type in utypes]:
             return False, pos
         return True, pos
-        i = context.skip_ws(i)
-        return ret, i
 
     def run(self, context):
         """
         Catches user type definitions
         Can include the whole type definition in case it's a structure
         Variable declarations aren't included
         """
@@ -64,15 +61,15 @@
                 enum = True
             if context.check_token(i, ["NEWLINE", "SEMI_COLON"]) is True and p == 0:
                 break
             if context.check_token(i, "IDENTIFIER"):
                 ids.append(context.peek_token(i))
             i += 1
         if context.check_token(i, "NEWLINE") is True and p <= 0:
-            if enum == True:
+            if enum is True:
                 context.sub = context.scope.inner(UserDefinedEnum)
             else:
                 context.sub = context.scope.inner(UserDefinedType)
             i = context.eol(i)
             return True, i
         elif context.check_token(i, "SEMI_COLON") is True:
             i += 1
```

### Comparing `norminette-3.3.51/norminette/rules/is_var_declaration.py` & `norminette-3.3.52/norminette/rules/is_var_declaration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from norminette.context import ControlStructure
 from norminette.scope import Function
 from norminette.context import GlobalScope
 from norminette.scope import UserDefinedType
 from norminette.rules import PrimaryRule
-import pdb
 
 lbrackets = ["LBRACE", "LPARENTHESIS", "LBRACKET"]
 rbrackets = ["RBRACE", "RPARENTHESIS", "RBRACKET"]
 
 misc_specifiers = [
     "CONST",
     "REGISTER",
@@ -31,14 +30,15 @@
     "LONG",
     "SHORT",
     "STRUCT",
     "ENUM",
     "UNION",
 ]
 
+
 class IsVarDeclaration(PrimaryRule):
     def __init__(self):
         super().__init__()
         self.priority = 75
         self.scope = [GlobalScope, UserDefinedType, Function, ControlStructure]
 
     def assignment_right_side(self, context, pos):
@@ -47,37 +47,51 @@
         while context.peek_token(i) and context.check_token(i, sep) is False:
             if context.check_token(i, lbrackets) is True:
                 i = context.skip_nest(i)
             i += 1
         return True, i
 
     def var_declaration(self, context, pos, identifier=False):
-        pclose = ["RPARENTHESIS", "NEWLINE", "SPACE", "TAB"]
         brackets = 0
         parenthesis = 0
         braces = 0
         i = pos
         ret_store = None
         ids = []
-        while context.peek_token(i) is not None and context.check_token(i, ["SEMI_COLON"]) is False:
-            if context.check_token(i, "IDENTIFIER") is True and braces == 0 and brackets == 0 and parenthesis == 0:
+        while (
+            context.peek_token(i) is not None
+            and context.check_token(i, ["SEMI_COLON"]) is False
+        ):
+            if (
+                context.check_token(i, "IDENTIFIER") is True
+                and braces == 0
+                and brackets == 0
+                and parenthesis == 0
+            ):
                 identifier = True
                 ids.append(context.peek_token(i))
             elif context.check_token(i, ["COMMENT", "MULT_COMMENT"]) is True:
                 i += 1
                 continue
-            elif context.check_token(i, ["COLON", "CONSTANT"]) is True and identifier == True:
+            elif (
+                context.check_token(i, ["COLON", "CONSTANT"]) is True
+                and identifier is True
+            ):
                 i += 1
                 continue
             elif context.check_token(i, lbrackets) is True:
                 if context.check_token(i, "LBRACE") is True:
                     braces += 1
                 if context.check_token(i, "LBRACKET") is True:
                     brackets += 1
-                if context.check_token(i, "LPARENTHESIS") is True and brackets == 0 and braces == 0:
+                if (
+                    context.check_token(i, "LPARENTHESIS") is True
+                    and brackets == 0
+                    and braces == 0
+                ):
                     ret, tmp = context.parenthesis_contain(i, ret_store)
                     if ret == "function" or ret == "pointer" or ret == "var":
                         ret_store = ret
                         identifier = True
                         tmp2 = tmp - 1
                         deep = 1
                         while tmp2 > 0 and deep > 0:
@@ -95,28 +109,38 @@
                 if context.check_token(i, "RBRACE") is True:
                     braces -= 1
                 if context.check_token(i, "RBRACKET") is True:
                     brackets -= 1
                 if context.check_token(i, "RPARENTHESIS") is True:
                     parenthesis -= 1
             elif context.check_token(i, "ASSIGN") is True:
-                if identifier == False:
+                if identifier is False:
                     return False, pos
                 ret, i = self.assignment_right_side(context, i + 1)
                 i -= 1
                 if ret is False:
                     return False, pos
-            elif context.check_token(i, ["SPACE", "TAB", "MULT", "BWISE_AND", "NEWLINE"] + misc_specifiers + type_specifiers):
+            elif context.check_token(
+                i,
+                ["SPACE", "TAB", "MULT", "BWISE_AND", "NEWLINE"]
+                + misc_specifiers
+                + type_specifiers,
+            ):
                 pass
-            elif context.check_token(i, "COMMA") is True and parenthesis == 0 and brackets == 0 and braces == 0:
+            elif (
+                context.check_token(i, "COMMA") is True
+                and parenthesis == 0
+                and brackets == 0
+                and braces == 0
+            ):
                 break
             elif parenthesis == 0 and brackets == 0 and braces == 0:
                 return False, 0
             i += 1
-        if identifier == False or braces > 0 or brackets > 0 or parenthesis > 0:
+        if identifier is False or braces > 0 or brackets > 0 or parenthesis > 0:
             return False, 0
         context.scope.vars_name.append(ids[-1])
         if context.check_token(i, "SEMI_COLON") is True:
             if brackets <= 0 and braces <= 0 and parenthesis <= 0:
                 return True, i
             else:
                 return False, 0
@@ -146,15 +170,14 @@
             if context.check_token(i, "LPARENTHESIS") is True:
                 p += 1
                 if identifier is True:
                     return False, pos
             elif context.check_token(i, "RPARENTHESIS") is True:
                 p -= 1
                 if identifier is True:
-                    par_pos = i
                     break
             elif context.check_token(i, "IDENTIFIER") is True:
                 identifier = True
             i += 1
         else:
             return False, pos
         i += 1
```

### Comparing `norminette-3.3.51/norminette/rules/rule.py` & `norminette-3.3.52/norminette/rules/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
         for rule in self.depends_on:
             if rule in registry.dependencies:
                 registry.dependencies[rule].append(self.name)
             else:
                 registry.dependencies[rule] = [self.name]
 
+
 class PrimaryRule(Rule):
     def __init__(self):
         super().__init__()
         self.primary = True
         self.priority = 0
         self.scope = []
```

### Comparing `norminette-3.3.51/norminette/scope.py` & `norminette-3.3.52/norminette/scope.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.51/norminette/tools/colors.py` & `norminette-3.3.52/norminette/tools/colors.py`

 * *Files identical despite different names*

