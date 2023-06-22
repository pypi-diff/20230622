# Comparing `tmp/typos-1.15.3.tar.gz` & `tmp/typos-1.15.4.tar.gz`

## Comparing `typos-1.15.3.tar` & `typos-1.15.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.3/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.3/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.3/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44486 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.3/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  7026151 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.3/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-06-21 19:54:53.000000 typos-1.15.3/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.3/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.3/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12622 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21534 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32485 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5919 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123      207 2023-06-21 19:54:53.000000 typos-1.15.3/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      123    52781 2023-06-21 19:54:52.000000 typos-1.15.3/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.3/PKG-INFO
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44486 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  7026151 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.4/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.4/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12622 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21814 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32485 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     5919 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123      207 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      123    52781 2023-06-22 15:19:35.000000 typos-1.15.4/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.4/PKG-INFO
```

### Comparing `typos-1.15.3/local_dependencies/typos-vars/Cargo.toml` & `typos-1.15.4/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.15.4/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/dictgen/Cargo.toml` & `typos-1.15.4/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/dictgen/src/map.rs` & `typos-1.15.4/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/dictgen/src/table.rs` & `typos-1.15.4/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/dictgen/src/trie.rs` & `typos-1.15.4/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos/Cargo.toml` & `typos-1.15.4/local_dependencies/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos/src/check.rs` & `typos-1.15.4/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos/src/dict.rs` & `typos-1.15.4/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos/src/tokens.rs` & `typos-1.15.4/local_dependencies/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos-dict/Cargo.toml` & `typos-1.15.4/local_dependencies/typos-dict/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.15.4/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/varcon-core/Cargo.toml` & `typos-1.15.4/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.15.4/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/varcon-core/src/lib.rs` & `typos-1.15.4/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/local_dependencies/varcon-core/src/parser.rs` & `typos-1.15.4/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/Cargo.toml` & `typos-1.15.4/rust_src/typos-cli/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.15.3"
+version = "1.15.4"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.3/rust_src/typos-cli/benches/checks.rs` & `typos-1.15.4/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/benches/corrections.rs` & `typos-1.15.4/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/benches/data.rs` & `typos-1.15.4/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.15.4/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/config.rs` & `typos-1.15.4/rust_src/typos-cli/src/config.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 use std::collections::HashMap;
 
