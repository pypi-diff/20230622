# Comparing `tmp/pyguess-0.1.0.tar.gz` & `tmp/pyguess-0.2.0.tar.gz`

## Comparing `pyguess-0.1.0.tar` & `pyguess-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pyguess-0.1.0/local_dependencies/guess-rs/Cargo.toml
--rw-r--r--   0     1000     1000     2810 2023-04-13 06:58:34.000000 pyguess-0.1.0/local_dependencies/guess-rs/benches/guess_bench.rs
--rw-r--r--   0     1000     1000     2810 2023-04-13 06:58:19.000000 pyguess-0.1.0/local_dependencies/guess-rs/benches/text_sim_bench.rs
--rw-r--r--   0     1000     1000     3142 2023-04-13 05:16:50.000000 pyguess-0.1.0/local_dependencies/guess-rs/src/candidate.rs
--rw-r--r--   0     1000     1000    15223 2023-04-13 07:42:03.000000 pyguess-0.1.0/local_dependencies/guess-rs/src/guess.rs
--rw-r--r--   0     1000     1000      457 2023-04-13 06:57:32.000000 pyguess-0.1.0/local_dependencies/guess-rs/src/lib.rs
--rw-r--r--   0     1000     1000     4331 2023-04-13 06:57:19.000000 pyguess-0.1.0/local_dependencies/guess-rs/src/main.rs
--rw-r--r--   0     1000     1000     6457 2023-04-13 07:41:21.000000 pyguess-0.1.0/local_dependencies/guess-rs/src/text_sim.rs
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pyguess-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000      183 2023-04-13 05:16:50.000000 pyguess-0.1.0/Pipfile
--rw-r--r--   0     1000     1000     3770 2023-04-13 08:10:28.000000 pyguess-0.1.0/Pipfile.lock
--rw-r--r--   0     1000     1000      249 2023-04-13 08:02:18.000000 pyguess-0.1.0/pyguess.pyi
--rw-r--r--   0     1000     1000      315 2023-04-13 07:51:22.000000 pyguess-0.1.0/pyproject.toml
--rw-r--r--   0     1000     1000     2367 2023-04-13 06:15:10.000000 pyguess-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000      138 2023-04-13 08:14:05.000000 pyguess-0.1.0/test_pyguess.py
--rw-r--r--   0     1000     1000    24622 2023-04-13 08:08:59.000000 pyguess-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 pyguess-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 pyguess-0.2.0/local_dependencies/guess-rs/Cargo.toml
+-rw-r--r--   0     1000     1000     3471 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/benches/guess_bench.rs
+-rw-r--r--   0     1000     1000    15793 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/addr.rs
+-rw-r--r--   0     1000     1000      671 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/candidate.rs
+-rw-r--r--   0     1000     1000     5077 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/config.rs
+-rw-r--r--   0     1000     1000    17940 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/guessr.rs
+-rw-r--r--   0     1000     1000     1553 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/lib.rs
+-rw-r--r--   0     1000     1000      550 2023-06-22 05:51:09.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/main.rs
+-rw-r--r--   0     1000     1000     2257 2023-06-13 12:39:45.000000 pyguess-0.2.0/local_dependencies/guess-rs/src/metrics.rs
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 pyguess-0.2.0/Cargo.toml
+-rw-r--r--   0     1000     1000      162 2023-06-22 05:51:09.000000 pyguess-0.2.0/Pipfile
+-rw-r--r--   0     1000     1000      840 2023-06-22 05:51:09.000000 pyguess-0.2.0/README.md
+-rw-r--r--   0     1000     1000      628 2023-06-22 05:51:09.000000 pyguess-0.2.0/examples/basic.py
+-rw-r--r--   0     1000     1000     1101 2023-06-22 05:51:09.000000 pyguess-0.2.0/examples/file.py
+-rw-r--r--   0     1000     1000     1816 2023-06-22 05:51:09.000000 pyguess-0.2.0/pyguess.pyi
+-rw-r--r--   0     1000     1000      944 2023-06-22 05:51:09.000000 pyguess-0.2.0/pyproject.toml
+-rw-r--r--   0     1000     1000     5487 2023-06-22 05:51:09.000000 pyguess-0.2.0/src/lib.rs
+-rw-r--r--   0     1000     1000        0 2023-06-22 05:51:09.000000 pyguess-0.2.0/tests/__init__.py
+-rw-r--r--   0     1000     1000      994 2023-06-22 05:51:09.000000 pyguess-0.2.0/tests/test_pyguess.py
+-rw-r--r--   0     1000     1000    27778 2023-06-20 14:50:10.000000 pyguess-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 pyguess-0.2.0/PKG-INFO
```

### Comparing `pyguess-0.1.0/local_dependencies/guess-rs/Cargo.toml` & `pyguess-0.2.0/local_dependencies/guess-rs/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "guess-rs"
-version = "0.1.0"
+version = "0.2.0"
 authors = ["Vladyslav Rezohlazov <vladyslav.rezohlazov@novalytica.com>"]
 edition = "2021"
 license = "MIT"
 description = "The library to Match Swiss Streets"
 keywords = ["guess-rs", "nlp", "street-processing", "text-processing"]
 categories = ["text-processing"]
