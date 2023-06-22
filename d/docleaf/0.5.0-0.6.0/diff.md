# Comparing `tmp/docleaf-0.5.0-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.6.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1074984 bytes, number of entries: 10
--rw-r--r--  4.6 unx     6823 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     3836 b- defN 23-Jun-18 17:03 docleaf/copied.py
--rw-r--r--  4.6 unx     3709 b- defN 23-Jun-18 17:03 docleaf/domains.py
--rw-r--r--  4.6 unx    20597 b- defN 23-Jun-18 17:03 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jun-18 17:03 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-18 17:03 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3031040 b- defN 23-Jun-18 17:03 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      775 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/RECORD
-10 files, 3070548 bytes uncompressed, 1073678 bytes compressed:  65.0%
+Zip file size: 1074955 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     6823 b- defN 23-Jun-20 20:51 docleaf-0.6.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-20 20:51 docleaf-0.6.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3573 b- defN 23-Jun-20 20:51 docleaf-0.6.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     3836 b- defN 23-Jun-20 20:51 docleaf/copied.py
+-rw-r--r--  4.6 unx     3709 b- defN 23-Jun-20 20:51 docleaf/domains.py
+-rw-r--r--  4.6 unx    17707 b- defN 23-Jun-20 20:51 docleaf/doxygen.py
+-rw-r--r--  4.6 unx       99 b- defN 23-Jun-20 20:51 docleaf/errors.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-20 20:51 docleaf/__init__.py
+-rwxr-xr-x  4.6 unx  3031552 b- defN 23-Jun-20 20:51 docleaf/backend.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      775 b- defN 23-Jun-20 20:51 docleaf-0.6.0.dist-info/RECORD
+10 files, 3068170 bytes uncompressed, 1073649 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: docleaf-0.5.0.dist-info/METADATA
+Filename: docleaf-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.5.0.dist-info/WHEEL
+Filename: docleaf-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.5.0.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.6.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: docleaf/copied.py
 Comment: 
 
 Filename: docleaf/domains.py
 Comment: 
@@ -21,11 +21,11 @@
 
 Filename: docleaf/__init__.py
 Comment: 
 
 Filename: docleaf/backend.cp39-win_amd64.pyd
 Comment: 
 
-Filename: docleaf-0.5.0.dist-info/RECORD
+Filename: docleaf-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docleaf/doxygen.py

```diff
@@ -152,14 +152,15 @@
             self.build_target(**attributes["target"]),
             self.directive_arguments,
             children,
         )
 
     def build_internal_reference(self, *children, **attributes):
         reference = sphinx.addnodes.pending_xref(
+            "",
             *children,
             reftype="ref",
             refdomain="std",
             refexplicit=True,
             refid=attributes["refid"],
             reftarget=attributes["refid"],
         )
@@ -213,19 +214,19 @@
 def render_node(node, node_manager):
     if node.type == "text":
         return [nodes.Text(node.text)]
 
     node_builder = node_manager.get_builder(node.type)
     children = render_node_list(node.children, node_manager)
 
-    if node.call_as == "source-text":
+    if node.call_as == "text-element":
         return node_builder("", "", *children, **node.attributes)
-    elif node.call_as == "source":
+    elif node.call_as == "element":
         return node_builder("", *children, **node.attributes)
-    elif node.call_as == "args":
+    elif node.call_as == "function":
         return node_builder(*children, **node.attributes)
     else:
         raise DocleafError("Call As not implemented: " + node.call_as)
 
 
 class Project:
     def __init__(self, root, xml):
@@ -278,129 +279,58 @@
             self.content_offset,
             self.block_text,
             self.state,
             self.state_machine,
         ]
 
 
-class ClassDirective(BaseDirective):
+class BasicDoxygenDirective(BaseDirective):
     has_content = True
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = True
     option_spec = {
         "project": directives.unchanged,
+        "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
         project_name = self.options["project"] or self.app.config.docleaf_default_project
         project = Project.get(self.app.config.docleaf_projects, project_name)
-
         skip_settings = get_skip_settings(self.app, self.options)
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
-
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_class(name, project.xml(), context, tracked_cache)
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
-
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
-
-
-class StructDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-    }
 
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-        skip_settings = get_skip_settings(self.app, self.options)
         context = backend.Context(
             project.root(),
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_struct(name, project.xml(), context, tracked_cache)
+        node_list = self.render_function(name, project.xml(), context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
-class EnumDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-        "skip-xml-nodes": directives.unchanged,
-    }
+class ClassDirective(BasicDoxygenDirective):
+    render_function = backend.render_class
 
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-        skip_settings = get_skip_settings(self.app, self.options)
 
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
+class StructDirective(BasicDoxygenDirective):
+    render_function = backend.render_struct
 
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_enum(name, project.xml(), context, tracked_cache)
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
+class EnumDirective(BasicDoxygenDirective):
+    render_function = backend.render_enum
 
 
-class FunctionDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-        "skip-xml-nodes": directives.unchanged,
-    }
-
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-        skip_settings = get_skip_settings(self.app, self.options)
-
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
-
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_function(name, project.xml(), context, tracked_cache)
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
-
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
+class FunctionDirective(BasicDoxygenDirective):
+    render_function = backend.render_function
 
 
 class GroupDirective(BaseDirective):
     has_content = True
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = True
@@ -553,18 +483,18 @@
 
 def setup(app: Sphinx):
     cache = backend.FileCache()
 
     context = ExtensionContext(app, cache)
 
     add_directive(context, "doxygenclass", ClassDirective)
-    add_directive(context, "doxygenstruct", StructDirective)
-    add_directive(context, "doxygenfunction", FunctionDirective)
     add_directive(context, "doxygenenum", EnumDirective)
+    add_directive(context, "doxygenfunction", FunctionDirective)
     add_directive(context, "doxygengroup", GroupDirective)
+    add_directive(context, "doxygenstruct", StructDirective)
 
     app.add_config_value("docleaf_projects", {}, "env")
     app.add_config_value("docleaf_default_project", None, "env")
     app.add_config_value("docleaf_doxygen_skip", [], "env")
     app.add_config_value("docleaf_domain_by_extension", {}, True)
 
     app.connect("env-get-outdated", calculate_files_to_refresh)
```

## Comparing `docleaf-0.5.0.dist-info/METADATA` & `docleaf-0.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,<6,!=5.0.0
 License-File: LICENSE.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Keywords: sphinx,doxygen
 Author-email: Michael Jones <michael.jones@docleaf.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://docleaf.io
 Project-URL: repository, https://github.com/docleaf-labs/docleaf
+Project-URL: homepage, https://docleaf.io
 Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
 
 <h1 align="center">
   Docleaf
 </h1>
 
 <p align="center">
```

## Comparing `docleaf-0.5.0.dist-info/license_files/LICENSE.md` & `docleaf-0.6.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

