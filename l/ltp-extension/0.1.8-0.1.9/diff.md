# Comparing `tmp/ltp_extension-0.1.8.tar.gz` & `tmp/ltp_extension-0.1.9.tar.gz`

## Comparing `ltp_extension-0.1.8.tar` & `ltp_extension-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/Cargo.toml
--rw-r--r--   0      501       20      683 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/LICENSE
--rw-r--r--   0      501       20     7329 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/README.md
--rw-r--r--   0      501       20     5540 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/examples/cws.rs
--rw-r--r--   0      501       20     6718 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/examples/ner.rs
--rw-r--r--   0      501       20     5891 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/examples/pos.rs
--rw-r--r--   0      501       20      849 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/examples/simple.rs
--rw-r--r--   0      501       20     6191 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/eisner.rs
--rw-r--r--   0      501       20     5312 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/entities.rs
--rw-r--r--   0      501       20    10794 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/hook.rs
--rw-r--r--   0      501       20      769 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/lib.rs
--rw-r--r--   0      501       20    14458 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/cws.rs
--rw-r--r--   0      501       20     2845 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/mod.rs
--rw-r--r--   0      501       20    11761 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/ner.rs
--rw-r--r--   0      501       20    12304 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/pos.rs
--rw-r--r--   0      501       20     2674 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/feature.rs
--rw-r--r--   0      501       20      771 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/mod.rs
--rw-r--r--   0      501       20    20290 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/model.rs
--rw-r--r--   0      501       20     2158 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/parameter.rs
--rw-r--r--   0      501       20     3322 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/serialization.rs
--rw-r--r--   0      501       20    18581 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/trainer.rs
--rw-r--r--   0      501       20    16790 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/stnsplit.rs
--rw-r--r--   0      501       20     2417 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/src/viterbi.rs
--rw-r--r--   0      501       20    85668 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/test/eisner.npz
--rw-r--r--   0      501       20  7699102 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/test/viterbi.npz
--rw-r--r--   0      501       20      355 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/vendor/schema/cws.avsc
--rw-r--r--   0      501       20      622 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/vendor/schema/ner.avsc
--rw-r--r--   0      501       20      622 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/local_dependencies/ltp/vendor/schema/pos.avsc
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 ltp_extension-0.1.8/Cargo.toml
--rw-r--r--   0      501       20      683 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/LICENSE
--rw-r--r--   0      501       20     6212 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/README.md
--rw-r--r--   0      501       20     6070 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/examples/benchmark.py
--rw-r--r--   0      501       20     4066 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/examples/benchmark2.py
--rw-r--r--   0      501       20     1167 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/examples/legacy_train.py
--rw-r--r--   0      501       20      145 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/ltp_extension/__init__.py
--rw-r--r--   0      501       20      246 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/ltp_extension/algorithms/__init__.py
--rw-r--r--   0      501       20     1562 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/ltp_extension/algorithms/algorithms.pyi
--rw-r--r--   0      501       20       32 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/ltp_extension/ltp_extension.pyi
--rw-r--r--   0      501       20      377 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/ltp_extension/perceptron/__init__.py
--rw-r--r--   0      501       20     8245 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/ltp_extension/perceptron/perceptron.pyi
--rw-r--r--   0      501       20       76 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/pyproject.toml
--rw-r--r--   0      501       20     1094 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/algorithms.rs
--rw-r--r--   0      501       20      899 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/hook.rs
--rw-r--r--   0      501       20     1637 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/lib.rs
--rw-r--r--   0      501       20     2087 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/alg.rs
--rw-r--r--   0      501       20     1246 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/com.rs
--rw-r--r--   0      501       20      353 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/mod.rs
--rw-r--r--   0      501       20    11851 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/model.rs
--rw-r--r--   0      501       20     7417 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/specialization/cws.rs
--rw-r--r--   0      501       20      151 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/specialization/mod.rs
--rw-r--r--   0      501       20     8161 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/specialization/ner.rs
--rw-r--r--   0      501       20     7834 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/specialization/pos.rs
--rw-r--r--   0      501       20    11155 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/perceptron/trainer.rs
--rw-r--r--   0      501       20     3906 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/src/stnsplit.rs
--rw-r--r--   0      501       20     5674 2022-09-11 09:37:00.000000 ltp_extension-0.1.8/utils/stub.py
--rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 ltp_extension-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 ltp_extension-0.1.9/local_dependencies/ltp/Cargo.toml
+-rw-r--r--   0      501       20      683 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/LICENSE
+-rw-r--r--   0      501       20     7329 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/README.md
+-rw-r--r--   0      501       20     5546 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/examples/cws.rs
+-rw-r--r--   0      501       20     6724 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/examples/ner.rs
+-rw-r--r--   0      501       20     5897 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/examples/pos.rs
+-rw-r--r--   0      501       20      849 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/examples/simple.rs
+-rw-r--r--   0      501       20     6191 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/eisner.rs
+-rw-r--r--   0      501       20     5312 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/entities.rs
+-rw-r--r--   0      501       20    10794 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/hook.rs
+-rw-r--r--   0      501       20      769 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/lib.rs
+-rw-r--r--   0      501       20    15163 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/cws.rs
+-rw-r--r--   0      501       20     2844 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/mod.rs
+-rw-r--r--   0      501       20    11761 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/ner.rs
+-rw-r--r--   0      501       20    12304 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/pos.rs
+-rw-r--r--   0      501       20     3416 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/feature.rs
+-rw-r--r--   0      501       20      771 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/mod.rs
+-rw-r--r--   0      501       20    21531 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/model.rs
+-rw-r--r--   0      501       20     2158 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/parameter.rs
+-rw-r--r--   0      501       20     3322 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/serialization.rs
+-rw-r--r--   0      501       20    18581 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/trainer.rs
+-rw-r--r--   0      501       20    16790 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/stnsplit.rs
+-rw-r--r--   0      501       20     2417 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/src/viterbi.rs
+-rw-r--r--   0      501       20    85668 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/test/eisner.npz
+-rw-r--r--   0      501       20  7699102 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/test/viterbi.npz
+-rw-r--r--   0      501       20      355 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/vendor/schema/cws.avsc
+-rw-r--r--   0      501       20      622 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/vendor/schema/ner.avsc
+-rw-r--r--   0      501       20      622 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/local_dependencies/ltp/vendor/schema/pos.avsc
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 ltp_extension-0.1.9/Cargo.toml
+-rw-r--r--   0      501       20      683 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/LICENSE
+-rw-r--r--   0      501       20     6212 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/README.md
+-rw-r--r--   0      501       20     6070 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/examples/benchmark.py
+-rw-r--r--   0      501       20     4066 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/examples/benchmark2.py
+-rw-r--r--   0      501       20     1138 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/examples/legacy_train.py
+-rw-r--r--   0      501       20      145 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/ltp_extension/__init__.py
+-rw-r--r--   0      501       20      246 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/ltp_extension/algorithms/__init__.py
+-rw-r--r--   0      501       20     1562 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/ltp_extension/algorithms/algorithms.pyi
+-rw-r--r--   0      501       20       32 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/ltp_extension/ltp_extension.pyi
+-rw-r--r--   0      501       20      418 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/ltp_extension/perceptron/__init__.py
+-rw-r--r--   0      501       20     9497 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/ltp_extension/perceptron/perceptron.pyi
+-rw-r--r--   0      501       20       76 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/pyproject.toml
+-rw-r--r--   0      501       20     1094 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/algorithms.rs
+-rw-r--r--   0      501       20      899 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/hook.rs
+-rw-r--r--   0      501       20     1701 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/lib.rs
+-rw-r--r--   0      501       20     2087 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/alg.rs
+-rw-r--r--   0      501       20     1246 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/com.rs
+-rw-r--r--   0      501       20      368 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/mod.rs
+-rw-r--r--   0      501       20    11851 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/model.rs
+-rw-r--r--   0      501       20    11519 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/specialization/cws.rs
+-rw-r--r--   0      501       20      166 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/specialization/mod.rs
+-rw-r--r--   0      501       20     8161 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/specialization/ner.rs
+-rw-r--r--   0      501       20     7834 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/specialization/pos.rs
+-rw-r--r--   0      501       20    11155 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/perceptron/trainer.rs
+-rw-r--r--   0      501       20     3906 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/src/stnsplit.rs
+-rw-r--r--   0      501       20     5674 2022-10-19 17:05:34.000000 ltp_extension-0.1.9/utils/stub.py
+-rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 ltp_extension-0.1.9/PKG-INFO
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/Cargo.toml` & `ltp_extension-0.1.9/local_dependencies/ltp/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ltp"
-version = "0.1.7"
+version = "0.1.8"
 edition = "2021"
 authors = ["ylfeng <ylfeng@ir.hit.edu.cn>"]
 description = "Language Technology Platform For Rust."
 homepage = "https://github.com/HIT-SCIR/ltp"
 repository = "https://github.com/HIT-SCIR/ltp"
 keywords = ["ltp", "nlp"]
 exclude = [".github"]
