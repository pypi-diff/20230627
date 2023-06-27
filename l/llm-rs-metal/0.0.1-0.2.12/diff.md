# Comparing `tmp/llm-rs-metal-0.0.1.tar.gz` & `tmp/llm_rs_metal-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-rs-metal-0.0.1.tar", last modified: Wed Jun 21 15:26:15 2023, max compression
+gzip compressed data
```

## Comparing `llm-rs-metal-0.0.1.tar` & `llm_rs_metal-0.2.12.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.257988 llm-rs-metal-0.0.1/
--rw-rw-rw-   0        0        0      909 2023-06-21 14:29:35.000000 llm-rs-metal-0.0.1/Cargo.toml
--rw-rw-rw-   0        0        0     1092 2023-04-17 13:07:01.000000 llm-rs-metal-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       79 2023-06-21 14:32:42.000000 llm-rs-metal-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      684 2023-06-21 15:26:15.257988 llm-rs-metal-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5046 2023-06-21 14:29:35.000000 llm-rs-metal-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.239738 llm-rs-metal-0.0.1/llm_rs/
--rw-rw-rw-   0        0        0      342 2023-05-23 15:29:45.000000 llm-rs-metal-0.0.1/llm_rs/__init__.py
--rw-rw-rw-   0        0        0    17364 2023-06-21 14:29:35.000000 llm-rs-metal-0.0.1/llm_rs/auto.py
--rw-rw-rw-   0        0        0     2200 2023-06-08 13:07:31.000000 llm-rs-metal-0.0.1/llm_rs/base_model.py
--rw-rw-rw-   0        0        0     1452 2023-06-08 13:07:31.000000 llm-rs-metal-0.0.1/llm_rs/config.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.241845 llm-rs-metal-0.0.1/llm_rs/convert/
--rw-rw-rw-   0        0        0       79 2023-05-24 13:55:11.000000 llm-rs-metal-0.0.1/llm_rs/convert/__init__.py
--rw-rw-rw-   0        0        0     2284 2023-06-21 14:29:35.000000 llm-rs-metal-0.0.1/llm_rs/convert/auto_converter.py
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.245841 llm-rs-metal-0.0.1/llm_rs/convert/models/
--rw-rw-rw-   0        0        0      204 2023-06-19 14:25:35.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/__init__.py
--rw-rw-rw-   0        0        0     5974 2023-05-28 07:33:50.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/_base.py
--rw-rw-rw-   0        0        0     3250 2023-05-23 15:29:45.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/bloom.py
--rw-rw-rw-   0        0        0     5331 2023-05-24 07:58:26.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/gpt2.py
--rw-rw-rw-   0        0        0     2074 2023-05-29 08:48:25.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/gptj.py
--rw-rw-rw-   0        0        0     2178 2023-05-23 15:29:45.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/gptneox.py
--rw-rw-rw-   0        0        0     6472 2023-05-23 15:29:45.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/llama.py
--rw-rw-rw-   0        0        0     1928 2023-05-23 15:29:45.000000 llm-rs-metal-0.0.1/llm_rs/convert/models/mpt.py
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.246963 llm-rs-metal-0.0.1/llm_rs/haystack/
--rw-rw-rw-   0        0        0        0 2023-06-21 14:29:35.000000 llm-rs-metal-0.0.1/llm_rs/haystack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.247968 llm-rs-metal-0.0.1/llm_rs/langchain/
--rw-rw-rw-   0        0        0       37 2023-06-21 08:36:30.000000 llm-rs-metal-0.0.1/llm_rs/langchain/__init__.py
--rw-rw-rw-   0        0        0     4391 2023-06-21 08:36:30.000000 llm-rs-metal-0.0.1/llm_rs/langchain/langchain.py
--rw-rw-rw-   0        0        0        0 2023-05-03 15:04:02.000000 llm-rs-metal-0.0.1/llm_rs/llm_rs.pyi
--rw-rw-rw-   0        0        0      616 2023-05-23 15:29:45.000000 llm-rs-metal-0.0.1/llm_rs/models.pyi
--rw-rw-rw-   0        0        0        0 2023-05-03 15:04:02.000000 llm-rs-metal-0.0.1/llm_rs/py.typed
--rw-rw-rw-   0        0        0     2983 2023-05-24 13:18:32.000000 llm-rs-metal-0.0.1/llm_rs/repository.py
--rw-rw-rw-   0        0        0      727 2023-05-03 15:04:02.000000 llm-rs-metal-0.0.1/llm_rs/results.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.252477 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/
--rw-rw-rw-   0        0        0      684 2023-06-21 15:26:15.000000 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      945 2023-06-21 15:26:15.000000 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 15:26:15.000000 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 15:25:40.000000 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      168 2023-06-21 15:26:15.000000 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-21 15:26:15.000000 llm-rs-metal-0.0.1/llm_rs_metal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1003 2023-06-21 15:25:19.000000 llm-rs-metal-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 15:26:15.257988 llm-rs-metal-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-06-21 15:25:32.000000 llm-rs-metal-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 15:26:15.256988 llm-rs-metal-0.0.1/src/
--rw-rw-rw-   0        0        0     7664 2023-06-08 13:07:31.000000 llm-rs-metal-0.0.1/src/configs.rs
--rw-rw-rw-   0        0        0     1750 2023-05-28 06:42:29.000000 llm-rs-metal-0.0.1/src/lib.rs
--rw-rw-rw-   0        0        0    18395 2023-06-08 13:07:31.000000 llm-rs-metal-0.0.1/src/model_base.rs
--rw-rw-rw-   0        0        0      315 2023-05-27 12:22:55.000000 llm-rs-metal-0.0.1/src/models.rs
--rw-rw-rw-   0        0        0     3288 2023-06-21 14:29:35.000000 llm-rs-metal-0.0.1/src/quantize.rs
--rw-rw-rw-   0        0        0     1413 2023-05-15 12:57:25.000000 llm-rs-metal-0.0.1/src/results.rs
--rw-rw-rw-   0        0        0     1892 2023-06-08 13:07:31.000000 llm-rs-metal-0.0.1/src/stopwords.rs
+-rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 llm_rs_metal-0.2.12/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     3317 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/CI-CuBLAS.yml
+-rw-r--r--   0     1001      123     2136 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/CI-Metal.yml
+-rw-r--r--   0     1001      123     3124 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/CI-OpenCL.yml
+-rw-r--r--   0     1001      123     6258 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3477 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.gitignore
+-rw-r--r--   0     1001      123       72 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/LICENSE
+-rw-r--r--   0     1001      123     7164 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/README.md
+-rw-r--r--   0     1001      123      702 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/build_scripts/pyproject_patcher.py
+-rw-r--r--   0     1001      123     1016 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/build_scripts/repair_windows_wheels.py
+-rw-r--r--   0     1001      123       16 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/build_scripts/requirements.txt
+-rw-r--r--   0     1001      123     4799 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/docs/requirements.txt
+-rw-r--r--   0     1001      123      424 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/examples/haystack_example.py
+-rw-r--r--   0     1001      123      764 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/examples/langchain_example.py
+-rw-r--r--   0     1001      123      334 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/__init__.py
+-rw-r--r--   0     1001      123    17102 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/auto.py
+-rw-r--r--   0     1001      123     2129 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1728 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2305 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5820 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123       48 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/haystack/__init__.py
+-rw-r--r--   0     1001      123     4878 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/haystack/haystack.py
+-rw-r--r--   0     1001      123       37 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/langchain/__init__.py
+-rw-r--r--   0     1001      123     4268 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/langchain/langchain.py
+-rw-r--r--   0     1001      123        0 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/py.typed
+-rw-r--r--   0     1001      123     2915 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/repository.py
+-rw-r--r--   0     1001      123      697 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/llm_rs/results.pyi
+-rw-r--r--   0     1001      123     1030 2023-06-27 13:32:16.000000 llm_rs_metal-0.2.12/pyproject.toml
+-rw-r--r--   0     1001      123     7863 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/configs.rs
+-rw-r--r--   0     1001      123     1700 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/lib.rs
+-rw-r--r--   0     1001      123    17963 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/models.rs
+-rw-r--r--   0     1001      123     3190 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/results.rs
+-rw-r--r--   0     1001      123     1821 2023-06-27 13:32:14.000000 llm_rs_metal-0.2.12/src/stopwords.rs
+-rw-r--r--   0     1001      123    62531 2023-06-27 13:32:25.000000 llm_rs_metal-0.2.12/Cargo.lock
+-rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 llm_rs_metal-0.2.12/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `llm-rs-metal-0.0.1/Cargo.toml` & `llm_rs_metal-0.2.12/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-00000000: 5b70 6163 6b61 6765 5d0d 0a6e 616d 6520  [package]..name 
-00000010: 3d20 226c 6c6d 2d72 7322 0d0a 7665 7273  = "llm-rs"..vers
-00000020: 696f 6e20 3d20 2230 2e32 2e31 3022 0d0a  ion = "0.2.10"..
-00000030: 6564 6974 696f 6e20 3d20 2232 3032 3122  edition = "2021"
-00000040: 0d0a 0d0a 2320 5365 6520 6d6f 7265 206b  ....# See more k
-00000050: 6579 7320 616e 6420 7468 6569 7220 6465  eys and their de
-00000060: 6669 6e69 7469 6f6e 7320 6174 2068 7474  finitions at htt
-00000070: 7073 3a2f 2f64 6f63 2e72 7573 742d 6c61  ps://doc.rust-la
-00000080: 6e67 2e6f 7267 2f63 6172 676f 2f72 6566  ng.org/cargo/ref
-00000090: 6572 656e 6365 2f6d 616e 6966 6573 742e  erence/manifest.
-000000a0: 6874 6d6c 0d0a 5b6c 6962 5d0d 0a6e 616d  html..[lib]..nam
-000000b0: 6520 3d20 226c 6c6d 5f72 7322 0d0a 6372  e = "llm_rs"..cr
-000000c0: 6174 652d 7479 7065 203d 205b 2263 6479  ate-type = ["cdy
-000000d0: 6c69 6222 5d0d 0a0d 0a5b 6465 7065 6e64  lib"]....[depend
-000000e0: 656e 6369 6573 5d0d 0a72 616e 6420 3d20  encies]..rand = 
-000000f0: 2230 2e38 2e35 220d 0a72 616e 645f 6368  "0.8.5"..rand_ch
-00000100: 6163 6861 203d 2022 302e 332e 3122 0d0a  acha = "0.3.1"..
-00000110: 6c6f 6720 203d 2020 2230 2e34 2e31 3722  log  =  "0.4.17"
-00000120: 0d0a 7365 7264 6520 3d20 2231 2e30 2e31  ..serde = "1.0.1
-00000130: 3633 220d 0a73 6572 6465 5f6a 736f 6e20  63"..serde_json 
-00000140: 3d20 2231 2e30 220d 0a6c 6c6d 203d 207b  = "1.0"..llm = {
-00000150: 2067 6974 203d 2022 6874 7470 733a 2f2f   git = "https://
-00000160: 6769 7468 7562 2e63 6f6d 2f72 7573 7466  github.com/rustf
-00000170: 6f72 6d65 7273 2f6c 6c6d 2e67 6974 222c  ormers/llm.git",
-00000180: 2072 6576 3d22 3362 6563 6437 3222 2020   rev="3becd72"  
-00000190: 7d0d 0a6c 6c6d 2d62 6173 6520 3d20 7b20  }..llm-base = { 
-000001a0: 6769 7420 3d20 2268 7474 7073 3a2f 2f67  git = "https://g
-000001b0: 6974 6875 622e 636f 6d2f 7275 7374 666f  ithub.com/rustfo
-000001c0: 726d 6572 732f 6c6c 6d2e 6769 7422 2c72  rmers/llm.git",r
-000001d0: 6576 3d22 3362 6563 6437 3222 207d 0d0a  ev="3becd72" }..
-000001e0: 0d0a 5b64 6570 656e 6465 6e63 6965 732e  ..[dependencies.
-000001f0: 7079 6f33 5d0d 0a76 6572 7369 6f6e 203d  pyo3]..version =
-00000200: 2022 302e 3139 2e30 220d 0a23 2022 6162   "0.19.0"..# "ab
-00000210: 6933 2d70 7933 3722 2074 656c 6c73 2070  i3-py37" tells p
-00000220: 796f 3320 2861 6e64 206d 6174 7572 696e  yo3 (and maturin
-00000230: 2920 746f 2062 7569 6c64 2075 7369 6e67  ) to build using
-00000240: 2074 6865 2073 7461 626c 6520 4142 4920   the stable ABI 
-00000250: 7769 7468 0d0a 2320 5079 7468 6f6e 2033  with..# Python 3
-00000260: 2e37 206f 7220 6c61 7465 722e 0d0a 6665  .7 or later...fe
-00000270: 6174 7572 6573 203d 205b 2261 6269 332d  atures = ["abi3-
-00000280: 7079 3337 222c 2265 7874 656e 7369 6f6e  py37","extension
-00000290: 2d6d 6f64 756c 6522 2c20 2267 656e 6572  -module", "gener
-000002a0: 6174 652d 696d 706f 7274 2d6c 6962 225d  ate-import-lib"]
-000002b0: 0d0a 0d0a 5b66 6561 7475 7265 735d 0d0a  ....[features]..
-000002c0: 6375 626c 6173 203d 205b 226c 6c6d 2f63  cublas = ["llm/c
-000002d0: 7562 6c61 7322 2c20 226c 6c6d 2d62 6173  ublas", "llm-bas
-000002e0: 652f 6375 626c 6173 225d 0d0a 636c 626c  e/cublas"]..clbl
-000002f0: 6173 7420 3d20 5b22 6c6c 6d2f 636c 626c  ast = ["llm/clbl
-00000300: 6173 7422 2c20 226c 6c6d 2d62 6173 652f  ast", "llm-base/
-00000310: 636c 626c 6173 7422 5d0d 0a6d 6574 616c  clblast"]..metal
-00000320: 203d 205b 226c 6c6d 2f6d 6574 616c 222c   = ["llm/metal",
-00000330: 2022 6c6c 6d2d 6261 7365 2f6d 6574 616c   "llm-base/metal
-00000340: 225d 0d0a 0d0a 5b70 6163 6b61 6765 2e6d  "]....[package.m
-00000350: 6574 6164 6174 612e 6d61 7475 7269 6e5d  etadata.maturin]
-00000360: 0d0a 6665 6174 7572 6573 203d 205b 2263  ..features = ["c
-00000370: 7562 6c61 7322 2c20 2263 6c62 6c61 7374  ublas", "clblast
-00000380: 222c 2022 6d65 7461 6c22 5d0d 0a         ", "metal"]..
+00000000: 5b70 6163 6b61 6765 5d0a 6e61 6d65 203d  [package].name =
+00000010: 2022 6c6c 6d2d 7273 220a 7665 7273 696f   "llm-rs".versio
+00000020: 6e20 3d20 2230 2e32 2e31 3222 0a65 6469  n = "0.2.12".edi
+00000030: 7469 6f6e 203d 2022 3230 3231 220a 0a23  tion = "2021"..#
+00000040: 2053 6565 206d 6f72 6520 6b65 7973 2061   See more keys a
+00000050: 6e64 2074 6865 6972 2064 6566 696e 6974  nd their definit
+00000060: 696f 6e73 2061 7420 6874 7470 733a 2f2f  ions at https://
+00000070: 646f 632e 7275 7374 2d6c 616e 672e 6f72  doc.rust-lang.or
+00000080: 672f 6361 7267 6f2f 7265 6665 7265 6e63  g/cargo/referenc
+00000090: 652f 6d61 6e69 6665 7374 2e68 746d 6c0a  e/manifest.html.
+000000a0: 5b6c 6962 5d0a 6e61 6d65 203d 2022 6c6c  [lib].name = "ll
+000000b0: 6d5f 7273 220a 6372 6174 652d 7479 7065  m_rs".crate-type
+000000c0: 203d 205b 2263 6479 6c69 6222 5d0a 0a5b   = ["cdylib"]..[
+000000d0: 6465 7065 6e64 656e 6369 6573 5d0a 7261  dependencies].ra
+000000e0: 6e64 203d 2022 302e 382e 3522 0a72 616e  nd = "0.8.5".ran
+000000f0: 645f 6368 6163 6861 203d 2022 302e 332e  d_chacha = "0.3.
+00000100: 3122 0a6c 6f67 2020 3d20 2022 302e 342e  1".log  =  "0.4.
+00000110: 3137 220a 7365 7264 6520 3d20 2231 2e30  17".serde = "1.0
+00000120: 2e31 3633 220a 7365 7264 655f 6a73 6f6e  .163".serde_json
+00000130: 203d 2022 312e 3022 0a0a 6c6c 6d20 3d20   = "1.0"..llm = 
+00000140: 7b20 6769 7420 3d20 2268 7474 7073 3a2f  { git = "https:/
+00000150: 2f67 6974 6875 622e 636f 6d2f 4c4c 756b  /github.com/LLuk
+00000160: 6173 3232 2f6c 6c6d 2e67 6974 222c 2062  as22/llm.git", b
+00000170: 7261 6e63 6820 3d20 2266 6561 742f 6375  ranch = "feat/cu
+00000180: 6461 2d6f 7065 6e63 6c2d 6163 6365 6c65  da-opencl-accele
+00000190: 7261 7469 6f6e 2220 207d 0a6c 6c6d 2d62  ration"  }.llm-b
+000001a0: 6173 6520 3d20 7b20 6769 7420 3d20 2268  ase = { git = "h
+000001b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001c0: 6d2f 4c4c 756b 6173 3232 2f6c 6c6d 2e67  m/LLukas22/llm.g
+000001d0: 6974 222c 2062 7261 6e63 6820 3d20 2266  it", branch = "f
+000001e0: 6561 742f 6375 6461 2d6f 7065 6e63 6c2d  eat/cuda-opencl-
+000001f0: 6163 6365 6c65 7261 7469 6f6e 2220 7d0a  acceleration" }.
+00000200: 0a5b 6465 7065 6e64 656e 6369 6573 2e70  .[dependencies.p
+00000210: 796f 335d 0a76 6572 7369 6f6e 203d 2022  yo3].version = "
+00000220: 302e 3139 2e30 220a 2320 2261 6269 332d  0.19.0".# "abi3-
+00000230: 7079 3337 2220 7465 6c6c 7320 7079 6f33  py37" tells pyo3
+00000240: 2028 616e 6420 6d61 7475 7269 6e29 2074   (and maturin) t
+00000250: 6f20 6275 696c 6420 7573 696e 6720 7468  o build using th
+00000260: 6520 7374 6162 6c65 2041 4249 2077 6974  e stable ABI wit
+00000270: 680a 2320 5079 7468 6f6e 2033 2e37 206f  h.# Python 3.7 o
+00000280: 7220 6c61 7465 722e 0a66 6561 7475 7265  r later..feature
+00000290: 7320 3d20 5b22 6162 6933 2d70 7933 3722  s = ["abi3-py37"
+000002a0: 2c22 6578 7465 6e73 696f 6e2d 6d6f 6475  ,"extension-modu
+000002b0: 6c65 222c 2022 6765 6e65 7261 7465 2d69  le", "generate-i
+000002c0: 6d70 6f72 742d 6c69 6222 5d0a 0a5b 6665  mport-lib"]..[fe
+000002d0: 6174 7572 6573 5d0a 6375 626c 6173 203d  atures].cublas =
+000002e0: 205b 226c 6c6d 2f63 7562 6c61 7322 2c20   ["llm/cublas", 
+000002f0: 226c 6c6d 2d62 6173 652f 6375 626c 6173  "llm-base/cublas
+00000300: 225d 0a63 6c62 6c61 7374 203d 205b 226c  "].clblast = ["l
+00000310: 6c6d 2f63 6c62 6c61 7374 222c 2022 6c6c  lm/clblast", "ll
+00000320: 6d2d 6261 7365 2f63 6c62 6c61 7374 225d  m-base/clblast"]
+00000330: 0a6d 6574 616c 203d 205b 226c 6c6d 2f6d  .metal = ["llm/m
+00000340: 6574 616c 222c 2022 6c6c 6d2d 6261 7365  etal", "llm-base
+00000350: 2f6d 6574 616c 225d 0a0a                 /metal"]..
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/auto.py` & `llm_rs_metal-0.2.12/llm_rs/auto.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,423 +1,427 @@
-from .config import QuantizationType,ContainerType,SessionConfig
-import os
-import pathlib
-from .models import Mpt,GptNeoX,GptJ,Gpt2,Bloom,Llama
-from .base_model import Model
-import logging
-from typing import Optional, List, Union,Type,Dict, Callable
-import os
-from enum import Enum, auto
-from dataclasses import dataclass
-import json
-from blake3 import blake3
-from huggingface_hub import snapshot_download
-from huggingface_hub.utils import validate_repo_id, HFValidationError
-from huggingface_hub import cached_assets_path
-
-class QuantizationVersions(Enum):
-    Not_Quantized=auto()
-    V1=auto()
-    V2=auto()
-
-class KnownModels(Enum):
-    GptNeoX = auto()
-    Mpt = auto()
-    GptJ = auto()
-    Gpt2 = auto()
-    Bloom = auto()
-    Llama = auto()
-
-
-_QUANTIZATION_TYPE_MAP = {
-    "Q4_0": QuantizationType.Q4_0,
-    "Q4_1": QuantizationType.Q4_1,
-    "Q5_0": QuantizationType.Q5_0,
-    "Q5_1": QuantizationType.Q5_1,
-    "Q8_0": QuantizationType.Q8_0,
-    "F16": QuantizationType.F16
-}
-
-_CONTAINER_TYPE_MAP = {
-    "GGML": ContainerType.GGML,
-    "GGJT": ContainerType.GGJT
-}
-
-_KNOWN_MODELS_MAP = {
-    KnownModels.GptNeoX: GptNeoX,
-    KnownModels.Mpt: Mpt,
-    KnownModels.GptJ: GptJ,
-    KnownModels.Gpt2: Gpt2,
-    KnownModels.Bloom: Bloom,
-    KnownModels.Llama: Llama
-}
-
-CURRENT_QUANTIZATION_VERSION = QuantizationVersions.V2
-
-class PathType(Enum):
-    DIR = auto()
-    FILE = auto()
-    REPO = auto()
-    UNKNOWN = auto() 
-
-def _get_path_type(path: Union[str,os.PathLike]) -> PathType:
-    p = pathlib.Path(path)
-    if p.is_file():
-        return PathType.FILE
-    elif p.is_dir():
-        return PathType.DIR
-    try:
-        validate_repo_id(str(path))
-        return PathType.REPO
-    except HFValidationError:
-        pass
-    return PathType.UNKNOWN
-
-
-@dataclass()
-class ModelMetadata():
-    """
-    A dataclass to store metadata about a model.
-    """
-    model: KnownModels
-    quantization: QuantizationType
-    container: ContainerType
-    quantization_version: QuantizationVersions=QuantizationVersions.Not_Quantized
-    converter:str="llm-rs"
-    hash:Optional[str]=None
-    base_model:Optional[str]=None
-
-    def add_hash(self,model_path:Union[str,os.PathLike]):
-        h  = blake3(max_threads=blake3.AUTO)
-        b  = bytearray(128_000_000)
-        mv = memoryview(b)
-        with open(model_path, 'rb', buffering=0) as f:
-            for n in iter(lambda : f.readinto(mv), 0):
-                h.update(mv[:n])
-        self.hash=h.hexdigest()
-
-    def serialize(self):
-        return {
-            "model": self.model.name,
-            "quantization": repr(self.quantization).split(".")[-1],
-            "quantization_version": self.quantization_version.name,
-            "container": repr(self.container).split(".")[-1],
-            "converter": self.converter,
-            "hash": self.hash,
-            "base_model": self.base_model
-        }
-    
-    @staticmethod
-    def deserialize(metadata_dict:Dict[str,str])->"ModelMetadata":
-        return ModelMetadata(
-            model = KnownModels[metadata_dict["model"]],
-            quantization = _QUANTIZATION_TYPE_MAP[metadata_dict["quantization"]],
-            quantization_version= QuantizationVersions[metadata_dict["quantization_version"]],
-            container = _CONTAINER_TYPE_MAP[metadata_dict["container"]],
-            converter = metadata_dict["converter"],
-            hash = metadata_dict.get("hash"),
-            base_model = metadata_dict.get("base_model")
-        )
-
-
-@dataclass
-class AutoConfig():
-    repo_type:Optional[str] = None
-    model_type: Optional[str] = None
-
-    @classmethod
-    def from_pretrained(
-        cls,
-        model_path_or_repo_id: Union[str, os.PathLike],
-        **kwargs,
-    ) -> 'AutoConfig':
-        path_type = _get_path_type(model_path_or_repo_id)
-        if path_type == PathType.UNKNOWN:
-            raise ValueError(
-                f"Model path '{model_path_or_repo_id}' doesn't exist.")
-        elif path_type == PathType.FILE:
-            raise ValueError(
-                f"Model path '{model_path_or_repo_id}' is a file. "
-                "Please provide a directory or a repo id.")
-        
-        auto_config = AutoConfig()
-        if path_type == PathType.DIR:
-            cls._update_from_dir(str(model_path_or_repo_id), auto_config)
-        elif path_type == PathType.REPO:
-            cls._update_from_repo(str(model_path_or_repo_id), auto_config)
-
-        return auto_config
-
-    @classmethod
-    def _update_from_repo(
-        cls,
-        repo_id: str,
-        auto_config: 'AutoConfig',
-    ) -> None:
-        path = snapshot_download(repo_id=repo_id, allow_patterns='config.json')
-        cls._update_from_dir(path, auto_config)
-
-    @classmethod
-    def _update_from_dir(cls, path: str, auto_config: 'AutoConfig') -> None:
-        resolved_path = (pathlib.Path(path) / 'config.json').resolve()
-        if resolved_path.is_file():
-            cls._update_from_file(str(resolved_path), auto_config)
-        else:
-            raise ValueError(f"Config path '{resolved_path}' doesn't exist.")
-
-    @classmethod
-    def _update_from_file(cls, path: str, auto_config: 'AutoConfig') -> None:
-        with open(path) as f:
-            config = json.load(f)
-        auto_config.model_type = config.get('model_type')
-        auto_config.repo_type = config.get('repo_type')
-
-class AutoModel():
-    """
-    Utility to load models, without having to specify the model type.
-    """
-    @classmethod
-    def load_metadata(cls,model_file:Union[str,os.PathLike])->ModelMetadata:
-        path = pathlib.Path(model_file)
-        if not path.is_file():
-            raise ValueError(f"Model file '{model_file}' is not a file!")
-        if not path.exists():
-            raise ValueError(f"Model file '{model_file}' does not exist!")
-
-        metadata_file = path.with_suffix(".meta")
-        if not metadata_file.exists():
-            raise ValueError(f"Model file '{model_file}' does not have a metadata file '{metadata_file}'! If you want to autoload this model, please specify the model type.")
-        
-        metadata = ModelMetadata.deserialize(json.loads(metadata_file.read_text()))
-        return metadata
-    
-    @classmethod
-    def _infer_model_type(cls,model_file:Union[str,os.PathLike],known_model:Optional[KnownModels]=None)->Type[Model]:
-        model_to_lookup = None
-        if known_model:
-            model_to_lookup = known_model
-        else:
-            metadata = cls.load_metadata(model_file)
-            model_to_lookup = metadata.model
-
-        if model_to_lookup in _KNOWN_MODELS_MAP:
-            return _KNOWN_MODELS_MAP[model_to_lookup]
-        else:
-            raise ValueError(f"Unknown model type '{model_to_lookup}'")
-            
-        
-    @classmethod
-    def from_file(cls, path:Union[str,os.PathLike],
-                  model_type: Optional[KnownModels] = None,
-                  session_config:SessionConfig=SessionConfig(),
-                  tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
-                  lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
-                  verbose:bool=False,
-                  use_hf_tokenizer:bool=True)->Model:
-        
-        tokenizer = tokenizer_path_or_repo_id
-        if use_hf_tokenizer and tokenizer is None:
-            metadata = cls.load_metadata(path)
-            tokenizer = metadata.base_model
-            if tokenizer is None or tokenizer == "":
-                raise ValueError(f"Model file '{path}' does not have a base_model specified in its metadata file but wants to use a huggingface-tokenizer! Please specify a base_model or expilicitly specify a tokenizer via `tokenizer_path_or_repo_id`.")
-
-        model = cls._infer_model_type(path,model_type)
-        return model(path,session_config,tokenizer_path_or_repo_id,lora_paths,verbose)
-    
-    @classmethod
-    def from_pretrained(cls,
-        model_path_or_repo_id: Union[str,os.PathLike],
-        model_file: Optional[str] = None,
-        model_type: Optional[KnownModels] = None,
-        session_config:SessionConfig=SessionConfig(),
-        tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
-        lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
-        verbose:bool=False,
-        use_hf_tokenizer:bool=True,
-        default_quantization:QuantizationType=QuantizationType.Q4_0,
-        default_container:ContainerType=ContainerType.GGJT)->Model:
-
-        path_type = _get_path_type(model_path_or_repo_id)
-
-        if path_type == PathType.UNKNOWN:
-            raise ValueError(f"Unknown path type for '{model_path_or_repo_id}'")
-        elif path_type == PathType.FILE:
-            return cls.from_file(model_path_or_repo_id,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
-        else:
-            if path_type == PathType.REPO:
-
-                try: 
-                    config = AutoConfig.from_pretrained(
-                        model_path_or_repo_id,
-                    )
-                except ValueError:
-                    logging.warning("Could not find config.json in repo, assuming GGML model...")
-                    config = AutoConfig(repo_type="GGML")
-                       
-
-                if config.repo_type != "GGML":
-                    logging.warning("Found normal HuggingFace model, starting conversion...")
-                    return cls.from_transformer(model_path_or_repo_id, session_config, tokenizer_path_or_repo_id, lora_paths, verbose, use_hf_tokenizer,default_quantization, default_container)
-            
-                resolved_path = cls._find_model_path_from_repo(str(model_path_or_repo_id),model_file)
-                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
-            
-            elif path_type == PathType.DIR:
-                resolved_path = cls._find_model_path_from_dir(str(model_path_or_repo_id),model_file)
-                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
-            
-            else:
-                raise ValueError(f"Unknown path type '{path_type}'")
-
-
-    @classmethod
-    def _find_model_path_from_dir(
-        cls,
-        directory: str,
-        filename: Optional[str] = None,
-    ) -> str:
-        path = pathlib.Path(directory).resolve()
-        if filename:
-            file = (path / filename)
-            if not file.is_file():
-                raise ValueError(
-                    f"Model file '{filename}' not found in '{path}'")
-            return str(file)
-
-        files = [
-            f for f in path.iterdir()
-            if f.is_file() and f.name.endswith('.bin')
-        ]
-
-        if len(files) == 0:
-            raise ValueError(f"No model files found in '{path}'")
-        elif len(files) > 1:
-            raise ValueError(
-                f"Multiple model files found in '{path}'! Please specify one of the following model files to load: '{','.join([f.name for f in files])}'"
-            )
-
-        return str(files[0].resolve())
-    
-    @classmethod
-    def _find_model_path_from_repo(
-        cls,
-        repo_id: str,
-        filename: Optional[str] = None,
-    ) -> str:
-        cache_directory = cached_assets_path("llm-rs",namespace=repo_id)
-        #we dont want to download the whole repo, just the metadata
-        directory = snapshot_download(repo_id=repo_id,
-                                allow_patterns='*.meta',
-                                local_dir=cache_directory)
-        path = pathlib.Path(directory).resolve()
-        files = [
-            f for f in path.iterdir()
-            if f.is_file() and f.name.endswith('.meta')
-        ]
-
-        if len(files) == 0 and filename is None:
-            raise ValueError(f"No model files found in '{repo_id}'! Either specify the model file via the `model_file` parameter or make sure the repository contains a *.meta files for each model.")
-        if len(files) > 1 and filename is None:
-            raise ValueError(
-                f"Multiple model files found in '{repo_id}'! Please specify one of the following model files to load: '{','.join([f.name.replace('.meta','.bin') for f in files])}' "
-            )
-        #if we have a filename, we can just download that file
-        filename = filename if filename else files[0].name.replace('.meta','.bin')
-        model_directory = snapshot_download(repo_id=repo_id,
-                                allow_patterns=filename,
-                                local_dir=cache_directory)
-        
-        return cls._find_model_path_from_dir(model_directory, filename=filename)
-    
-    @classmethod
-    def from_transformer(cls,
-        model_path_or_repo_id: Union[str,os.PathLike],
-        session_config:SessionConfig=SessionConfig(),
-        tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
-        lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
-        verbose:bool=False,
-        use_hf_tokenizer:bool=True,
-        default_quantization:QuantizationType=QuantizationType.Q4_0,
-        default_container:ContainerType=ContainerType.GGJT):
-        
-        try:
-            from .convert import AutoConverter
-            from .convert.auto_converter import get_name_from_config
-            from transformers import AutoConfig
-        except ImportError:
-            raise ImportError("Model conversion needs additional dependencies. Please install 'llm-rs[convert]' to use this functionality!")
-        
-
-        config = AutoConfig.from_pretrained(model_path_or_repo_id,trust_remote_code=True)
-        model_name = get_name_from_config(config)
-        export_path = cached_assets_path("llm-rs",namespace=model_name)
-        converted_model = AutoConverter.convert(model_path_or_repo_id,export_path)
-        if default_quantization != QuantizationType.F16:
-            converted_model = AutoQuantizer.quantize(converted_model,quantization=default_quantization,container=default_container)
-        return cls.from_file(converted_model,None,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
-    
-# Hack to make the quantization type enum hashable
-_APPENDIX_MAP = {
-    QuantizationType.Q4_0.__repr__(): "q4_0",
-    QuantizationType.Q4_1.__repr__(): "q4_1",
-    QuantizationType.Q5_0.__repr__(): "q5_0",
-    QuantizationType.Q5_1.__repr__(): "q5_1",
-    QuantizationType.Q8_0.__repr__(): "q8_0",
-}
-
-class AutoQuantizer():
-    """
-    Utility to quantize models, without having to specify the model type.
-    """
-    @staticmethod
-    def quantize(
-        model_file:Union[str,os.PathLike],
-        target_path:Optional[Union[str,os.PathLike]]=None,
-        quantization:QuantizationType=QuantizationType.Q4_0,
-        container:ContainerType=ContainerType.GGJT,
-        callback:Optional[Callable[[str],None]]=None
-        )->Union[str,os.PathLike]:
-        metadata=AutoModel.load_metadata(model_file)
-        if metadata.quantization != QuantizationType.F16:
-            raise ValueError(f"Model '{model_file}' is already quantized to '{metadata.quantization}'")
-
-        model_type = AutoModel._infer_model_type(model_file)
-
-        if target_path is None:
-            target_path = os.path.dirname(model_file)
-            
-        def build_target_name()->str:
-            output_path = pathlib.Path(target_path)
-            if output_path.is_file():
-                return str(output_path)
-            else:
-                output_path.mkdir(parents=True,exist_ok=True)
-                model_path = pathlib.Path(model_file)
-                appendix = ""
-
-                if quantization.__repr__() in _APPENDIX_MAP:
-                    appendix += f"-{_APPENDIX_MAP[quantization.__repr__()]}"
-
-                if container == ContainerType.GGJT:
-                    appendix += "-ggjt"
-            
-                filename = model_path.stem.replace("-f16","") + appendix + model_path.suffix
-                return str(output_path / filename)
-
-        target_file = build_target_name()
-        if pathlib.Path(target_file).exists():
-            logging.warning(f"Target file '{target_file}' already exists, skipping quantization")
-            return target_file
-        
-        logging.info(f"Quantizing model '{model_file}' to '{target_file}'")
-        model_type.quantize(str(model_file),target_file,quantization,container,callback=callback)
-
-        metadata_file = pathlib.Path(target_file).with_suffix(".meta")
-        quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=CURRENT_QUANTIZATION_VERSION,base_model=metadata.base_model)
-        quantized_metadata.add_hash(target_file)
-        logging.info(f"Writing metadata file '{metadata_file}'")
-        metadata_file.write_text(json.dumps(quantized_metadata.serialize(),indent=4))
-        logging.info(f"Finished quantizing model '{model_file}' to '{target_file}'")
-        return target_file
-
-
+from .config import QuantizationType,ContainerType,SessionConfig
+import os
+import pathlib
+from .models import Mpt,GptNeoX,GptJ,Gpt2,Bloom,Llama
+from .base_model import Model
+import logging
+from typing import Optional, List, Union,Type,Dict, Callable
+import os
+from enum import Enum, auto
+from dataclasses import dataclass
+import json
+from blake3 import blake3
+from huggingface_hub import snapshot_download
+from huggingface_hub.utils import validate_repo_id, HFValidationError
+from huggingface_hub import cached_assets_path
+
+class QuantizationVersions(Enum):
+    Not_Quantized=auto()
+    V1=auto()
+    V2=auto()
+
+class KnownModels(Enum):
+    GptNeoX = auto()
+    Mpt = auto()
+    GptJ = auto()
+    Gpt2 = auto()
+    Bloom = auto()
+    Llama = auto()
+
+
+_QUANTIZATION_TYPE_MAP = {
+    "Q4_0": QuantizationType.Q4_0,
+    "Q4_1": QuantizationType.Q4_1,
+    "Q5_0": QuantizationType.Q5_0,
+    "Q5_1": QuantizationType.Q5_1,
+    "Q8_0": QuantizationType.Q8_0,
+    "F16": QuantizationType.F16
+}
+
+_CONTAINER_TYPE_MAP = {
+    "GGML": ContainerType.GGML,
+    "GGJT": ContainerType.GGJT
+}
+
+_KNOWN_MODELS_MAP = {
+    KnownModels.GptNeoX: GptNeoX,
+    KnownModels.Mpt: Mpt,
+    KnownModels.GptJ: GptJ,
+    KnownModels.Gpt2: Gpt2,
+    KnownModels.Bloom: Bloom,
+    KnownModels.Llama: Llama
+}
+
+CURRENT_QUANTIZATION_VERSION = QuantizationVersions.V2
+
+class PathType(Enum):
+    DIR = auto()
+    FILE = auto()
+    REPO = auto()
+    UNKNOWN = auto() 
+
+def _get_path_type(path: Union[str,os.PathLike]) -> PathType:
+    p = pathlib.Path(path)
+    if p.is_file():
+        return PathType.FILE
+    elif p.is_dir():
+        return PathType.DIR
+    try:
+        validate_repo_id(str(path))
+        return PathType.REPO
+    except HFValidationError:
+        pass
+    return PathType.UNKNOWN
+
+
+@dataclass()
+class ModelMetadata():
+    """
+    A dataclass to store metadata about a model.
+    """
+    model: KnownModels
+    quantization: QuantizationType
+    container: ContainerType
+    quantization_version: QuantizationVersions=QuantizationVersions.Not_Quantized
+    converter:str="llm-rs"
+    hash:Optional[str]=None
+    base_model:Optional[str]=None
+
+    def add_hash(self,model_path:Union[str,os.PathLike]):
+        h  = blake3(max_threads=blake3.AUTO)
+        b  = bytearray(128_000_000)
+        mv = memoryview(b)
+        with open(model_path, 'rb', buffering=0) as f:
+            for n in iter(lambda : f.readinto(mv), 0):
+                h.update(mv[:n])
+        self.hash=h.hexdigest()
+
+    def serialize(self):
+        return {
+            "model": self.model.name,
+            "quantization": repr(self.quantization).split(".")[-1],
+            "quantization_version": self.quantization_version.name,
+            "container": repr(self.container).split(".")[-1],
+            "converter": self.converter,
+            "hash": self.hash,
+            "base_model": self.base_model
+        }
+    
+    @staticmethod
+    def deserialize(metadata_dict:Dict[str,str])->"ModelMetadata":
+        return ModelMetadata(
+            model = KnownModels[metadata_dict["model"]],
+            quantization = _QUANTIZATION_TYPE_MAP[metadata_dict["quantization"]],
+            quantization_version= QuantizationVersions[metadata_dict["quantization_version"]],
+            container = _CONTAINER_TYPE_MAP[metadata_dict["container"]],
+            converter = metadata_dict["converter"],
+            hash = metadata_dict.get("hash"),
+            base_model = metadata_dict.get("base_model")
+        )
+
+
+@dataclass
+class AutoConfig():
+    repo_type:Optional[str] = None
+    model_type: Optional[str] = None
+
+    @classmethod
+    def from_pretrained(
+        cls,
+        model_path_or_repo_id: Union[str, os.PathLike],
+        **kwargs,
+    ) -> 'AutoConfig':
+        path_type = _get_path_type(model_path_or_repo_id)
+        if path_type == PathType.UNKNOWN:
+            raise ValueError(
+                f"Model path '{model_path_or_repo_id}' doesn't exist.")
+        elif path_type == PathType.FILE:
+            raise ValueError(
+                f"Model path '{model_path_or_repo_id}' is a file. "
+                "Please provide a directory or a repo id.")
+        
+        auto_config = AutoConfig()
+        if path_type == PathType.DIR:
+            cls._update_from_dir(str(model_path_or_repo_id), auto_config)
+        elif path_type == PathType.REPO:
+            cls._update_from_repo(str(model_path_or_repo_id), auto_config)
+
+        return auto_config
+
+    @classmethod
+    def _update_from_repo(
+        cls,
+        repo_id: str,
+        auto_config: 'AutoConfig',
+    ) -> None:
+        path = snapshot_download(repo_id=repo_id, allow_patterns='config.json')
+        cls._update_from_dir(path, auto_config)
+
+    @classmethod
+    def _update_from_dir(cls, path: str, auto_config: 'AutoConfig') -> None:
+        resolved_path = (pathlib.Path(path) / 'config.json').resolve()
+        if resolved_path.is_file():
+            cls._update_from_file(str(resolved_path), auto_config)
+        else:
+            raise ValueError(f"Config path '{resolved_path}' doesn't exist.")
+
+    @classmethod
+    def _update_from_file(cls, path: str, auto_config: 'AutoConfig') -> None:
+        with open(path) as f:
+            config = json.load(f)
+        auto_config.model_type = config.get('model_type')
+        auto_config.repo_type = config.get('repo_type')
+
+class AutoModel():
+    """
+    Utility to load models, without having to specify the model type.
+    """
+    @classmethod
+    def load_metadata(cls,model_file:Union[str,os.PathLike])->ModelMetadata:
+        path = pathlib.Path(model_file)
+        if not path.is_file():
+            raise ValueError(f"Model file '{model_file}' is not a file!")
+        if not path.exists():
+            raise ValueError(f"Model file '{model_file}' does not exist!")
+
+        metadata_file = path.with_suffix(".meta")
+        if not metadata_file.exists():
+            raise ValueError(f"Model file '{model_file}' does not have a metadata file '{metadata_file}'! If you want to autoload this model, please specify the model type.")
+        
+        metadata = ModelMetadata.deserialize(json.loads(metadata_file.read_text()))
+        return metadata
+    
+    @classmethod
+    def _infer_model_type(cls,model_file:Union[str,os.PathLike],known_model:Optional[KnownModels]=None)->Type[Model]:
+        model_to_lookup = None
+        if known_model:
+            model_to_lookup = known_model
+        else:
+            metadata = cls.load_metadata(model_file)
+            model_to_lookup = metadata.model
+
+        if model_to_lookup in _KNOWN_MODELS_MAP:
+            return _KNOWN_MODELS_MAP[model_to_lookup]
+        else:
+            raise ValueError(f"Unknown model type '{model_to_lookup}'")
+            
+        
+    @classmethod
+    def from_file(cls, path:Union[str,os.PathLike],
+                  model_type: Optional[KnownModels] = None,
+                  session_config:SessionConfig=SessionConfig(),
+                  tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
+                  lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
+                  verbose:bool=False,
+                  use_hf_tokenizer:bool=True)->Model:
+        
+        tokenizer = tokenizer_path_or_repo_id
+        if use_hf_tokenizer and tokenizer is None:
+            try:
+                metadata = cls.load_metadata(path)
+                tokenizer = metadata.base_model
+            except Exception as e:
+                logging.warning(f"Could not load metadata for model '{path}'!")
+
+            if tokenizer is None or tokenizer == "":
+                logging.warning(f"Model file '{path}' does not have a base_model specified in its metadata file but wants to use a huggingface-tokenizer! Please expilicitly specify a tokenizer via `tokenizer_path_or_repo_id` if you intend to use a huggingface-tokenizer.")
+
+        model = cls._infer_model_type(path,model_type)
+        return model(path,session_config,tokenizer_path_or_repo_id,lora_paths,verbose)
+    
+    @classmethod
+    def from_pretrained(cls,
+        model_path_or_repo_id: Union[str,os.PathLike],
+        model_file: Optional[str] = None,
+        model_type: Optional[KnownModels] = None,
+        session_config:SessionConfig=SessionConfig(),
+        tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
+        lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
+        verbose:bool=False,
+        use_hf_tokenizer:bool=True,
+        default_quantization:QuantizationType=QuantizationType.Q4_0,
+        default_container:ContainerType=ContainerType.GGJT)->Model:
+
+        path_type = _get_path_type(model_path_or_repo_id)
+
+        if path_type == PathType.UNKNOWN:
+            raise ValueError(f"Unknown path type for '{model_path_or_repo_id}'")
+        elif path_type == PathType.FILE:
+            return cls.from_file(model_path_or_repo_id,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+        else:
+            if path_type == PathType.REPO:
+
+                try: 
+                    config = AutoConfig.from_pretrained(
+                        model_path_or_repo_id,
+                    )
+                except ValueError:
+                    logging.warning("Could not find config.json in repo, assuming GGML model...")
+                    config = AutoConfig(repo_type="GGML")
+                       
+
+                if config.repo_type != "GGML":
+                    logging.warning("Found normal HuggingFace model, starting conversion...")
+                    return cls.from_transformer(model_path_or_repo_id, session_config, tokenizer_path_or_repo_id, lora_paths, verbose, use_hf_tokenizer,default_quantization, default_container)
+            
+                resolved_path = cls._find_model_path_from_repo(str(model_path_or_repo_id),model_file)
+                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+            
+            elif path_type == PathType.DIR:
+                resolved_path = cls._find_model_path_from_dir(str(model_path_or_repo_id),model_file)
+                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+            
+            else:
+                raise ValueError(f"Unknown path type '{path_type}'")
+
+
+    @classmethod
+    def _find_model_path_from_dir(
+        cls,
+        directory: str,
+        filename: Optional[str] = None,
+    ) -> str:
+        path = pathlib.Path(directory).resolve()
+        if filename:
+            file = (path / filename)
+            if not file.is_file():
+                raise ValueError(
+                    f"Model file '{filename}' not found in '{path}'")
+            return str(file)
+
+        files = [
+            f for f in path.iterdir()
+            if f.is_file() and f.name.endswith('.bin')
+        ]
+
+        if len(files) == 0:
+            raise ValueError(f"No model files found in '{path}'")
+        elif len(files) > 1:
+            raise ValueError(
+                f"Multiple model files found in '{path}'! Please specify one of the following model files to load: '{','.join([f.name for f in files])}'"
+            )
+
+        return str(files[0].resolve())
+    
+    @classmethod
+    def _find_model_path_from_repo(
+        cls,
+        repo_id: str,
+        filename: Optional[str] = None,
+    ) -> str:
+        cache_directory = cached_assets_path("llm-rs",namespace=repo_id)
+        #we dont want to download the whole repo, just the metadata
+        directory = snapshot_download(repo_id=repo_id,
+                                allow_patterns='*.meta',
+                                local_dir=cache_directory)
+        path = pathlib.Path(directory).resolve()
+        files = [
+            f for f in path.iterdir()
+            if f.is_file() and f.name.endswith('.meta')
+        ]
+
+        if len(files) == 0 and filename is None:
+            raise ValueError(f"No model files found in '{repo_id}'! Either specify the model file via the `model_file` parameter or make sure the repository contains a *.meta files for each model.")
+        if len(files) > 1 and filename is None:
+            raise ValueError(
+                f"Multiple model files found in '{repo_id}'! Please specify one of the following model files to load: '{','.join([f.name.replace('.meta','.bin') for f in files])}' "
+            )
+        #if we have a filename, we can just download that file
+        filename = filename if filename else files[0].name.replace('.meta','.bin')
+        model_directory = snapshot_download(repo_id=repo_id,
+                                allow_patterns=filename,
+                                local_dir=cache_directory)
+        
+        return cls._find_model_path_from_dir(model_directory, filename=filename)
+    
+    @classmethod
+    def from_transformer(cls,
+        model_path_or_repo_id: Union[str,os.PathLike],
+        session_config:SessionConfig=SessionConfig(),
+        tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
+        lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
+        verbose:bool=False,
+        use_hf_tokenizer:bool=True,
+        default_quantization:QuantizationType=QuantizationType.Q4_0,
+        default_container:ContainerType=ContainerType.GGJT):
+        
+        try:
+            from .convert import AutoConverter
+            from .convert.auto_converter import get_name_from_config
+            from transformers import AutoConfig
+        except ImportError:
+            raise ImportError("Model conversion needs additional dependencies. Please install 'llm-rs[convert]' to use this functionality!")
+        
+
+        config = AutoConfig.from_pretrained(model_path_or_repo_id,trust_remote_code=True)
+        model_name = get_name_from_config(config)
+        export_path = cached_assets_path("llm-rs",namespace=model_name)
+        converted_model = AutoConverter.convert(model_path_or_repo_id,export_path)
+        if default_quantization != QuantizationType.F16:
+            converted_model = AutoQuantizer.quantize(converted_model,quantization=default_quantization,container=default_container)
+        return cls.from_file(converted_model,None,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+    
+# Hack to make the quantization type enum hashable
+_APPENDIX_MAP = {
+    QuantizationType.Q4_0.__repr__(): "q4_0",
+    QuantizationType.Q4_1.__repr__(): "q4_1",
+    QuantizationType.Q5_0.__repr__(): "q5_0",
+    QuantizationType.Q5_1.__repr__(): "q5_1",
+    QuantizationType.Q8_0.__repr__(): "q8_0",
+}
+
+class AutoQuantizer():
+    """
+    Utility to quantize models, without having to specify the model type.
+    """
+    @staticmethod
+    def quantize(
+        model_file:Union[str,os.PathLike],
+        target_path:Optional[Union[str,os.PathLike]]=None,
+        quantization:QuantizationType=QuantizationType.Q4_0,
+        container:ContainerType=ContainerType.GGJT,
+        callback:Optional[Callable[[str],None]]=None
+        )->Union[str,os.PathLike]:
+        metadata=AutoModel.load_metadata(model_file)
+        if metadata.quantization != QuantizationType.F16:
+            raise ValueError(f"Model '{model_file}' is already quantized to '{metadata.quantization}'")
+
+        model_type = AutoModel._infer_model_type(model_file)
+
+        if target_path is None:
+            target_path = os.path.dirname(model_file)
+            
+        def build_target_name()->str:
+            output_path = pathlib.Path(target_path)
+            if output_path.is_file():
+                return str(output_path)
+            else:
+                output_path.mkdir(parents=True,exist_ok=True)
+                model_path = pathlib.Path(model_file)
+                appendix = ""
+
+                if quantization.__repr__() in _APPENDIX_MAP:
+                    appendix += f"-{_APPENDIX_MAP[quantization.__repr__()]}"
+
+                if container == ContainerType.GGJT:
+                    appendix += "-ggjt"
+            
+                filename = model_path.stem.replace("-f16","") + appendix + model_path.suffix
+                return str(output_path / filename)
+
+        target_file = build_target_name()
+        if pathlib.Path(target_file).exists():
+            logging.warning(f"Target file '{target_file}' already exists, skipping quantization")
+            return target_file
+        
+        logging.info(f"Quantizing model '{model_file}' to '{target_file}'")
+        model_type.quantize(str(model_file),target_file,quantization,container,callback=callback)
+
+        metadata_file = pathlib.Path(target_file).with_suffix(".meta")
+        quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=CURRENT_QUANTIZATION_VERSION,base_model=metadata.base_model)
+        quantized_metadata.add_hash(target_file)
+        logging.info(f"Writing metadata file '{metadata_file}'")
+        metadata_file.write_text(json.dumps(quantized_metadata.serialize(),indent=4))
+        logging.info(f"Finished quantizing model '{model_file}' to '{target_file}'")
+        return target_file
+
+
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/auto_converter.py` & `llm_rs_metal-0.2.12/llm_rs/convert/auto_converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-from transformers import AutoConfig
-import os
-from typing import Union
-from .models import MPTConverter,GptNeoXConverter,GptJConverter,Gpt2Converter,BloomConverter,LlamaConverter
-import logging 
-import pathlib
-
-
-_ARCHITECTURE_CONVERTER_MAP = {
-    "MPTForCausalLM": MPTConverter,
-    "GPTNeoXForCausalLM": GptNeoXConverter,
-    "GPTJForCausalLM": GptJConverter,
-    "GPT2LMHeadModel": Gpt2Converter,
-    "BloomForCausalLM":BloomConverter,
-    "LLaMAForCausalLM":LlamaConverter
-}
-
-class AutoConverter():
-
-    @staticmethod
-    def convert(pretrained_model_name_or_path:Union[str,os.PathLike],output_path:Union[str,os.PathLike])->str:
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path,trust_remote_code=True)
-        architecture = config.architectures[0]
-        model_name = get_name_from_config(config)
-
-        adapter=None
-        if architecture not in _ARCHITECTURE_CONVERTER_MAP:
-            raise ValueError(f"Unsupported architecture '{architecture}' for '{model_name}'")
-        adapter = _ARCHITECTURE_CONVERTER_MAP[architecture]
-
-        output_file = build_path(output_path,model_name)
-        if os.path.exists(output_file):
-            logging.warning(f"Skipping {model_name} via {adapter.__name__} because '{output_file}' already exists!")
-            return output_file
-        
-        logging.info(f"Converting {model_name} via {adapter.__name__} to '{output_file}'")
-        adapter(pretrained_model_name_or_path).convert(output_file)
-        return output_file
-
-
-def get_name_from_config(config:AutoConfig)->str:
-    raw_name:str = ""
-    if hasattr(config,"name_or_path"):
-        raw_name = config.name_or_path
-    elif hasattr(config,"model_type"):
-        raw_name = config.model_type
-    else:
-        raw_name = config.architectures[0]
-    return raw_name.split("/")[-1]
-
-
-def build_path(output_path:Union[str,os.PathLike],model_name:str)->str:
-    output_path = pathlib.Path(output_path)
-    #User specified a file, so just use that
-    if output_path.is_file():
-        return output_path
-
-    #User specified a directory => auto generate a file name
-    output_path.mkdir(parents=True,exist_ok=True)
-    return os.path.join(output_path,f"{model_name}-f16.bin")
-    
+from transformers import AutoConfig
+import os
+from typing import Union
+from .models import MPTConverter,GptNeoXConverter,GptJConverter,Gpt2Converter,BloomConverter,LlamaConverter
+import logging 
+import pathlib
+
+
+_ARCHITECTURE_CONVERTER_MAP = {
+    "MPTForCausalLM": MPTConverter,
+    "GPTNeoXForCausalLM": GptNeoXConverter,
+    "GPTJForCausalLM": GptJConverter,
+    "GPT2LMHeadModel": Gpt2Converter,
+    "BloomForCausalLM":BloomConverter,
+    "LLaMAForCausalLM":LlamaConverter,
+    "LlamaForCausalLM":LlamaConverter #Open-LLaMA uses this as architecture name
+}
+
+class AutoConverter():
+
+    @staticmethod
+    def convert(pretrained_model_name_or_path:Union[str,os.PathLike],output_path:Union[str,os.PathLike])->str:
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path,trust_remote_code=True)
+        architecture = config.architectures[0]
+        model_name = get_name_from_config(config)
+
+        adapter=None
+        if architecture not in _ARCHITECTURE_CONVERTER_MAP:
+            raise ValueError(f"Unsupported architecture '{architecture}' for '{model_name}'")
+        adapter = _ARCHITECTURE_CONVERTER_MAP[architecture]
+
+        output_file = build_path(output_path,model_name)
+        if os.path.exists(output_file):
+            logging.warning(f"Skipping {model_name} via {adapter.__name__} because '{output_file}' already exists!")
+            return output_file
+        
+        logging.info(f"Converting {model_name} via {adapter.__name__} to '{output_file}'")
+        adapter(pretrained_model_name_or_path).convert(output_file)
+        return output_file
+
+
+def get_name_from_config(config:AutoConfig)->str:
+    raw_name:str = ""
+    if hasattr(config,"name_or_path"):
+        raw_name = config.name_or_path
+    elif hasattr(config,"model_type"):
+        raw_name = config.model_type
+    else:
+        raw_name = config.architectures[0]
+    return raw_name.split("/")[-1]
+
+
+def build_path(output_path:Union[str,os.PathLike],model_name:str)->str:
+    output_path = pathlib.Path(output_path)
+    #User specified a file, so just use that
+    if output_path.is_file():
+        return output_path
+
+    #User specified a directory => auto generate a file name
+    output_path.mkdir(parents=True,exist_ok=True)
+    return os.path.join(output_path,f"{model_name}-f16.bin")
+
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/_base.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/_base.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-from abc import ABC, abstractmethod
-from typing import Union,Tuple,Any,Optional,BinaryIO
-from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
-import os
-import struct
-from enum import Enum
-import logging
-import numpy as np
-from ...config import QuantizationType,ContainerType
-from ...auto import ModelMetadata, KnownModels, QuantizationVersions
-import pathlib
-import json
-import torch
-
-GGML_MAGIC = 0x67676D6C
-GGMF_MAGIC = 0x67676D66
-GGJT_MAGIC = 0x67676a74
-
-class FileTypes(Enum):
-    FP32 = 0
-    FP16 = 1
-
-class BaseAdapter(ABC):
-    model_type:KnownModels=None
-    file_magic:int=GGML_MAGIC
-    version:int=1
-
-    def  __init__(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None) -> None:
-        self.pretrained_model_name_or_path = pretrained_model_name_or_path
-        self.config,self.tokenizer,self.model= self.load(pretrained_model_name_or_path,pretrained_tokenizer_name_or_path)
-
-    @abstractmethod
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoConfig,AutoTokenizer,AutoModelForCausalLM]:
-        ...
-
-    @abstractmethod
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        ...
-
-    def _write_vocabulary(self,out_file:BinaryIO):
-        # TODO: temporary hack to not deal with implementing the tokenizer
-        logging.info(f"Processing vocabulary with size {self.config.vocab_size}")
-        dot_token = self.tokenizer.encode(".")[0]
-        for i in range(self.config.vocab_size):
-            text = self.tokenizer.decode([dot_token, i]).encode("utf-8")
-            # remove the first byte (it's always '.')
-            text = text[1:]
-            out_file.write(struct.pack("i", len(text)))
-            out_file.write(text)
-
-
-    def _filter_weights(self,name:str,weight:torch.Tensor)->bool:
-        """Filter weights that should be skipped"""
-        return False
-    
-    def _filter_weights_after_rename(self,name:str,weight:torch.Tensor)->bool:
-        """Filter weights that should be skipped"""
-        return False
-    
-    def _filter_f16_weights(self,name:str,data:np.ndarray)->bool:
-        """Filter weights that should be stored as fp16"""
-        n_dims = len(data.shape)
-        return name.endswith(".weight") and n_dims == 2
-    
-    def _rename_weights(self,name:str)->str:
-        """Rename weights that should be renamed"""
-        return name
-    
-    def _transform_weights(self,name:str,weight:torch.Tensor)->torch.Tensor:
-        """Transform weights that should be transformed"""
-        return weight
-    
-    def _write_weights(self,out_file:BinaryIO):
-        weights = self.model.state_dict()
-        for name, weight in weights.items():
-            
-
-            if self._filter_weights(name,weight):
-                logging.info(f"Skipping layer '{name}'")
-                continue
-            
-            name = self._rename_weights(name)
-            weight = self._transform_weights(name,weight)
-            if self._filter_weights_after_rename(name,weight):
-                logging.info(f"Skipping layer '{name}'")
-                continue
-
-            data = weight.squeeze().numpy()
-            n_dims = len(data.shape);    
-            type = FileTypes.FP32
-
-            if self._filter_f16_weights(name,data):
-                data = data.astype(np.float16)
-                type = FileTypes.FP16
-            else:
-                data = data.astype(np.float32)
-
-            encoded_name = name.encode("utf-8")
-            out_file.write(struct.pack("iii", n_dims, len(encoded_name), type.value))
-
-            if self.file_magic == GGJT_MAGIC or self.file_magic == GGMF_MAGIC:
-                out_file.write(struct.pack("i" * len(data.shape), *data.shape[::-1]))
-            else:
-                for i in range(n_dims):
-                    out_file.write(struct.pack("i", data.shape[n_dims - 1 - i]))
-            out_file.write(encoded_name)
-
-
-            if self.file_magic == GGJT_MAGIC:
-                # pad to 32 bytes
-                out_file.seek((out_file.tell() + 31) & -32)
-
-            # data
-            data.tofile(out_file)
-            logging.info(f"Converted layer '{name}' with shape {data.shape}")
-
-
-    def write_magic(self,out_file:BinaryIO):
-        out_file.write(struct.pack("i", self.file_magic))
-        if self.file_magic == GGJT_MAGIC or self.file_magic == GGMF_MAGIC:
-            out_file.write(struct.pack("i", self.version))
-
-    def write_file_type(self,out_file:BinaryIO,file_type:FileTypes=FileTypes.FP16):
-        out_file.write(struct.pack("i", file_type.value))
-
-
-
-    def convert(self,output_file:Union[str,os.PathLike])->None:
-
-        with open(output_file, "wb") as out_file:
-            # write magic
-            self.write_magic(out_file)
-            logging.info(f"Processing hyperparameters ...")
-            self._write_hyperparameters(out_file)
-            self.write_file_type(out_file)
-
-            self._write_vocabulary(out_file)
-            self._write_weights(out_file)
-            logging.info(f"Done converting model to GGML format. Saved to '{output_file}'")
-
-        #Create the *.meta file needed for automatic loading
-        metadata_file = pathlib.Path(output_file).with_suffix(".meta")
-        metadata = ModelMetadata(
-            model = self.model_type,
-            quantization = QuantizationType.F16,
-            container = ContainerType.GGML,
-            quantization_version=QuantizationVersions.Not_Quantized,
-            base_model=str(self.pretrained_model_name_or_path),
-            )
-        metadata.add_hash(output_file)
-        metadata_file.write_text(json.dumps(metadata.serialize(),indent=4))
-        
-        logging.info(f"Created metadata file at '{output_file}'")
-
+from abc import ABC, abstractmethod
+from typing import Union,Tuple,Any,Optional,BinaryIO
+from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
+import os
+import struct
+from enum import Enum
+import logging
+import numpy as np
+from ...config import QuantizationType,ContainerType
+from ...auto import ModelMetadata, KnownModels, QuantizationVersions
+import pathlib
+import json
+import torch
+
+GGML_MAGIC = 0x67676D6C
+GGMF_MAGIC = 0x67676D66
+GGJT_MAGIC = 0x67676a74
+
+class FileTypes(Enum):
+    FP32 = 0
+    FP16 = 1
+
+class BaseAdapter(ABC):
+    model_type:KnownModels=None
+    file_magic:int=GGML_MAGIC
+    version:int=1
+
+    def  __init__(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None) -> None:
+        self.pretrained_model_name_or_path = pretrained_model_name_or_path
+        self.config,self.tokenizer,self.model= self.load(pretrained_model_name_or_path,pretrained_tokenizer_name_or_path)
+
+    @abstractmethod
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoConfig,AutoTokenizer,AutoModelForCausalLM]:
+        ...
+
+    @abstractmethod
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        ...
+
+    def _write_vocabulary(self,out_file:BinaryIO):
+        # TODO: temporary hack to not deal with implementing the tokenizer
+        logging.info(f"Processing vocabulary with size {self.config.vocab_size}")
+        dot_token = self.tokenizer.encode(".")[0]
+        for i in range(self.config.vocab_size):
+            text = self.tokenizer.decode([dot_token, i]).encode("utf-8")
+            # remove the first byte (it's always '.')
+            text = text[1:]
+            out_file.write(struct.pack("i", len(text)))
+            out_file.write(text)
+
+
+    def _filter_weights(self,name:str,weight:torch.Tensor)->bool:
+        """Filter weights that should be skipped"""
+        return False
+    
+    def _filter_weights_after_rename(self,name:str,weight:torch.Tensor)->bool:
+        """Filter weights that should be skipped"""
+        return False
+    
+    def _filter_f16_weights(self,name:str,data:np.ndarray)->bool:
+        """Filter weights that should be stored as fp16"""
+        n_dims = len(data.shape)
+        return name.endswith(".weight") and n_dims == 2
+    
+    def _rename_weights(self,name:str)->str:
+        """Rename weights that should be renamed"""
+        return name
+    
+    def _transform_weights(self,name:str,weight:torch.Tensor)->torch.Tensor:
+        """Transform weights that should be transformed"""
+        return weight
+    
+    def _write_weights(self,out_file:BinaryIO):
+        weights = self.model.state_dict()
+        for name, weight in weights.items():
+            
+
+            if self._filter_weights(name,weight):
+                logging.info(f"Skipping layer '{name}'")
+                continue
+            
+            name = self._rename_weights(name)
+            weight = self._transform_weights(name,weight)
+            if self._filter_weights_after_rename(name,weight):
+                logging.info(f"Skipping layer '{name}'")
+                continue
+
+            data = weight.squeeze().numpy()
+            n_dims = len(data.shape);    
+            type = FileTypes.FP32
+
+            if self._filter_f16_weights(name,data):
+                data = data.astype(np.float16)
+                type = FileTypes.FP16
+            else:
+                data = data.astype(np.float32)
+
+            encoded_name = name.encode("utf-8")
+            out_file.write(struct.pack("iii", n_dims, len(encoded_name), type.value))
+
+            if self.file_magic == GGJT_MAGIC or self.file_magic == GGMF_MAGIC:
+                out_file.write(struct.pack("i" * len(data.shape), *data.shape[::-1]))
+            else:
+                for i in range(n_dims):
+                    out_file.write(struct.pack("i", data.shape[n_dims - 1 - i]))
+            out_file.write(encoded_name)
+
+
+            if self.file_magic == GGJT_MAGIC:
+                # pad to 32 bytes
+                out_file.seek((out_file.tell() + 31) & -32)
+
+            # data
+            data.tofile(out_file)
+            logging.info(f"Converted layer '{name}' with shape {data.shape}")
+
+
+    def write_magic(self,out_file:BinaryIO):
+        out_file.write(struct.pack("i", self.file_magic))
+        if self.file_magic == GGJT_MAGIC or self.file_magic == GGMF_MAGIC:
+            out_file.write(struct.pack("i", self.version))
+
+    def write_file_type(self,out_file:BinaryIO,file_type:FileTypes=FileTypes.FP16):
+        out_file.write(struct.pack("i", file_type.value))
+
+
+
+    def convert(self,output_file:Union[str,os.PathLike])->None:
+
+        with open(output_file, "wb") as out_file:
+            # write magic
+            self.write_magic(out_file)
+            logging.info(f"Processing hyperparameters ...")
+            self._write_hyperparameters(out_file)
+            self.write_file_type(out_file)
+
+            self._write_vocabulary(out_file)
+            self._write_weights(out_file)
+            logging.info(f"Done converting model to GGML format. Saved to '{output_file}'")
+
+        #Create the *.meta file needed for automatic loading
+        metadata_file = pathlib.Path(output_file).with_suffix(".meta")
+        metadata = ModelMetadata(
+            model = self.model_type,
+            quantization = QuantizationType.F16,
+            container = ContainerType.GGML,
+            quantization_version=QuantizationVersions.Not_Quantized,
+            base_model=str(self.pretrained_model_name_or_path),
+            )
+        metadata.add_hash(output_file)
+        metadata_file.write_text(json.dumps(metadata.serialize(),indent=4))
+        
+        logging.info(f"Created metadata file at '{output_file}'")
+
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/bloom.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/bloom.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import numpy as np
-from ._base import BaseAdapter
-from typing import Union,Tuple,Optional,BinaryIO 
-from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig,BloomForCausalLM
-import os
-import torch
-import struct
-import numpy as np
-from ...auto import KnownModels
-
-#based on https://github.com/NouamaneTazi/bloomz.cpp/blob/main/convert-hf-to-ggml.py
-
-conv_map = {
-    'word_embeddings'       : 'tok_embeddings',
-    "word_embeddings_layernorm": 'norm',
-        'input_layernorm'        : 'attention_norm',
-        'self_attention.query_key_value': 'attention.query_key_value',
-        'self_attention.dense':          'attention.wo',
-        'post_attention_layernorm': 'ffn_norm',
-        'mlp.dense_h_to_4h'           : 'feed_forward.w1',
-        'mlp.dense_4h_to_h'           : 'feed_forward.w2',
-        'ln_f'                        : 'output_norm',
-        'lm_head' : 'output',
-        }
-
-class BloomConverter(BaseAdapter):
-    model_type:KnownModels=KnownModels.Bloom
-
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
-        
-        model = BloomForCausalLM.from_pretrained(
-            pretrained_model_name_or_path,
-            torch_dtype=torch.float16,
-            low_cpu_mem_usage=True,
-            )
-        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
-        return config,tokenizer,model
-    
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        hyperparameters = self.config.to_dict()
-        hyperparameters["multiple_of"] = 1
-        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
-        out_file.write(struct.pack("i", hyperparameters["hidden_size"]))
-        out_file.write(struct.pack("i", hyperparameters["multiple_of"]))
-        out_file.write(struct.pack("i", hyperparameters["n_head"]))
-        out_file.write(struct.pack("i", hyperparameters["n_layer"]))
-
-    def _rename_weights(self, name: str) -> str:
-        #Arrrrrg i hate this, but upstream is inconsistent with naming
-        nn = name
-        if name != "lm_head.weight":
-            nn = nn.split(".")[1:]
-        else:
-            nn = nn.split(".")
-
-        if nn[0] == "h":
-            nn[0] = "layers"
-            mapped = conv_map[".".join(nn[2:-1])]
-            name = ".".join(nn[:2] + [mapped] + nn[-1:])
-        else:
-            mapped = conv_map[".".join(nn[:-1])]
-            name = ".".join([mapped] + nn[-1:])
-        return name
-
-    def _transform_weights(self, name: str, weight: torch.Tensor) ->  torch.Tensor:
-        if "query_key_value" in name:
-            q, k, v = weight.reshape(self.config.n_head, 3, -1).unbind(1)
-            return torch.cat([q, k, v], dim=0).reshape_as(weight)
-        return weight
-    
-    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
+import numpy as np
+from ._base import BaseAdapter
+from typing import Union,Tuple,Optional,BinaryIO 
+from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig,BloomForCausalLM
+import os
+import torch
+import struct
+import numpy as np
+from ...auto import KnownModels
+
+#based on https://github.com/NouamaneTazi/bloomz.cpp/blob/main/convert-hf-to-ggml.py
+
+conv_map = {
+    'word_embeddings'       : 'tok_embeddings',
+    "word_embeddings_layernorm": 'norm',
+        'input_layernorm'        : 'attention_norm',
+        'self_attention.query_key_value': 'attention.query_key_value',
+        'self_attention.dense':          'attention.wo',
+        'post_attention_layernorm': 'ffn_norm',
+        'mlp.dense_h_to_4h'           : 'feed_forward.w1',
+        'mlp.dense_4h_to_h'           : 'feed_forward.w2',
+        'ln_f'                        : 'output_norm',
+        'lm_head' : 'output',
+        }
+
+class BloomConverter(BaseAdapter):
+    model_type:KnownModels=KnownModels.Bloom
+
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
+        
+        model = BloomForCausalLM.from_pretrained(
+            pretrained_model_name_or_path,
+            torch_dtype=torch.float16,
+            low_cpu_mem_usage=True,
+            )
+        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
+        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+        return config,tokenizer,model
+    
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        hyperparameters = self.config.to_dict()
+        hyperparameters["multiple_of"] = 1
+        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
+        out_file.write(struct.pack("i", hyperparameters["hidden_size"]))
+        out_file.write(struct.pack("i", hyperparameters["multiple_of"]))
+        out_file.write(struct.pack("i", hyperparameters["n_head"]))
+        out_file.write(struct.pack("i", hyperparameters["n_layer"]))
+
+    def _rename_weights(self, name: str) -> str:
+        #Arrrrrg i hate this, but upstream is inconsistent with naming
+        nn = name
+        if name != "lm_head.weight":
+            nn = nn.split(".")[1:]
+        else:
+            nn = nn.split(".")
+
+        if nn[0] == "h":
+            nn[0] = "layers"
+            mapped = conv_map[".".join(nn[2:-1])]
+            name = ".".join(nn[:2] + [mapped] + nn[-1:])
+        else:
+            mapped = conv_map[".".join(nn[:-1])]
+            name = ".".join([mapped] + nn[-1:])
+        return name
+
+    def _transform_weights(self, name: str, weight: torch.Tensor) ->  torch.Tensor:
+        if "query_key_value" in name:
+            q, k, v = weight.reshape(self.config.n_head, 3, -1).unbind(1)
+            return torch.cat([q, k, v], dim=0).reshape_as(weight)
+        return weight
+    
+    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
         return name.endswith("attn.masked_bias") or name.endswith(".attn.bias")
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/gpt2.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/gpt2.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import numpy as np
-from ._base import BaseAdapter
-from typing import Union,Tuple,Optional,BinaryIO 
-from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig,GPT2LMHeadModel
-import os
-import torch
-import struct
-import numpy as np
-from ...auto import KnownModels
-import re
-
-#based on https://github.com/ggerganov/ggml/blob/master/examples/gpt-2/convert-h5-to-ggml.py
-class Gpt2Converter(BaseAdapter):
-    model_type:KnownModels=KnownModels.Gpt2
-
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
-        
-        model = GPT2LMHeadModel.from_pretrained(
-            pretrained_model_name_or_path,
-            torch_dtype=torch.float16,
-            low_cpu_mem_usage=True,
-            )
-        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
-        return config,tokenizer,model
-    
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        hyperparameters = self.config.to_dict()
-        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
-        out_file.write(struct.pack("i", hyperparameters["n_positions"]))
-        out_file.write(struct.pack("i", hyperparameters["n_embd"]))
-        out_file.write(struct.pack("i", hyperparameters["n_head"]))
-        out_file.write(struct.pack("i", hyperparameters["n_layer"]))
-
-
-    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
-        return name.endswith("attn.masked_bias") or name.endswith(".attn.bias") 
-    
-    def _rename_weights(self, name: str) -> str:
-        new_name=name
-        # rename headers to keep compatibility
-        # cerebras renames, see https://github.com/ggerganov/ggml/blob/master/examples/gpt-2/convert-cerebras-to-ggml.py
-        if name == "transformer.ln_f.weight":
-            new_name = "model/ln_f/g"
-        elif name == "transformer.ln_f.bias":
-            new_name = "model/ln_f/b"
-        elif name == "transformer.wte.weight":
-            new_name = "model/wte"
-        elif name == "transformer.wpe.weight":
-            new_name = "model/wpe"
-        elif name == "lm_head.weight":
-            new_name = "model/lm_head"
-        elif re.match(r"transformer.h\.\d+\.ln_1\.weight", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/ln_1/g"
-        elif re.match(r"transformer.h\.\d+\.ln_1\.bias", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/ln_1/b"
-        elif re.match(r"transformer.h\.\d+\.attn\.c_attn\.weight", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/attn/c_attn/w"
-        elif re.match(r"transformer.h\.\d+\.attn\.c_attn\.bias", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/attn/c_attn/b"
-        elif re.match(r"transformer.h\.\d+\.attn\.c_proj\.weight", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/attn/c_proj/w"
-        elif re.match(r"transformer.h.\d+.attn.c_proj.bias", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/attn/c_proj/b"
-        elif re.match(r"transformer.h.\d+.ln_2.weight", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/ln_2/g"
-        elif re.match(r"transformer.h.\d+.ln_2.bias", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/ln_2/b"
-        elif re.match(r"transformer.h.\d+.mlp.c_fc.weight", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/mlp/c_fc/w"
-        elif re.match(r"transformer.h.\d+.mlp.c_fc.bias", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/mlp/c_fc/b"
-        elif re.match(r"transformer.h.\d+.mlp.c_proj.weight", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/mlp/c_proj/w"
-        elif re.match(r"transformer.h.\d+.mlp.c_proj.bias", name):
-            i = re.findall("\d+", name)[0]
-            new_name = f"model/h{i}/mlp/c_proj/b"
-
-        return new_name
-    
-    def _write_vocabulary(self, out_file: BinaryIO):
-        # write the vocabulary size
-        out_file.write(struct.pack("i", self.config.vocab_size))
-        return super()._write_vocabulary(out_file)
-
-    def _transform_weights(self, name: str, weight: torch.Tensor) -> torch.Tensor:
-        # for efficiency - transpose these matrices:
-        if name.endswith("/mlp/c_proj/w") or name.endswith("/mlp/c_fc/w") or name.endswith("/attn/c_proj/w") or name.endswith("/attn/c_attn/w"):
-            #see this issue: https://github.com/pytorch/pytorch/issues/50275
-            return weight.transpose(0,1)
-        return weight
-    
-    def _filter_f16_weights(self, name: str, data: np.ndarray) -> bool:
-        n_dims = len(data.shape)
-        return (name == "model/wte" or name == "model/lm_head" or name[-2:] == "/g" or name[-2:] == "/w") and n_dims == 2
-
-    
-
+import numpy as np
+from ._base import BaseAdapter
+from typing import Union,Tuple,Optional,BinaryIO 
+from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig,GPT2LMHeadModel
+import os
+import torch
+import struct
+import numpy as np
+from ...auto import KnownModels
+import re
+
+#based on https://github.com/ggerganov/ggml/blob/master/examples/gpt-2/convert-h5-to-ggml.py
+class Gpt2Converter(BaseAdapter):
+    model_type:KnownModels=KnownModels.Gpt2
+
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
+        
+        model = GPT2LMHeadModel.from_pretrained(
+            pretrained_model_name_or_path,
+            torch_dtype=torch.float16,
+            low_cpu_mem_usage=True,
+            )
+        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
+        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+        return config,tokenizer,model
+    
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        hyperparameters = self.config.to_dict()
+        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
+        out_file.write(struct.pack("i", hyperparameters["n_positions"]))
+        out_file.write(struct.pack("i", hyperparameters["n_embd"]))
+        out_file.write(struct.pack("i", hyperparameters["n_head"]))
+        out_file.write(struct.pack("i", hyperparameters["n_layer"]))
+
+
+    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
+        return name.endswith("attn.masked_bias") or name.endswith(".attn.bias") 
+    
+    def _rename_weights(self, name: str) -> str:
+        new_name=name
+        # rename headers to keep compatibility
+        # cerebras renames, see https://github.com/ggerganov/ggml/blob/master/examples/gpt-2/convert-cerebras-to-ggml.py
+        if name == "transformer.ln_f.weight":
+            new_name = "model/ln_f/g"
+        elif name == "transformer.ln_f.bias":
+            new_name = "model/ln_f/b"
+        elif name == "transformer.wte.weight":
+            new_name = "model/wte"
+        elif name == "transformer.wpe.weight":
+            new_name = "model/wpe"
+        elif name == "lm_head.weight":
+            new_name = "model/lm_head"
+        elif re.match(r"transformer.h\.\d+\.ln_1\.weight", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/ln_1/g"
+        elif re.match(r"transformer.h\.\d+\.ln_1\.bias", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/ln_1/b"
+        elif re.match(r"transformer.h\.\d+\.attn\.c_attn\.weight", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/attn/c_attn/w"
+        elif re.match(r"transformer.h\.\d+\.attn\.c_attn\.bias", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/attn/c_attn/b"
+        elif re.match(r"transformer.h\.\d+\.attn\.c_proj\.weight", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/attn/c_proj/w"
+        elif re.match(r"transformer.h.\d+.attn.c_proj.bias", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/attn/c_proj/b"
+        elif re.match(r"transformer.h.\d+.ln_2.weight", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/ln_2/g"
+        elif re.match(r"transformer.h.\d+.ln_2.bias", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/ln_2/b"
+        elif re.match(r"transformer.h.\d+.mlp.c_fc.weight", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/mlp/c_fc/w"
+        elif re.match(r"transformer.h.\d+.mlp.c_fc.bias", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/mlp/c_fc/b"
+        elif re.match(r"transformer.h.\d+.mlp.c_proj.weight", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/mlp/c_proj/w"
+        elif re.match(r"transformer.h.\d+.mlp.c_proj.bias", name):
+            i = re.findall("\d+", name)[0]
+            new_name = f"model/h{i}/mlp/c_proj/b"
+
+        return new_name
+    
+    def _write_vocabulary(self, out_file: BinaryIO):
+        # write the vocabulary size
+        out_file.write(struct.pack("i", self.config.vocab_size))
+        return super()._write_vocabulary(out_file)
+
+    def _transform_weights(self, name: str, weight: torch.Tensor) -> torch.Tensor:
+        # for efficiency - transpose these matrices:
+        if name.endswith("/mlp/c_proj/w") or name.endswith("/mlp/c_fc/w") or name.endswith("/attn/c_proj/w") or name.endswith("/attn/c_attn/w"):
+            #see this issue: https://github.com/pytorch/pytorch/issues/50275
+            return weight.transpose(0,1)
+        return weight
+    
+    def _filter_f16_weights(self, name: str, data: np.ndarray) -> bool:
+        n_dims = len(data.shape)
+        return (name == "model/wte" or name == "model/lm_head" or name[-2:] == "/g" or name[-2:] == "/w") and n_dims == 2
+
+    
+
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/gptj.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/gptj.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import numpy as np
-from ._base import BaseAdapter
-from typing import Union,Tuple,Optional,BinaryIO 
-from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig,GPTJForCausalLM
-import os
-import torch
-import struct
-import numpy as np
-from ...auto import KnownModels
-
-#based on https://github.com/ggerganov/ggml/blob/master/examples/gpt-j/convert-h5-to-ggml.py
-class GptJConverter(BaseAdapter):
-    model_type:KnownModels=KnownModels.GptJ
-
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
-        
-        model = GPTJForCausalLM.from_pretrained(
-            pretrained_model_name_or_path,
-            torch_dtype=torch.float16,
-            low_cpu_mem_usage=True,
-            )
-        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
-        return config,tokenizer,model
-    
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        hyperparameters = self.config.to_dict()
-        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
-        out_file.write(struct.pack("i", hyperparameters["n_positions"]))
-        out_file.write(struct.pack("i", hyperparameters["n_embd"]))
-        out_file.write(struct.pack("i", hyperparameters["n_head"]))
-        out_file.write(struct.pack("i", hyperparameters["n_layer"]))
-        out_file.write(struct.pack("i", hyperparameters["rotary_dim"]))
-
-    def _write_vocabulary(self, out_file: BinaryIO):
-        # write the vocabulary size
-        out_file.write(struct.pack("i", self.config.vocab_size))
-        return super()._write_vocabulary(out_file)
-    
-
-    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
+import numpy as np
+from ._base import BaseAdapter
+from typing import Union,Tuple,Optional,BinaryIO 
+from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig,GPTJForCausalLM
+import os
+import torch
+import struct
+import numpy as np
+from ...auto import KnownModels
+
+#based on https://github.com/ggerganov/ggml/blob/master/examples/gpt-j/convert-h5-to-ggml.py
+class GptJConverter(BaseAdapter):
+    model_type:KnownModels=KnownModels.GptJ
+
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
+        
+        model = GPTJForCausalLM.from_pretrained(
+            pretrained_model_name_or_path,
+            torch_dtype=torch.float16,
+            low_cpu_mem_usage=True,
+            )
+        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
+        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+        return config,tokenizer,model
+    
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        hyperparameters = self.config.to_dict()
+        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
+        out_file.write(struct.pack("i", hyperparameters["n_positions"]))
+        out_file.write(struct.pack("i", hyperparameters["n_embd"]))
+        out_file.write(struct.pack("i", hyperparameters["n_head"]))
+        out_file.write(struct.pack("i", hyperparameters["n_layer"]))
+        out_file.write(struct.pack("i", hyperparameters["rotary_dim"]))
+
+    def _write_vocabulary(self, out_file: BinaryIO):
+        # write the vocabulary size
+        out_file.write(struct.pack("i", self.config.vocab_size))
+        return super()._write_vocabulary(out_file)
+    
+
+    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
         return name.endswith("attn.masked_bias") or name.endswith(".attn.bias")
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/gptneox.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/gptneox.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import numpy as np
-from ._base import BaseAdapter
-from typing import Union,Tuple,Optional,BinaryIO 
-from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
-import os
-import torch
-import struct
-import numpy as np
-from ...auto import KnownModels
-
-#based on https://github.com/ggerganov/ggml/tree/master/examples/gpt-neox
-class GptNeoXConverter(BaseAdapter):
-    model_type:KnownModels=KnownModels.GptNeoX
-
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
-        
-        model = AutoModelForCausalLM.from_pretrained(
-            pretrained_model_name_or_path,
-            torch_dtype=torch.float16,
-            low_cpu_mem_usage=True,
-            )
-        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
-        return config,tokenizer,model
-    
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        hyperparameters = self.config.to_dict()
-        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
-        out_file.write(struct.pack("i", hyperparameters["max_position_embeddings"]))
-        out_file.write(struct.pack("i", hyperparameters["hidden_size"]))
-        out_file.write(struct.pack("i", hyperparameters["num_attention_heads"]))
-        out_file.write(struct.pack("i", hyperparameters["num_hidden_layers"]))
-        out_file.write(struct.pack("i", int(hyperparameters["rotary_pct"]*(hyperparameters["hidden_size"]//hyperparameters["num_attention_heads"]))))
-        out_file.write(struct.pack("i", hyperparameters["use_parallel_residual"] if "use_parallel_residual" in hyperparameters else True))
-
-
-    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
-        return name.endswith(".attention.masked_bias") or     \
-       name.endswith(".attention.bias") or \
+import numpy as np
+from ._base import BaseAdapter
+from typing import Union,Tuple,Optional,BinaryIO 
+from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
+import os
+import torch
+import struct
+import numpy as np
+from ...auto import KnownModels
+
+#based on https://github.com/ggerganov/ggml/tree/master/examples/gpt-neox
+class GptNeoXConverter(BaseAdapter):
+    model_type:KnownModels=KnownModels.GptNeoX
+
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
+        
+        model = AutoModelForCausalLM.from_pretrained(
+            pretrained_model_name_or_path,
+            torch_dtype=torch.float16,
+            low_cpu_mem_usage=True,
+            )
+        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
+        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+        return config,tokenizer,model
+    
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        hyperparameters = self.config.to_dict()
+        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
+        out_file.write(struct.pack("i", hyperparameters["max_position_embeddings"]))
+        out_file.write(struct.pack("i", hyperparameters["hidden_size"]))
+        out_file.write(struct.pack("i", hyperparameters["num_attention_heads"]))
+        out_file.write(struct.pack("i", hyperparameters["num_hidden_layers"]))
+        out_file.write(struct.pack("i", int(hyperparameters["rotary_pct"]*(hyperparameters["hidden_size"]//hyperparameters["num_attention_heads"]))))
+        out_file.write(struct.pack("i", hyperparameters["use_parallel_residual"] if "use_parallel_residual" in hyperparameters else True))
+
+
+    def _filter_weights(self, name: str, weight: torch.Tensor) -> bool:
+        return name.endswith(".attention.masked_bias") or     \
+       name.endswith(".attention.bias") or \
        name.endswith(".attention.rotary_emb.inv_freq")
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/llama.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/llama.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-from ._base import BaseAdapter,GGJT_MAGIC
-from typing import Union,Tuple,Optional,BinaryIO,List,Iterable
-from transformers import LlamaConfig,LlamaForCausalLM,LlamaTokenizer,AutoConfig,AutoTokenizer,AutoModelForCausalLM
-import os
-import torch
-import struct
-from ...auto import KnownModels
-import re
-import numpy as np
-import logging
-
-#based on https://github.com/ggerganov/llama.cpp/blob/master/convert.py
-class LlamaConverter(BaseAdapter):
-    model_type:KnownModels=KnownModels.Llama
-    file_magic=GGJT_MAGIC
-
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoConfig,AutoTokenizer,AutoModelForCausalLM]:
-        config = LlamaConfig.from_pretrained(pretrained_model_name_or_path)
-        
-        model = LlamaForCausalLM.from_pretrained(
-            pretrained_model_name_or_path,
-            torch_dtype=torch.float16,
-            low_cpu_mem_usage=True,
-            )
-        
-        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
-        tokenizer = LlamaTokenizer.from_pretrained(tokenizer_name)
-
-        def make_tensors_list() -> List[str]:
-            ret = [
-                'tok_embeddings.weight',
-                'norm.weight',
-                'output.weight',
-            ]
-            for i in range(80):  # maximum number of layer
-                ret += [
-                    f'layers.{i}.attention.wq.weight',
-                    f'layers.{i}.attention.wk.weight',
-                    f'layers.{i}.attention.wv.weight',
-                    f'layers.{i}.attention.wo.weight',
-                    f'layers.{i}.attention_norm.weight',
-                    f'layers.{i}.feed_forward.w1.weight',
-                    f'layers.{i}.feed_forward.w2.weight',
-                    f'layers.{i}.feed_forward.w3.weight',
-                    f'layers.{i}.ffn_norm.weight',
-                ]
-            return ret
-
-        self.TENSORS_LIST = make_tensors_list()
-        self.TENSORS_SET = set(self.TENSORS_LIST)
-
-        self.mapping = {
-            "model.layers.{i}.self_attn.q_proj.weight": "layers.{i}.attention.wq.weight",
-            "model.layers.{i}.self_attn.k_proj.weight": "layers.{i}.attention.wk.weight",
-            "model.layers.{i}.self_attn.v_proj.weight": "layers.{i}.attention.wv.weight",
-            "model.layers.{i}.self_attn.o_proj.weight": "layers.{i}.attention.wo.weight",
-            "model.layers.{i}.mlp.gate_proj.weight": "layers.{i}.feed_forward.w1.weight",
-            "model.layers.{i}.mlp.down_proj.weight": "layers.{i}.feed_forward.w2.weight",
-            "model.layers.{i}.mlp.up_proj.weight": "layers.{i}.feed_forward.w3.weight",
-            "model.layers.{i}.input_layernorm.weight": "layers.{i}.attention_norm.weight",
-            "model.layers.{i}.post_attention_layernorm.weight": "layers.{i}.ffn_norm.weight",
-        }
-
-        return config,tokenizer,model
-    
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        hyperparameters = self.config.to_dict()
-        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
-        out_file.write(struct.pack("i", hyperparameters["hidden_size"]))
-        out_file.write(struct.pack("i", 256))
-        out_file.write(struct.pack("i", hyperparameters["num_attention_heads"]))
-        out_file.write(struct.pack("i", hyperparameters["num_hidden_layers"]))
-        out_file.write(struct.pack("i", hyperparameters["hidden_size"]//hyperparameters["num_attention_heads"])) # rot (obsolete)
-
-    def _rename_weights(self, name: str) -> str:
-        if name == "model.embed_tokens.weight":
-            return "tok_embeddings.weight"
-        elif name == "model.norm.weight":
-            return "norm.weight"
-        elif name == "lm_head.weight":
-            return "output.weight"
-        
-        for old, new in self.mapping.items():
-            pattern = old.replace("{i}", "(\d+)")
-            match = re.fullmatch(pattern, name)
-            if match:
-                return new.replace("{i}", match.group(1))
-            
-        return name
-    
-    def _transform_weights(self, name: str, weight: torch.Tensor) -> torch.Tensor:
-        to_permut = [r"layers.(\d+).attention.wq.weight",r"layers.(\d+).attention.wk.weight"]
-        for pattern in to_permut:
-            match = re.fullmatch(pattern, name)
-            if match:
-                n_heads = self.config.num_attention_heads
-                numpy_weights:np.ndarray = weight.numpy()
-                reshaped = (numpy_weights.reshape(n_heads, 2, numpy_weights.shape[0] // n_heads // 2, *numpy_weights.shape[1:])
-                   .swapaxes(1, 2)
-                   .reshape(numpy_weights.shape))
-                logging.info(f"Permuting {name} from {weight.shape} to {reshaped.shape}")
-                return torch.from_numpy(reshaped)
-        return weight
-    
-    def _filter_weights_after_rename(self, name: str, weight: torch.Tensor) -> bool:
-            return name not in self.TENSORS_SET
-    
-
-    def _write_vocabulary(self,out_file:BinaryIO):
-        sentence_piece_tokenizer = self.tokenizer.sp_model
-
-        logging.info(f"Processing vocabulary with size {self.config.vocab_size}")
-        def sentencepiece_tokens() -> Iterable[Tuple[bytes, float]]:
-            tokenizer = sentence_piece_tokenizer
-            for i in range(tokenizer.vocab_size()):
-                text: bytes
-                if tokenizer.is_unknown(i):
-                    text = " \u2047 ".encode("utf-8")
-                elif tokenizer.is_control(i):
-                    text = b""
-                elif tokenizer.is_byte(i):
-                    piece = tokenizer.id_to_piece(i)
-                    if len(piece) != 6:
-                        raise Exception(f"Invalid token: {piece}")
-                    byte_value = int(piece[3:-1], 16)
-                    text = struct.pack("B", byte_value)
-                else:
-                    text = tokenizer.id_to_piece(i).replace("\u2581", " ").encode("utf-8")
-                score: float = tokenizer.get_score(i)
-                yield text, score
-
-        for text, score in sentencepiece_tokens():
-            out_file.write(struct.pack("i", len(text)))
-            out_file.write(text)
-            out_file.write(struct.pack("f", score))
-
-    
-
+from ._base import BaseAdapter,GGJT_MAGIC
+from typing import Union,Tuple,Optional,BinaryIO,List,Iterable
+from transformers import LlamaConfig,LlamaForCausalLM,LlamaTokenizer,AutoConfig,AutoTokenizer,AutoModelForCausalLM
+import os
+import torch
+import struct
+from ...auto import KnownModels
+import re
+import numpy as np
+import logging
+
+#based on https://github.com/ggerganov/llama.cpp/blob/master/convert.py
+class LlamaConverter(BaseAdapter):
+    model_type:KnownModels=KnownModels.Llama
+    file_magic=GGJT_MAGIC
+
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoConfig,AutoTokenizer,AutoModelForCausalLM]:
+        config = LlamaConfig.from_pretrained(pretrained_model_name_or_path)
+        
+        model = LlamaForCausalLM.from_pretrained(
+            pretrained_model_name_or_path,
+            torch_dtype=torch.float16,
+            low_cpu_mem_usage=True,
+            )
+        
+        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else pretrained_model_name_or_path 
+        tokenizer = LlamaTokenizer.from_pretrained(tokenizer_name)
+
+        def make_tensors_list() -> List[str]:
+            ret = [
+                'tok_embeddings.weight',
+                'norm.weight',
+                'output.weight',
+            ]
+            for i in range(80):  # maximum number of layer
+                ret += [
+                    f'layers.{i}.attention.wq.weight',
+                    f'layers.{i}.attention.wk.weight',
+                    f'layers.{i}.attention.wv.weight',
+                    f'layers.{i}.attention.wo.weight',
+                    f'layers.{i}.attention_norm.weight',
+                    f'layers.{i}.feed_forward.w1.weight',
+                    f'layers.{i}.feed_forward.w2.weight',
+                    f'layers.{i}.feed_forward.w3.weight',
+                    f'layers.{i}.ffn_norm.weight',
+                ]
+            return ret
+
+        self.TENSORS_LIST = make_tensors_list()
+        self.TENSORS_SET = set(self.TENSORS_LIST)
+
+        self.mapping = {
+            "model.layers.{i}.self_attn.q_proj.weight": "layers.{i}.attention.wq.weight",
+            "model.layers.{i}.self_attn.k_proj.weight": "layers.{i}.attention.wk.weight",
+            "model.layers.{i}.self_attn.v_proj.weight": "layers.{i}.attention.wv.weight",
+            "model.layers.{i}.self_attn.o_proj.weight": "layers.{i}.attention.wo.weight",
+            "model.layers.{i}.mlp.gate_proj.weight": "layers.{i}.feed_forward.w1.weight",
+            "model.layers.{i}.mlp.down_proj.weight": "layers.{i}.feed_forward.w2.weight",
+            "model.layers.{i}.mlp.up_proj.weight": "layers.{i}.feed_forward.w3.weight",
+            "model.layers.{i}.input_layernorm.weight": "layers.{i}.attention_norm.weight",
+            "model.layers.{i}.post_attention_layernorm.weight": "layers.{i}.ffn_norm.weight",
+        }
+
+        return config,tokenizer,model
+    
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        hyperparameters = self.config.to_dict()
+        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
+        out_file.write(struct.pack("i", hyperparameters["hidden_size"]))
+        out_file.write(struct.pack("i", 256))
+        out_file.write(struct.pack("i", hyperparameters["num_attention_heads"]))
+        out_file.write(struct.pack("i", hyperparameters["num_hidden_layers"]))
+        out_file.write(struct.pack("i", hyperparameters["hidden_size"]//hyperparameters["num_attention_heads"])) # rot (obsolete)
+
+    def _rename_weights(self, name: str) -> str:
+        if name == "model.embed_tokens.weight":
+            return "tok_embeddings.weight"
+        elif name == "model.norm.weight":
+            return "norm.weight"
+        elif name == "lm_head.weight":
+            return "output.weight"
+        
+        for old, new in self.mapping.items():
+            pattern = old.replace("{i}", "(\d+)")
+            match = re.fullmatch(pattern, name)
+            if match:
+                return new.replace("{i}", match.group(1))
+            
+        return name
+    
+    def _transform_weights(self, name: str, weight: torch.Tensor) -> torch.Tensor:
+        to_permut = [r"layers.(\d+).attention.wq.weight",r"layers.(\d+).attention.wk.weight"]
+        for pattern in to_permut:
+            match = re.fullmatch(pattern, name)
+            if match:
+                n_heads = self.config.num_attention_heads
+                numpy_weights:np.ndarray = weight.numpy()
+                reshaped = (numpy_weights.reshape(n_heads, 2, numpy_weights.shape[0] // n_heads // 2, *numpy_weights.shape[1:])
+                   .swapaxes(1, 2)
+                   .reshape(numpy_weights.shape))
+                logging.info(f"Permuting {name} from {weight.shape} to {reshaped.shape}")
+                return torch.from_numpy(reshaped)
+        return weight
+    
+    def _filter_weights_after_rename(self, name: str, weight: torch.Tensor) -> bool:
+            return name not in self.TENSORS_SET
+    
+
+    def _write_vocabulary(self,out_file:BinaryIO):
+        sentence_piece_tokenizer = self.tokenizer.sp_model
+
+        logging.info(f"Processing vocabulary with size {self.config.vocab_size}")
+        def sentencepiece_tokens() -> Iterable[Tuple[bytes, float]]:
+            tokenizer = sentence_piece_tokenizer
+            for i in range(tokenizer.vocab_size()):
+                text: bytes
+                if tokenizer.is_unknown(i):
+                    text = " \u2047 ".encode("utf-8")
+                elif tokenizer.is_control(i):
+                    text = b""
+                elif tokenizer.is_byte(i):
+                    piece = tokenizer.id_to_piece(i)
+                    if len(piece) != 6:
+                        raise Exception(f"Invalid token: {piece}")
+                    byte_value = int(piece[3:-1], 16)
+                    text = struct.pack("B", byte_value)
+                else:
+                    text = tokenizer.id_to_piece(i).replace("\u2581", " ").encode("utf-8")
+                score: float = tokenizer.get_score(i)
+                yield text, score
+
+        for text, score in sentencepiece_tokens():
+            out_file.write(struct.pack("i", len(text)))
+            out_file.write(text)
+            out_file.write(struct.pack("f", score))
+
+    
+
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/convert/models/mpt.py` & `llm_rs_metal-0.2.12/llm_rs/convert/models/mpt.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from ._base import BaseAdapter
-from typing import Union,Tuple,Optional,BinaryIO 
-from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
-import os
-import torch
-import struct
-from ...auto import KnownModels
-
-#based on https://github.com/ggerganov/ggml/blob/master/examples/mpt/convert-h5-to-ggml.py
-class MPTConverter(BaseAdapter):
-    model_type:KnownModels=KnownModels.Mpt
-    
-    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path,trust_remote_code=True)
-        
-        model = AutoModelForCausalLM.from_pretrained(
-            pretrained_model_name_or_path,
-            torch_dtype=torch.float16,
-            trust_remote_code=True,
-            low_cpu_mem_usage=True,
-            )
-        
-        #MPT uses the `EleutherAI/gpt-neox-20b` tokenizer => use it if no tokenizer is specified
-        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else "EleutherAI/gpt-neox-20b" 
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
-        return config,tokenizer,model
-    
-    def _write_hyperparameters(self,out_file:BinaryIO):
-        hyperparameters = self.config.to_dict()
-        out_file.write(struct.pack("i", hyperparameters["d_model"]))
-        out_file.write(struct.pack("i", hyperparameters["max_seq_len"]))
-        out_file.write(struct.pack("i", hyperparameters["n_heads"]))
-        out_file.write(struct.pack("i", hyperparameters["n_layers"]))
-        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
-        out_file.write(struct.pack("f", hyperparameters["attn_config"]["alibi_bias_max"]))
+from ._base import BaseAdapter
+from typing import Union,Tuple,Optional,BinaryIO 
+from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
+import os
+import torch
+import struct
+from ...auto import KnownModels
+
+#based on https://github.com/ggerganov/ggml/blob/master/examples/mpt/convert-h5-to-ggml.py
+class MPTConverter(BaseAdapter):
+    model_type:KnownModels=KnownModels.Mpt
+    
+    def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoTokenizer,AutoModelForCausalLM]:
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path,trust_remote_code=True)
+        
+        model = AutoModelForCausalLM.from_pretrained(
+            pretrained_model_name_or_path,
+            torch_dtype=torch.float16,
+            trust_remote_code=True,
+            low_cpu_mem_usage=True,
+            )
+        
+        #MPT uses the `EleutherAI/gpt-neox-20b` tokenizer => use it if no tokenizer is specified
+        tokenizer_name = pretrained_tokenizer_name_or_path if pretrained_tokenizer_name_or_path else "EleutherAI/gpt-neox-20b" 
+        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+        return config,tokenizer,model
+    
+    def _write_hyperparameters(self,out_file:BinaryIO):
+        hyperparameters = self.config.to_dict()
+        out_file.write(struct.pack("i", hyperparameters["d_model"]))
+        out_file.write(struct.pack("i", hyperparameters["max_seq_len"]))
+        out_file.write(struct.pack("i", hyperparameters["n_heads"]))
+        out_file.write(struct.pack("i", hyperparameters["n_layers"]))
+        out_file.write(struct.pack("i", hyperparameters["vocab_size"]))
+        out_file.write(struct.pack("f", hyperparameters["attn_config"]["alibi_bias_max"]))
         out_file.write(struct.pack("f", hyperparameters["attn_config"]["clip_qkv"] or 0.0))
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/models.pyi` & `llm_rs_metal-0.2.12/llm_rs/models.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from .base_model import Model
-    
-class Llama(Model):
-    """
-    Wrapper around all Llama based models.
-    """
-    ...
-    
-    
-class GptJ(Model):
-    """
-    Wrapper around all GPTJ based models.
-    """
-    ...
-    
-class Gpt2(Model):
-    """
-    Wrapper around all GPT2 based models.
-    """
-    ...
-    
-class Bloom(Model):
-    """
-    Wrapper around all Bloom based models.
-    """
-    ...
-    
-class GptNeoX(Model):
-    """
-    Wrapper around all GPT-NeoX based models.
-    """
-    ...
-
-class Mpt(Model):
-    """
-    Wrapper around all Mpt based models.
-    """
+from .base_model import Model
+    
+class Llama(Model):
+    """
+    Wrapper around all Llama based models.
+    """
+    ...
+    
+    
+class GptJ(Model):
+    """
+    Wrapper around all GPTJ based models.
+    """
+    ...
+    
+class Gpt2(Model):
+    """
+    Wrapper around all GPT2 based models.
+    """
+    ...
+    
+class Bloom(Model):
+    """
+    Wrapper around all Bloom based models.
+    """
+    ...
+    
+class GptNeoX(Model):
+    """
+    Wrapper around all GPT-NeoX based models.
+    """
+    ...
+
+class Mpt(Model):
+    """
+    Wrapper around all Mpt based models.
+    """
     ...
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/repository.py` & `llm_rs_metal-0.2.12/llm_rs/repository.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from huggingface_hub import HfApi, CommitOperationAdd, CommitOperationDelete
-from huggingface_hub import create_repo,metadata_update,cached_assets_path
-from typing import List, Optional, Union
-import json
-import os
-import pathlib
-import logging 
-
-class Repository():
-    def __init__(self,name:str,user_or_organization:Optional[str]=None,token:Optional[str]=None,private:bool=False) -> None:
-        
-        self.name = f"{user_or_organization}/{name}" if user_or_organization else name
-        self.api = HfApi(token=token)
-
-        try:
-            self.url = str(create_repo(self.name,token=token,private=private))
-            self.name = self.url.replace(f"{self.api.endpoint}/","")
-            # Uplaod the config file
-            config_path = cached_assets_path("llm-rs",namespace=self.name) / "config.json"
-            with open(config_path,"w") as f:
-                f.write(json.dumps({"repo_type":"GGML"}))
-            self.api.create_commit(
-                self.name,
-                operations=[CommitOperationAdd(path_in_repo="config.json", path_or_fileobj=config_path)],
-                commit_message="Auto initialized repo via llm-rs",)
-            
-            metadata={}
-            metadata["pipeline_tag"]= "text-generation"
-            metadata["tags"] = ["llm-rs","ggml"]
-            metadata_update(self.name, metadata, token=token)
-            
-        except Exception as e:
-            self.url = create_repo(self.name,token=token,private=private,exist_ok=True)
-            self.name = self.url.replace(f"{self.api.endpoint}/","")
-
-    def upload(self,model_file:Union[str,os.PathLike],delete_old:bool=True):
-        # search for the metadata file
-        path = pathlib.Path(model_file)
-        metadata_path = path.with_suffix(".meta")
-
-        if not path.exists():
-            raise FileNotFoundError(f"Could not find model file {model_file}")
-        
-        if delete_old:
-            to_delete = [path.name]
-            if metadata_path.exists():
-                to_delete.append(metadata_path.name)
-
-            for n in to_delete:
-                try:
-                    self.api.create_commit(
-                        self.name,
-                        operations=[CommitOperationDelete(path_in_repo=n,is_folder=False)],
-                        commit_message=f"Delete old file: '{n}'",
-                        )
-                except Exception as e:
-                    logging.error(f"Could not delete old file {n} from repo {self.name}")
-            
-
-        upload_operations = [CommitOperationAdd(path_in_repo=path.name, path_or_fileobj=path)] 
-        if metadata_path.exists():
-            upload_operations.append(CommitOperationAdd(path_in_repo=metadata_path.name, path_or_fileobj=metadata_path))
-        
-        self.api.create_commit(
-            self.name,
-            upload_operations,
-            commit_message=f"Upload new model file: '{path.name}'",)
-
+from huggingface_hub import HfApi, CommitOperationAdd, CommitOperationDelete
+from huggingface_hub import create_repo,metadata_update,cached_assets_path
+from typing import List, Optional, Union
+import json
+import os
+import pathlib
+import logging 
+
+class Repository():
+    def __init__(self,name:str,user_or_organization:Optional[str]=None,token:Optional[str]=None,private:bool=False) -> None:
+        
+        self.name = f"{user_or_organization}/{name}" if user_or_organization else name
+        self.api = HfApi(token=token)
+
+        try:
+            self.url = str(create_repo(self.name,token=token,private=private))
+            self.name = self.url.replace(f"{self.api.endpoint}/","")
+            # Uplaod the config file
+            config_path = cached_assets_path("llm-rs",namespace=self.name) / "config.json"
+            with open(config_path,"w") as f:
+                f.write(json.dumps({"repo_type":"GGML"}))
+            self.api.create_commit(
+                self.name,
+                operations=[CommitOperationAdd(path_in_repo="config.json", path_or_fileobj=config_path)],
+                commit_message="Auto initialized repo via llm-rs",)
+            
+            metadata={}
+            metadata["pipeline_tag"]= "text-generation"
+            metadata["tags"] = ["llm-rs","ggml"]
+            metadata_update(self.name, metadata, token=token)
+            
+        except Exception as e:
+            self.url = create_repo(self.name,token=token,private=private,exist_ok=True)
+            self.name = self.url.replace(f"{self.api.endpoint}/","")
+
+    def upload(self,model_file:Union[str,os.PathLike],delete_old:bool=True):
+        # search for the metadata file
+        path = pathlib.Path(model_file)
+        metadata_path = path.with_suffix(".meta")
+
+        if not path.exists():
+            raise FileNotFoundError(f"Could not find model file {model_file}")
+        
+        if delete_old:
+            to_delete = [path.name]
+            if metadata_path.exists():
+                to_delete.append(metadata_path.name)
+
+            for n in to_delete:
+                try:
+                    self.api.create_commit(
+                        self.name,
+                        operations=[CommitOperationDelete(path_in_repo=n,is_folder=False)],
+                        commit_message=f"Delete old file: '{n}'",
+                        )
+                except Exception as e:
+                    logging.error(f"Could not delete old file {n} from repo {self.name}")
+            
+
+        upload_operations = [CommitOperationAdd(path_in_repo=path.name, path_or_fileobj=path)] 
+        if metadata_path.exists():
+            upload_operations.append(CommitOperationAdd(path_in_repo=metadata_path.name, path_or_fileobj=metadata_path))
+        
+        self.api.create_commit(
+            self.name,
+            upload_operations,
+            commit_message=f"Upload new model file: '{path.name}'",)
+
```