-readme = "README.md"
+readme = "../README.md"
 homepage = "https://github.com/Novalytica/guess-rs/guess"
-repository = "https://github.com/Novalytica/guess-rs"
+repository = "https://github.com/Novalytica/guess-rs.git"
 
 [lib]
 name = "guess_rs"
 path = "src/lib.rs"
 
 [[bin]]
 name = "guess"
@@ -23,9 +23,10 @@
 name = "guess_bench"
 harness = false
 
 [dependencies]
 strsim = "0.10.0"
 unicode-segmentation = "1.10.0"
 threadpool = "1.8.1"
-regex = "1.6.0"
+regex = "1.8.4"
 toml = "0.7.3"
+clap = { version = "4.3.3", features = ["derive"] }
```

### Comparing `pyguess-0.1.0/local_dependencies/guess-rs/src/guess.rs` & `pyguess-0.2.0/local_dependencies/guess-rs/src/addr.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,504 +1,478 @@
-//! This module provides matching on official Switzerland streets
-
 use crate::{
-    candidate::{Candidate, Error as CandidateError, Sens, SimResult, Text},
-    text_sim::{self, Config, StringMetric},
+    config::{Args, Config, UBound},
+    guessr, StringMetric,
 };
-
 use regex::Regex;
-use std::{fs, io, path::PathBuf, process};
+use std::{fs, io};
 use toml::Value;
 