@@ -39,15 +39,15 @@
 cedarwood = "0.4"
 
 # 断句避免过多内存申请
 smallvec = { version = "1" }
 # 数据集 shuffle
 rand = { version = "0.8" }
 # 特征裁剪
-binary-heap-plus = { version = "0.4.1" }
+binary-heap-plus = { version = "0.5" }
 
 # 并行
 rayon = { version = "1.5", optional = true }
 
 # 序列化
 serde = { version = "1.0", features = ["derive"], optional = true }
 serde_json = { version = "1.0", optional = true }
@@ -61,11 +61,11 @@
 default = []
 char-type = []
 cross-char = []
 parallel = ["rayon"]
 serialization = ["serde", "serde_json", "apache-avro"]
 
 [dev-dependencies]
-clap = { version = "3", features = ["derive"] }
+clap = { version = "4", features = ["derive"] }
 
 ndarray = "0.15"
 ndarray-npy = { version = "0.8", features = ["npz"] }
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/LICENSE` & `ltp_extension-0.1.9/local_dependencies/ltp/LICENSE`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/README.md` & `ltp_extension-0.1.9/local_dependencies/ltp/README.md`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/examples/cws.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/examples/cws.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use anyhow::Result;
-use clap::{ArgEnum, Parser};
+use clap::{Parser, ValueEnum};
 use itertools::Itertools;
 use ltp::perceptron::SerdeCWSModel;
 use ltp::{Algorithm, CWSDefinition as Definition, Codec, Format, ModelSerde, PaMode, Trainer};
 use std::collections::HashMap;
 use std::fs::File;
 use std::io::{BufRead, BufReader, Write};
 
@@ -11,30 +11,30 @@
 #[clap(author, version, about, long_about = None)]
 enum Args {
     Train(Train),
     Eval(Eval),
     Predict(Predict),
 }
 