### Comparing `llm-rs-metal-0.0.1/llm_rs/results.pyi` & `llm_rs_metal-0.2.12/llm_rs/results.pyi`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from enum import Enum
-
-class StopReason(Enum):
-    """
-    The reason why generation was stopped.
-    """
-    EndToken=0,
-    MaxLength=1,
-    UserCancelled=2
-
-class GenerationTimes():
-    """
-    Contains the time taken for each step of generation in milliseconds.
-    """
-    @property
-    def total(self)->int: ...
-    @property
-    def generation(self)->int: ...
-    @property
-    def prompt_feeding(self)->int: ...
-    
-class GenerationResult():
-    """
-    Containes the result of a generation and the time taken for each step.
-    """
-    @property
-    def text(self)->str: ...
-    @property
-    def times(self)->GenerationTimes: ...
-    @property
+from enum import Enum
+
+class StopReason(Enum):
+    """
+    The reason why generation was stopped.
+    """
+    EndToken=0,
+    MaxLength=1,
+    UserCancelled=2
+
+class GenerationTimes():
+    """
+    Contains the time taken for each step of generation in milliseconds.
+    """
+    @property
+    def total(self)->int: ...
+    @property
+    def generation(self)->int: ...
+    @property
+    def prompt_feeding(self)->int: ...
+    
+class GenerationResult():
+    """
+    Containes the result of a generation and the time taken for each step.
+    """
+    @property
+    def text(self)->str: ...
+    @property
+    def times(self)->GenerationTimes: ...
+    @property
     def stop_reason(self)->StopReason: ...