+use kstring::KString;
+
 #[derive(Debug, Clone, Default, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 #[serde(rename_all = "kebab-case")]
 pub struct Config {
     pub files: Walk,
     pub default: EngineConfig,
@@ -144,114 +146,122 @@
 }
 
 #[derive(Debug, Clone, Default, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 #[serde(transparent)]
 pub struct TypeEngineConfig {
-    pub patterns: std::collections::HashMap<kstring::KString, GlobEngineConfig>,
+    pub patterns: std::collections::HashMap<KString, GlobEngineConfig>,
 }
 
 impl TypeEngineConfig {
     pub fn from_defaults() -> Self {
-        let empty = Self::default();
-        Self {
-            patterns: empty.patterns().collect(),
-        }
+        let patterns = [
+            (
+                KString::from("lock"),
+                GlobEngineConfig {
+                    extend_glob: Vec::new(),
+                    engine: EngineConfig {
+                        check_file: Some(false),
+                        ..Default::default()
+                    },
+                },
+            ),
+            (
+                KString::from("vim"),
+                GlobEngineConfig {
+                    extend_glob: Vec::new(),
+                    engine: EngineConfig {
+                        dict: Some(DictConfig {
+                            extend_identifiers: maplit::hashmap! {
+                                "windo".into() => "windo".into(),
+                            },
+                            ..Default::default()
+                        }),
+                        ..Default::default()
+                    },
+                },
+            ),
+            (
+                KString::from("vimscript"),
+                GlobEngineConfig {
+                    extend_glob: Vec::new(),
+                    engine: EngineConfig {
+                        dict: Some(DictConfig {
+                            extend_identifiers: maplit::hashmap! {
+                                "windo".into() => "windo".into(),
+                            },
+                            ..Default::default()
+                        }),
+                        ..Default::default()
+                    },
+                },
+            ),
+            (
+                KString::from("rust"),
+                GlobEngineConfig {
+                    extend_glob: Vec::new(),
+                    engine: EngineConfig {
+                        dict: Some(DictConfig {
+                            extend_identifiers: maplit::hashmap! {
+                                "flate2".into() => "flate2".into(),
+                            },
+                            extend_words: maplit::hashmap! {
+                                "ser".into() => "ser".into(),
+                            },
+                            ..Default::default()
+                        }),
+                        ..Default::default()
+                    },
+                },
+            ),
+            (
+                KString::from("py"),
+                GlobEngineConfig {
+                    extend_glob: Vec::new(),
+                    engine: EngineConfig {
+                        dict: Some(DictConfig {
+                            extend_identifiers: maplit::hashmap! {
+                                "NDArray".into() => "NDArray".into(),
+                            },
+                            ..Default::default()
+                        }),
+                        ..Default::default()
+                    },
+                },
+            ),
+            (
+                KString::from("cert"),
+                GlobEngineConfig {
+                    extend_glob: Vec::new(),
+                    engine: EngineConfig {
+                        check_file: Some(false),
+                        ..Default::default()
+                    },
+                },
+            ),
+        ]
+        .into_iter()
+        .collect();
+        Self { patterns }
     }
 
     pub fn update(&mut self, source: &Self) {
         for (type_name, engine) in source.patterns.iter() {
             self.patterns
                 .entry(type_name.to_owned())
                 .or_insert_with(GlobEngineConfig::default)
                 .update(engine);
         }
     }
 
     pub fn patterns(&self) -> impl Iterator<Item = (kstring::KString, GlobEngineConfig)> {
-        let mut patterns = self.patterns.clone();
-        patterns
-            .entry("lock".into())
-            .or_insert_with(|| GlobEngineConfig {
-                extend_glob: Vec::new(),
-                engine: EngineConfig {
-                    check_file: Some(false),
-                    ..Default::default()
-                },
-            });
-        patterns
-            .entry("vim".into())
-            .or_insert_with(|| GlobEngineConfig {
-                extend_glob: Vec::new(),
-                engine: EngineConfig {
-                    dict: Some(DictConfig {
-                        extend_identifiers: maplit::hashmap! {
-                            "windo".into() => "windo".into(),
-                        },
-                        ..Default::default()
-                    }),
-                    ..Default::default()
-                },
-            });
-        patterns
-            .entry("vimscript".into())
-            .or_insert_with(|| GlobEngineConfig {
-                extend_glob: Vec::new(),
-                engine: EngineConfig {
-                    dict: Some(DictConfig {
-                        extend_identifiers: maplit::hashmap! {
-                            "windo".into() => "windo".into(),
-                        },
-                        ..Default::default()
-                    }),
-                    ..Default::default()
-                },
-            });
-        patterns
-            .entry("rust".into())
-            .or_insert_with(|| GlobEngineConfig {
-                extend_glob: Vec::new(),
-                engine: EngineConfig {
-                    dict: Some(DictConfig {
-                        extend_identifiers: maplit::hashmap! {
-                            "flate2".into() => "flate2".into(),
-                        },
-                        extend_words: maplit::hashmap! {
-                            "ser".into() => "ser".into(),
-                        },
-                        ..Default::default()
-                    }),
-                    ..Default::default()
-                },
-            });
-        patterns
-            .entry("py".into())
-            .or_insert_with(|| GlobEngineConfig {
-                extend_glob: Vec::new(),
-                engine: EngineConfig {
-                    dict: Some(DictConfig {
-                        extend_identifiers: maplit::hashmap! {
-                            "NDArray".into() => "NDArray".into(),
-                        },
-                        ..Default::default()
-                    }),
-                    ..Default::default()
-                },
-            });
-        patterns
-            .entry("cert".into())
-            .or_insert_with(|| GlobEngineConfig {
-                extend_glob: Vec::new(),
-                engine: EngineConfig {
-                    check_file: Some(false),
-                    ..Default::default()
-                },
-            });
-        patterns.into_iter()
+        let mut engine = Self::from_defaults();
+        engine.update(self);
+        engine.patterns.into_iter()
     }
 }
 
 #[derive(Debug, Clone, Default, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 //#[serde(deny_unknown_fields)]  // Doesn't work with `flatten`
 #[serde(default)]
 #[serde(rename_all = "kebab-case")]
```

### Comparing `typos-1.15.3/rust_src/typos-cli/src/default_types.rs` & `typos-1.15.4/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/dict.rs` & `typos-1.15.4/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/file.rs` & `typos-1.15.4/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/file_type.rs` & `typos-1.15.4/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/policy.rs` & `typos-1.15.4/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/rust_src/typos-cli/src/report.rs` & `typos-1.15.4/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.3/Cargo.lock` & `typos-1.15.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1627,15 +1627,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.15.3"
+version = "1.15.4"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
```

### Comparing `typos-1.15.3/PKG-INFO` & `typos-1.15.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.15.3
+Version: 1.15.4
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