-#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, ArgEnum)]
+#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, ValueEnum)]
 enum AlgorithmArg {
     Ap,
     Pa,
     PaI,
     PaII,
 }
 
 #[derive(Parser, Debug)]
 #[clap(author, version, about, long_about = None)]
 struct Train {
     #[clap(long, value_parser, default_value_t = 10)]
     epoch: usize,
     #[clap(short, long, value_parser, default_value_t = true)]
     shuffle: bool,
-    #[clap(arg_enum, value_parser, default_value_t = AlgorithmArg::Ap)]
+    #[clap(value_enum, value_parser, default_value_t = AlgorithmArg::Ap)]
     algorithm: AlgorithmArg,
     #[clap(long, value_parser, default_value_t = 8)]
     ap_threads: usize,
     #[clap(long, value_parser, default_value_t = 0.5)]
     pa_margin: f64,
 
     #[clap(long, value_parser, default_value_t = 8)]
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/examples/ner.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/examples/ner.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use anyhow::Result;
-use clap::{ArgEnum, Parser};
+use clap::{Parser, ValueEnum};
 use itertools::Itertools;
 use ltp::perceptron::SerdeNERModel;
 use ltp::{Algorithm, Codec, Format, ModelSerde, NERDefinition as Definition, PaMode, Trainer};
 use std::collections::HashMap;
 use std::fs::File;
 use std::io::{BufRead, BufReader, Write};
 
@@ -11,30 +11,30 @@
 #[clap(author, version, about, long_about = None)]
 enum Args {
     Train(Train),
     Eval(Eval),
     Predict(Predict),
 }
 
-#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, ArgEnum)]
+#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, ValueEnum)]
 enum AlgorithmArg {
     Ap,
     Pa,
     PaI,
     PaII,
 }
 
 #[derive(Parser, Debug)]
 #[clap(author, version, about, long_about = None)]
 struct Train {
     #[clap(long, value_parser, default_value_t = 10)]
     epoch: usize,
     #[clap(short, long, value_parser, default_value_t = true)]
     shuffle: bool,
-    #[clap(arg_enum, value_parser, default_value_t = AlgorithmArg::Ap)]
+    #[clap(value_enum, value_parser, default_value_t = AlgorithmArg::Ap)]
     algorithm: AlgorithmArg,
     #[clap(long, value_parser, default_value_t = 8)]
     ap_threads: usize,
     #[clap(long, value_parser, default_value_t = 0.5)]
     pa_margin: f64,
 
     #[clap(long, value_parser, default_value_t = 8)]
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/examples/pos.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/examples/pos.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use anyhow::Result;
-use clap::{ArgEnum, Parser};
+use clap::{Parser, ValueEnum};
 use itertools::Itertools;
 use ltp::perceptron::SerdePOSModel;
 use ltp::{Algorithm, Codec, Format, ModelSerde, POSDefinition as Definition, PaMode, Trainer};
 use std::collections::HashMap;
 use std::fs::File;
 use std::io::{BufRead, BufReader, Write};
 
@@ -11,30 +11,30 @@
 #[clap(author, version, about, long_about = None)]
 enum Args {
     Train(Train),
     Eval(Eval),
     Predict(Predict),
 }
 
-#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, ArgEnum)]
+#[derive(Copy, Clone, Debug, PartialEq, Eq, PartialOrd, Ord, ValueEnum)]
 enum AlgorithmArg {
     Ap,
     Pa,
     PaI,
     PaII,
 }
 
 #[derive(Parser, Debug)]
 #[clap(author, version, about, long_about = None)]
 struct Train {
     #[clap(long, value_parser, default_value_t = 10)]
     epoch: usize,
     #[clap(short, long, value_parser, default_value_t = true)]
     shuffle: bool,
-    #[clap(arg_enum, value_parser, default_value_t = AlgorithmArg::Ap)]
+    #[clap(value_enum, value_parser, default_value_t = AlgorithmArg::Ap)]
     algorithm: AlgorithmArg,
     #[clap(long, value_parser, default_value_t = 8)]
     ap_threads: usize,
     #[clap(long, value_parser, default_value_t = 0.5)]
     pa_margin: f64,
 
     #[clap(long, value_parser, default_value_t = 8)]
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/examples/simple.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/examples/simple.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/eisner.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/eisner.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/entities.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/entities.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/hook.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/hook.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/lib.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/cws.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/cws.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #[cfg(feature = "parallel")]
 use rayon::prelude::*;
 #[cfg(feature = "serialization")]
 use serde::{Deserialize, Serialize};
 use std::io::{BufRead, BufReader, Read, Write};
 
 /// Character type.
-#[cfg(feature = "char-type")]
 #[derive(Debug, Clone, Copy, Hash, PartialEq, Eq)]
 #[repr(u8)]
 pub enum CharacterType {
     /// Digit character. (e.g. 0, 1, 2, ...)
     Digit = 1,
 
     /// Roman character. (e.g. A, B, C, ...)
@@ -29,15 +28,14 @@
     /// Kanji (a.k.a. Hanzi or Hanja) character. (e.g. 漢, 字, ...)
     Kanji = 5,
 
     /// Other character.
     Other = 6,
 }
 
-#[cfg(feature = "char-type")]
 impl CharacterType {
     pub fn get_type(c: char) -> Self {
         match u32::from(c) {
             0x30..=0x39 | 0xFF10..=0xFF19 => Self::Digit,
             0x41..=0x5A | 0x61..=0x7A | 0xFF21..=0xFF3A | 0xFF41..=0xFF5A => Self::Roman,
             0x3040..=0x3096 => Self::Hiragana,
             0x30A0..=0x30FA | 0x30FC..=0x30FF | 0xFF66..=0xFF9F => Self::Katakana,
@@ -113,14 +111,24 @@
                 #[cfg(feature = "char-type")]
                 buf_feature!(
                     buffer,
                     feature,
                     "c{}",
                     CharacterType::get_type(pre_char) as u8
                 );
+
+                // TYPE(ch[-1]) TYPE(ch[0])
+                buf_feature!(
+                    buffer,
+                    feature,
+                    "d{}{}",
+                    CharacterType::get_type(pre_char) as u8,
+                    CharacterType::get_type(cur_char) as u8
+                );
+
                 if pre2_char != char_null {
                     // ch[-2]
                     buf_feature!(buffer, feature, "0{}", pre2_char);
                     // ch[-2]ch[-1]
                     buf_feature!(buffer, feature, "5{}{}", pre2_char, pre_char);
                     // ch[-2]ch[0]
                     #[cfg(feature = "cross-char")]
@@ -380,8 +388,22 @@
             sentence.len(),
             buffer.len(),
             buffer.len() / sentence.len()
         );
 
         Ok(())
     }
+
+    #[test]
+    fn test_features() -> Result<()> {
+        let define = Define::default();
+        let (_, num_han) = define.parse_char_features("1汉")?;
+        let (_, roman_han) = define.parse_char_features("a汉")?;
+        let (_, num_roman) = define.parse_char_features("1a")?;
+
+        println!("数字+汉字: {:?}", num_han);
+        println!("字母+汉字: {:?}", roman_han);
+        println!("数字+字母: {:?}", num_roman);
+
+        Ok(())
+    }
 }
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/mod.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 macro_rules! buf_feature {
     ($dst:expr, $feat:tt, $($arg:tt)*) => {
         write!($dst, $($arg)*)?;
         $feat.push($dst.len());
     };
 }
 
-
 pub trait CommonDefinePredict {}
 
 impl CommonDefinePredict for POSDefinition {}
 
 impl CommonDefinePredict for NERDefinition {}
 
 pub trait GenericItem<'a> {
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/ner.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/ner.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/definition/pos.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/definition/pos.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/feature.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/feature.rs`

 * *Files 20% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         self.into_iter().collect()
     }
 }
 
 pub trait TraitFeaturesTrainUtils: Clone {
     fn feature_num(&self) -> usize;
     fn insert_feature(&mut self, key: String, value: usize);
+    fn remove_feature(&mut self, key: &str) -> Option<usize>;
     fn put_feature(&mut self, key: String, value: usize);
+    fn del_feature(&mut self, key: &str) -> Option<usize>;
 }
 
 impl<T> TraitFeature for &T
 where
     T: TraitFeature,
 {
     fn get_with_key(&self, key: &str) -> Option<usize> {
@@ -64,31 +66,49 @@
         self.deref().feature_num()
     }
 
     fn insert_feature(&mut self, key: String, value: usize) {
         self.deref().put_feature(key, value)
     }
 
+    fn remove_feature(&mut self, key: &str) -> Option<usize> {
+        self.deref().del_feature(key)
+    }
+
     fn put_feature(&mut self, key: String, value: usize) {
         self.deref().insert_feature(key, value)
     }
+
+    fn del_feature(&mut self, key: &str) -> Option<usize> {
+        self.deref().remove_feature(key)
+    }
 }
 
 impl<T> TraitFeaturesTrainUtils for Arc<T>
 where
     T: TraitFeaturesTrainUtils,
 {
     fn feature_num(&self) -> usize {
         self.deref().feature_num()
     }
+
     fn insert_feature(&mut self, key: String, value: usize) {
-        self.deref().insert_feature(key, value)
+        self.deref().put_feature(key, value)
+    }
+
+    fn remove_feature(&mut self, key: &str) -> Option<usize> {
+        self.deref().del_feature(key)
     }
+
     fn put_feature(&mut self, key: String, value: usize) {
-        self.deref().put_feature(key, value)
+        self.deref().insert_feature(key, value)
+    }
+
+    fn del_feature(&mut self, key: &str) -> Option<usize> {
+        self.deref().remove_feature(key)
     }
 }
 
 // HashMap
 
 impl TraitFeature for HashMap<String, usize> {
     fn get_with_key(&self, key: &str) -> Option<usize> {
@@ -101,11 +121,19 @@
         self.len()
     }
 
     fn insert_feature(&mut self, key: String, value: usize) {
         self.insert(key, value);
     }
 
+    fn remove_feature(&mut self, key: &str) -> Option<usize> {
+        self.remove(key)
+    }
+
     fn put_feature(&mut self, key: String, value: usize) {
         self.insert(key, value);
     }
+
+    fn del_feature(&mut self, key: &str) -> Option<usize> {
+        self.remove(key)
+    }
 }
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/mod.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/mod.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/model.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/model.rs`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 use std::fmt::{Debug, Display, Formatter};
 use std::iter::zip;
 use std::mem::swap;
 
 #[cfg_attr(feature = "serialization", derive(Serialize, Deserialize))]
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub enum PaMode<Param>
-    where
-        Param: TraitParameter,
+where
+    Param: TraitParameter,
 {
     Pa,
     PaI(Param),
     PaII(Param),
 }
 
 impl<Param: TraitParameter> Default for PaMode<Param> {
@@ -32,69 +32,71 @@
         PaMode::Pa
     }
 }
 
 #[cfg_attr(feature = "serialization", derive(Serialize, Deserialize))]
 #[derive(Default, Debug, Clone)]
 pub struct Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Define: Definition,
-        Feature: TraitFeature,
-        ParamStorage: TraitParameterStorage<Param>,
-        Param: TraitParameter,
+where
+    Define: Definition,
+    Feature: TraitFeature,
+    ParamStorage: TraitParameterStorage<Param>,
+    Param: TraitParameter,
 {
     pub definition: Define,
     pub features: Feature,
     pub parameters: ParamStorage,
     #[cfg_attr(feature = "serialization", serde(skip_serializing))]
     __phantom: Option<Param>,
 }
 
 impl<Define, Feature, ParamStorage, Param> Display
-for Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
-        Define: Definition,
+    for Perceptron<Define, Feature, ParamStorage, Param>
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
+    Define: Definition,
 {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "Perceptron [ Num of Params: {} Precision: {} ]",
             self.parameters.len(),
             std::any::type_name::<Param>()
         )
     }
 }
 
 unsafe impl<Define, Feature, ParamStorage, Param> Send
-for Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
-        Define: Definition,
-{}
+    for Perceptron<Define, Feature, ParamStorage, Param>
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
+    Define: Definition,
+{
+}
 
 unsafe impl<Define, Feature, ParamStorage, Param> Sync
-for Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
-        Define: Definition,
-{}
+    for Perceptron<Define, Feature, ParamStorage, Param>
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
+    Define: Definition,
+{
+}
 
 impl<Define, Feature, ParamStorage, Param> Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
-        Define: Definition,
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
+    Define: Definition,
 {
     pub fn new_with_parameters(
         definition: Define,
         features: Feature,
         parameters: ParamStorage,
     ) -> Self {
         Perceptron {
@@ -196,82 +198,97 @@
             self.viterbi_decode(features)
         } else {
             self.simple_decode(features)
         }
     }
 
     pub fn evaluate(&self, inputs: &[Vec<String>], labels: &[usize]) -> (usize, usize, usize) {
-        let features: Vec<_> = inputs.iter().map(|f| self.features.get_vector_string(f)).collect();
+        let features: Vec<_> = inputs
+            .iter()
+            .map(|f| self.features.get_vector_string(f))
+            .collect();
         let preds = self.decode(&features);
         self.definition.evaluate(&preds, labels)
     }
 }
 
 impl<Define, Feature, ParamStorage, Param> Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
-        Define: Definition + CommonDefinePredict,
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
+    Define: Definition + CommonDefinePredict,
 {
     pub fn predict_with_buffer(
         &self,
         sentence: <Define::RawFeature as GenericItem>::Item,
         buffer: &mut Vec<u8>,
     ) -> Result<<Define::Prediction as GenericItem>::Item> {
-        let (fragment, features) = self.definition.parse_features_with_buffer(&sentence, buffer)?;
+        let (fragment, features) = self
+            .definition
+            .parse_features_with_buffer(&sentence, buffer)?;
         let features: Vec<_> = features
             .iter()
             .map(|f| self.features.get_vector_str(f))
             .collect();
         let preds = self.decode(&features);
 
         Ok(self.definition.predict(&sentence, &fragment, &preds))
     }
 }
 
 impl<Feature, ParamStorage, Param> Perceptron<POSDefinition, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
 {
     pub fn predict(&self, sentence: &[&str]) -> Result<Vec<&str>> {
         let mut buffer = Vec::with_capacity(sentence.len() * 180);
         self.predict_with_buffer(sentence, &mut buffer)
     }
 }
 
 impl<Feature, ParamStorage, Param> Perceptron<NERDefinition, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
 {
     pub fn predict(&self, sentence: (&[&str], &[&str])) -> Result<Vec<&str>> {
         let mut buffer = Vec::with_capacity(sentence.0.len() * 150);
         self.predict_with_buffer(sentence, &mut buffer)
     }
 }
 
-use crate::{get_entities, CWSDefinition, POSDefinition, NERDefinition};
+use crate::{get_entities, CWSDefinition, NERDefinition, POSDefinition};
 
 impl<Feature, ParamStorage, Param> Perceptron<CWSDefinition, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param>,
+where
+    Feature: TraitFeature,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param>,
 {
+    pub fn check_feature(&self, feature: &str) -> Option<usize> {
+        self.features.get_with_key(feature)
+    }
+
     pub fn predict<'a>(&self, sentence: &'a str) -> Result<Vec<&'a str>> {
         let mut buffer = Vec::with_capacity(sentence.len() * 20);
         self.predict_with_buffer(sentence, &mut buffer)
     }
 