```

### Comparing `llm-rs-metal-0.0.1/src/configs.rs` & `llm_rs_metal-0.2.12/src/configs.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,258 +1,274 @@
-use crate::stopwords::StopWordHandler;
-use llm::{InferenceParameters, InferenceSessionConfig, ModelKVMemoryType, TokenBias};
-use pyo3::{prelude::*, types::PyBytes};
-use serde::{Deserialize, Serialize};
-
-#[pyclass]
-#[pyo3(module = "llm_rs.config")]
-#[derive(Clone, Serialize, Deserialize)]
-pub struct GenerationConfig {
-    #[pyo3(get, set)]
-    pub top_k: usize,
-    #[pyo3(get, set)]
-    pub top_p: f32,
-    #[pyo3(get, set)]
-    pub temperature: f32,
-    #[pyo3(get, set)]
-    pub repetition_penalty: f32,
-    #[pyo3(get, set)]
-    pub repetition_penalty_last_n: usize,
-    #[pyo3(get, set)]
-    pub seed: u64,
-    #[pyo3(get, set)]
-    pub max_new_tokens: Option<usize>,
-    #[pyo3(get, set)]
-    pub stop_words: Option<Vec<String>>,
-    pub stop_word_handler: Option<StopWordHandler>,
-}
-
-impl Default for GenerationConfig {
-    fn default() -> Self {
-        Self {
-            top_k: 40,
-            top_p: 0.95,
-            temperature: 0.80,
-            repetition_penalty: 1.30,
-            repetition_penalty_last_n: 512,
-            seed: 42,
-            max_new_tokens: None,
-            stop_words: None,
-            stop_word_handler: None,
-        }
-    }
-}
-
-impl GenerationConfig {
-    pub fn init_stop_words(&mut self, model: &dyn llm::Model) {
-        if self.stop_words.is_some() {
-            let stopwords = self.stop_words.clone().unwrap();
-            self.stop_word_handler = Some(StopWordHandler::new(model, &stopwords));
-        } else {
-            self.stop_word_handler = None;
-        }
-    }
-}
-
-#[pymethods]
-impl GenerationConfig {
-    #[new]
-    #[allow(clippy::too_many_arguments)]
-    fn new(
-        top_k: Option<usize>,
-        top_p: Option<f32>,
-        temperature: Option<f32>,
-        repetition_penalty: Option<f32>,
-        repetition_penalty_last_n: Option<usize>,
-        seed: Option<u64>,
-        max_new_tokens: Option<usize>,
-        stop_words: Option<Vec<String>>,
-    ) -> Self {
-        GenerationConfig {
-            top_k: top_k.unwrap_or(40),
-            top_p: top_p.unwrap_or(0.95),
-            temperature: temperature.unwrap_or(0.80),
-            repetition_penalty: repetition_penalty.unwrap_or(1.30),
-            repetition_penalty_last_n: repetition_penalty_last_n.unwrap_or(512),
-            seed: seed.unwrap_or(42),
-            max_new_tokens,
-            stop_words,
-            stop_word_handler: None,
-        }
-    }
-
-    pub fn __setstate__(&mut self, state: &PyBytes) -> PyResult<()> {
-        *self = serde_json::from_slice(state.as_bytes()).unwrap();
-        Ok(())
-    }
-    pub fn __getstate__<'py>(&self, py: Python<'py>) -> PyResult<&'py PyBytes> {
-        Ok(PyBytes::new(py, &serde_json::to_vec(&self).unwrap()))
-    }
-
-    #[allow(clippy::type_complexity)]
-    pub fn __getnewargs__(
-        &self,
-    ) -> PyResult<(
-        usize,
-        f32,
-        f32,
-        f32,
-        usize,
-        u64,
-        Option<usize>,
-        Option<Vec<String>>,
-    )> {
-        Ok((
-            self.top_k,
-            self.top_p,
-            self.temperature,
-            self.repetition_penalty,
-            self.repetition_penalty_last_n,
-            self.seed,
-            self.max_new_tokens,
-            self.stop_words.clone(),
-        ))
-    }
-}
-
-impl GenerationConfig {
-    pub fn to_llm_params(&self, n_threads: usize, n_batch: usize) -> InferenceParameters {
-        InferenceParameters {
-            n_threads,
-            n_batch,
-            sampler: std::sync::Arc::new(llm::samplers::TopPTopK {
-                top_k: self.top_k,
-                top_p: self.top_p,
-                temperature: self.temperature,
-                repeat_penalty: self.repetition_penalty,
-                repetition_penalty_last_n: self.repetition_penalty_last_n,
-                bias_tokens: TokenBias::default(),
-            }),
-        }
-    }
-}
-
-#[pyclass]
-#[pyo3(module = "llm_rs.config")]
-#[derive(Clone, Copy, Debug, PartialEq, Serialize, Deserialize)]
-pub enum Precision {
-    FP32,
-    FP16,
-}
-
-#[pymethods]
-impl Precision {
-    #[new]
-    fn new(value: usize) -> Self {
-        match value {
-            16 => Precision::FP16,
-            32 => Precision::FP32,
-            _ => panic!("Invalid precision value"),
-        }
-    }
-
-    pub fn __setstate__(&mut self, state: &PyBytes) -> PyResult<()> {
-        *self = serde_json::from_slice(state.as_bytes()).unwrap();
-        Ok(())
-    }
-    pub fn __getstate__<'py>(&self, py: Python<'py>) -> PyResult<&'py PyBytes> {
-        Ok(PyBytes::new(py, &serde_json::to_vec(&self).unwrap()))
-    }
-
-    pub fn __getnewargs__(&self) -> PyResult<(usize,)> {
-        //Hack to get pyo3 enum pickle serializable
-        match self {
-            Precision::FP16 => Ok((16_usize,)),
-            Precision::FP32 => Ok((32_usize,)),
-        }
-    }
-}
-
-impl Precision {
-    pub fn to_llama_rs_memory_type(self) -> ModelKVMemoryType {
-        match self {
-            Precision::FP16 => ModelKVMemoryType::Float16,
-            Precision::FP32 => ModelKVMemoryType::Float32,
-        }
-    }
-}
-
-#[pyclass]
-#[pyo3(module = "llm_rs.config")]
-#[derive(Clone, Copy, Serialize, Deserialize)]
-pub struct SessionConfig {
-    #[pyo3(get, set)]
-    pub threads: usize,
-    #[pyo3(get, set)]
-    pub batch_size: usize,
-    #[pyo3(get)]
-    pub context_length: usize,
-    #[pyo3(get, set)]
-    pub keys_memory_type: Precision,
-    #[pyo3(get, set)]
-    pub values_memory_type: Precision,
-    #[pyo3(get)]
-    pub prefer_mmap: bool,
-}
-
-impl Default for SessionConfig {
-    fn default() -> Self {
-        Self {
-            threads: 8,
-            batch_size: 8,
-            context_length: 2048,
-            keys_memory_type: Precision::FP16,
-            values_memory_type: Precision::FP16,
-            prefer_mmap: true,
-        }
-    }
-}
-
-#[pymethods]
-impl SessionConfig {
-    #[new]
-    #[allow(clippy::too_many_arguments)]
-    fn new(
-        threads: Option<usize>,
-        batch_size: Option<usize>,
-        context_length: Option<usize>,
-        keys_memory_type: Option<Precision>,
-        values_memory_type: Option<Precision>,
-        prefer_mmap: Option<bool>,
-    ) -> Self {
-        SessionConfig {
-            threads: threads.unwrap_or(8),
-            batch_size: batch_size.unwrap_or(8),
-            context_length: context_length.unwrap_or(2048),
-            keys_memory_type: keys_memory_type.unwrap_or(Precision::FP16),
-            values_memory_type: values_memory_type.unwrap_or(Precision::FP16),
-            prefer_mmap: prefer_mmap.unwrap_or(true),
-        }
-    }
-
-    pub fn __setstate__(&mut self, state: &PyBytes) -> PyResult<()> {
-        *self = serde_json::from_slice(state.as_bytes()).unwrap();
-        Ok(())
-    }
-    pub fn __getstate__<'py>(&self, py: Python<'py>) -> PyResult<&'py PyBytes> {
-        Ok(PyBytes::new(py, &serde_json::to_vec(&self).unwrap()))
-    }
-    pub fn __getnewargs__(&self) -> PyResult<(usize, usize, usize, Precision, Precision, bool)> {
-        Ok((
-            self.threads,
-            self.batch_size,
-            self.context_length,
-            self.keys_memory_type,
-            self.values_memory_type,
-            self.prefer_mmap,
-        ))
-    }
-}
-
-impl SessionConfig {
-    pub fn to_llm_params(self) -> InferenceSessionConfig {
-        InferenceSessionConfig {
-            memory_k_type: self.keys_memory_type.to_llama_rs_memory_type(),
-            memory_v_type: self.values_memory_type.to_llama_rs_memory_type(),
-        }
-    }
-}
+use crate::stopwords::StopWordHandler;
+use llm::{InferenceParameters, InferenceSessionConfig, ModelKVMemoryType, TokenBias};
+use pyo3::{prelude::*, types::PyBytes};
+use serde::{Deserialize, Serialize};
+
+#[pyclass]
+#[pyo3(module = "llm_rs.config")]
+#[derive(Clone, Serialize, Deserialize)]
+pub struct GenerationConfig {
+    #[pyo3(get, set)]
+    pub top_k: usize,
+    #[pyo3(get, set)]
+    pub top_p: f32,
+    #[pyo3(get, set)]
+    pub temperature: f32,
+    #[pyo3(get, set)]
+    pub repetition_penalty: f32,
+    #[pyo3(get, set)]
+    pub repetition_penalty_last_n: usize,
+    #[pyo3(get, set)]
+    pub seed: u64,
+    #[pyo3(get, set)]
+    pub max_new_tokens: Option<usize>,
+    #[pyo3(get, set)]
+    pub stop_words: Option<Vec<String>>,
+    pub stop_word_handler: Option<StopWordHandler>,
+}
+
+impl Default for GenerationConfig {
+    fn default() -> Self {
+        Self {
+            top_k: 40,
+            top_p: 0.95,
+            temperature: 0.80,
+            repetition_penalty: 1.30,
+            repetition_penalty_last_n: 512,
+            seed: 42,
+            max_new_tokens: None,
+            stop_words: None,
+            stop_word_handler: None,
+        }
+    }
+}
+
+impl GenerationConfig {
+    pub fn init_stop_words(&mut self, model: &dyn llm::Model) {
+        if self.stop_words.is_some() {
+            let stopwords = self.stop_words.clone().unwrap();
+            self.stop_word_handler = Some(StopWordHandler::new(model, &stopwords));
+        } else {
+            self.stop_word_handler = None;
+        }
+    }
+}
+
+#[pymethods]
+impl GenerationConfig {
+    #[new]
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        top_k: Option<usize>,
+        top_p: Option<f32>,
+        temperature: Option<f32>,
+        repetition_penalty: Option<f32>,
+        repetition_penalty_last_n: Option<usize>,
+        seed: Option<u64>,
+        max_new_tokens: Option<usize>,
+        stop_words: Option<Vec<String>>,
+    ) -> Self {
+        GenerationConfig {
+            top_k: top_k.unwrap_or(40),
+            top_p: top_p.unwrap_or(0.95),
+            temperature: temperature.unwrap_or(0.80),
+            repetition_penalty: repetition_penalty.unwrap_or(1.30),
+            repetition_penalty_last_n: repetition_penalty_last_n.unwrap_or(512),
+            seed: seed.unwrap_or(42),
+            max_new_tokens,
+            stop_words,
+            stop_word_handler: None,
+        }
+    }
+
+    pub fn __setstate__(&mut self, state: &PyBytes) -> PyResult<()> {
+        *self = serde_json::from_slice(state.as_bytes()).unwrap();
+        Ok(())
+    }
+    pub fn __getstate__<'py>(&self, py: Python<'py>) -> PyResult<&'py PyBytes> {
+        Ok(PyBytes::new(py, &serde_json::to_vec(&self).unwrap()))
+    }
+
+    #[allow(clippy::type_complexity)]
+    pub fn __getnewargs__(
+        &self,
+    ) -> PyResult<(
+        usize,
+        f32,
+        f32,
+        f32,
+        usize,
+        u64,
+        Option<usize>,
+        Option<Vec<String>>,
+    )> {
+        Ok((
+            self.top_k,
+            self.top_p,
+            self.temperature,
+            self.repetition_penalty,
+            self.repetition_penalty_last_n,
+            self.seed,
+            self.max_new_tokens,
+            self.stop_words.clone(),
+        ))
+    }
+}
+
+impl GenerationConfig {
+    pub fn to_llm_params(&self, n_threads: usize) -> InferenceParameters {
+        InferenceParameters {
+            n_threads,
+            sampler: std::sync::Arc::new(llm::samplers::TopPTopK {
+                top_k: self.top_k,
+                top_p: self.top_p,
+                temperature: self.temperature,
+                repeat_penalty: self.repetition_penalty,
+                repetition_penalty_last_n: self.repetition_penalty_last_n,
+                bias_tokens: TokenBias::default(),
+            }),
+        }
+    }
+}
+
+#[pyclass]
+#[pyo3(module = "llm_rs.config")]
+#[derive(Clone, Copy, Debug, PartialEq, Serialize, Deserialize)]
+pub enum Precision {
+    FP32,
+    FP16,
+}
+
+#[pymethods]
+impl Precision {
+    #[new]
+    fn new(value: usize) -> Self {
+        match value {
+            16 => Precision::FP16,
+            32 => Precision::FP32,
+            _ => panic!("Invalid precision value"),
+        }
+    }
+
+    pub fn __setstate__(&mut self, state: &PyBytes) -> PyResult<()> {
+        *self = serde_json::from_slice(state.as_bytes()).unwrap();
+        Ok(())
+    }
+    pub fn __getstate__<'py>(&self, py: Python<'py>) -> PyResult<&'py PyBytes> {
+        Ok(PyBytes::new(py, &serde_json::to_vec(&self).unwrap()))
+    }
+
+    pub fn __getnewargs__(&self) -> PyResult<(usize,)> {
+        //Hack to get pyo3 enum pickle serializable
+        match self {
+            Precision::FP16 => Ok((16_usize,)),
+            Precision::FP32 => Ok((32_usize,)),
+        }
+    }
+}
+
+impl Precision {
+    pub fn to_llama_rs_memory_type(self) -> ModelKVMemoryType {
+        match self {
+            Precision::FP16 => ModelKVMemoryType::Float16,
+            Precision::FP32 => ModelKVMemoryType::Float32,
+        }
+    }
+}
+
+#[pyclass]
+#[pyo3(module = "llm_rs.config")]
+#[derive(Clone, Copy, Serialize, Deserialize)]
+pub struct SessionConfig {
+    #[pyo3(get, set)]
+    pub threads: usize,
+    #[pyo3(get, set)]
+    pub batch_size: usize,
+    #[pyo3(get)]
+    pub context_length: usize,
+    #[pyo3(get, set)]
+    pub keys_memory_type: Precision,
+    #[pyo3(get, set)]
+    pub values_memory_type: Precision,
+    #[pyo3(get)]
+    pub prefer_mmap: bool,
+    #[pyo3(get)]
+    pub use_gpu: bool,
+    #[pyo3(get)]
+    pub gpu_layers: Option<usize>,
+}
+
+impl Default for SessionConfig {
+    fn default() -> Self {
+        Self {
+            threads: 8,
+            batch_size: 8,
+            context_length: 2048,
+            keys_memory_type: Precision::FP16,
+            values_memory_type: Precision::FP16,
+            prefer_mmap: true,
+            use_gpu: false,
+            gpu_layers: None,
+        }
+    }
+}
+
+#[pymethods]
+impl SessionConfig {
+    #[new]
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        threads: Option<usize>,
+        batch_size: Option<usize>,
+        context_length: Option<usize>,
+        keys_memory_type: Option<Precision>,
+        values_memory_type: Option<Precision>,
+        prefer_mmap: Option<bool>,
+        use_gpu: Option<bool>,
+        gpu_layers: Option<usize>,
+    ) -> Self {
+        SessionConfig {
+            threads: threads.unwrap_or(8),
+            batch_size: batch_size.unwrap_or(8),
+            context_length: context_length.unwrap_or(2048),
+            keys_memory_type: keys_memory_type.unwrap_or(Precision::FP16),
+            values_memory_type: values_memory_type.unwrap_or(Precision::FP16),
+            prefer_mmap: prefer_mmap.unwrap_or(true),
+            use_gpu: use_gpu.unwrap_or(false),
+            gpu_layers,
+        }
+    }
+
+    pub fn __setstate__(&mut self, state: &PyBytes) -> PyResult<()> {
+        *self = serde_json::from_slice(state.as_bytes()).unwrap();
+        Ok(())
+    }
+    pub fn __getstate__<'py>(&self, py: Python<'py>) -> PyResult<&'py PyBytes> {
+        Ok(PyBytes::new(py, &serde_json::to_vec(&self).unwrap()))
+    }
+    #[allow(clippy::type_complexity)]
+    pub fn __getnewargs__(
+        &self,
+    ) -> PyResult<(usize, usize, usize, Precision, Precision, bool, bool, usize)> {
+        Ok((
+            self.threads,
+            self.batch_size,
+            self.context_length,
+            self.keys_memory_type,
+            self.values_memory_type,
+            self.prefer_mmap,
+            self.use_gpu,
+            self.gpu_layers.unwrap_or(0),
+        ))
+    }
+}
+
+impl SessionConfig {
+    pub fn to_llm_params(self) -> InferenceSessionConfig {
+        InferenceSessionConfig {
+            memory_k_type: self.keys_memory_type.to_llama_rs_memory_type(),
+            memory_v_type: self.values_memory_type.to_llama_rs_memory_type(),
+            n_batch: self.batch_size,
+            use_gpu: self.use_gpu,
+        }
+    }
+}
```

### Comparing `llm-rs-metal-0.0.1/src/lib.rs` & `llm_rs_metal-0.2.12/src/lib.rs`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-use pyo3::prelude::*;
-
-mod configs;
-mod model_base;
-mod models;
-mod quantize;
-mod results;
-mod stopwords;
-
-#[pymodule]
-fn llm_rs(_py: Python, m: &PyModule) -> PyResult<()> {
-    let config_module = PyModule::new(_py, "config")?;
-    config_module.add_class::<configs::GenerationConfig>()?;
-    config_module.add_class::<configs::Precision>()?;
-    config_module.add_class::<configs::SessionConfig>()?;
-    config_module.add_class::<quantize::ContainerType>()?;
-    config_module.add_class::<quantize::QuantizationType>()?;
-    m.add_submodule(config_module)?;
-
-    let results_module = PyModule::new(_py, "results")?;
-    results_module.add_class::<results::GenerationTimes>()?;
-    results_module.add_class::<results::StopReason>()?;
-    results_module.add_class::<results::GenerationResult>()?;
-    m.add_submodule(results_module)?;
-
-    let models_module = PyModule::new(_py, "models")?;
-    models_module.add_class::<models::Llama>()?;
-    models_module.add_class::<models::GptJ>()?;
-    models_module.add_class::<models::Gpt2>()?;
-    models_module.add_class::<models::GptNeoX>()?;
-    models_module.add_class::<models::Bloom>()?;
-    models_module.add_class::<models::Mpt>()?;
-    m.add_submodule(models_module)?;
-
-    //hacky but apparently the only way to get a submodule to work on all platforms with typehints
-    //see https://github.com/PyO3/pyo3/issues/759
-    _py.import("sys")?
-        .getattr("modules")?
-        .set_item("llm_rs.config", config_module)?;
-
-    _py.import("sys")?
-        .getattr("modules")?
-        .set_item("llm_rs.results", results_module)?;
-
-    _py.import("sys")?
-        .getattr("modules")?
-        .set_item("llm_rs.models", models_module)?;
-
-    Ok(())
-}
+use pyo3::prelude::*;
+
+mod configs;
+mod model_base;
+mod models;
+mod quantize;
+mod results;
+mod stopwords;
+
+#[pymodule]
+fn llm_rs(_py: Python, m: &PyModule) -> PyResult<()> {
+    let config_module = PyModule::new(_py, "config")?;
+    config_module.add_class::<configs::GenerationConfig>()?;
+    config_module.add_class::<configs::Precision>()?;
+    config_module.add_class::<configs::SessionConfig>()?;
+    config_module.add_class::<quantize::ContainerType>()?;
+    config_module.add_class::<quantize::QuantizationType>()?;
+    m.add_submodule(config_module)?;
+
+    let results_module = PyModule::new(_py, "results")?;
+    results_module.add_class::<results::GenerationTimes>()?;
+    results_module.add_class::<results::StopReason>()?;
+    results_module.add_class::<results::GenerationResult>()?;
+    m.add_submodule(results_module)?;
+
+    let models_module = PyModule::new(_py, "models")?;
+    models_module.add_class::<models::Llama>()?;
+    models_module.add_class::<models::GptJ>()?;
+    models_module.add_class::<models::Gpt2>()?;
+    models_module.add_class::<models::GptNeoX>()?;
+    models_module.add_class::<models::Bloom>()?;
+    models_module.add_class::<models::Mpt>()?;
+    m.add_submodule(models_module)?;
+
+    //hacky but apparently the only way to get a submodule to work on all platforms with typehints
+    //see https://github.com/PyO3/pyo3/issues/759
+    _py.import("sys")?
+        .getattr("modules")?
+        .set_item("llm_rs.config", config_module)?;
+
+    _py.import("sys")?
+        .getattr("modules")?
+        .set_item("llm_rs.results", results_module)?;
+
+    _py.import("sys")?
+        .getattr("modules")?
+        .set_item("llm_rs.models", models_module)?;
+
+    Ok(())
+}
```

