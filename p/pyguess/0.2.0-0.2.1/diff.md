# Comparing `tmp/pyguess-0.2.0.tar.gz` & `tmp/pyguess-0.2.1.tar.gz`

## Comparing `pyguess-0.2.0.tar` & `pyguess-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 pyguess-0.2.0/local_dependencies/guess-rs/Cargo.toml
--rw-r--r--   0     1000     1000     3471 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/benches/guess_bench.rs
--rw-r--r--   0     1000     1000    15793 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/addr.rs
--rw-r--r--   0     1000     1000      671 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/candidate.rs
--rw-r--r--   0     1000     1000     5077 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/config.rs
--rw-r--r--   0     1000     1000    17940 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/guessr.rs
--rw-r--r--   0     1000     1000     1553 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/lib.rs
--rw-r--r--   0     1000     1000      550 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/main.rs
--rw-r--r--   0     1000     1000     2257 2023-06-13 12:39:45.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/metrics.rs
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 pyguess-0.2.0/Cargo.toml
--rw-r--r--   0     1000     1000      162 2023-06-22 05:51:09.000000 pyguess-0.2.0/Pipfile
--rw-r--r--   0     1000     1000      840 2023-06-22 05:51:09.000000 pyguess-0.2.0/README.md
--rw-r--r--   0     1000     1000      628 2023-06-22 05:51:09.000000 pyguess-0.2.0/examples/basic.py
--rw-r--r--   0     1000     1000     1101 2023-06-22 05:51:09.000000 pyguess-0.2.0/examples/file.py
--rw-r--r--   0     1000     1000     1816 2023-06-22 05:51:09.000000 pyguess-0.2.0/pyguess.pyi
--rw-r--r--   0     1000     1000      944 2023-06-22 05:51:09.000000 pyguess-0.2.0/pyproject.toml
--rw-r--r--   0     1000     1000     5487 2023-06-22 05:51:09.000000 pyguess-0.2.0/src/lib.rs
--rw-r--r--   0     1000     1000        0 2023-06-22 05:51:09.000000 pyguess-0.2.0/tests/__init__.py
--rw-r--r--   0     1000     1000      994 2023-06-22 05:51:09.000000 pyguess-0.2.0/tests/test_pyguess.py
--rw-r--r--   0     1000     1000    27778 2023-06-20 14:50:10.000000 pyguess-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 pyguess-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 pyguess-0.2.1/local_dependencies/guess-rs/Cargo.toml
+-rw-r--r--   0     1000     1000     3270 2023-06-22 11:06:07.000000 pyguess-0.2.1/local_dependencies/guess-rs/benches/guess_bench.rs
+-rw-r--r--   0     1000     1000    15050 2023-06-22 11:06:07.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/addr.rs
+-rw-r--r--   0     1000     1000      671 2023-06-22 05:51:09.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/candidate.rs
+-rw-r--r--   0     1000     1000     4615 2023-06-22 11:06:07.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/config.rs
+-rw-r--r--   0     1000     1000    17756 2023-06-22 11:06:07.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/guessr.rs
+-rw-r--r--   0     1000     1000     1553 2023-06-22 05:51:09.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/lib.rs
+-rw-r--r--   0     1000     1000      550 2023-06-22 05:51:09.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/main.rs
+-rw-r--r--   0     1000     1000     2257 2023-06-13 12:39:45.000000 pyguess-0.2.1/local_dependencies/guess-rs/src/metrics.rs
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 pyguess-0.2.1/Cargo.toml
+-rw-r--r--   0     1000     1000      162 2023-06-22 05:51:09.000000 pyguess-0.2.1/Pipfile
+-rw-r--r--   0     1000     1000      781 2023-06-22 11:06:07.000000 pyguess-0.2.1/README.md
+-rw-r--r--   0     1000     1000      579 2023-06-22 11:06:07.000000 pyguess-0.2.1/examples/basic.py
+-rw-r--r--   0     1000     1000     1052 2023-06-22 11:06:07.000000 pyguess-0.2.1/examples/file.py
+-rw-r--r--   0     1000     1000     1623 2023-06-22 11:06:07.000000 pyguess-0.2.1/pyguess.pyi
+-rw-r--r--   0     1000     1000      945 2023-06-22 11:06:07.000000 pyguess-0.2.1/pyproject.toml
+-rw-r--r--   0     1000     1000     5243 2023-06-22 11:06:07.000000 pyguess-0.2.1/src/lib.rs
+-rw-r--r--   0     1000     1000        0 2023-06-22 05:51:09.000000 pyguess-0.2.1/tests/__init__.py
+-rw-r--r--   0     1000     1000      948 2023-06-22 11:06:07.000000 pyguess-0.2.1/tests/test_pyguess.py
+-rw-r--r--   0     1000     1000    27778 2023-06-22 11:00:12.000000 pyguess-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 pyguess-0.2.1/PKG-INFO
```

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/Cargo.toml` & `pyguess-0.2.1/local_dependencies/guess-rs/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "guess-rs"
-version = "0.2.0"
+version = "0.2.1"
 authors = ["Vladyslav Rezohlazov <vladyslav.rezohlazov@novalytica.com>"]
 edition = "2021"
 license = "MIT"
 description = "The library to Match Swiss Streets"
 keywords = ["guess-rs", "nlp", "street-processing", "text-processing"]
 categories = ["text-processing"]
 readme = "../README.md"
```

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/benches/guess_bench.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/benches/guess_bench.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use guess_rs::{addr, guessr::STREET_NAMES_FILE, *};
 
 fn bench_street_matcher(c: &mut Criterion) {
-    c.bench_function("Guess Location::Place", |b| {
-        b.iter(|| {
-            Location::Place(black_box("Bern City".to_string())).guess(&Config::default(), None);
-        })
-    });
-
     c.bench_function("Guess address with Location::Place", |b| {
         b.iter(|| {
             guessr::guess_address(
                 black_box("ch de saint-cierges 3"),
                 black_box(Location::Place("bercher".to_string())),
                 black_box(Config::default()),
             )
@@ -77,27 +71,27 @@
             )
             .unwrap()
         })
     });
 
     c.bench_function("Search in file (JaroWinkler)", |b| {
         b.iter(|| {
-            let cfg = Config::new(0.6, 0.8, 100, StringMetric::JaroWinkler, None, None, None);
+            let cfg = Config::new(0.6, 0.8, 100, StringMetric::JaroWinkler, None, None);
             guessr::search_in_candidates_file(
                 black_box("ch de saint-cierges 3,fas23dfsfsdf"),
                 black_box(&cfg.path_to_streets.join(STREET_NAMES_FILE)),
                 black_box(&cfg),
             )
             .unwrap()
         })
     });
 
     c.bench_function("Search in file (Jaro)", |b| {
         b.iter(|| {
-            let cfg = Config::new(0.5, 0.8, 500, StringMetric::Jaro, None, None, None);
+            let cfg = Config::new(0.5, 0.8, 500, StringMetric::Jaro, None, None);
             guessr::search_in_candidates_file(
                 black_box("ch de saint-cierges 3"),
                 black_box(&cfg.path_to_streets.join("street_names.txt")),
                 black_box(&cfg),
             )
             .unwrap()
         })
```

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/addr.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/addr.rs`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,34 @@
 use toml::Value;
 
 pub(crate) const PLACE_UBOUND: f64 = 0.8;
 const STRING_METRIC_PLACE: StringMetric = StringMetric::JaroWinkler;
 const FILE_EXTENSION: &str = "toml";
 const FORWARD_SLASH_REPL: &str = "%2C";
 pub(crate) const STREETS_DATA_PATH: &str = "../misc/data/streets_data";
-pub(crate) const PLACES_PATH: &str = "../misc/data/places.txt";
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub enum Location {
     Place(String),
     Zip(usize),
     Empty,
 }
 
 impl Location {
-    pub fn guess(&self, config: &Config, candidates: Option<Vec<String>>) -> Self {
+    pub fn guess(&self, config: &Config, candidates: Vec<String>) -> Self {
         match self {
             Self::Place(place) => {
                 let config = Config {
                     ubound: UBound::new(PLACE_UBOUND),
                     max_candidates: 1,
                     metric_fn: STRING_METRIC_PLACE.into(),
                     ..config.clone()
                 };
-                let guessed_location = if let Some(candidates) = candidates {
-                    guessr::search_in_candidates_list(place, &candidates, &config)
-                } else {
-                    guessr::search_in_candidates_file(place, &config.path_to_places, &config)
-                };
+                let guessed_location =
+                    guessr::search_in_candidates_list(place, &candidates, &config);
                 guessed_location.ok().map_or(Self::Empty, |location| {
                     Self::Place(location[0].sequence.to_string())
                 })
             }
             _ => self.clone(),
         }
     }
@@ -286,43 +282,29 @@
 }
 
 #[inline]
 fn get_all_streets_empty_loc(value: &Value) -> (Vec<String>, Location) {
     (get_all_streets(value), Location::Empty)
 }
 
-fn streets_from_location_list(
+pub(crate) fn streets_from_location(
     value: &Value,
     location: &Location,
     config: &Config,
 ) -> (Vec<String>, Location) {
     let locations = get_locations(value);
-    match location.guess(config, Some(locations)) {
+    match location.guess(config, locations) {
         Location::Empty => get_all_streets_empty_loc(value),
         guessed_location => value.get(&guessed_location.to_string()).map_or_else(
             || get_all_streets_empty_loc(value),
             |x| (iter_from_toml_value(x).collect(), guessed_location),
         ),
     }
 }
 
-pub(crate) fn streets_from_location(
-    value: &Value,
-    location: &Location,
-    config: &Config,
-) -> (Vec<String>, Location) {
-    match location.guess(config, None) {
-        Location::Empty => streets_from_location_list(value, location, config),
-        guessed_location => value.get(&guessed_location.to_string()).map_or_else(
-            || streets_from_location_list(value, location, config),
-            |x| (iter_from_toml_value(x).collect(), guessed_location),
-        ),
-    }
-}
-
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_remove_building_number() {
         let actual = remove_building_number("industriestrasse 2a");
```

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/candidate.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/candidate.rs`

 * *Files identical despite different names*

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/config.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/config.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::addr::{PLACES_PATH, PLACE_UBOUND, STREETS_DATA_PATH};
+use crate::addr::{PLACE_UBOUND, STREETS_DATA_PATH};
 use crate::metrics::{StringMetric, StringMetricFn};
 use clap::Parser;
 use std::path::PathBuf;
 use std::thread;
 
 pub const DEFAULT_UBOUND: f64 = 0.6;
 
@@ -37,27 +37,25 @@
 pub struct Config {
     pub ubound: UBound,
     pub place_ubound: UBound,
     pub max_candidates: usize,
     pub metric_fn: StringMetricFn,
     pub max_threads: usize,
     pub path_to_streets: PathBuf,
-    pub path_to_places: PathBuf,
 }
 
 impl Default for Config {
     fn default() -> Self {
         Self {
             ubound: UBound::default(),
             place_ubound: UBound::new(PLACE_UBOUND),
             max_candidates: 1,
             metric_fn: StringMetric::default().into(),
             max_threads: thread::available_parallelism().unwrap().get(),
             path_to_streets: PathBuf::from(STREETS_DATA_PATH),
-            path_to_places: PathBuf::from(PLACES_PATH),
         }
     }
 }
 
 impl Config {
     /// `ubound` - an upper threshold of the `similarity` between
     ///            candidate and target that still should be kept
@@ -66,52 +64,45 @@
     ///
     /// `metric` - a string metric to use for text matching
     ///
     /// `max_threads` - a number of threads to use during the file matching
     ///
     /// `path_to_streets` - a path to "streets_data/" folder
     ///
-    /// `path_to_places` - a path to "places.txt" file
-    ///
     /// # Panics
     /// Panics if the sensitivity value is lower than 0.0 or larger than 1.0
     pub fn new(
         ubound: f64,
         place_ubound: f64,
         max_candidates: usize,
         metric: StringMetric,
         max_threads: Option<usize>,
         path_to_streets: Option<String>,
-        path_to_places: Option<String>,
     ) -> Self {
         Self {
             ubound: UBound::new(ubound),
             place_ubound: UBound::new(place_ubound),
             max_candidates,
             metric_fn: metric.into(),
             max_threads: max_threads
                 .unwrap_or_else(|| thread::available_parallelism().unwrap().get()),
             path_to_streets: PathBuf::from(
                 path_to_streets.unwrap_or_else(|| String::from(STREETS_DATA_PATH)),
             ),
-            path_to_places: PathBuf::from(
-                path_to_places.unwrap_or_else(|| String::from(PLACES_PATH)),
-            ),
         }
     }
 
     pub fn from_args(args: &Args) -> Self {
         Self::new(
             args.sens,
             args.place_sens,
             args.results,
             args.metric,
             args.threads,
             args.streets.clone(),
-            args.places.clone(),
         )
     }
 }
 
 #[derive(Parser, Debug)]
 #[command(author, version, about, long_about = None)]
 pub struct Args {
@@ -124,18 +115,14 @@
     #[arg(short, long, default_value_t=StringMetric::default())]
     pub(crate) metric: StringMetric,
 
     /// Path to streets_data folder (see misc/data as an example)
     #[arg(long)]
     pub(crate) streets: Option<String>,
 
-    /// Path to places.txt file
-    #[arg(long)]
-    pub(crate) places: Option<String>,
-
     /// The place where to search street
     #[arg(short, long)]
     pub(crate) place: Option<String>,
 
     /// The postal code where to search street
     #[arg(short, long)]
     pub(crate) zip: Option<usize>,
```

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/guessr.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/guessr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -127,26 +127,25 @@
         Ok(sort_and_keep_max_cands(matches, config.max_candidates))
     } else {
         Err(GError::NotFound(sequence.to_string()))
     }
 }
 
 /// Search for a candidate street(s) to a target street within a Postal Code (`zip`).
-/// All official street candidates here grouped into files named by a Postal Code.
+/// All official street candidates here grouped into files named by a street name.
 /// `zip` must be a valid Switzerland Postal Code represented officially by government.
-/// Otherwise, if `zip` did not match any of existings Postal Codes in the directory,
-/// the search on the WHOLE directory (all files inside a directory) is provided.
-/// Also, if a candidate was not found within a given `zip`, the same logic (search on all files) is applied.
+/// Otherwise, if `zip` did not match any of existings Postal Codes in the street name file,
+/// the search on all streets in the file is provided.
+/// Also, if a candidate was not found within a given `zip`, the same logic (search on all streets) is applied.
 ///
 /// Search for a candidate street(s) to a target street within a Swiss peace of territory, assigned to the Postal Code (called `place`).
-/// All official street candidates here grouped into files named by `place`.
-/// `place` could be an invalid name. In this case, the matcher will try to search for `place` candidate inside a `places.txt` file.
-/// If `place` did not match any of existings Postal Codes in the directory,
-/// the search on the WHOLE directory (all files inside a directory) is provided.
-/// Also, if a candidate was not found within a given `zip`, the same logic (search on all files) is applied.
+/// All official street candidates here grouped into files named by street names.
+/// `place` could be an invalid name. In this case, the matcher will try to search for `place` candidate inside a guessed street name file.
+/// If `place` did not match any of existings Postal Codes in the file,
+/// the search on all streets in the file is provided.
 ///
 /// # Examples
 ///
 /// ```rust
 /// # use guess_rs::{Location, self as guessr, Config};
 /// #
 /// # fn main() {
@@ -370,15 +369,14 @@
         let cfg = Config::new(
             0.5,
             addr::PLACE_UBOUND,
             1,
             StringMetric::default(),
             None,
             None,
-            None,
         );
         let matches =
             search_in_candidates_file("qu du seujet 36", &PathBuf::from(DATA_FILE), &cfg).unwrap();
         assert_eq!(Candidate::from("quai du seujet"), matches[0]);
     }
 
     #[test]
@@ -496,15 +494,14 @@
         let cfg = Config::new(
             0.5,
             addr::PLACE_UBOUND,
             1,
             StringMetric::JaroWinkler,
             None,
             None,
-            None,
         );
         let matches = search_in_candidates_list(
             "foo",
             &["foobar", "foa", "2foo", "abcd"]
                 .into_iter()
                 .map(|x| x.to_string())
                 .collect::<Vec<String>>(),
```

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/lib.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/main.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyguess-0.2.0/local_dependencies/guess-rs/src/metrics.rs` & `pyguess-0.2.1/local_dependencies/guess-rs/src/metrics.rs`

 * *Files identical despite different names*

### Comparing `pyguess-0.2.0/Cargo.toml` & `pyguess-0.2.1/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyguess"
-version = "0.2.0"
+version = "0.2.1"
 authors = ["Vladyslav Rezohlazov <vladyslav.rezohlazov@novalytica.com>"]
 edition = "2021"
 license = "MIT"
 description = "The Python bindings to guess-rs"
 keywords = ["guess_rs"]
 readme = "README.md"
 homepage = "https://github.com/Novalytica/guess-rs/pyguess"
```

### Comparing `pyguess-0.2.0/README.md` & `pyguess-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 
 <a id="orgc7de4f4"></a>
 
 # Usage
 
     import pyguess
     from pyguess import Config, Candidate
-    
+
     config = Config(
         path_to_streets="../misc/data/streets_data",
-        path_to_places="../misc/data/places.txt",
     )
     candidate = pyguess.guess_address("Rigistrasse 10", "Pfaffikon", config)
-    
-    assert candidate == Candidate("rigistrasse 10", "pfäffikon zh")
 
+    assert candidate == Candidate("rigistrasse 10", "pfäffikon zh")
```

### Comparing `pyguess-0.2.0/examples/file.py` & `pyguess-0.2.1/examples/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import tqdm
 
 import pyguess
 from pyguess import Config
 
 config = Config(
     path_to_streets="../../misc/data/streets_data",
-    path_to_places="../../misc/data/places.txt",
 )
 DELIMITER = "\t"
 HEADER = ["orig_street", "orig_location", "guessed_street", "guessed_location"]
 
 with open("../../misc/data_examples/examples.csv") as file_in:
     reader = csv.reader(file_in, delimiter=DELIMITER)
     next(reader)
```

### Comparing `pyguess-0.2.0/pyguess.pyi` & `pyguess-0.2.1/pyguess.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -3,44 +3,39 @@
         self,
         ubound: float | None = None,
         place_ubound: float | None = None,
         max_candidates: int | None = None,
         metric: str | None = None,
         max_threads: int | None = None,
         path_to_streets: str | None = None,
-        path_to_places: str | None = None,
     ): ...
     @property
     def ubound(self) -> float | None: ...
     @property
     def place_ubound(self) -> float | None: ...
     @property
     def max_candidates(self) -> int | None: ...
     @property
     def metric(self) -> str | None: ...
     @property
     def max_threads(self) -> int | None: ...
     @property
     def path_to_streets(self) -> str | None: ...
-    @property
-    def path_to_places(self) -> str | None: ...
     @ubound.setter
     def ubound(self, value: float | None) -> None: ...
     @place_ubound.setter
     def place_ubound(self, value: float | None) -> None: ...
     @max_candidates.setter
     def max_candidates(self, value: int | None) -> None: ...
     @metric.setter
     def metric(self, value: str | None) -> None: ...
     @max_threads.setter
     def max_threads(self, value: int | None) -> None: ...
     @path_to_streets.setter
     def path_to_streets(self, value: str | None) -> None: ...
-    @path_to_places.setter
-    def path_to_places(self, value: str | None) -> None: ...
 
 class Candidate:
     def __init__(self, street: str, location: str | int | None): ...
     @property
     def street(self) -> str | int: ...
     @property
     def location(self) -> str | int | None: ...
```

### Comparing `pyguess-0.2.0/pyproject.toml` & `pyguess-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pyguess"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [tool.isort]
```

### Comparing `pyguess-0.2.0/src/lib.rs` & `pyguess-0.2.1/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -52,38 +52,35 @@
 struct PyConfig {
     ubound: Option<f64>,
     place_ubound: Option<f64>,
     max_candidates: Option<usize>,
     metric: Option<String>,
     max_threads: Option<usize>,
     path_to_streets: Option<String>,
-    path_to_places: Option<String>,
 }
 
 #[pymethods]
 impl PyConfig {
     /// Create a new PyConfig instance
     #[new]
     fn new(
         ubound: Option<f64>,
         place_ubound: Option<f64>,
         max_candidates: Option<usize>,
         metric: Option<String>,
         max_threads: Option<usize>,
         path_to_streets: Option<String>,
-        path_to_places: Option<String>,
     ) -> Self {
         Self {
             ubound,
             place_ubound,
             max_candidates,
             metric,
             max_threads,
             path_to_streets,
-            path_to_places,
         }
     }
 }
 
 impl From<PyConfig> for Config {
     fn from(pyconfig: PyConfig) -> Self {
         let default_config = Self::default();
@@ -98,17 +95,14 @@
             metric_fn: pyconfig.metric.map_or(default_config.metric_fn, |x| {
                 Into::<StringMetric>::into(x).into()
             }),
             max_threads: pyconfig.max_threads.unwrap_or(default_config.max_threads),
             path_to_streets: pyconfig
                 .path_to_streets
                 .map_or(default_config.path_to_streets, PathBuf::from),
-            path_to_places: pyconfig
-                .path_to_places
-                .map_or(default_config.path_to_places, PathBuf::from),
         }
     }
 }
 
 /// A guess candidate
 #[derive(Clone)]
 #[pyclass(get_all, set_all, name = "Candidate")]
```

### Comparing `pyguess-0.2.0/tests/test_pyguess.py` & `pyguess-0.2.1/tests/test_pyguess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import unittest
 
 import pyguess
 from pyguess import Candidate, Config
 
 CONFIG = Config(
     path_to_streets="../misc/data/streets_data",
-    path_to_places="../misc/data/places.txt",
 )
 EXAMPLES = [
     (
         "rigistr. 10",
         "Pfaffikon",
         Candidate("rigistrasse 10", "pfäffikon zh"),
     ),
```

### Comparing `pyguess-0.2.0/Cargo.lock` & `pyguess-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "guess-rs"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "clap",
  "criterion",
  "pretty_assertions",
  "regex",
  "strsim",
  "threadpool",
@@ -574,15 +574,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyguess"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "guess-rs",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
```

### Comparing `pyguess-0.2.0/PKG-INFO` & `pyguess-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyguess
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: The Python bindings to guess-rs
 Keywords: guess_rs
 Home-Page: https://github.com/Novalytica/guess-rs/pyguess
 Author: Vladyslav Rezohlazov <vladyslav.rezohlazov@novalytica.com>
 Author-email: Vladyslav Rezohlazov <vladyslav.rezohlazov@novalytica.com>
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/Novalytica/guess-rs.git
 
 <div align="center">
 
 # pyguess
 The Python library to Guess Swiss Streets
@@ -49,17 +49,15 @@
 
 <a id="orgc7de4f4"></a>
 
 # Usage
 
     import pyguess
     from pyguess import Config, Candidate
-    
+
     config = Config(
         path_to_streets="../misc/data/streets_data",
-        path_to_places="../misc/data/places.txt",
     )
     candidate = pyguess.guess_address("Rigistrasse 10", "Pfaffikon", config)
-    
-    assert candidate == Candidate("rigistrasse 10", "pfäffikon zh")
 
+    assert candidate == Candidate("rigistrasse 10", "pfäffikon zh")
```