-    pub fn predict_with_buffer<'a>(&self, sentence: &'a str, buffer: &mut Vec<u8>) -> Result<Vec<&'a str>> {
-        let (fragments, features) = self.definition.parse_features_with_buffer(&sentence, buffer)?;
+    pub fn predict_with_buffer<'a>(
+        &self,
+        sentence: &'a str,
+        buffer: &mut Vec<u8>,
+    ) -> Result<Vec<&'a str>> {
+        let (fragments, features) = self
+            .definition
+            .parse_features_with_buffer(&sentence, buffer)?;
         let features: Vec<_> = features
             .iter()
             .map(|f| self.features.get_vector_str(f))
             .collect();
         let preds = self.decode(&features);
 
         let preds = self.definition.to_labels(&preds);
@@ -283,34 +300,67 @@
                 let end = fragments[end + 1];
                 &sentence[start..end]
             })
             .collect::<Vec<_>>())
     }
 }
 
+impl<Feature, ParamStorage, Param> Perceptron<CWSDefinition, Feature, ParamStorage, Param>
+where
+    Feature: TraitFeature + TraitFeaturesTrainUtils,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param> + TraitParameterStorageCompressUtils<Param>,
+{
+    pub fn add_core_rule(&mut self, key: &str, s: Param, b: Param, m: Param, e: Param) {
+        if self.features.get_with_key(key).is_none() {
+            let feature_num = self.parameters.len() / 4;
+            self.features.insert_feature(String::from(key), feature_num);
+
+            // S B M E
+            self.parameters.push(s);
+            self.parameters.push(b);
+            self.parameters.push(m);
+            self.parameters.push(e);
+        }
+    }
+
+    pub fn enable_feature_rule(&mut self, key: &str, feature: &str) {
+        if let Some(index) = self.features.get_with_key(key) {
+            self.features.insert_feature(feature.to_string(), index);
+        }
+    }
+
+    pub fn disable_feature_rule(&mut self, feature: &str) -> Option<usize> {
+        self.features.remove_feature(feature)
+    }
+}
+
 // 模型训练
 impl<Define, Feature, ParamStorage, Param> Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature + TraitFeaturesTrainUtils,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param> + TraitParameterStorageTrainUtils<Param>,