### Comparing `llm-rs-metal-0.0.1/src/quantize.rs` & `llm_rs_metal-0.2.12/src/quantize.rs`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-use llm_base::QuantizeProgress;
-use pyo3::prelude::*;
-
-use std::{
-    io::{BufReader, BufWriter},
-    path::PathBuf,
-};
-
-use llm::{quantize, QuantizeError};
-
-#[pyclass]
-#[derive(Clone, Copy, Debug, PartialEq)]
-#[allow(clippy::upper_case_acronyms)]
-pub enum ContainerType {
-    GGML,
-    GGJT,
-}
-
-#[pyclass]
-#[derive(Clone, Copy, Debug, PartialEq)]
-pub enum QuantizationType {
-    Q4_0,
-    Q4_1,
-    Q5_0,
-    Q5_1,
-    Q8_0,
-    F16,
-}
-
-pub fn _quantize<M: llm::KnownModel + 'static>(
-    source: PathBuf,
-    destination: PathBuf,
-    container: ContainerType,
-    quantization: QuantizationType,
-    progress_callback: impl Fn(String),
-) -> Result<(), QuantizeError> {
-    let container = match container {
-        ContainerType::GGML => llm_base::ggml::format::SaveContainerType::Ggml,
-        ContainerType::GGJT => llm_base::ggml::format::SaveContainerType::GgjtV3,
-    };
-
-    let quantization = match quantization {
-        QuantizationType::Q4_0 => Ok(llm_base::ggml::Type::Q4_0),
-        QuantizationType::Q4_1 => Ok(llm_base::ggml::Type::Q4_1),
-        QuantizationType::Q5_0 => Ok(llm_base::ggml::Type::Q5_0),
-        QuantizationType::Q5_1 => Ok(llm_base::ggml::Type::Q5_1),
-        QuantizationType::Q8_0 => Ok(llm_base::ggml::Type::Q8_0),
-        QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
-            element_type: llm_base::ggml::Type::F16,
-        }),
-    }?;
-
-    let mut source_reader = BufReader::new(std::fs::File::open(&source)?);
-    let mut destination_reader = BufWriter::new(std::fs::File::create(destination)?);
-    let vocabulary = llm::VocabularySource::Model.retrieve(&source).unwrap();
-
-    quantize::<M, _, _>(
-        &mut source_reader,
-        &mut destination_reader,
-        vocabulary,
-        container,
-        quantization,
-        |progress| match progress {
-            QuantizeProgress::HyperparametersLoaded => {
-                progress_callback("Loaded hyperparameters".to_string())
-            }
-            QuantizeProgress::TensorLoading {
-                name,
-                dims,
-                element_type,
-                n_elements,
-            } => progress_callback(format!(
-                "Loading tensor `{name}` ({n_elements} ({dims:?}) {element_type} elements)"
-            )),
-            QuantizeProgress::TensorQuantizing { name } => {
-                progress_callback(format!("Quantizing tensor `{name}`"))
-            }
-            QuantizeProgress::TensorQuantized {
-                name,
-                original_size,
-                reduced_size,
-                history,
-            } => progress_callback(format!(
-        "Quantized tensor `{name}` from {original_size} to {reduced_size} bytes ({history:?})"
-    )),
-            QuantizeProgress::TensorSkipped { name, size } => {
-                progress_callback(format!("Skipped tensor `{name}` ({size} bytes)"))
-            }
-            QuantizeProgress::Finished {
-                original_size,
-                reduced_size,
-                history,
-            } => progress_callback(format!(
-                "Finished quantization from {original_size} to {reduced_size} bytes ({history:?})"
-            )),
-        },
-    )
-}
+use llm_base::QuantizeProgress;
+use pyo3::prelude::*;
+
+use std::{
+    io::{BufReader, BufWriter},
+    path::PathBuf,
+};
+
+use llm::{quantize, QuantizeError};
+
+#[pyclass]
+#[derive(Clone, Copy, Debug, PartialEq)]
+#[allow(clippy::upper_case_acronyms)]
+pub enum ContainerType {
+    GGML,
+    GGJT,
+}
+
+#[pyclass]
+#[derive(Clone, Copy, Debug, PartialEq)]
+pub enum QuantizationType {
+    Q4_0,
+    Q4_1,
+    Q5_0,
+    Q5_1,
+    Q8_0,
+    F16,
+}
+
+pub fn _quantize<M: llm::KnownModel + 'static>(
+    source: PathBuf,
+    destination: PathBuf,
+    container: ContainerType,
+    quantization: QuantizationType,
+    progress_callback: impl Fn(String),
+) -> Result<(), QuantizeError> {
+    let container = match container {
+        ContainerType::GGML => llm_base::ggml::format::SaveContainerType::Ggml,
+        ContainerType::GGJT => llm_base::ggml::format::SaveContainerType::GgjtV3,
+    };
+
+    let quantization = match quantization {
+        QuantizationType::Q4_0 => Ok(llm_base::ggml::Type::Q4_0),
+        QuantizationType::Q4_1 => Ok(llm_base::ggml::Type::Q4_1),
+        QuantizationType::Q5_0 => Ok(llm_base::ggml::Type::Q5_0),
+        QuantizationType::Q5_1 => Ok(llm_base::ggml::Type::Q5_1),
+        QuantizationType::Q8_0 => Ok(llm_base::ggml::Type::Q8_0),
+        QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
+            element_type: llm_base::ggml::Type::F16,
+        }),
+    }?;
+
+    let mut source_reader = BufReader::new(std::fs::File::open(&source)?);
+    let mut destination_reader = BufWriter::new(std::fs::File::create(destination)?);
+    let vocabulary = llm::VocabularySource::Model.retrieve(&source).unwrap();
+
+    quantize::<M, _, _>(
+        &mut source_reader,
+        &mut destination_reader,
+        vocabulary,
+        container,
+        quantization,
+        |progress| match progress {
+            QuantizeProgress::HyperparametersLoaded => {
+                progress_callback("Loaded hyperparameters".to_string())
+            }
+            QuantizeProgress::TensorLoading {
+                name,
+                dims,
+                element_type,
+                n_elements,
+            } => progress_callback(format!(
+                "Loading tensor `{name}` ({n_elements} ({dims:?}) {element_type} elements)"
+            )),
+            QuantizeProgress::TensorQuantizing { name } => {
+                progress_callback(format!("Quantizing tensor `{name}`"))
+            }
+            QuantizeProgress::TensorQuantized {
+                name,
+                original_size,
+                reduced_size,
+                history,
+            } => progress_callback(format!(
+        "Quantized tensor `{name}` from {original_size} to {reduced_size} bytes ({history:?})"
+    )),
+            QuantizeProgress::TensorSkipped { name, size } => {
+                progress_callback(format!("Skipped tensor `{name}` ({size} bytes)"))
+            }
+            QuantizeProgress::Finished {
+                original_size,
+                reduced_size,
+                history,
+            } => progress_callback(format!(
+                "Finished quantization from {original_size} to {reduced_size} bytes ({history:?})"
+            )),
+        },
+    )
+}
```

### Comparing `llm-rs-metal-0.0.1/src/stopwords.rs` & `llm_rs_metal-0.2.12/src/stopwords.rs`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-use serde::{Deserialize, Serialize};
-use std::collections::HashSet;
-
-#[derive(Clone, Serialize, Deserialize)]
-struct Buffer<T> {
-    pub data: Vec<T>,
-    capacity: usize,
-}
-
-impl<T> Buffer<T> {
-    fn new(capacity: usize) -> Self {
-        Buffer {
-            data: Vec::with_capacity(capacity),
-            capacity,
-        }
-    }
-
-    fn push(&mut self, item: T) {
-        if self.data.len() == self.capacity {
-            self.data.remove(0);
-        }
-        self.data.push(item);
-    }
-}
-
-#[derive(Clone, Serialize, Deserialize)]
-pub struct StopWordHandler {
-    pub stop_words: HashSet<Vec<u8>>,
-    buffer: Buffer<u8>,
-}
-
-impl StopWordHandler {
-    pub fn new(model: &dyn llm::Model, stop_words: &[String]) -> StopWordHandler {
-        let tokenized_stop_words: HashSet<Vec<u8>> = stop_words
-            .iter()
-            .map(|word| {
-                model
-                    .vocabulary()
-                    .tokenize(word, false)
-                    .unwrap()
-                    .iter()
-                    .flat_map(|(encoding, _)| encoding.to_owned())
-                    .collect::<Vec<u8>>()
-            })
-            .collect();
-
-        let capacity = tokenized_stop_words
-            .iter()
-            .map(|v| v.len())
-            .max()
-            .unwrap_or(0);
-
-        StopWordHandler {
-            stop_words: tokenized_stop_words,
-            buffer: Buffer::new(capacity),
-        }
-    }
-
-    pub fn process(&mut self, new_tokens: Vec<u8>) -> bool {
-        for token in new_tokens {
-            self.buffer.push(token);
-            for i in 0..self.buffer.data.len() {
-                let slice = self.buffer.data[i..].to_vec();
-                if self.stop_words.contains(&slice) {
-                    return true;
-                }
-            }
-        }
-        false
-    }
-}
+use serde::{Deserialize, Serialize};
+use std::collections::HashSet;
+
+#[derive(Clone, Serialize, Deserialize)]
+struct Buffer<T> {
+    pub data: Vec<T>,
+    capacity: usize,
+}
+
+impl<T> Buffer<T> {
+    fn new(capacity: usize) -> Self {
+        Buffer {
+            data: Vec::with_capacity(capacity),
+            capacity,
+        }
+    }
+
+    fn push(&mut self, item: T) {
+        if self.data.len() == self.capacity {
+            self.data.remove(0);
+        }
+        self.data.push(item);
+    }
+}
+
+#[derive(Clone, Serialize, Deserialize)]
+pub struct StopWordHandler {
+    pub stop_words: HashSet<Vec<u8>>,
+    buffer: Buffer<u8>,
+}
+
+impl StopWordHandler {
+    pub fn new(model: &dyn llm::Model, stop_words: &[String]) -> StopWordHandler {
+        let tokenized_stop_words: HashSet<Vec<u8>> = stop_words
+            .iter()
+            .map(|word| {
+                model
+                    .vocabulary()
+                    .tokenize(word, false)
+                    .unwrap()
+                    .iter()
+                    .flat_map(|(encoding, _)| encoding.to_owned())
+                    .collect::<Vec<u8>>()
+            })
+            .collect();
+
+        let capacity = tokenized_stop_words
+            .iter()
+            .map(|v| v.len())
+            .max()
+            .unwrap_or(0);
+
+        StopWordHandler {
+            stop_words: tokenized_stop_words,
+            buffer: Buffer::new(capacity),
+        }
+    }
+
+    pub fn process(&mut self, new_tokens: Vec<u8>) -> bool {
+        for token in new_tokens {
+            self.buffer.push(token);
+            for i in 0..self.buffer.data.len() {
+                let slice = self.buffer.data[i..].to_vec();
+                if self.stop_words.contains(&slice) {
+                    return true;
+                }
+            }
+        }
+        false
+    }
+}
```

