# Comparing `tmp/typos-1.15.4.tar.gz` & `tmp/typos-1.15.5.tar.gz`

## Comparing `typos-1.15.4.tar` & `typos-1.15.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44486 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  7026151 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.4/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-06-22 15:19:35.000000 typos-1.15.4/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.4/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.4/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12622 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21814 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32485 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5919 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123      207 2023-06-22 15:19:35.000000 typos-1.15.4/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      123    52781 2023-06-22 15:19:35.000000 typos-1.15.4/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.4/PKG-INFO
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.5/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44720 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.5/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.5/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.5/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.5/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  7026151 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-06-22 17:37:01.000000 typos-1.15.5/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.5/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.5/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12622 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21859 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32621 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     5919 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123      207 2023-06-22 17:37:01.000000 typos-1.15.5/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      123    52781 2023-06-22 17:37:01.000000 typos-1.15.5/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.5/PKG-INFO
```

### Comparing `typos-1.15.4/local_dependencies/typos/Cargo.toml` & `typos-1.15.5/local_dependencies/typos/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos"
-version = "0.10.13"
+version = "0.10.14"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.4/local_dependencies/typos/src/check.rs` & `typos-1.15.5/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/typos/src/dict.rs` & `typos-1.15.5/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/typos/src/tokens.rs` & `typos-1.15.5/local_dependencies/typos/src/tokens.rs`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         // Generally a language would be `{XID_Start}{XID_Continue}*` but going with only
         // `{XID_Continue}+` because XID_Continue is a superset of XID_Start and rather catch odd
         // or unexpected cases than strip off start characters to a word since we aren't doing a
         // proper word boundary parse
-        take_while1(is_xid_continue).parse_next(input)
+        take_while(1.., is_xid_continue).parse_next(input)
     }
 
     fn ignore<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
@@ -197,15 +197,18 @@
 
     fn other<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        (one_of(|c| !is_xid_continue(c)), take_while0(is_ignore_char))
+        (
+            one_of(|c| !is_xid_continue(c)),
+            take_while(0.., is_ignore_char),
+        )
             .recognize()
             .parse_next(input)
     }
 
     fn ordinal_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
@@ -215,39 +218,43 @@
         fn is_sep(c: impl AsChar) -> bool {
             let c = c.as_char();
             // Avoid markdown throwing off our ordinal detection
             ['_'].contains(&c)
         }
 
         (
-            take_while0(is_sep),
-            take_while1(is_dec_digit),
+            take_while(0.., is_sep),
+            take_while(1.., is_dec_digit),
             alt((('s', 't'), ('n', 'd'), ('r', 'd'), ('t', 'h'))),
-            take_while0(is_sep),
+            take_while(0.., is_sep),
         )
             .recognize()
             .parse_next(input)
     }
 
     fn dec_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        take_while1(is_dec_digit_with_sep).parse_next(input)
+        take_while(1.., is_dec_digit_with_sep).parse_next(input)
     }
 
     fn hex_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        preceded(('0', alt(('x', 'X'))), take_while1(is_hex_digit_with_sep)).parse_next(input)
+        preceded(
+            ('0', alt(('x', 'X'))),
+            take_while(1.., is_hex_digit_with_sep),
+        )
+        .parse_next(input)
     }
 
     fn css_color<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
@@ -321,15 +328,15 @@
 
     fn base64_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        let (padding, captured) = take_while1(is_base64_digit).parse_next(input.clone())?;
+        let (padding, captured) = take_while(1.., is_base64_digit).parse_next(input.clone())?;
 
         const CHUNK: usize = 4;
         let padding_offset = input.offset_to(&padding);
         let mut padding_len = CHUNK - padding_offset % CHUNK;
         if padding_len == CHUNK {
             padding_len = 0;
         }
@@ -356,57 +363,57 @@
     fn email_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         (
-            take_while1(is_localport_char),
+            take_while(1.., is_localport_char),
             '@',
-            take_while1(is_domain_char),
+            take_while(1.., is_domain_char),
         )
             .recognize()
             .parse_next(input)
     }
 
     fn url_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         (
             opt(terminated(
-                take_while1(is_scheme_char),
+                take_while(1.., is_scheme_char),
                 // HACK: Technically you can skip `//` if you don't have a domain but that would
                 // get messy to support.
                 (':', '/', '/'),
             )),
             (
                 opt(terminated(url_userinfo, '@')),
-                take_while1(is_domain_char),
-                opt(preceded(':', take_while1(AsChar::is_dec_digit))),
+                take_while(1.., is_domain_char),
+                opt(preceded(':', take_while(1.., AsChar::is_dec_digit))),
             ),
             '/',
             // HACK: Too lazy to enumerate
-            take_while0(is_path_query_fragment),
+            take_while(0.., is_path_query_fragment),
         )
             .recognize()
             .parse_next(input)
     }
 
     fn url_userinfo<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         (
-            take_while1(is_localport_char),
-            opt(preceded(':', take_while0(is_localport_char))),
+            take_while(1.., is_localport_char),
+            opt(preceded(':', take_while(0.., is_localport_char))),
         )
             .recognize()
             .parse_next(input)
     }
 
     fn c_escape<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