-        Define: Definition,
+where
+    Feature: TraitFeature + TraitFeaturesTrainUtils,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param> + TraitParameterStorageTrainUtils<Param>,
+    Define: Definition,
 {
     // 被动攻击算法
     pub fn pa_train_iter(
         &mut self,
         inputs: &[Vec<String>],
         labels: &[usize],
         total: &mut [Param],
         timestamp: &mut [usize],
         current: usize,
         mode: &PaMode<Param>,
     ) {
         let label_num = self.definition.label_num();
-        let features: Vec<_> = inputs.iter().map(|f| self.features.get_vector_string(f)).collect();
+        let features: Vec<_> = inputs
+            .iter()
+            .map(|f| self.features.get_vector_string(f))
+            .collect();
         let preds = self.decode(&features);
 
         if labels.ne(&preds) {
             let errors = zip(labels, &preds)
                 .enumerate()
                 .filter(|&(_, (gold, pred))| gold != pred);
 
@@ -411,15 +461,18 @@
         inputs: &[Vec<String>],
         labels: &[usize],
         total: &mut [Param],
         timestamp: &mut [usize],
         current: usize,
     ) {
         let label_num = self.definition.label_num();
-        let features: Vec<_> = inputs.iter().map(|f| self.features.get_vector_string(f)).collect();
+        let features: Vec<_> = inputs
+            .iter()
+            .map(|f| self.features.get_vector_string(f))
+            .collect();
         let preds = self.decode(&features);
 
         if labels.ne(&preds) {
             for (idx, (&gold, &pred)) in zip(labels, &preds)
                 .enumerate()
                 .filter(|&(_, (gold, pred))| gold != pred)
             {
@@ -462,15 +515,18 @@
             }
         }
     }
 
     // 并行 averaged perceptron 算法
     pub fn ap_train_parallel_iter(&mut self, inputs: &[Vec<String>], labels: &[usize]) {
         let label_num = self.definition.label_num();
-        let features: Vec<_> = inputs.iter().map(|f| self.features.get_vector_string(f)).collect();
+        let features: Vec<_> = inputs
+            .iter()
+            .map(|f| self.features.get_vector_string(f))
+            .collect();
         let preds = self.decode(&features);
 
         if labels.ne(&preds) {
             for (idx, (&gold, &pred)) in zip(labels, &preds)
                 .enumerate()
                 .filter(|&(_, (gold, pred))| gold != pred)
             {
@@ -489,19 +545,19 @@
             }
         }
     }
 }
 
 // 模型压缩
 impl<Define, Feature, ParamStorage, Param> Perceptron<Define, Feature, ParamStorage, Param>
-    where
-        Feature: TraitFeature + TraitFeaturesTrainUtils + TraitFeatureCompressUtils,
-        Param: TraitParameter,
-        ParamStorage: TraitParameterStorage<Param> + TraitParameterStorageCompressUtils<Param>,
-        Define: Definition,
+where
+    Feature: TraitFeature + TraitFeaturesTrainUtils + TraitFeatureCompressUtils,
+    Param: TraitParameter,
+    ParamStorage: TraitParameterStorage<Param> + TraitParameterStorageCompressUtils<Param>,
+    Define: Definition,
 {
     fn param_score(parameters: &ParamStorage, label_num: usize, feature: usize) -> Param {
         let mut score = Param::zero();
         let start = feature * label_num;
         let end = start + label_num;
         for i in start..end {
             score += parameters[i].abs();
```

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/parameter.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/parameter.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/serialization.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/serialization.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/perceptron/trainer.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/perceptron/trainer.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/stnsplit.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/stnsplit.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/src/viterbi.rs` & `ltp_extension-0.1.9/local_dependencies/ltp/src/viterbi.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/test/eisner.npz` & `ltp_extension-0.1.9/local_dependencies/ltp/test/eisner.npz`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/test/viterbi.npz` & `ltp_extension-0.1.9/local_dependencies/ltp/test/viterbi.npz`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/vendor/schema/ner.avsc` & `ltp_extension-0.1.9/local_dependencies/ltp/vendor/schema/ner.avsc`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/local_dependencies/ltp/vendor/schema/pos.avsc` & `ltp_extension-0.1.9/local_dependencies/ltp/vendor/schema/pos.avsc`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/Cargo.toml` & `ltp_extension-0.1.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ltp-extension"
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 authors = ["ylfeng <ylfeng@ir.hit.edu.cn>"]
 description = "Rust Extension For Language Technology Platform(Python)."
 homepage = "https://github.com/HIT-SCIR/ltp"
 repository = "https://github.com/HIT-SCIR/ltp"
 keywords = ["ltp", "nlp"]
 exclude = [".github"]
```

### Comparing `ltp_extension-0.1.8/LICENSE` & `ltp_extension-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/README.md` & `ltp_extension-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/examples/benchmark.py` & `ltp_extension-0.1.9/examples/benchmark.py`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/examples/benchmark2.py` & `ltp_extension-0.1.9/examples/benchmark2.py`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/examples/legacy_train.py` & `ltp_extension-0.1.9/examples/legacy_train.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-from ltp_extension.perceptron import (
-    Algorithm,
-    CWSModel,
-    CWSTrainer,
-    Model,
-    ModelType,
-    Trainer,
-)
+from ltp_extension.perceptron import Algorithm, CWSModel, CWSTrainer, Model, ModelType, Trainer
 
 
 def train_cws():
     ap = Algorithm("AP")
     pa = Algorithm("Pa")
     pai = Algorithm("PaI", 0.5)
     paii = Algorithm("PaII", 0.5)
```

### Comparing `ltp_extension-0.1.8/ltp_extension/algorithms/algorithms.pyi` & `ltp_extension-0.1.9/ltp_extension/algorithms/algorithms.pyi`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/ltp_extension/perceptron/perceptron.pyi` & `ltp_extension-0.1.9/ltp_extension/perceptron/perceptron.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,54 @@
 
     def __init__(self, algorithm, param=None):
         pass
 
 class CWSModel:
     def __init__(self, path):
         pass
+    def add_feature_rule(self, core, feature, s, b, m, e):
+        """
+        自定义新feature
+        """
+        pass
     def batch_predict(self, batch_text, threads=8):
         """
         Predict batched sentences
         """
         pass
+    def disable_cut(self, a, b):
+        """
+        关闭连续不同类型之间的强制切分
+        """
+        pass
+    def disable_cut_d(self, a, b):
+        """
+        关闭连续不同类型之间的强制切分
+        """
+        pass
+    def disable_feature_rule(self, core, feature, s, b, m, e):
+        """
+        移除自定义新 feature
+        """
+        pass
+    def enable_cut(self, a, b):
+        """
+        开启连续不同类型之间的强制切分
+        """
+        pass
+    def enable_cut_d(self, a, b):
+        """
+        开启连续不同类型之间的强制切分
+        """
+        pass
+    def enable_feature_rule(self, core, feature):
+        """
+        启用自定义新 feature
+        """
+        pass
     @staticmethod
     def load(path):
         """
         Load Model from a path
         """
         pass
     def predict(self, text):
@@ -103,14 +138,24 @@
     @property
     def verbose(self):
         """
         Get the value of the verbose parameter.
         """
         pass
 
+class CharacterType:
+    """
+    Digit: Digit character. (e.g. 0, 1, 2, ...)
+    Roman: Roman character. (e.g. A, B, C, ...)
+    Hiragana: Japanese Hiragana character. (e.g. あ, い, う, ...)
+    Katakana: Japanese Katakana character. (e.g. ア, イ, ウ, ...)
+    Kanji: Kanji (a.k.a. Hanzi or Hanja) character. (e.g. 漢, 字, ...)
+    Other: Other character.
+    """
+
 class Model:
     def __init__(self, path, model_type=ModelType.Auto):
         pass
     def batch_predict(self, *args, threads=8):
         """
         Predict batched sentences
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ltp_extension-0.1.8/src/algorithms.rs` & `ltp_extension-0.1.9/src/algorithms.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/src/hook.rs` & `ltp_extension-0.1.9/src/hook.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/src/lib.rs` & `ltp_extension-0.1.9/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 mod perceptron;
 mod stnsplit;
 
 use crate::perceptron::{ModelType, PyModel, PyTrainer};
 pub use algorithms::{py_eisner, py_get_entities, py_viterbi_decode_postprocess};
 use hook::PyHook;
 pub use perceptron::{
-    PyAlgorithm, PyCWSModel, PyCWSTrainer, PyNERModel, PyNERTrainer, PyPOSModel, PyPOSTrainer,
+    CharacterType, PyAlgorithm, PyCWSModel, PyCWSTrainer, PyNERModel, PyNERTrainer, PyPOSModel,
+    PyPOSTrainer,
 };
 use pyo3::prelude::*;
 use stnsplit::StnSplit;
 
-
 /// LTP Module
 #[pymodule]
 fn ltp_extension(py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
 
     // Algorithms Module
     let algorithms = PyModule::new(py, "algorithms")?;
@@ -37,14 +37,15 @@
     // Perceptron Module
     let perceptron = PyModule::new(py, "perceptron")?;
     perceptron.add_class::<PyModel>()?;
     perceptron.add_class::<ModelType>()?;
     perceptron.add_class::<PyTrainer>()?;
     perceptron.add_class::<PyAlgorithm>()?;
 
+    perceptron.add_class::<CharacterType>()?;
     perceptron.add_class::<PyCWSModel>()?;
     perceptron.add_class::<PyCWSTrainer>()?;
 
     perceptron.add_class::<PyPOSModel>()?;
     perceptron.add_class::<PyPOSTrainer>()?;
 
     perceptron.add_class::<PyNERModel>()?;
```

### Comparing `ltp_extension-0.1.8/src/perceptron/alg.rs` & `ltp_extension-0.1.9/src/perceptron/alg.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/src/perceptron/com.rs` & `ltp_extension-0.1.9/src/perceptron/com.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/src/perceptron/model.rs` & `ltp_extension-0.1.9/src/perceptron/model.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/src/perceptron/specialization/cws.rs` & `ltp_extension-0.1.9/src/perceptron/specialization/ner.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,102 @@
 use crate::impl_model;
 use crate::perceptron::{Perceptron, PyAlgorithm};
-use ltp::perceptron::{CWSDefinition as Definition, Trainer};
+use ltp::perceptron::{NERDefinition as Definition, Trainer};
 use pyo3::prelude::*;
 use pyo3::types::{PyList, PyString, PyTuple};
 use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 
 pub type Model = Perceptron<Definition>;
 
-#[pyclass(module = "ltp_extension.perceptron", name = "CWSModel", subclass)]
+#[pyclass(module = "ltp_extension.perceptron", name = "NERModel", subclass)]
 #[pyo3(text_signature = "(self, path)")]
 #[derive(Clone, Serialize, Deserialize, Default, Debug)]
-pub struct PyCWSModel {
+pub struct PyNERModel {
     pub model: Model,
 }
 
-impl_model!(PyCWSModel);
+impl_model!(PyNERModel);
 
 #[pymethods]
-impl PyCWSModel {
+impl PyNERModel {
     #[new]
     pub fn new(path: &str) -> PyResult<Self> {
         Ok(Self::inner_load(path)?)
     }
 
     #[args(args = "*", threads = 8)]
     pub fn __call__(&self, py: Python, args: &PyTuple, threads: usize) -> PyResult<PyObject> {
         let first = args.get_item(0)?;
         let is_single = match first.get_type().name()? {
-            "str" => true,
-            "list" => false,
+            "list" => match first.get_item(0)?.get_type().name()? {
+                "str" => true,
+                "list" => false,
+                name => {
+                    return Err(pyo3::exceptions::PyValueError::new_err(format!(
+                        "type list(\"{}\") has not been supported",
+                        name
+                    )));
+                }
+            },
             name => {
                 return Err(pyo3::exceptions::PyValueError::new_err(format!(
                     "type \"{}\" has not been supported",
                     name
                 )));
             }
         };
 
         match is_single {
-            true => self.predict(py, args.get_item(0)?.extract()?),
-            false => self.batch_predict(py, args.get_item(0)?.extract()?, threads),
+            true => self.predict(
+                py,
+                args.get_item(0)?.extract()?,
+                args.get_item(1)?.extract()?,
+            ),
+            false => self.batch_predict(
+                py,
+                args.get_item(0)?.extract()?,
+                args.get_item(1)?.extract()?,
+                threads,
+            ),
         }
     }
 
     /// Predict a sentence
-    #[pyo3(text_signature = "(self, text)")]
-    pub fn predict(&self, py: Python, text: &str) -> PyResult<PyObject> {
+    #[pyo3(text_signature = "(self, words, pos)")]
+    pub fn predict(&self, py: Python, words: Vec<&str>, pos: Vec<&str>) -> PyResult<PyObject> {
         Ok(PyList::new(
             py,
             self.model
-                .predict(text)?
+                .predict((&words, &pos))?
                 .into_iter()
                 .map(|s| PyString::new(py, s)),
         )
             .into())
     }
 
     /// Predict batched sentences
     #[args(threads = "8")]
-    #[pyo3(text_signature = "(self, batch_text, threads=8)")]
+    #[pyo3(text_signature = "(self, batch_words, batch_pos , threads=8)")]
     pub fn batch_predict(
         &self,
         py: Python,
-        batch_text: Vec<&str>,
+        batch_words: Vec<Vec<&str>>,
+        batch_pos: Vec<Vec<&str>>,
         threads: usize,
     ) -> PyResult<PyObject> {
         let pool = rayon::ThreadPoolBuilder::new()
             .num_threads(threads)
             .build()
             .unwrap();
         let result: Result<Vec<Vec<_>>, _> = pool.install(|| {
-            batch_text
+            batch_words
                 .into_par_iter()
-                .map(|text| self.model.predict(text))
+                .zip(batch_pos)
+                .map(|(words, pos)| self.model.predict((&words, &pos)))
                 .collect()
         });
         let result = result?;
         let res = PyList::new(py, Vec::<&PyList>::with_capacity(result.len()));
         for snt in result {
             let snt_res = PyList::new(py, Vec::<&PyString>::with_capacity(snt.len()));
             for tag in snt {
@@ -102,27 +121,27 @@
     }
 
     fn __repr__(&self) -> String {
         format!("{}", self.model)
     }
 }
 
-#[pyclass(module = "ltp_extension.perceptron", name = "CWSTrainer", subclass)]
-#[pyo3(text_signature = "(self)")]
+#[pyclass(module = "ltp_extension.perceptron", name = "NERTrainer", subclass)]
+#[pyo3(text_signature = "(self, labels)")]
 #[derive(Clone, Serialize, Deserialize, Default, Debug)]
-pub struct PyCWSTrainer {
+pub struct PyNERTrainer {
     pub trainer: Trainer<Definition>,
 }
 
 #[pymethods]
-impl PyCWSTrainer {
+impl PyNERTrainer {
     #[new]
-    pub fn new() -> PyResult<Self> {
+    pub fn new(labels: Vec<String>) -> PyResult<Self> {
         Ok(Self {
-            trainer: Trainer::new(),
+            trainer: Trainer::new_with_define(Definition::new(labels)),
         })
     }
 
     /// Get the value of the epoch parameter.
     #[getter]
     pub fn get_epoch(&self) -> PyResult<usize> {
         Ok(self.trainer.epoch)
@@ -240,25 +259,25 @@
     pub fn load_eval_data(&mut self, data: &str) -> PyResult<()> {
         self.trainer.eval_set = Some(self.trainer.load_dataset(data)?);
         Ok(())
     }
 
     /// Train a Segmentor model
     #[pyo3(text_signature = "(self)")]
-    pub fn train(&self) -> PyResult<PyCWSModel> {
-        let model = PyCWSModel {
+    pub fn train(&self) -> PyResult<PyNERModel> {
+        let model = PyNERModel {
             model: self.trainer.build()?,
         };
 
         Ok(model)
     }
 
     /// Eval a Segmentor model
     #[pyo3(text_signature = "(self, model)")]
-    pub fn eval(&self, model: &PyCWSModel) -> PyResult<()> {
+    pub fn eval(&self, model: &PyNERModel) -> PyResult<()> {
         self.trainer.evaluate(&model.model)?;
         Ok(())
     }
 
     fn __repr__(&self) -> String {
         format!("{}", self.trainer)
     }
```

### Comparing `ltp_extension-0.1.8/src/perceptron/specialization/ner.rs` & `ltp_extension-0.1.9/src/perceptron/specialization/pos.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 use crate::impl_model;
 use crate::perceptron::{Perceptron, PyAlgorithm};
-use ltp::perceptron::{NERDefinition as Definition, Trainer};
+use ltp::perceptron::{POSDefinition as Definition, Trainer};
 use pyo3::prelude::*;
 use pyo3::types::{PyList, PyString, PyTuple};
 use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 
 pub type Model = Perceptron<Definition>;
 
-#[pyclass(module = "ltp_extension.perceptron", name = "NERModel", subclass)]
+#[pyclass(module = "ltp_extension.perceptron", name = "POSModel", subclass)]
 #[pyo3(text_signature = "(self, path)")]
 #[derive(Clone, Serialize, Deserialize, Default, Debug)]
-pub struct PyNERModel {
+pub struct PyPOSModel {
     pub model: Model,
 }
 
-impl_model!(PyNERModel);
+impl_model!(PyPOSModel);
 
 #[pymethods]
-impl PyNERModel {
+impl PyPOSModel {
     #[new]
     pub fn new(path: &str) -> PyResult<Self> {
         Ok(Self::inner_load(path)?)
     }
 
     #[args(args = "*", threads = 8)]
     pub fn __call__(&self, py: Python, args: &PyTuple, threads: usize) -> PyResult<PyObject> {
@@ -43,60 +43,49 @@
                     "type \"{}\" has not been supported",
                     name
                 )));
             }
         };
 
         match is_single {
-            true => self.predict(
-                py,
-                args.get_item(0)?.extract()?,
-                args.get_item(1)?.extract()?,
-            ),
-            false => self.batch_predict(
-                py,
-                args.get_item(0)?.extract()?,
-                args.get_item(1)?.extract()?,
-                threads,
-            ),
+            true => self.predict(py, args.get_item(0)?.extract()?),
+            false => self.batch_predict(py, args.get_item(0)?.extract()?, threads),
         }
     }
 
     /// Predict a sentence
-    #[pyo3(text_signature = "(self, words, pos)")]
-    pub fn predict(&self, py: Python, words: Vec<&str>, pos: Vec<&str>) -> PyResult<PyObject> {
+    #[pyo3(text_signature = "(self, words)")]
+    pub fn predict(&self, py: Python, words: Vec<&str>) -> PyResult<PyObject> {
         Ok(PyList::new(
             py,
             self.model
-                .predict((&words, &pos))?
+                .predict(&words)?
                 .into_iter()
                 .map(|s| PyString::new(py, s)),
         )
             .into())
     }
 
     /// Predict batched sentences
     #[args(threads = "8")]
-    #[pyo3(text_signature = "(self, batch_words, batch_pos , threads=8)")]
+    #[pyo3(text_signature = "(self, batch_words, threads=8)")]
     pub fn batch_predict(
         &self,
         py: Python,
         batch_words: Vec<Vec<&str>>,
-        batch_pos: Vec<Vec<&str>>,
         threads: usize,
     ) -> PyResult<PyObject> {
         let pool = rayon::ThreadPoolBuilder::new()
             .num_threads(threads)
             .build()
             .unwrap();
         let result: Result<Vec<Vec<_>>, _> = pool.install(|| {
             batch_words
                 .into_par_iter()
-                .zip(batch_pos)
-                .map(|(words, pos)| self.model.predict((&words, &pos)))
+                .map(|text| self.model.predict(&text))
                 .collect()
         });
         let result = result?;
         let res = PyList::new(py, Vec::<&PyList>::with_capacity(result.len()));
         for snt in result {
             let snt_res = PyList::new(py, Vec::<&PyString>::with_capacity(snt.len()));
             for tag in snt {
@@ -121,23 +110,23 @@
     }
 
     fn __repr__(&self) -> String {
         format!("{}", self.model)
     }
 }
 
-#[pyclass(module = "ltp_extension.perceptron", name = "NERTrainer", subclass)]
+#[pyclass(module = "ltp_extension.perceptron", name = "POSTrainer", subclass)]
 #[pyo3(text_signature = "(self, labels)")]
 #[derive(Clone, Serialize, Deserialize, Default, Debug)]
-pub struct PyNERTrainer {
+pub struct PyPOSTrainer {
     pub trainer: Trainer<Definition>,
 }
 
 #[pymethods]
-impl PyNERTrainer {
+impl PyPOSTrainer {
     #[new]
     pub fn new(labels: Vec<String>) -> PyResult<Self> {
         Ok(Self {
             trainer: Trainer::new_with_define(Definition::new(labels)),
         })
     }
 
@@ -259,25 +248,25 @@
     pub fn load_eval_data(&mut self, data: &str) -> PyResult<()> {
         self.trainer.eval_set = Some(self.trainer.load_dataset(data)?);
         Ok(())
     }
 
     /// Train a Segmentor model
     #[pyo3(text_signature = "(self)")]
-    pub fn train(&self) -> PyResult<PyNERModel> {
-        let model = PyNERModel {
+    pub fn train(&self) -> PyResult<PyPOSModel> {
+        let model = PyPOSModel {
             model: self.trainer.build()?,
         };
 
         Ok(model)
     }
 
     /// Eval a Segmentor model
     #[pyo3(text_signature = "(self, model)")]
-    pub fn eval(&self, model: &PyNERModel) -> PyResult<()> {
+    pub fn eval(&self, model: &PyPOSModel) -> PyResult<()> {
         self.trainer.evaluate(&model.model)?;
         Ok(())
     }
 
     fn __repr__(&self) -> String {
         format!("{}", self.trainer)
     }
```

### Comparing `ltp_extension-0.1.8/src/perceptron/trainer.rs` & `ltp_extension-0.1.9/src/perceptron/trainer.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/src/stnsplit.rs` & `ltp_extension-0.1.9/src/stnsplit.rs`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/utils/stub.py` & `ltp_extension-0.1.9/utils/stub.py`

 * *Files identical despite different names*

### Comparing `ltp_extension-0.1.8/PKG-INFO` & `ltp_extension-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltp-extension
-Version: 0.1.8
+Version: 0.1.9
 Summary: Rust Extension For Language Technology Platform(Python).
 Keywords: ltp,nlp
 Home-Page: https://github.com/HIT-SCIR/ltp
 Author: ylfeng <ylfeng@ir.hit.edu.cn>
 Author-email: ylfeng <ylfeng@ir.hit.edu.cn>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/HIT-SCIR/ltp
```