-const PLACE_SENS: f64 = 0.6;
-const NUM_TO_KEEP_FILTERED_STREETS: usize = 500;
-const ALGO_TO_FILTER_STREETS: StringMetric = StringMetric::Jaro;
-const PATH_TO_PLACES: &str = "../misc/data/places.txt";
-const PATH_TO_STREET_NAMES: &str = "../misc/data/streets_data/street_names.txt";
-const PATH_TO_STREETS_DATA: &str = "../misc/data/streets_data";
-
-#[derive(Debug, PartialEq, Eq, Clone)]
-pub struct Place(pub(crate) String);
-
-impl Place {
-    pub fn new(value: &str) -> Self {
-        let cfg = Config::new(Sens::new(PLACE_SENS), 1, StringMetric::JaroWinkler, None);
-        Self(
-            text_sim::fast_cmp_with_file(
-                &Text::new(value.to_string()),
-                &PathBuf::from(PATH_TO_PLACES),
-                &cfg,
-            )
-            .map_or(String::new(), |candidates| candidates[0].text.clone()),
-        )
+pub(crate) const PLACE_UBOUND: f64 = 0.8;
+const STRING_METRIC_PLACE: StringMetric = StringMetric::JaroWinkler;
+const FILE_EXTENSION: &str = "toml";
+const FORWARD_SLASH_REPL: &str = "%2C";
+pub(crate) const STREETS_DATA_PATH: &str = "../misc/data/streets_data";
+pub(crate) const PLACES_PATH: &str = "../misc/data/places.txt";
+
+#[derive(Debug, Clone, PartialEq, Eq)]
+pub enum Location {
+    Place(String),
+    Zip(usize),
+    Empty,
+}
+
+impl Location {
+    pub fn guess(&self, config: &Config, candidates: Option<Vec<String>>) -> Self {
+        match self {
+            Self::Place(place) => {
+                let config = Config {
+                    ubound: UBound::new(PLACE_UBOUND),
+                    max_candidates: 1,
+                    metric_fn: STRING_METRIC_PLACE.into(),
+                    ..config.clone()
+                };
+                let guessed_location = if let Some(candidates) = candidates {
+                    guessr::search_in_candidates_list(place, &candidates, &config)
+                } else {
+                    guessr::search_in_candidates_file(place, &config.path_to_places, &config)
+                };
+                guessed_location.ok().map_or(Self::Empty, |location| {
+                    Self::Place(location[0].sequence.to_string())
+                })
+            }
+            _ => self.clone(),
+        }
     }
-}
 
-impl ToString for Place {
-    fn to_string(&self) -> String {
-        self.0.to_owned()
+    pub fn from_args(args: &Args) -> Self {
+        if let Some(place) = args.place.clone() {
+            Location::Place(place)
+        } else if let Some(zip) = args.zip {
+            Location::Zip(zip)
+        } else {
+            Location::Empty
+        }
     }
 }
 
-#[derive(Debug, PartialEq, Eq, Clone)]
-pub struct Plz(pub(crate) String);
-
-impl ToString for Plz {
+impl ToString for Location {
     fn to_string(&self) -> String {
-        self.0.to_owned()
-    }
-}
-
-impl Plz {
-    pub fn new(value: usize) -> Self {
-        Self(value.to_string())
+        match self {
+            Self::Place(place) => place.to_string(),
+            Self::Zip(zip) => zip.to_string(),
+            Self::Empty => panic!("Trying to convert Location::Empty to String"),
+        }
     }
 }
 
 #[inline]
-fn filter_distant_streets(street: &Text, cfg: &Config) -> Vec<String> {
-    text_sim::fast_cmp_with_file(street, &PathBuf::from(PATH_TO_STREET_NAMES), cfg)
-        .unwrap_or_default()
-        .into_iter()
-        .map(|c| c.text)
-        .collect()
+pub(crate) fn contains_numbers(street: &str) -> bool {
+    street.chars().filter(|ch| ch.is_numeric()).count() > 0
 }
 
-#[inline]
-fn find_street_name(street: &Text, cfg: &Config) -> SimResult {
-    let filter_cfg = Config {
-        num_to_keep: NUM_TO_KEEP_FILTERED_STREETS,
-        metric_func: ALGO_TO_FILTER_STREETS.into(),
-        ..*cfg
-    };
-    text_sim::cmp_with_arr(&filter_distant_streets(street, &filter_cfg), street, cfg)
-}
-
-// #[derive(Debug)]
-// pub enum Error {
-//     Io(io::Error),
-//     CError(CandidateError),
-//     DoesNotContainNumbers,
-// }
-
-// impl fmt::Display for Error {
-//     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-//         match self {
-//             Self::CError(err) => f.write_str(&err.to_string()),
-//             Self::Io(err) => f.write_str(&err.to_string()),
-//             Self::DoesNotContainNumbers => f.write_str("DoesNotContainNumbers"),
-//         }
-//     }
-// }
-
-#[derive(Debug)]
-pub struct Street {
-    pub value: Text,
-    pub file: StreetFile,
-}
-
-impl PartialEq for Street {
-    fn eq(&self, other: &Self) -> bool {
-        self.value.eq(&other.value)
-    }
-}
-
-impl Street {
-    pub fn new(street: &str, cfg: Option<Config>) -> Result<Self, CandidateError> {
-        // TODO: add here Error spreading instead of exiting
-        if !Self::contains_numbers(street) {
-            eprintln!(
-                "Argument 'street' must contain street number! Got: '{}'",
-                street
-            );
-            process::exit(1);
-        }
-        let street = Text::new(Self::clean(street));
-        Ok(Self {
-            file: StreetFile::new(&find_street_name(&street, &cfg.unwrap_or_default())?[0].text)?,
-            value: street,
-        })
-    }
-
-    #[inline]
-    pub(crate) fn contains_numbers(street: &str) -> bool {
-        street.chars().filter(|ch| ch.is_numeric()).count() > 0
-    }
-
-    #[inline]
-    pub(crate) fn clean(street: &str) -> String {
-        let mut street = street
-            .trim()
-            .to_lowercase()
-            .replace("str.", "strasse")
-            .replace("av. ", "avenue ")
-            .replace("rt ", "route ")
-            .replace("st.", "saint")
-            .replace("st-", "saint");
-        // Matches: '76 chemin des clos' or 'a4 résidence du golf'
-        if Self::starts_with_number(&street) {
-            let (num, street_name) = street.split_once(' ').expect("matched by regexp");
-            street = format!("{} {}", street_name, num);
-        }
-        // Matches: eisfeldstrasse 21/23, milchstrasse 2-10a, milchstrasse 2,10a, bernstrasse 7 8
-        match Regex::new(r"(.*?\s\d*?\s?[a-zA-Z]?)[\./,\-\+\s–\\]")
-            .unwrap()
-            .find(&street)
-        {
-            // but not bernstrasse 7 A
-            Some(mat) if !Regex::new(r"\s\d*?\s[a-zA-Z]$").unwrap().is_match(&street) => {
-                mat.as_str().to_string()
+fn find_street_name<'a>(
+    street: &'a str,
+    number1: Option<&'a str>,
+    number2: Option<String>,
+) -> Option<&'a str> {
+    let mut idxs = Vec::new();
+
+    if let Some(number) = number1 {
+        idxs.push(street.find(number).unwrap());
+    }
+    if let Some(number) = number2 {
+        idxs.push(street.find(&number).unwrap());
+    }
+    idxs.iter().min().map(|min_idx| street[..*min_idx].trim())
+}
+
+fn parse_many_streets(street: &str) -> Vec<String> {
+    if !contains_numbers(street) {
+        return Vec::new();
+    }
+    let re = Regex::new(r"(\d+([a-zA-Z]-[a-zA-Z]|[a-zA-Z])?)[,/]").unwrap();
+    let mut numbers = re
+        .captures_iter(street)
+        .map(|captures| captures.get(1).unwrap().as_str())
+        .collect::<Vec<&str>>();
+
+    // Capture last number in the list
+    if !numbers.is_empty() {
+        let idx = street.find(numbers.last().unwrap()).unwrap() + numbers.last().unwrap().len();
+        let re = Regex::new(r"^\d+([a-zA-Z]-[a-zA-Z]|[a-zA-Z])?\b").unwrap();
+        let chars_to_trim: &[char] = &[',', '/', ' '];
+        if let Some(mat) = re.find(street[idx..].trim_matches(chars_to_trim)) {
+            let matches = mat.as_str().split('-').collect::<Vec<&str>>();
+            if matches.len() == 1 || (matches.len() == 2 && matches[1].parse::<u32>().is_err()) {
+                numbers.push(mat.as_str());
             }
-            _ => street,
         }
     }
 
-    #[inline]
-    pub(crate) fn starts_with_number(street: &str) -> bool {
-        Regex::new(r"^\d+,?\s.+").unwrap().is_match(street)
-            || Regex::new(r"^\w\d+,?\s").unwrap().is_match(street)
-    }
-}
-
-#[derive(Debug)]
-pub struct StreetFile {
-    values: Value,
-}
-
-impl StreetFile {
-    pub fn new(street_name: &str) -> io::Result<Self> {
-        let filename = format!(
-            "{}/{}.toml",
-            PATH_TO_STREETS_DATA,
-            street_name.replace('/', "%2C")
-        );
-        Ok(Self {
-            values: toml::from_str::<Value>(&fs::read_to_string(filename)?).unwrap_or_else(|_| {
-                unimplemented!(
-                    "Should implement From<toml::Error> for io::Error [since toml 0.7.3]"
-                )
-            }),
+    let re = Regex::new(r"(\d+)-(\d+)").unwrap();
+    let numbers_ranges = re
+        .captures_iter(street)
+        .flat_map(|captures| {
+            let start_num_range = captures.get(1).unwrap().as_str().parse::<usize>().unwrap();
+            let end_num_range = captures.get(2).unwrap().as_str().parse::<usize>().unwrap();
+            start_num_range..=end_num_range
         })
-    }
+        .map(|x| x.to_string())
+        .collect::<Vec<String>>();
 
-    #[inline]
-    fn iter_over_strings_from(value: &Value) -> impl Iterator<Item = String> + '_ {
-        value
-            .as_array()
-            .unwrap()
+    numbers.extend(
+        &numbers_ranges
             .iter()
-            .map(|v| v.to_string().replace('\"', ""))
-    }
+            .map(|x| x.as_str())
+            .collect::<Vec<&str>>(),
+    );
+
+    let street_name = if let Some(street_name) = find_street_name(
+        street,
+        numbers.first().copied(),
+        numbers_ranges.first().cloned(),
+    ) {
+        street_name
+    } else {
+        return vec![street.trim().to_string()];
+    };
 
-    #[inline]
-    fn get_all_streets(&self) -> Vec<String> {
-        let mut values = self
-            .values
-            .as_table()
-            .expect("correct table structure")
-            .iter()
-            .flat_map(|(_, v)| Self::iter_over_strings_from(v))
-            .collect::<Vec<String>>();
-        values.sort();
-        values.dedup();
-        values
-    }
+    numbers.sort();
+    numbers.dedup();
 
-    fn get_streets_by<T>(&self, location: Option<&T>) -> (Vec<String>, bool)
-    where
-        T: ToString,
-    {
-        if let Some(location) = location {
-            if let Some(v) = self.values.get(&location.to_string()) {
-                return (Self::iter_over_strings_from(v).collect(), true);
+    let re_numbers_range = Regex::new(r"([a-zA-Z])-([a-zA-Z])").unwrap();
+    let re_number = Regex::new(r"^(\d+)[a-zA-Z]").unwrap();
+    numbers
+        .iter()
+        .flat_map(|x| match re_numbers_range.captures(x) {
+            Some(captures) => {
+                let number = re_number.captures(x).unwrap().get(1).unwrap().as_str();
+                let start_char = captures.get(1).unwrap().as_str().chars().next().unwrap();
+                let end_char = captures.get(2).unwrap().as_str().chars().next().unwrap();
+                (start_char..=end_char)
+                    .map(|ch| format!("{} {}{}", street_name, number, ch))
+                    .collect::<Vec<String>>()
             }
-        }
-        (self.get_all_streets(), false)
-    }
-}
-
-pub struct StreetConfig<T> {
-    pub location: Option<T>,
-    pub cfg: Config,
+            None => vec![format!("{} {}", street_name, x)],
+        })
+        .collect()
 }
 
-impl<T> Default for StreetConfig<T> {
-    fn default() -> Self {
-        Self {
-            location: None,
-            cfg: Config::default(),
+fn split_streets(street: &str) -> Vec<String> {
+    let re = Regex::new(r"(.*?)/([^0-9]|(3-|1[.]|4[b ]))").unwrap();
+    let mut streets: Vec<String> = Vec::new();
+    let mut prefix: Option<&str> = None;
+    for captures in re.captures_iter(street) {
+        streets.push(prefix.unwrap_or_default().to_string() + captures.get(1).unwrap().as_str());
+        if let Some(mat) = captures.get(2) {
+            prefix = Some(mat.as_str());
         }
     }
-}
-
-impl<T> StreetConfig<T> {
-    pub fn new(location: Option<T>, sens: f64, num_to_keep: usize, algo: StringMetric) -> Self {
-        Self {
-            location,
-            cfg: Config::new(Sens::new(sens), num_to_keep, algo, None),
+    if let Some(last_street) = streets.last() {
+        let idx = street.find(last_street).unwrap() + last_street.len();
+        if idx < street.len() {
+            let chars_to_trim: &[char] = &['/', ' '];
+            streets.push(street[idx..].trim_matches(chars_to_trim).to_string());
         }
     }
-
-    pub fn default_with(location: T) -> Self {
-        Self {
-            location: Some(location),
-            cfg: Config::default(),
-        }
+    if streets.is_empty() {
+        return vec![street.to_string()];
     }
+    streets
 }
 
-/// Search for a candidate street(s) to a target street within a Postal Code (`plz`).
-/// All official street candidates here grouped into files named by a Postal Code.
-/// `plz` must be a valid Switzerland Postal Code represented officially by government.
-/// Otherwise, if `plz` did not match any of existings Postal Codes in the directory,
-/// the search on the WHOLE directory (all files inside a directory) is provided.
-/// Also, if a candidate was not found within a given `plz`, the same logic (search on all files) is applied.
-///
-/// Search for a candidate street(s) to a target street within a Swiss peace of territory, assigned to the Postal Code (called `place`).
-/// All official street candidates here grouped into files named by `place`.
-/// `place` could be an invalid name. In this case, the matcher will try to search for `place` candidate inside a `places.txt` file.
-/// If `place` did not match any of existings Postal Codes in the directory,
-/// the search on the WHOLE directory (all files inside a directory) is provided.
-/// Also, if a candidate was not found within a given `plz`, the same logic (search on all files) is applied.
-///
-/// # Examples
-///
-/// ```rust
-/// # use guess_rs::{Plz, Street, guess};
-/// #
-/// # fn main() {
-/// #     let street = Street::new("qu du seujet 36", None).unwrap();
-/// #     let mat = guess::find_matches(&street, Some(Plz::new(1201)), None);
-/// #     assert_eq!(mat.0.unwrap().text, "quai du seujet 36".to_string());
-/// # }
-/// ```
-///
-/// ```rust
-/// # use guess_rs::{Place, Street, guess};
-/// #
-/// # fn main() {
-/// #     let street = Street::new("aarstrasse 76", None).unwrap();
-/// #     let mat = guess::find_matches(&street, Some(Place::new("Bern")), None);
-/// #     assert_eq!(mat.0.unwrap().text, "aarstrasse 76".to_string());
-/// # }
-/// ```
-///
-/// # Panics
-///
-/// Panics if `street` does not contain a number (as each valid street MUST contain an any number)
-pub fn find_matches<T>(
-    street: &Street,
-    street_cfg: StreetConfig<T>,
-) -> io::Result<(Option<Candidate>, Option<T>)>
-where
-    T: ToString,
-{
-    let (street_candidates, is_found_in_loc) =
-        street.file.get_streets_by(street_cfg.location.as_ref());
-    Ok((
-        text_sim::cmp_with_arr(&street_candidates, &street.value, &street_cfg.cfg)
-            .ok()
-            .map(|mat| mat[0].clone()),
-        if is_found_in_loc {
-            street_cfg.location
-        } else {
-            None
-        },
-    ))
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-
-    const STREET_WITHOUT_NUMBERS: &str = "Bernstrasse";
-    const STREET_WITH_NUMBER: &str = "Bernstrasse 7";
-
-    #[test]
-    #[ignore]
-    fn max_sensitivity() {
-        // Some random string in the input
-        let street = "FdsfdsfsdfssFSDfdsfsdfsBernstrasse 7";
-        let street = Street::new(street, None);
-        assert!(
-            matches!(street, Err(_)),
-            "Expected NotFound error, but the value was {:?}",
-            street
-        );
-    }
-
-    #[test]
-    fn street_contains_numbers() {
-        assert!(Street::contains_numbers(STREET_WITH_NUMBER))
-    }
-
-    #[test]
-    fn street_does_not_contain_numbers() {
-        assert!(!Street::contains_numbers(STREET_WITHOUT_NUMBERS))
-    }
-
-    #[test]
-    #[should_panic(expected = "must contain street number")]
-    fn no_numbers_in_street_plz() {
-        find_matches::<Plz>(
-            &Street::new(STREET_WITHOUT_NUMBERS, None).unwrap(),
-            StreetConfig::default(),
-        )
-        .unwrap();
-    }
-
-    fn assert_clean_street(expected_street: &str, street_to_clean: &str) {
-        assert_eq!(
-            expected_street.to_string(),
-            Street::new(street_to_clean, None).unwrap().value.cleaned
-        );
+pub(crate) fn detect_streets(street: &str) -> Vec<String> {
+    if street.contains('/') {
+        split_streets(street)
+    } else {
+        vec![street.to_string()]
     }
+    .iter()
+    .flat_map(|street| parse_many_streets(street))
+    .collect()
+}
 
-    #[test]
-    fn clean_street() {
-        assert_clean_street("bernstrasse7", "   Bernstrasse 7   ");
-        assert_clean_street("bernstrassea4", "   a4 Bernstrasse   ");
-        assert_clean_street("bernstrasse4", "   4 Bernstrasse   ");
-        assert_clean_street("bernstrasse4a", "   Bernstrasse 4a, 5, 6   ");
-        assert_clean_street("bernstrasse4a", "   Bernstrasse 4a 5 6   ");
-        assert_clean_street("bernstrasse4a", "   Bernstrasse 4a-5-6   ");
-        assert_clean_street("bernstrasse4a", "   Bernstrasse 4a/5/6   ");
-        assert_clean_street("bernstrasse4a", "   Bernstrasse 4a. 5 6   ");
-        assert_clean_street("bernstrasse4a", "  Bernstrasse 4 A fasdfs");
-    }
+#[inline]
+pub(crate) fn starts_with_number(street: &str) -> bool {
+    Regex::new(r"^\d+,?\s.+").unwrap().is_match(street)
+        || Regex::new(r"^\w\d+,?\s").unwrap().is_match(street)
+}
+
+pub fn replace_prefixes(mut street: String) -> String {
+    street = street.replace("str.", "strasse");
+    let replacements = [
+        (r"\bst-", "saint-"),
+        (r"\brt ", "route "),
+        (r"\bst\.", "saint"),
+        (r"\bav\.", "avenue"),
+    ];
+    for (pattern, replacement) in replacements.iter() {
+        let re = Regex::new(pattern).unwrap();
+        street = re.replace_all(&street, *replacement).to_string();
+    }
+    street
+}
+
+pub(crate) fn remove_building_number(street: &str) -> String {
+    let re = Regex::new(r"\b\d+[a-zA-Z]?$").unwrap();
+    re.replace_all(street, "").to_string().trim().to_string()
+}
+
+pub fn clean_street(street: &str) -> String {
+    let mut street = replace_prefixes(street.trim().to_lowercase());
+    // Matches: '76 chemin des clos', 'a4 résidence du golf', etc.
+    if starts_with_number(&street) {
+        let (num, street_name) = street.split_once(' ').expect("matched by regexp");
+        street = format!("{} {}", street_name, num);
+    }
+    // Regex to match streets in different format like:
+    // eisfeldstrasse 21/23, milchstrasse 2-10a, milchstrasse 2,10a, bernstrasse 7 8, etc.
+    let re = Regex::new(r"(.*?\s\d*?\s?[a-zA-Z]?)[\./,\-\+\s–\\]").unwrap();
+    let street = match re.find(&street) {
+        Some(mat) => {
+            // Regex to replace spaces between street number and its letter,
+            // e.g. bernstrasse 4 a
+            let re = Regex::new(r"\s(\d+)\s+([a-zA-Z])").unwrap();
+            let chars_to_trim: &[char] = &[',', '.', '-', '_', '/', ' ', ':', ';'];
+            let mat = re.replace_all(mat.as_str().trim_matches(chars_to_trim), " $1$2");
+            mat.to_string()
+        }
+        _ => street,
+    };
+    street
+}
 
-    #[test]
-    fn match_with_place() {
-        let location = Place::new("bercher");
-        assert_eq!(
-            find_matches(
-                &Street::new("ch de saint-cierges 3", None).unwrap(),
-                StreetConfig::default_with(location.to_owned()),
-            )
-            .unwrap(),
-            (
-                Some(Candidate::from("chemin de saint-cierges 3")),
-                Some(location)
-            )
-        );
-    }
+pub fn open_street_file(street: &str, config: &Config) -> io::Result<Value> {
+    // let mut path_to_street_file = config.path_to_streets.clone();
+    let path_to_street_file = config.path_to_streets.join(format!(
+        "{}.{}",
+        street.replace('/', FORWARD_SLASH_REPL),
+        FILE_EXTENSION
+    ));
+    Ok(
+        toml::from_str::<Value>(&fs::read_to_string(path_to_street_file)?).unwrap_or_else(|_| {
+            unimplemented!("Should use new error and implement From<toml::Error> and From<io::Error> [since toml 0.7.3]")
+        }),
+    )
+}
 
-    #[test]
-    #[ignore]
-    fn match_without_place() {
-        let mat = find_matches::<Place>(
-            &Street::new("ch de saint-cierges 3", None).unwrap(),
-            StreetConfig::default(),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("chemin de saint-cierges 3")), None)
-        );
-    }
+#[inline]
+fn iter_from_toml_value(value: &Value) -> impl Iterator<Item = String> + '_ {
+    value
+        .as_array()
+        .unwrap()
+        .iter()
+        .map(|x| x.to_string().replace('\"', ""))
+}
+
+fn get_all_streets(value: &Value) -> Vec<String> {
+    let mut values = value
+        .as_table()
+        .expect("correct table structure")
+        .iter()
+        .flat_map(|(_, v)| iter_from_toml_value(v))
+        .collect::<Vec<String>>();
+    values.sort();
+    values.dedup();
+    values
+}
+
+fn get_locations(value: &Value) -> Vec<String> {
+    value
+        .as_table()
+        .unwrap()
+        .iter()
+        .map(|(k, _)| k.to_string())
+        .collect()
+}
 
-    #[test]
-    fn match_with_plz() {
-        let location = Plz::new(1201);
-        let mat = find_matches(
-            &Street::new("qu du seujet 36", None).unwrap(),
-            StreetConfig::default_with(location.to_owned()),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("quai du seujet 36")), Some(location))
-        );
-    }
+#[inline]
+fn get_all_streets_empty_loc(value: &Value) -> (Vec<String>, Location) {
+    (get_all_streets(value), Location::Empty)
+}
 
-    #[test]
-    #[ignore]
-    fn match_without_plz() {
-        let mat = find_matches::<Plz>(
-            &Street::new("qu du seujet 36", None).unwrap(),
-            StreetConfig::default(),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("quai du seujet 36")), None)
-        );
+fn streets_from_location_list(
+    value: &Value,
+    location: &Location,
+    config: &Config,
+) -> (Vec<String>, Location) {
+    let locations = get_locations(value);
+    match location.guess(config, Some(locations)) {
+        Location::Empty => get_all_streets_empty_loc(value),
+        guessed_location => value.get(&guessed_location.to_string()).map_or_else(
+            || get_all_streets_empty_loc(value),
+            |x| (iter_from_toml_value(x).collect(), guessed_location),
+        ),
     }
+}
 
-    #[test]
-    #[ignore]
-    fn match_with_wrong_plz() {
-        let mat = find_matches(
-            &Street::new("qu du seujet 36", None).unwrap(),
-            StreetConfig::default_with(Plz::new(1231231)),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("quai du seujet 36")), None)
-        );
+pub(crate) fn streets_from_location(
+    value: &Value,
+    location: &Location,
+    config: &Config,
+) -> (Vec<String>, Location) {
+    match location.guess(config, None) {
+        Location::Empty => streets_from_location_list(value, location, config),
+        guessed_location => value.get(&guessed_location.to_string()).map_or_else(
+            || streets_from_location_list(value, location, config),
+            |x| (iter_from_toml_value(x).collect(), guessed_location),
+        ),
     }
+}
 
-    #[test]
-    #[ignore]
-    fn match_with_wrong_first_word() {
-        let location = Plz::new(1201);
-        let mat = find_matches(
-            &Street::new("uai du seujet 36", None).unwrap(),
-            StreetConfig::default_with(location.to_owned()),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("quai du seujet 36")), Some(location))
-        );
-    }
+#[cfg(test)]
+mod tests {
+    use super::*;
 
     #[test]
-    #[ignore]
-    fn match_with_wrong_first_word_no_plz() {
-        let mat = find_matches::<Plz>(
-            &Street::new("uai du seujet 36", None).unwrap(),
-            StreetConfig::default(),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("quai du seujet 36")), None)
-        );
+    fn test_remove_building_number() {
+        let actual = remove_building_number("industriestrasse 2a");
+        let expected = "industriestrasse".to_string();
+        assert_eq!(actual, expected);
     }
 
     #[test]
-    #[ignore]
-    fn match_with_wrong_first_word_wrong_plz() {
-        let location = Plz::new(2132131);
-        let mat = find_matches(
-            &Street::new("uai du seujet 36", None).unwrap(),
-            StreetConfig::default_with(location),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("quai du seujet 36")), None)
-        );
+    fn test_split_streets() {
+        let expected = vec!["Haupstrasse 5"];
+        let actual = split_streets("Haupstrasse 5");
+        assert_eq!(actual, expected);
     }
 
-    #[test]
-    fn match_wil_place() {
-        let location = Place::new("Wil SG");
-        let mat = find_matches(
-            &Street::new("Zürcherstrasse 3", None).unwrap(),
-            StreetConfig::default_with(location),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("zürcherstrasse 3")), None)
-        );
+    fn assert_detect_streets(expected: &[&str], street_to_detect: &str) {
+        let mut actual = detect_streets(street_to_detect);
+        let mut expected = expected
+            .iter()
+            .map(|x| x.to_string())
+            .collect::<Vec<String>>();
+        actual.sort();
+        expected.sort();
+        assert_eq!(actual, expected);
     }
 
     #[test]
-    fn match_pfaffikon_place() {
-        let location = Place::new("Pfäffikon");
-        let mat = find_matches(
-            &Street::new("Rigistrasse 10", None).unwrap(),
-            StreetConfig::default_with(location.clone()),
-        );
-        assert_eq!(
-            mat.unwrap(),
-            (Some(Candidate::from("rigistrasse 10")), None)
-        );
-        assert_eq!(location.to_string(), String::from("Pfäffikon ZG"));
+    fn test_detect_streets() {
+        let expected = &[
+            (
+                vec![
+                    "Weinsteig 206",
+                    "Weinsteig 208",
+                    "Weinsteig 210",
+                    "Weinsteig 212",
+                    "Weinsteig 214",
+                    "Weinsteig 216",
+                    "Haupstrasse 26",
+                    "Haupstrasse 26a",
+                    "Haupstrasse 26b",
+                    "Haupstrasse 26c",
+                ],
+                "Weinsteig 206/208/210/212/214/216/Haupstrasse 26/26a-c",
+            ),
+            (
+                vec!["1. Gangstrasse 10", "3-Eidgenossen 30"],
+                "1. Gangstrasse 10/3-Eidgenossen 30",
+            ),
+            (
+                vec![
+                    "Haupstrasse 30",
+                    "Haupstrasse 31",
+                    "Haupstrasse 32",
+                    "Haupstrasse 34",
+                    "Haupstrasse 35",
+                    "Haupstrasse 36",
+                ],
+                "Haupstrasse 30, 31, 32, 34-36",
+            ),
+            (
+                vec![
+                    "Haupstrasse 30",
+                    "Haupstrasse 31",
+                    "Haupstrasse 32",
+                    "Haupstrasse 33",
+                    "Haupstrasse 35",
+                    "Haupstrasse 36",
+                    "Haupstrasse 37",
+                    "Haupstrasse 38",
+                    "Haupstrasse 39",
+                    "Haupstrasse 40",
+                ],
+                "Haupstrasse 30-33, 35-40",
+            ),
+            (vec!["Haupstrasse 10"], "Haupstrasse 10"),
+            (vec!["Wanistrassse 1"], "Wanistrassse 1, «Logistikzentrum»"),
+            (
+                vec![
+                    "Im Sihlhof 20",
+                    "Im Sihlhof 23",
+                    "Im Sihlhof 4",
+                    "Im Sihlhof 2",
+                    "Im Sihlhof 28",
+                    "Im Sihlhof 27",
+                    "Im Sihlhof 24",
+                    "Im Sihlhof 21",
+                    "Im Sihlhof 1",
+                    "Im Sihlhof 25",
+                    "Im Sihlhof 22",
+                    "Im Sihlhof 29",
+                    "Im Sihlhof 26",
+                ],
+                "Im Sihlhof 1, 2, 4, 20-29, «The Jay» ",
+            ),
+            (
+                vec!["Via Santa Caterina 1", "Largo Zorzi 1"],
+                "Largo Zorzi 1 / Via Santa Caterina 1",
+            ),
+            (
+                vec!["Route des Paquays 105"],
+                "Chemin de la Confrerie / Route des Paquays 105",
+            ),
+            (
+                vec![
+                    "Schlossackerstrasse 11",
+                    "Schlossackerstrasse 7",
+                    "Schlossackerstrasse 9",
+                    "Schlossackerstrasse 13",
+                    "Hegifeldstrasse 85",
+                    "Hegifeldstrasse 89",
+                    "Hegifeldstrasse 87",
+                    "Schlossackerstrasse 5",
+                ],
+                "Schlossackerstrasse 5, 7, 9, 11, 13 / Hegifeldstrasse 85, 87, 89",
+            ),
+            (vec!["Fadenstrasse 26"], "Fadenstrasse 26, 4Viertel"),
+            (
+                vec![
+                    "Zentrum 2",
+                    "Zentrum 3a",
+                    "Zentrum 2a",
+                    "Zentrum 2b",
+                    "Zentrum 3",
+                    "Zentrum 3b",
+                ],
+                "Zentrum 2, 2a, 2b, 3, 3a, 3b, «Zentrumsüberbauung»",
+            ),
+            (
+                vec![
+                    "Rheinstrasse 3",
+                    "Bahnhofstrasse 3",
+                    "Schützenstrasse 6",
+                    "Schützenstrasse 10",
+                    "Schützenstrasse 8",
+                    "Schützenstrasse 4",
+                    "Rheinstrasse 5",
+                    "Schützenstrasse 12",
+                ],
+                "Bahnhofstrasse 3 / Rheinstrasse 3, 5/ Schützenstrasse 4, 6, 8, 10, 12",
+            ),
+            (
+                vec![
+                    "Neuchlenstrasse 7",
+                    "Neuchlenstrasse 7a",
+                    "Neuchlenstrasse 11",
+                ],
+                "Neuchlenstrasse 7/7a/11",
+            ),
+        ];
+        for (expected, street) in expected.iter() {
+            assert_detect_streets(expected, street);
+        }
     }
 }
```

### Comparing `pyguess-0.1.0/Cargo.lock` & `pyguess-0.2.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,73 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
-name = "atty"
-version = "0.2.14"
+name = "anstream"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -49,14 +87,20 @@
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "ciborium"
@@ -83,48 +127,75 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
 dependencies = [
+ "clap_builder",
+ "clap_derive",
+ "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
+dependencies = [
+ "anstream",
+ "anstyle",
  "bitflags",
  "clap_lex",
- "indexmap",
- "textwrap",
+ "strsim",
 ]
 
 [[package]]
-name = "clap_lex"
-version = "0.2.4"
+name = "clap_derive"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
- "os_str_bytes",
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.14",
 ]
 
 [[package]]
+name = "clap_lex"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "criterion"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
- "atty",
  "cast",
  "ciborium",
  "clap",
  "criterion-plot",
+ "is-terminal",
  "itertools",
- "lazy_static",
  "num-traits",
+ "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
  "serde_derive",
  "serde_json",
@@ -204,17 +275,39 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "guess-rs"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
+ "clap",
  "criterion",
  "pretty_assertions",
  "regex",
  "strsim",
  "threadpool",
  "toml",
  "unicode-segmentation",
@@ -229,32 +322,35 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
-name = "hermit-abi"
-version = "0.1.19"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -263,14 +359,37 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
+name = "is-terminal"
+version = "0.4.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "io-lifetimes",
+ "rustix",
+ "windows-sys",
+]
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -287,30 +406,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "lazy_static"
-version = "1.4.0"
+name = "libc"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
-name = "libc"
-version = "0.2.141"
+name = "linux-raw-sys"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -325,26 +444,26 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.2.15"
@@ -373,20 +492,14 @@
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
-
-[[package]]
 name = "output_vt100"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "628223faebab4e3e40667ee0b2336d34a5b960ff60ea743ddfdbcf7770bcfb66"
 dependencies = [
  "winapi",
 ]
@@ -399,23 +512,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "plotters"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
@@ -461,74 +574,74 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyguess"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "guess-rs",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset 0.9.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -560,37 +673,51 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+
+[[package]]
+name = "rustix"
+version = "0.37.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys",
+]
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
@@ -681,23 +808,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
-
-[[package]]
-name = "textwrap"
-version = "0.16.0"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "threadpool"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
 dependencies = [
@@ -763,14 +884,20 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "walkdir"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
  "winapi-util",
@@ -869,77 +996,77 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
 dependencies = [
```