@@ -414,33 +421,38 @@
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         // We don't know whether the string we are parsing is a literal string (no escaping) or
         // regular string that does escaping. The escaped letter might be part of a word, or it
         // might not be. Rather than guess and be wrong part of the time and correct people's words
         // incorrectly, we opt for just not evaluating it at all.
-        preceded(take_while1(is_escape), take_while0(is_xid_continue)).parse_next(input)
+        preceded(take_while(1.., is_escape), take_while(0.., is_xid_continue)).parse_next(input)
     }
 
     fn printf<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        preceded('%', take_while1(is_xid_continue)).parse_next(input)
+        preceded('%', take_while(1.., is_xid_continue)).parse_next(input)
     }
 
     fn take_many0<I, E, F>(mut f: F) -> impl FnMut(I) -> IResult<I, <I as Stream>::Slice, E>
     where
         I: Stream,
         F: winnow::Parser<I, <I as Stream>::Slice, E>,
         E: winnow::error::ParseError<I>,
     {
-        move |i: I| repeat0(f.by_ref()).map(|()| ()).recognize().parse_next(i)
+        move |i: I| {
+            repeat(0.., f.by_ref())
+                .map(|()| ())
+                .recognize()
+                .parse_next(i)
+        }
     }
 
     #[inline]
     fn is_dec_digit(i: impl AsChar + Copy) -> bool {
         i.is_dec_digit()
     }
```

### Comparing `typos-1.15.4/local_dependencies/typos-vars/Cargo.toml` & `typos-1.15.5/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.15.5/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/varcon-core/Cargo.toml` & `typos-1.15.5/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.15.5/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/varcon-core/src/lib.rs` & `typos-1.15.5/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/varcon-core/src/parser.rs` & `typos-1.15.5/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/typos-dict/Cargo.toml` & `typos-1.15.5/local_dependencies/typos-dict/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.15.5/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/dictgen/Cargo.toml` & `typos-1.15.5/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/dictgen/src/map.rs` & `typos-1.15.5/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/dictgen/src/table.rs` & `typos-1.15.5/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/local_dependencies/dictgen/src/trie.rs` & `typos-1.15.5/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/Cargo.toml` & `typos-1.15.5/rust_src/typos-cli/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.15.4"
+version = "1.15.5"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.4/rust_src/typos-cli/benches/checks.rs` & `typos-1.15.5/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/benches/corrections.rs` & `typos-1.15.5/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/benches/data.rs` & `typos-1.15.5/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.15.5/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.15.5/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.15.5/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.15.5/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/config.rs` & `typos-1.15.5/rust_src/typos-cli/src/config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use std::collections::HashMap;
 
 use kstring::KString;
 
+pub const SUPPORTED_FILE_NAMES: &[&str] = &["typos.toml", "_typos.toml", ".typos.toml"];
+
 #[derive(Debug, Clone, Default, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 #[serde(rename_all = "kebab-case")]
 pub struct Config {
     pub files: Walk,
     pub default: EngineConfig,
@@ -13,17 +15,15 @@
     pub type_: TypeEngineConfig,
     #[serde(skip)]
     pub overrides: EngineConfig,
 }
 
 impl Config {
     pub fn from_dir(cwd: &std::path::Path) -> Result<Option<Self>, anyhow::Error> {
-        let config = if let Some(path) =
-            find_project_file(cwd, &["typos.toml", "_typos.toml", ".typos.toml"])
-        {
+        let config = if let Some(path) = find_project_file(cwd, SUPPORTED_FILE_NAMES) {
             log::debug!("Loading {}", path.display());
             Some(Self::from_file(&path)?)
         } else {
             None
         };
         Ok(config)
     }
```

### Comparing `typos-1.15.4/rust_src/typos-cli/src/default_types.rs` & `typos-1.15.5/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/dict.rs` & `typos-1.15.5/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/file.rs` & `typos-1.15.5/rust_src/typos-cli/src/file.rs`

 * *Files 1% similar despite different names*

```diff
@@ -680,14 +680,20 @@
     let entry = match entry {
         Ok(entry) => entry,
         Err(err) => {
             report_error(err, reporter)?;
             return Ok(());
         }
     };
+    if crate::config::SUPPORTED_FILE_NAMES
+        .iter()
+        .any(|n| *n == entry.file_name())
+    {
+        return Ok(());
+    }
     if entry.file_type().map(|t| t.is_file()).unwrap_or(true) {
         let explicit = entry.depth() == 0;
         let (path, lookup_path) = if entry.is_stdin() {
             let path = std::path::Path::new("-");
             (path, std::env::current_dir()?)
         } else {
             let path = entry.path();
```

### Comparing `typos-1.15.4/rust_src/typos-cli/src/file_type.rs` & `typos-1.15.5/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/policy.rs` & `typos-1.15.5/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/rust_src/typos-cli/src/report.rs` & `typos-1.15.5/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.4/Cargo.lock` & `typos-1.15.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1611,15 +1611,15 @@
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typos"
-version = "0.10.13"
+version = "0.10.14"
 dependencies = [
  "anyhow",
  "bstr",
  "itertools",
  "once_cell",
  "serde",
  "simdutf8",
@@ -1627,15 +1627,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.15.4"
+version = "1.15.5"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
```

### Comparing `typos-1.15.4/PKG-INFO` & `typos-1.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.15.4
+Version: 1.15.5
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

