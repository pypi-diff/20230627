# Comparing `tmp/tensora-0.0.7.tar.gz` & `tmp/tensora-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensora-0.0.7.tar", last modified: Fri Jun 16 11:43:57 2023, max compression
+gzip compressed data, was "tensora-0.0.8.tar", last modified: Tue Jun 27 10:40:05 2023, max compression
```

## Comparing `tensora-0.0.7.tar` & `tensora-0.0.8.tar`

### file list

```diff
@@ -1,784 +1,784 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.257709 tensora-0.0.7/
--rw-rw-r--   0 david     (1000) david     (1000)     1057 2020-07-08 11:47:39.000000 tensora-0.0.7/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      226 2020-07-08 11:47:39.000000 tensora-0.0.7/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     9253 2023-06-16 11:43:57.257709 tensora-0.0.7/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     8222 2020-07-08 11:47:39.000000 tensora-0.0.7/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-16 09:49:57.000000 tensora-0.0.7/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-16 11:43:57.257709 tensora-0.0.7/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     3033 2023-06-16 11:18:58.000000 tensora-0.0.7/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.193709 tensora-0.0.7/src/taco/.github/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/.github/workflows/
--rw-r--r--   0 david     (1000) david     (1000)     2651 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/.github/workflows/buildandtest.yml
--rw-r--r--   0 david     (1000) david     (1000)     1214 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/.github/workflows/cuda-test-manual.yml
--rw-r--r--   0 david     (1000) david     (1000)      202 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/.gitmodules
--rw-r--r--   0 david     (1000) david     (1000)     6274 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)     1693 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/Doxyfile
--rw-r--r--   0 david     (1000) david     (1000)     1172 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     6553 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/apps/
--rw-r--r--   0 david     (1000) david     (1000)       38 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/apps/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/apps/tensor_times_vector/
--rw-r--r--   0 david     (1000) david     (1000)      961 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/apps/tensor_times_vector/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)      376 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/apps/tensor_times_vector/README.md
--rw-r--r--   0 david     (1000) david     (1000)      502 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/apps/tensor_times_vector/tensor_times_vector.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/ci/
--rw-r--r--   0 david     (1000) david     (1000)     4380 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/ci/test-pr.md
--rw-r--r--   0 david     (1000) david     (1000)     4838 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/ci/test-pr.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/
--rw-r--r--   0 david     (1000) david     (1000)      437 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/codegen/
--rw-r--r--   0 david     (1000) david     (1000)     2693 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/codegen/module.h
--rw-r--r--   0 david     (1000) david     (1000)     1080 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/component.h
--rw-r--r--   0 david     (1000) david     (1000)     1938 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/coordinate.h
--rw-r--r--   0 david     (1000) david     (1000)      878 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/cuda.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/error/
--rw-r--r--   0 david     (1000) david     (1000)     1066 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/error/error_messages.h
--rw-r--r--   0 david     (1000) david     (1000)     3318 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/error.h
--rw-r--r--   0 david     (1000) david     (1000)     7184 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/format.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.201709 tensora-0.0.7/src/taco/include/taco/index_notation/
--rw-r--r--   0 david     (1000) david     (1000)     4642 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/README.md
--rw-r--r--   0 david     (1000) david     (1000)    49557 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation.h
--rw-r--r--   0 david     (1000) david     (1000)    14329 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes.h
--rw-r--r--   0 david     (1000) david     (1000)     1879 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h
--rw-r--r--   0 david     (1000) david     (1000)     1520 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_printer.h
--rw-r--r--   0 david     (1000) david     (1000)     4625 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_rewriter.h
--rw-r--r--   0 david     (1000) david     (1000)     7113 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_visitor.h
--rw-r--r--   0 david     (1000) david     (1000)     2180 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/intrinsic.h
--rw-r--r--   0 david     (1000) david     (1000)     8874 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/iteration_algebra.h
--rw-r--r--   0 david     (1000) david     (1000)      793 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/iteration_algebra_printer.h
--rw-r--r--   0 david     (1000) david     (1000)     2252 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/kernel.h
--rw-r--r--   0 david     (1000) david     (1000)     2423 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/properties.h
--rw-r--r--   0 david     (1000) david     (1000)     2685 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/property_pointers.h
--rw-r--r--   0 david     (1000) david     (1000)    23213 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/provenance_graph.h
--rw-r--r--   0 david     (1000) david     (1000)      929 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/index_notation/schedule.h
--rw-r--r--   0 david     (1000) david     (1000)     3389 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/tensor_operator.h
--rw-r--r--   0 david     (1000) david     (1000)     7475 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/index_notation/transformations.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/ir/
--rw-r--r--   0 david     (1000) david     (1000)    19034 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir.h
--rw-r--r--   0 david     (1000) david     (1000)      922 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_generators.h
--rw-r--r--   0 david     (1000) david     (1000)     2997 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_printer.h
--rw-r--r--   0 david     (1000) david     (1000)     2404 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_rewriter.h
--rw-r--r--   0 david     (1000) david     (1000)      410 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_verifier.h
--rw-r--r--   0 david     (1000) david     (1000)     4808 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/ir_visitor.h
--rw-r--r--   0 david     (1000) david     (1000)      349 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/ir/simplify.h
--rw-r--r--   0 david     (1000) david     (1000)      611 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir/workspace_rewriter.h
--rw-r--r--   0 david     (1000) david     (1000)     1772 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/ir_tags.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/lower/
--rw-r--r--   0 david     (1000) david     (1000)    10339 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/iterator.h
--rw-r--r--   0 david     (1000) david     (1000)     1871 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/lower.h
--rw-r--r--   0 david     (1000) david     (1000)     3053 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/lowerer_impl.h
--rw-r--r--   0 david     (1000) david     (1000)    25459 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/lowerer_impl_imperative.h
--rw-r--r--   0 david     (1000) david     (1000)     8039 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/merge_lattice.h
--rw-r--r--   0 david     (1000) david     (1000)     2212 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/lower/mode.h
--rw-r--r--   0 david     (1000) david     (1000)     3232 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_compressed.h
--rw-r--r--   0 david     (1000) david     (1000)     1512 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_dense.h
--rw-r--r--   0 david     (1000) david     (1000)     8570 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_impl.h
--rw-r--r--   0 david     (1000) david     (1000)     2069 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/lower/mode_format_singleton.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/parser/
--rw-r--r--   0 david     (1000) david     (1000)     1903 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/parser/einsum_parser.h
--rw-r--r--   0 david     (1000) david     (1000)      789 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/parser/lexer.h
--rw-r--r--   0 david     (1000) david     (1000)     3015 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/parser/parser.h
--rw-r--r--   0 david     (1000) david     (1000)      629 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/parser/schedule_parser.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/storage/
--rw-r--r--   0 david     (1000) david     (1000)     2388 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/array.h
--rw-r--r--   0 david     (1000) david     (1000)     1650 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/coordinate.h
--rw-r--r--   0 david     (1000) david     (1000)     1499 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/file_io_mtx.h
--rw-r--r--   0 david     (1000) david     (1000)     2509 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/file_io_rb.h
--rw-r--r--   0 david     (1000) david     (1000)      916 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/file_io_tns.h
--rw-r--r--   0 david     (1000) david     (1000)     2451 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/index.h
--rw-r--r--   0 david     (1000) david     (1000)     1746 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/pack.h
--rw-r--r--   0 david     (1000) david     (1000)     2289 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/storage.h
--rw-r--r--   0 david     (1000) david     (1000)    10031 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/typed_index.h
--rw-r--r--   0 david     (1000) david     (1000)    10673 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/storage/typed_value.h
--rw-r--r--   0 david     (1000) david     (1000)     8556 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/storage/typed_vector.h
--rw-r--r--   0 david     (1000) david     (1000)     1232 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/taco_tensor_t.h
--rw-r--r--   0 david     (1000) david     (1000)     1386 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/target.h
--rw-r--r--   0 david     (1000) david     (1000)    47778 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/tensor.h
--rw-r--r--   0 david     (1000) david     (1000)     7001 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/type.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/include/taco/util/
--rw-r--r--   0 david     (1000) david     (1000)    10527 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/collections.h
--rw-r--r--   0 david     (1000) david     (1000)     1056 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/comparable.h
--rw-r--r--   0 david     (1000) david     (1000)     2072 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/env.h
--rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/files.h
--rw-r--r--   0 david     (1000) david     (1000)     9333 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/fill.h
--rw-r--r--   0 david     (1000) david     (1000)      523 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/functions.h
--rw-r--r--   0 david     (1000) david     (1000)     3183 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/intrusive_ptr.h
--rw-r--r--   0 david     (1000) david     (1000)      483 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/name_generator.h
--rw-r--r--   0 david     (1000) david     (1000)      352 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/printable.h
--rw-r--r--   0 david     (1000) david     (1000)     1874 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/scopedmap.h
--rw-r--r--   0 david     (1000) david     (1000)     1124 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/scopedset.h
--rw-r--r--   0 david     (1000) david     (1000)      339 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/singleton.h
--rw-r--r--   0 david     (1000) david     (1000)     2598 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/strings.h
--rw-r--r--   0 david     (1000) david     (1000)     4597 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/timers.h
--rw-r--r--   0 david     (1000) david     (1000)      300 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/include/taco/util/uncopyable.h
--rw-r--r--   0 david     (1000) david     (1000)     2886 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/util/variadic.h
--rw-r--r--   0 david     (1000) david     (1000)      884 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco/version.h.in
--rw-r--r--   0 david     (1000) david     (1000)      196 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/include/taco.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/misc/
--rw-r--r--   0 david     (1000) david     (1000)      523 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/misc/mainpage.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.205709 tensora-0.0.7/src/taco/python_bindings/
--rw-r--r--   0 david     (1000) david     (1000)     1333 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)      584 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/Makefile
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/include/
--rw-r--r--   0 david     (1000) david     (1000)      342 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyDatatypes.h
--rw-r--r--   0 david     (1000) david     (1000)      372 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyFormat.h
--rw-r--r--   0 david     (1000) david     (1000)      269 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyIndexNotation.h
--rw-r--r--   0 david     (1000) david     (1000)      288 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyParsers.h
--rw-r--r--   0 david     (1000) david     (1000)      242 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyTensor.h
--rw-r--r--   0 david     (1000) david     (1000)      247 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyTensorIO.h
--rw-r--r--   0 david     (1000) david     (1000)      168 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/include/pyeinsum.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/
--rw-rw-r--   0 david     (1000) david     (1000)     1304 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.appveyor.yml
--rw-rw-r--   0 david     (1000) david     (1000)      523 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.clang-format
--rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.clang-tidy
--rw-rw-r--   0 david     (1000) david     (1000)     2196 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.cmake-format.yaml
--rw-rw-r--   0 david     (1000) david     (1000)       75 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.git
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/
--rw-rw-r--   0 david     (1000) david     (1000)    14415 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/CONTRIBUTING.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 david     (1000) david     (1000)     1270 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
--rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 david     (1000) david     (1000)      669 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
--rw-rw-r--   0 david     (1000) david     (1000)     1180 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/question.md
--rw-rw-r--   0 david     (1000) david     (1000)      559 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/dependabot.yml
--rw-rw-r--   0 david     (1000) david     (1000)      116 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/labeler.yml
--rw-rw-r--   0 david     (1000) david     (1000)       50 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/labeler_merged.yml
--rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/pull_request_template.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.209709 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/
--rw-rw-r--   0 david     (1000) david     (1000)    24549 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/ci.yml
--rw-rw-r--   0 david     (1000) david     (1000)     2117 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/configure.yml
--rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/format.yml
--rw-rw-r--   0 david     (1000) david     (1000)      333 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/labeler.yml
--rw-rw-r--   0 david     (1000) david     (1000)     2497 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/pip.yml
--rw-rw-r--   0 david     (1000) david     (1000)      452 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.gitignore
--rw-rw-r--   0 david     (1000) david     (1000)     2460 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 david     (1000) david     (1000)       62 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/.readthedocs.yml
--rw-rw-r--   0 david     (1000) david     (1000)    10364 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/CMakeLists.txt
--rw-rw-r--   0 david     (1000) david     (1000)     1684 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      256 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     8064 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/README.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/
--rw-rw-r--   0 david     (1000) david     (1000)      705 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/Doxyfile
--rw-rw-r--   0 david     (1000) david     (1000)     7417 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/Makefile
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/_static/
--rw-rw-r--   0 david     (1000) david     (1000)      254 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/_static/theme_overrides.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/
--rw-rw-r--   0 david     (1000) david     (1000)     3937 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/chrono.rst
--rw-rw-r--   0 david     (1000) david     (1000)     3398 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/custom.rst
--rw-rw-r--   0 david     (1000) david     (1000)    14288 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/eigen.rst
--rw-rw-r--   0 david     (1000) david     (1000)     3889 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/functional.rst
--rw-rw-r--   0 david     (1000) david     (1000)     1556 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/index.rst
--rw-rw-r--   0 david     (1000) david     (1000)    11680 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/overview.rst
--rw-rw-r--   0 david     (1000) david     (1000)     9703 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/stl.rst
--rw-rw-r--   0 david     (1000) david     (1000)     9372 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/strings.rst
--rw-rw-r--   0 david     (1000) david     (1000)    45877 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/classes.rst
--rw-rw-r--   0 david     (1000) david     (1000)     8420 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/embedding.rst
--rw-rw-r--   0 david     (1000) david     (1000)    14171 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/exceptions.rst
--rw-rw-r--   0 david     (1000) david     (1000)    25078 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/functions.rst
--rw-rw-r--   0 david     (1000) david     (1000)    12444 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/misc.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/index.rst
--rw-rw-r--   0 david     (1000) david     (1000)    16538 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/numpy.rst
--rw-rw-r--   0 david     (1000) david     (1000)     7878 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/object.rst
--rw-rw-r--   0 david     (1000) david     (1000)     5125 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/utilities.rst
--rw-rw-r--   0 david     (1000) david     (1000)     6366 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/smart_ptrs.rst
--rw-rw-r--   0 david     (1000) david     (1000)     9369 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/basics.rst
--rw-rw-r--   0 david     (1000) david     (1000)     2974 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/benchmark.py
--rw-rw-r--   0 david     (1000) david     (1000)     3168 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/benchmark.rst
--rw-rw-r--   0 david     (1000) david     (1000)    73677 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/changelog.rst
--rw-rw-r--   0 david     (1000) david     (1000)    16122 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/classes.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.213709 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/cmake/
--rw-rw-r--   0 david     (1000) david     (1000)      273 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/cmake/index.rst
--rw-rw-r--   0 david     (1000) david     (1000)    25511 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/compiling.rst
--rw-rw-r--   0 david     (1000) david     (1000)    12095 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/conf.py
--rw-rw-r--   0 david     (1000) david     (1000)    14592 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/faq.rst
--rw-rw-r--   0 david     (1000) david     (1000)      613 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/index.rst
--rw-rw-r--   0 david     (1000) david     (1000)     3277 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/installing.rst
--rw-rw-r--   0 david     (1000) david     (1000)     3062 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/limitations.rst
--rw-rw-r--   0 david     (1000) david     (1000)    58510 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11-logo.png
--rw-rw-r--   0 david     (1000) david     (1000)    44653 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.png
--rw-rw-r--   0 david     (1000) david     (1000)    87708 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-rw-r--   0 david     (1000) david     (1000)    41121 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.png
--rw-rw-r--   0 david     (1000) david     (1000)    85853 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-rw-r--   0 david     (1000) david     (1000)     2113 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/reference.rst
--rw-rw-r--   0 david     (1000) david     (1000)     4028 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/release.rst
--rw-rw-r--   0 david     (1000) david     (1000)      168 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)    21940 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/docs/upgrade.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/python_bindings/pybind11/include/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.217709 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/
--rw-rw-r--   0 david     (1000) david     (1000)    21412 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 david     (1000) david     (1000)     6118 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 david     (1000) david     (1000)    95557 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 david     (1000) david     (1000)     8185 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 david     (1000) david     (1000)      120 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/common.h
--rw-rw-r--   0 david     (1000) david     (1000)     2037 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.217709 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/
--rw-rw-r--   0 david     (1000) david     (1000)    27823 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 david     (1000) david     (1000)    40452 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 david     (1000) david     (1000)     3602 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 david     (1000) david     (1000)    16397 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 david     (1000) david     (1000)    16375 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 david     (1000) david     (1000)     1486 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/typeid.h
--rw-rw-r--   0 david     (1000) david     (1000)    29086 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 david     (1000) david     (1000)     7843 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 david     (1000) david     (1000)     5079 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 david     (1000) david     (1000)     3709 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 david     (1000) david     (1000)     6084 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 david     (1000) david     (1000)    69310 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 david     (1000) david     (1000)     9085 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 david     (1000) david     (1000)     2049 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/options.h
--rw-rw-r--   0 david     (1000) david     (1000)   111558 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 david     (1000) david     (1000)    66118 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/pytypes.h
--rw-rw-r--   0 david     (1000) david     (1000)    14136 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 david     (1000) david     (1000)    23912 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.217709 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/
--rw-rw-r--   0 david     (1000) david     (1000)      217 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/__main__.py
--rw-rw-r--   0 david     (1000) david     (1000)      202 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/_version.py
--rw-rw-r--   0 david     (1000) david     (1000)      137 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/_version.pyi
--rw-rw-r--   0 david     (1000) david     (1000)      663 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/commands.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/py.typed
--rw-rw-r--   0 david     (1000) david     (1000)    15110 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/setup_helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     1899 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/setup_helpers.pyi
--rw-rw-r--   0 david     (1000) david     (1000)      118 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)     2185 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     3499 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/
--rw-rw-r--   0 david     (1000) david     (1000)    15362 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/CMakeLists.txt
--rw-rw-r--   0 david     (1000) david     (1000)     4841 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/conftest.py
--rw-rw-r--   0 david     (1000) david     (1000)    11157 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/constructor_stats.h
--rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/cross_module_gil_utils.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      376 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/env.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/pytest.ini
--rw-rw-r--   0 david     (1000) david     (1000)     7074 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/test_files.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/pytest.ini
--rw-rw-r--   0 david     (1000) david     (1000)     2581 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-rw-r--   0 david     (1000) david     (1000)     2144 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/local_bindings.h
--rw-rw-r--   0 david     (1000) david     (1000)     5389 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/object.h
--rw-rw-r--   0 david     (1000) david     (1000)     5285 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     3647 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_tests.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     2733 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_tests.h
--rw-rw-r--   0 david     (1000) david     (1000)      626 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pytest.ini
--rw-rw-r--   0 david     (1000) david     (1000)      736 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)      864 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_async.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      558 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_async.py
--rw-rw-r--   0 david     (1000) david     (1000)     8048 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_buffers.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     4946 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_buffers.py
--rw-rw-r--   0 david     (1000) david     (1000)    13475 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_builtin_casters.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    17214 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_builtin_casters.py
--rw-rw-r--   0 david     (1000) david     (1000)     3702 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_call_policies.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     5728 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_call_policies.py
--rw-rw-r--   0 david     (1000) david     (1000)     6600 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_callbacks.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     4405 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_callbacks.py
--rw-rw-r--   0 david     (1000) david     (1000)     3406 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_chrono.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     6276 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_chrono.py
--rw-rw-r--   0 david     (1000) david     (1000)    21623 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_class.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    14273 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_class.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 david     (1000) david     (1000)     2639 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-rw-r--   0 david     (1000) david     (1000)      656 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/embed.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 david     (1000) david     (1000)     1175 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 david     (1000) david     (1000)     1259 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 david     (1000) david     (1000)     1653 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-rw-r--   0 david     (1000) david     (1000)      152 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/main.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 david     (1000) david     (1000)     1357 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 david     (1000) david     (1000)     1333 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-rw-r--   0 david     (1000) david     (1000)      166 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/test.py
--rw-rw-r--   0 david     (1000) david     (1000)     5346 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     1522 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.py
--rw-rw-r--   0 david     (1000) david     (1000)     9629 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_copy_move.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     4645 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_copy_move.py
--rw-rw-r--   0 david     (1000) david     (1000)     5513 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     4015 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.py
--rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_docstring_options.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     1630 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_docstring_options.py
--rw-rw-r--   0 david     (1000) david     (1000)    16867 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eigen.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    28282 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eigen.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/
--rw-rw-r--   0 david     (1000) david     (1000)     1758 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/CMakeLists.txt
--rw-rw-r--   0 david     (1000) david     (1000)      637 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/catch.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      554 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/external_module.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    10209 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      219 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.py
--rw-rw-r--   0 david     (1000) david     (1000)     2610 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_enum.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     7694 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_enum.py
--rw-rw-r--   0 david     (1000) david     (1000)     2628 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      768 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval.py
--rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval_call.py
--rw-rw-r--   0 david     (1000) david     (1000)     7862 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_exceptions.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     6753 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    16562 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_factory_constructors.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    16637 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_factory_constructors.py
--rw-rw-r--   0 david     (1000) david     (1000)     1760 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_gil_scoped.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     3128 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_gil_scoped.py
--rw-rw-r--   0 david     (1000) david     (1000)     3381 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_iostream.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     5799 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_iostream.py
--rw-rw-r--   0 david     (1000) david     (1000)     6489 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    10048 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.py
--rw-rw-r--   0 david     (1000) david     (1000)     4333 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_local_bindings.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     8102 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_local_bindings.py
--rw-rw-r--   0 david     (1000) david     (1000)    19446 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    17310 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.py
--rw-rw-r--   0 david     (1000) david     (1000)     3742 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_modules.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     2841 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_modules.py
--rw-rw-r--   0 david     (1000) david     (1000)     8863 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     9495 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.py
--rw-rw-r--   0 david     (1000) david     (1000)    17781 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_array.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    18647 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_array.py
--rw-rw-r--   0 david     (1000) david     (1000)    17721 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    13484 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.py
--rw-rw-r--   0 david     (1000) david     (1000)     3832 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     9709 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.py
--rw-rw-r--   0 david     (1000) david     (1000)     2731 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_opaque_types.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     1906 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_opaque_types.py
--rw-rw-r--   0 david     (1000) david     (1000)     8431 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_operator_overloading.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     4136 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_operator_overloading.py
--rw-rw-r--   0 david     (1000) david     (1000)     4945 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pickling.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pickling.py
--rw-rw-r--   0 david     (1000) david     (1000)    13347 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pytypes.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    13720 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pytypes.py
--rw-rw-r--   0 david     (1000) david     (1000)    13120 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     5966 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.py
--rw-rw-r--   0 david     (1000) david     (1000)    17913 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_smart_ptr.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     9620 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_smart_ptr.py
--rw-rw-r--   0 david     (1000) david     (1000)    12793 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     8557 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl.py
--rw-rw-r--   0 david     (1000) david     (1000)     4403 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl_binders.cpp
--rw-rw-r--   0 david     (1000) david     (1000)     7182 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl_binders.py
--rw-rw-r--   0 david     (1000) david     (1000)     4458 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      765 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.py
--rw-rw-r--   0 david     (1000) david     (1000)      603 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_union.cpp
--rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_union.py
--rw-rw-r--   0 david     (1000) david     (1000)    18454 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_virtual_functions.cpp
--rw-rw-r--   0 david     (1000) david     (1000)    11646 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_virtual_functions.py
--rw-rw-r--   0 david     (1000) david     (1000)     2558 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/valgrind-numpy-scipy.supp
--rw-rw-r--   0 david     (1000) david     (1000)     3103 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tests/valgrind-python.supp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.225709 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/
--rw-rw-r--   0 david     (1000) david     (1000)     2295 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 david     (1000) david     (1000)     3105 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 david     (1000) david     (1000)     9977 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindPythonLibsNew.cmake
--rwxrwxr-x   0 david     (1000) david     (1000)     1427 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/check-style.sh
--rw-rw-r--   0 david     (1000) david     (1000)      952 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 david     (1000) david     (1000)     1121 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/libsize.py
--rwxrwxr-x   0 david     (1000) david     (1000)     1202 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/make_changelog.py
--rw-rw-r--   0 david     (1000) david     (1000)    14003 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 david     (1000) david     (1000)     7010 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 david     (1000) david     (1000)     9172 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)     1822 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/python_bindings/pybind11/tools/setup_main.py.in
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/pytaco/
--rw-r--r--   0 david     (1000) david     (1000)       57 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     1542 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/numpy_license.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/
--rw-r--r--   0 david     (1000) david     (1000)       51 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)   111090 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/taco_tensor.py
--rw-r--r--   0 david     (1000) david     (1000)     2248 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/tensorIO.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/source/
--rw-r--r--   0 david     (1000) david     (1000)     2526 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/conf.py
--rw-r--r--   0 david     (1000) david     (1000)      480 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/index.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/source/rst_files/
--rw-r--r--   0 david     (1000) david     (1000)      114 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/as_np_dt.rst
--rw-r--r--   0 david     (1000) david     (1000)      102 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/datatype.rst
--rw-r--r--   0 david     (1000) david     (1000)       87 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/dtype_object.rst
--rw-r--r--   0 david     (1000) david     (1000)      458 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/expr_funcs.rst
--rw-r--r--   0 david     (1000) david     (1000)      780 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/file_io.rst
--rw-r--r--   0 david     (1000) david     (1000)      111 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/format.rst
--rw-r--r--   0 david     (1000) david     (1000)       73 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/format_class.rst
--rw-r--r--   0 david     (1000) david     (1000)       71 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/format_funcs.rst
--rw-r--r--   0 david     (1000) david     (1000)       91 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/idx_exp_obj.rst
--rw-r--r--   0 david     (1000) david     (1000)     1028 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/index_expressions.rst
--rw-r--r--   0 david     (1000) david     (1000)       79 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/index_vars.rst
--rw-r--r--   0 david     (1000) david     (1000)      131 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/iv_funcs.rst
--rw-r--r--   0 david     (1000) david     (1000)       71 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/mode_format.rst
--rw-r--r--   0 david     (1000) david     (1000)      152 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/parsers.rst
--rw-r--r--   0 david     (1000) david     (1000)      199 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/sched.rst
--rw-r--r--   0 david     (1000) david     (1000)       62 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensor_class.rst
--rw-r--r--   0 david     (1000) david     (1000)     1233 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensor_info.rst
--rw-r--r--   0 david     (1000) david     (1000)       63 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensors.rst
--rw-r--r--   0 david     (1000) david     (1000)      312 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/source/rst_files/udfs.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/python_bindings/src/
--rw-r--r--   0 david     (1000) david     (1000)     4505 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyDatatypes.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11285 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyFormat.cpp
--rw-r--r--   0 david     (1000) david     (1000)    34934 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyIndexNotation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3194 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyParsers.cpp
--rw-r--r--   0 david     (1000) david     (1000)    18175 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyTensor.cpp
--rw-r--r--   0 david     (1000) david     (1000)      805 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pyTensorIO.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4379 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/src/pytaco.cpp
--rw-r--r--   0 david     (1000) david     (1000)    10971 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/python_bindings/unit_tests.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/src/
--rw-r--r--   0 david     (1000) david     (1000)     1031 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/CMakeLists.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/src/codegen/
--rw-r--r--   0 david     (1000) david     (1000)    19006 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3120 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen.h
--rw-r--r--   0 david     (1000) david     (1000)    17904 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_c.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1454 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_c.h
--rw-r--r--   0 david     (1000) david     (1000)    49177 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_cuda.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3090 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/codegen_cuda.h
--rw-r--r--   0 david     (1000) david     (1000)     5739 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/codegen/module.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1925 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/cuda.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.229709 tensora-0.0.7/src/taco/src/error/
--rw-r--r--   0 david     (1000) david     (1000)     5070 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error/error_checks.cpp
--rw-r--r--   0 david     (1000) david     (1000)      902 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error/error_checks.h
--rw-r--r--   0 david     (1000) david     (1000)     1309 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error/error_messages.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1730 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/error.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11646 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/format.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.233709 tensora-0.0.7/src/taco/src/index_notation/
--rw-r--r--   0 david     (1000) david     (1000)      356 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/README.md
--rw-r--r--   0 david     (1000) david     (1000)   116223 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2791 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1049 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes_abstract.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7250 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_printer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11661 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_rewriter.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2942 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/index_notation_visitor.cpp
--rw-r--r--   0 david     (1000) david     (1000)    40775 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/intrinsic.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8065 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/iteration_algebra.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1309 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/iteration_algebra_printer.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4292 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/kernel.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4914 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/properties.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3423 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/property_pointers.cpp
--rw-r--r--   0 david     (1000) david     (1000)    58668 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/provenance_graph.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1424 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/index_notation/schedule.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4853 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/tensor_operator.cpp
--rw-r--r--   0 david     (1000) david     (1000)    74399 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/index_notation/transformations.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.233709 tensora-0.0.7/src/taco/src/ir/
--rw-r--r--   0 david     (1000) david     (1000)      239 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/ir/README.md
--rw-r--r--   0 david     (1000) david     (1000)    26833 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1805 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_generators.cpp
--rw-r--r--   0 david     (1000) david     (1000)    15742 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_printer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    10832 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_rewriter.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8912 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_verifier.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4411 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/ir_visitor.cpp
--rw-r--r--   0 david     (1000) david     (1000)    19916 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/simplify.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2669 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir/workspace_rewriter.cpp
--rw-r--r--   0 david     (1000) david     (1000)      573 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/ir_tags.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.233709 tensora-0.0.7/src/taco/src/lower/
--rw-r--r--   0 david     (1000) david     (1000)      260 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/README.md
--rw-r--r--   0 david     (1000) david     (1000)     7225 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/expr_tools.cpp
--rw-r--r--   0 david     (1000) david     (1000)      870 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/expr_tools.h
--rw-r--r--   0 david     (1000) david     (1000)     6683 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_forest.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1020 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_forest.h
--rw-r--r--   0 david     (1000) david     (1000)     8081 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_graph.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2945 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/iteration_graph.h
--rw-r--r--   0 david     (1000) david     (1000)    23959 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/iterator.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2021 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/lower.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3152 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/lowerer_impl.cpp
--rw-r--r--   0 david     (1000) david     (1000)   170132 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/lowerer_impl_imperative.cpp
--rw-r--r--   0 david     (1000) david     (1000)    49768 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/merge_lattice.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2880 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/mode.cpp
--rw-r--r--   0 david     (1000) david     (1000)      879 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_access.cpp
--rw-r--r--   0 david     (1000) david     (1000)      819 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/mode_access.h
--rw-r--r--   0 david     (1000) david     (1000)    11956 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_compressed.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2878 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_dense.cpp
--rw-r--r--   0 david     (1000) david     (1000)     8358 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_impl.cpp
--rw-r--r--   0 david     (1000) david     (1000)     6169 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/lower/mode_format_singleton.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2930 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/tensor_path.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2200 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/lower/tensor_path.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.237709 tensora-0.0.7/src/taco/src/parser/
--rw-r--r--   0 david     (1000) david     (1000)      293 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/parser/README.md
--rw-r--r--   0 david     (1000) david     (1000)     9758 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/parser/einsum_parser.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3565 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/parser/lexer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11905 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/parser/parser.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7141 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/parser/schedule_parser.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.237709 tensora-0.0.7/src/taco/src/storage/
--rw-r--r--   0 david     (1000) david     (1000)      152 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/README.md
--rw-r--r--   0 david     (1000) david     (1000)     5348 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/array.cpp
--rw-r--r--   0 david     (1000) david     (1000)    12244 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/file_io_mtx.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13141 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/file_io_rb.cpp
--rw-r--r--   0 david     (1000) david     (1000)     4661 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/file_io_tns.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3551 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/index.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7948 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/pack.cpp
--rw-r--r--   0 david     (1000) david     (1000)     6004 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/storage.cpp
--rw-r--r--   0 david     (1000) david     (1000)    18028 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/storage/typed_index.cpp
--rw-r--r--   0 david     (1000) david     (1000)    23635 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/storage/typed_value.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2366 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/taco_tensor_t.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1904 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/target.cpp
--rw-r--r--   0 david     (1000) david     (1000)    47292 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/tensor.cpp
--rw-r--r--   0 david     (1000) david     (1000)     9240 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/type.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.237709 tensora-0.0.7/src/taco/src/util/
--rw-r--r--   0 david     (1000) david     (1000)      635 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/util/env.cpp
--rw-r--r--   0 david     (1000) david     (1000)      512 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/util/files.cpp
--rw-r--r--   0 david     (1000) david     (1000)      880 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/src/util/name_generator.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1062 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/src/util/strings.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/
--rw-r--r--   0 david     (1000) david     (1000)      931 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)     3773 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/README_testing.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/
--rw-rw-r--   0 david     (1000) david     (1000)      546 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.appveyor.yml
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/.devcontainer/
--rw-rw-r--   0 david     (1000) david     (1000)      519 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.devcontainer/Dockerfile
--rw-rw-r--   0 david     (1000) david     (1000)       83 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.devcontainer/devcontainer.json
--rw-rw-r--   0 david     (1000) david     (1000)      687 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.editorconfig
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 20:50:05.000000 tensora-0.0.7/src/taco/test/bats/.git
--rwxrwxr-x   0 david     (1000) david     (1000)       41 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.gitattributes
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.gitignore
--rw-rw-r--   0 david     (1000) david     (1000)      800 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/.travis.yml
--rw-rw-r--   0 david     (1000) david     (1000)      219 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/AUTHORS
--rw-rw-r--   0 david     (1000) david     (1000)      386 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/Dockerfile
--rw-rw-r--   0 david     (1000) david     (1000)     2535 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/LICENSE.md
--rw-rw-r--   0 david     (1000) david     (1000)    23464 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/bin/
--rwxrwxr-x   0 david     (1000) david     (1000)     1675 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/bin/bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/contrib/
--rwxrwxr-x   0 david     (1000) david     (1000)     3795 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/contrib/release.sh
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/contrib/rpm/
--rw-rw-r--   0 david     (1000) david     (1000)     1575 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/contrib/rpm/bats.spec
--rwxrwxr-x   0 david     (1000) david     (1000)     7973 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/contrib/semver
--rw-rw-r--   0 david     (1000) david     (1000)      147 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docker-compose.override.dist
--rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docker-compose.yml
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/docs/
--rw-rw-r--   0 david     (1000) david     (1000)     7042 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)      211 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CODEOWNERS
--rw-rw-r--   0 david     (1000) david     (1000)     3643 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CODE_OF_CONDUCT.md
--rw-rw-r--   0 david     (1000) david     (1000)    17557 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/CONTRIBUTING.md
--rw-rw-r--   0 david     (1000) david     (1000)      317 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.241709 tensora-0.0.7/src/taco/test/bats/docs/examples/
--rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/examples/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      604 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/examples/package-tarball
--rwxrwxr-x   0 david     (1000) david     (1000)      869 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/examples/package-tarball.bats
--rw-rw-r--   0 david     (1000) david     (1000)     3979 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/releasing.md
--rw-rw-r--   0 david     (1000) david     (1000)     2338 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/usage.md
--rw-rw-r--   0 david     (1000) david     (1000)      287 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/docs/versions.md
--rwxrwxr-x   0 david     (1000) david     (1000)      627 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/install.sh
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/lib/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/lib/bats-core/
--rw-rw-r--   0 david     (1000) david     (1000)      827 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/preprocessing.bash
--rw-rw-r--   0 david     (1000) david     (1000)     2646 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/test_functions.bash
--rw-rw-r--   0 david     (1000) david     (1000)     4197 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/tracing.bash
--rw-rw-r--   0 david     (1000) david     (1000)     1002 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/lib/bats-core/validator.bash
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/libexec/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/
--rwxrwxr-x   0 david     (1000) david     (1000)     5567 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats
--rwxrwxr-x   0 david     (1000) david     (1000)     5654 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-file
--rwxrwxr-x   0 david     (1000) david     (1000)     2386 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-suite
--rwxrwxr-x   0 david     (1000) david     (1000)     4762 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-test
--rwxrwxr-x   0 david     (1000) david     (1000)     3436 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-junit
--rwxrwxr-x   0 david     (1000) david     (1000)     4421 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-pretty
--rwxrwxr-x   0 david     (1000) david     (1000)       32 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-tap
--rwxrwxr-x   0 david     (1000) david     (1000)     1308 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-preprocess
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/man/
--rw-rw-r--   0 david     (1000) david     (1000)      427 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/Makefile
--rw-rw-r--   0 david     (1000) david     (1000)      253 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/README.md
--rw-rw-r--   0 david     (1000) david     (1000)     3836 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.1
--rw-rw-r--   0 david     (1000) david     (1000)     3544 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.1.ronn
--rw-rw-r--   0 david     (1000) david     (1000)     4928 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.7
--rw-rw-r--   0 david     (1000) david     (1000)     4510 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/man/bats.7.ronn
--rw-rw-r--   0 david     (1000) david     (1000)      641 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/package.json
--rwxrwxr-x   0 david     (1000) david     (1000)      277 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/shellcheck.sh
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.245709 tensora-0.0.7/src/taco/test/bats/test/
--rwxrwxr-x   0 david     (1000) david     (1000)    20307 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/bats.bats
--rw-rw-r--   0 david     (1000) david     (1000)     7356 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/file_setup_teardown.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/test/fixtures/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/
--rw-rw-r--   0 david     (1000) david     (1000)      171 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/ambiguous
--rw-rw-r--   0 david     (1000) david     (1000)      179 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/ambiguous.bash
--rwxrwxr-x   0 david     (1000) david     (1000)      295 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/cmd_using_stdin.bash
--rw-rw-r--   0 david     (1000) david     (1000)       35 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/dos_line.bats
--rw-rw-r--   0 david     (1000) david     (1000)      233 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/duplicate-tests.bats
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/empty.bats
--rw-rw-r--   0 david     (1000) david     (1000)      138 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/environment.bats
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/expand_var_in_test_name.bats
--rw-rw-r--   0 david     (1000) david     (1000)      104 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/exported_function.bats
--rw-rw-r--   0 david     (1000) david     (1000)     1186 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/external_function_calls.bats
--rw-rw-r--   0 david     (1000) david     (1000)       72 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing.bats
--rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_and_passing.bats
--rw-rw-r--   0 david     (1000) david     (1000)       80 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_helper.bats
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_setup.bats
--rw-rw-r--   0 david     (1000) david     (1000)       83 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/failing_teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/intact.bats
--rw-rw-r--   0 david     (1000) david     (1000)      118 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/load.bats
--rw-rw-r--   0 david     (1000) david     (1000)      239 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/loop_keep_IFS.bats
--rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/no-final-newline.bats
--rw-rw-r--   0 david     (1000) david     (1000)      331 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/output.bats
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/parallel.bats
--rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing.bats
--rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing_and_failing.bats
--rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing_and_skipping.bats
--rw-rw-r--   0 david     (1000) david     (1000)      106 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/passing_failing_and_skipping.bats
--rw-rw-r--   0 david     (1000) david     (1000)      109 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/quoted_and_unquoted_test_names.bats
--rw-rw-r--   0 david     (1000) david     (1000)      501 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/read_from_stdin.bats
--rw-rw-r--   0 david     (1000) david     (1000)       81 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter.bats
--rw-rw-r--   0 david     (1000) david     (1000)      179 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter_in_setup.bats
--rw-rw-r--   0 david     (1000) david     (1000)      113 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter_in_teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)      266 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/setup.bats
--rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/single_line.bats
--rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/skipped.bats
--rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/skipped_with_parens.bats
--rw-rw-r--   0 david     (1000) david     (1000)       72 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file.bats
--rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file_in_setup.bats
--rw-rw-r--   0 david     (1000) david     (1000)      104 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file_in_teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)      169 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)      267 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/test_helper.bash
--rw-rw-r--   0 david     (1000) david     (1000)      331 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/unbound_variable.bats
--rw-rw-r--   0 david     (1000) david     (1000)       50 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/unofficial_bash_strict_mode.bash
--rw-rw-r--   0 david     (1000) david     (1000)       92 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/unofficial_bash_strict_mode.bats
--rw-rw-r--   0 david     (1000) david     (1000)      593 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/whitespace.bats
--rw-rw-r--   0 david     (1000) david     (1000)       24 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/without_trailing_newline.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/
--rw-rw-r--   0 david     (1000) david     (1000)       25 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/no_setup_file.bats
--rw-rw-r--   0 david     (1000) david     (1000)       26 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/no_teardown_file.bats
--rw-rw-r--   0 david     (1000) david     (1000)      317 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file.bats
--rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file2.bats
--rw-rw-r--   0 david     (1000) david     (1000)       91 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_does_not_leak_env.bats
--rw-rw-r--   0 david     (1000) david     (1000)       69 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_does_not_leak_env2.bats
--rw-rw-r--   0 david     (1000) david     (1000)      125 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_even_if_all_tests_are_skipped.bats
--rw-rw-r--   0 david     (1000) david     (1000)       84 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_failed.bats
--rw-rw-r--   0 david     (1000) david     (1000)       71 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_halfway_error.bats
--rw-rw-r--   0 david     (1000) david     (1000)      117 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file.bats
--rw-rw-r--   0 david     (1000) david     (1000)      117 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file2.bats
--rw-rw-r--   0 david     (1000) david     (1000)       96 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_after_failing_test.bats
--rw-rw-r--   0 david     (1000) david     (1000)      152 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_after_long_test.bats
--rw-rw-r--   0 david     (1000) david     (1000)      108 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_does_not_leak.bats
--rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_does_not_leak2.bats
--rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_even_if_all_tests_are_skipped.bats
--rw-rw-r--   0 david     (1000) david     (1000)       57 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_failed.bats
--rw-rw-r--   0 david     (1000) david     (1000)       75 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_halfway_error.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/
--rw-rw-r--   0 david     (1000) david     (1000)      191 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/parallel-preserve-environment.bats
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/parallel.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/
--rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file.bats
--rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file1.bats
--rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file2.bats
--rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file3.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel1.bats
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel2.bats
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel3.bats
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/parallel/suite/parallel4.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.197709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/empty/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/empty/.gitkeep
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/
--rw-rw-r--   0 david     (1000) david     (1000)       65 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/a.bats
--rw-rw-r--   0 david     (1000) david     (1000)       66 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/b.bats
--rw-rw-r--   0 david     (1000) david     (1000)       68 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/filter/c.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/multiple/
--rw-rw-r--   0 david     (1000) david     (1000)       25 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/multiple/a.bats
--rw-rw-r--   0 david     (1000) david     (1000)       73 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/multiple/b.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.249709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/subsuite/
--rw-rw-r--   0 david     (1000) david     (1000)       40 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/subsuite/test2.bats
--rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/recursive/test.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/single/
--rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/single/test.bats
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/
--rw-rw-r--   0 david     (1000) david     (1000)      319 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-setup-and-teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)      194 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-setup.bats
--rw-rw-r--   0 david     (1000) david     (1000)      158 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)      245 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-test-and-teardown.bats
--rw-rw-r--   0 david     (1000) david     (1000)      131 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/fixtures/suite/skip/skip-in-test.bats
--rw-rw-r--   0 david     (1000) david     (1000)     2116 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/install.bats
--rw-rw-r--   0 david     (1000) david     (1000)      583 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/junit-formatter.bats
--rw-rw-r--   0 david     (1000) david     (1000)     2323 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/parallell.bats
--rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/root.bats
--rwxrwxr-x   0 david     (1000) david     (1000)     4913 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/suite.bats
--rw-rw-r--   0 david     (1000) david     (1000)     1034 2023-06-15 20:50:06.000000 tensora-0.0.7/src/taco/test/bats/test/test_helper.bash
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/data/
--rw-r--r--   0 david     (1000) david     (1000)      119 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/2tensor.mtx
--rw-r--r--   0 david     (1000) david     (1000)       36 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/3tensor.tns
--rw-r--r--   0 david     (1000) david     (1000)      267 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d33.mtx
--rw-r--r--   0 david     (1000) david     (1000)       66 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d33.ttx
--rw-r--r--   0 david     (1000) david     (1000)      136 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d432.ttx
--rw-r--r--   0 david     (1000) david     (1000)       88 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/d567.ttx
--rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/ds33.mtx
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/data/qcd/
--rw-r--r--   0 david     (1000) david     (1000)    11615 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/theta.ttx
--rw-r--r--   0 david     (1000) david     (1000)       64 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/theta_simple.ttx
--rw-r--r--   0 david     (1000) david     (1000)      555 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/z.ttx
--rw-r--r--   0 david     (1000) david     (1000)       52 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/qcd/z_simple.ttx
--rw-r--r--   0 david     (1000) david     (1000)     1487 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/rua_32.mtx
--rw-r--r--   0 david     (1000) david     (1000)     1986 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/data/rua_32.rb
--rw-r--r--   0 david     (1000) david     (1000)     4650 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/expr_factory.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2589 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/expr_factory.h
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/test/gtest/
--rw-r--r--   0 david     (1000) david     (1000)     1475 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/gtest/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      155 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/gtest/README.TAC
--rw-r--r--   0 david     (1000) david     (1000)   365644 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/gtest/gtest-all.cc
--rw-r--r--   0 david     (1000) david     (1000)   849134 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/gtest/gtest.h
--rw-r--r--   0 david     (1000) david     (1000)     4788 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/op_factory.h
--rwxr-xr-x   0 david     (1000) david     (1000)    12555 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/taco-cli-test.bats
--rw-r--r--   0 david     (1000) david     (1000)     7165 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test-iteration_algebra.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1110 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test-typedcomponent-memory.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1897 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3618 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test.h
--rw-r--r--   0 david     (1000) david     (1000)     3125 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test_properties.cpp
--rw-r--r--   0 david     (1000) david     (1000)    11493 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test_tensors.cpp
--rw-r--r--   0 david     (1000) david     (1000)     5687 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/test_tensors.h
--rw-r--r--   0 david     (1000) david     (1000)    12251 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-api.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2561 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-copyprop.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1310 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-error.cpp
--rw-r--r--   0 david     (1000) david     (1000)      493 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-expr-reduction.cpp
--rw-r--r--   0 david     (1000) david     (1000)     5044 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-expr.cpp
--rw-r--r--   0 david     (1000) david     (1000)    43783 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-expr_storage.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3200 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-format-mm-permute.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2112 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-format.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1044 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-index.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13133 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-index_notation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2306 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-indexexpr.cpp
--rw-r--r--   0 david     (1000) david     (1000)     2918 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-indexstmt.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3609 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-io.cpp
--rw-r--r--   0 david     (1000) david     (1000)    55894 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-lower.cpp
--rw-r--r--   0 david     (1000) david     (1000)    59718 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-merge_lattice.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7101 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-parafac.cpp
--rw-r--r--   0 david     (1000) david     (1000)     1837 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-qcd.cpp
--rw-r--r--   0 david     (1000) david     (1000)       68 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-regression.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3602 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-schedule-parser.cpp
--rw-r--r--   0 david     (1000) david     (1000)    76554 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-scheduling-eval.cpp
--rw-r--r--   0 david     (1000) david     (1000)    32561 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-scheduling.cpp
--rw-r--r--   0 david     (1000) david     (1000)    14078 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-storage.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3573 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-storage_alloc.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13383 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-tensor.cpp
--rw-r--r--   0 david     (1000) david     (1000)    13605 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-tensor_types.cpp
--rw-r--r--   0 david     (1000) david     (1000)    14092 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-transformation.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3574 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-transpose.cpp
--rw-r--r--   0 david     (1000) david     (1000)     3576 2020-07-08 22:41:29.000000 tensora-0.0.7/src/taco/test/tests-type.cpp
--rw-r--r--   0 david     (1000) david     (1000)    19463 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-windowing.cpp
--rw-r--r--   0 david     (1000) david     (1000)    17609 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/test/tests-workspaces.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/taco/tools/
--rw-r--r--   0 david     (1000) david     (1000)      490 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/tools/CMakeLists.txt
--rw-r--r--   0 david     (1000) david     (1000)    52311 2023-01-16 18:11:38.000000 tensora-0.0.7/src/taco/tools/taco.cpp
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora/
--rw-rw-r--   0 david     (1000) david     (1000)      148 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    19747 2023-01-16 18:11:03.000000 tensora-0.0.7/src/tensora/compile.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora/expression/
--rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:57:19.000000 tensora-0.0.7/src/tensora/expression/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5267 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/expression/ast.py
--rw-rw-r--   0 david     (1000) david     (1000)     1676 2023-06-15 20:57:23.000000 tensora-0.0.7/src/tensora/expression/parser.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora/format/
--rw-rw-r--   0 david     (1000) david     (1000)       94 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/format/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1305 2020-07-08 11:47:39.000000 tensora-0.0.7/src/tensora/format/format.py
--rw-rw-r--   0 david     (1000) david     (1000)     1502 2023-06-16 10:05:44.000000 tensora-0.0.7/src/tensora/format/parser.py
--rw-rw-r--   0 david     (1000) david     (1000)     7052 2023-06-15 20:57:23.000000 tensora-0.0.7/src/tensora/function.py
--rw-rw-r--   0 david     (1000) david     (1000)    23902 2023-06-15 20:57:23.000000 tensora-0.0.7/src/tensora/tensor.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.253709 tensora-0.0.7/src/tensora.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     9253 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)    33517 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-06-16 11:43:57.000000 tensora-0.0.7/src/tensora.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-16 11:43:57.257709 tensora-0.0.7/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     4741 2023-06-15 20:57:19.000000 tensora-0.0.7/tests/test_combinatorically.py
--rw-r--r--   0 david     (1000) david     (1000)     2852 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_compile.py
--rw-rw-r--   0 david     (1000) david     (1000)     2685 2023-06-15 20:57:23.000000 tensora-0.0.7/tests/test_expression.py
--rw-rw-r--   0 david     (1000) david     (1000)     1686 2023-06-15 20:57:23.000000 tensora-0.0.7/tests/test_format.py
--rw-rw-r--   0 david     (1000) david     (1000)     9370 2020-07-08 11:47:39.000000 tensora-0.0.7/tests/test_from_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     2901 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_function.py
--rw-r--r--   0 david     (1000) david     (1000)      583 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_numpy.py
--rw-rw-r--   0 david     (1000) david     (1000)      668 2020-07-08 11:47:39.000000 tensora-0.0.7/tests/test_operators.py
--rw-rw-r--   0 david     (1000) david     (1000)    10193 2023-01-16 18:11:03.000000 tensora-0.0.7/tests/test_tensor.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.514374 tensora-0.0.8/
+-rw-rw-r--   0 david     (1000) david     (1000)     1057 2020-07-08 11:47:39.000000 tensora-0.0.8/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      226 2020-07-08 11:47:39.000000 tensora-0.0.8/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     9253 2023-06-27 10:40:05.514374 tensora-0.0.8/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     8222 2020-07-08 11:47:39.000000 tensora-0.0.8/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-27 10:32:33.000000 tensora-0.0.8/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-27 10:40:05.514374 tensora-0.0.8/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     3033 2023-06-27 10:33:29.000000 tensora-0.0.8/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.426375 tensora-0.0.8/src/taco/.github/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/.github/workflows/
+-rw-r--r--   0 david     (1000) david     (1000)     2651 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/.github/workflows/buildandtest.yml
+-rw-r--r--   0 david     (1000) david     (1000)     1214 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/.github/workflows/cuda-test-manual.yml
+-rw-r--r--   0 david     (1000) david     (1000)      202 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/.gitmodules
+-rw-r--r--   0 david     (1000) david     (1000)     6274 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)     1693 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/Doxyfile
+-rw-r--r--   0 david     (1000) david     (1000)     1172 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     6553 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/apps/
+-rw-r--r--   0 david     (1000) david     (1000)       38 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/apps/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/apps/tensor_times_vector/
+-rw-r--r--   0 david     (1000) david     (1000)      961 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/apps/tensor_times_vector/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)      376 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/apps/tensor_times_vector/README.md
+-rw-r--r--   0 david     (1000) david     (1000)      502 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/apps/tensor_times_vector/tensor_times_vector.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/ci/
+-rw-r--r--   0 david     (1000) david     (1000)     4380 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/ci/test-pr.md
+-rw-r--r--   0 david     (1000) david     (1000)     4838 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/ci/test-pr.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/include/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.438374 tensora-0.0.8/src/taco/include/taco/
+-rw-r--r--   0 david     (1000) david     (1000)      437 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.438374 tensora-0.0.8/src/taco/include/taco/codegen/
+-rw-r--r--   0 david     (1000) david     (1000)     2693 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/codegen/module.h
+-rw-r--r--   0 david     (1000) david     (1000)     1080 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/component.h
+-rw-r--r--   0 david     (1000) david     (1000)     1938 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/coordinate.h
+-rw-r--r--   0 david     (1000) david     (1000)      878 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/cuda.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.438374 tensora-0.0.8/src/taco/include/taco/error/
+-rw-r--r--   0 david     (1000) david     (1000)     1066 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/error/error_messages.h
+-rw-r--r--   0 david     (1000) david     (1000)     3318 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/error.h
+-rw-r--r--   0 david     (1000) david     (1000)     7184 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/format.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.438374 tensora-0.0.8/src/taco/include/taco/index_notation/
+-rw-r--r--   0 david     (1000) david     (1000)     4642 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/index_notation/README.md
+-rw-r--r--   0 david     (1000) david     (1000)    49557 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/index_notation.h
+-rw-r--r--   0 david     (1000) david     (1000)    14329 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_nodes.h
+-rw-r--r--   0 david     (1000) david     (1000)     1879 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h
+-rw-r--r--   0 david     (1000) david     (1000)     1520 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_printer.h
+-rw-r--r--   0 david     (1000) david     (1000)     4625 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_rewriter.h
+-rw-r--r--   0 david     (1000) david     (1000)     7113 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_visitor.h
+-rw-r--r--   0 david     (1000) david     (1000)     2180 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/index_notation/intrinsic.h
+-rw-r--r--   0 david     (1000) david     (1000)     8874 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/iteration_algebra.h
+-rw-r--r--   0 david     (1000) david     (1000)      793 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/iteration_algebra_printer.h
+-rw-r--r--   0 david     (1000) david     (1000)     2252 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/index_notation/kernel.h
+-rw-r--r--   0 david     (1000) david     (1000)     2423 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/properties.h
+-rw-r--r--   0 david     (1000) david     (1000)     2685 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/property_pointers.h
+-rw-r--r--   0 david     (1000) david     (1000)    23213 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/provenance_graph.h
+-rw-r--r--   0 david     (1000) david     (1000)      929 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/index_notation/schedule.h
+-rw-r--r--   0 david     (1000) david     (1000)     3389 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/tensor_operator.h
+-rw-r--r--   0 david     (1000) david     (1000)     7475 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/index_notation/transformations.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.442375 tensora-0.0.8/src/taco/include/taco/ir/
+-rw-r--r--   0 david     (1000) david     (1000)    19034 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir/ir.h
+-rw-r--r--   0 david     (1000) david     (1000)      922 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir/ir_generators.h
+-rw-r--r--   0 david     (1000) david     (1000)     2997 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir/ir_printer.h
+-rw-r--r--   0 david     (1000) david     (1000)     2404 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir/ir_rewriter.h
+-rw-r--r--   0 david     (1000) david     (1000)      410 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/ir/ir_verifier.h
+-rw-r--r--   0 david     (1000) david     (1000)     4808 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir/ir_visitor.h
+-rw-r--r--   0 david     (1000) david     (1000)      349 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/ir/simplify.h
+-rw-r--r--   0 david     (1000) david     (1000)      611 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir/workspace_rewriter.h
+-rw-r--r--   0 david     (1000) david     (1000)     1772 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/ir_tags.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.442375 tensora-0.0.8/src/taco/include/taco/lower/
+-rw-r--r--   0 david     (1000) david     (1000)    10339 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/iterator.h
+-rw-r--r--   0 david     (1000) david     (1000)     1871 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/lower.h
+-rw-r--r--   0 david     (1000) david     (1000)     3053 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/lowerer_impl.h
+-rw-r--r--   0 david     (1000) david     (1000)    25459 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/lowerer_impl_imperative.h
+-rw-r--r--   0 david     (1000) david     (1000)     8039 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/merge_lattice.h
+-rw-r--r--   0 david     (1000) david     (1000)     2212 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/lower/mode.h
+-rw-r--r--   0 david     (1000) david     (1000)     3232 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/mode_format_compressed.h
+-rw-r--r--   0 david     (1000) david     (1000)     1512 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/mode_format_dense.h
+-rw-r--r--   0 david     (1000) david     (1000)     8570 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/mode_format_impl.h
+-rw-r--r--   0 david     (1000) david     (1000)     2069 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/lower/mode_format_singleton.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.442375 tensora-0.0.8/src/taco/include/taco/parser/
+-rw-r--r--   0 david     (1000) david     (1000)     1903 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/parser/einsum_parser.h
+-rw-r--r--   0 david     (1000) david     (1000)      789 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/parser/lexer.h
+-rw-r--r--   0 david     (1000) david     (1000)     3015 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/parser/parser.h
+-rw-r--r--   0 david     (1000) david     (1000)      629 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/parser/schedule_parser.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.446375 tensora-0.0.8/src/taco/include/taco/storage/
+-rw-r--r--   0 david     (1000) david     (1000)     2388 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/storage/array.h
+-rw-r--r--   0 david     (1000) david     (1000)     1650 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/storage/coordinate.h
+-rw-r--r--   0 david     (1000) david     (1000)     1499 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/storage/file_io_mtx.h
+-rw-r--r--   0 david     (1000) david     (1000)     2509 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/storage/file_io_rb.h
+-rw-r--r--   0 david     (1000) david     (1000)      916 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/storage/file_io_tns.h
+-rw-r--r--   0 david     (1000) david     (1000)     2451 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/storage/index.h
+-rw-r--r--   0 david     (1000) david     (1000)     1746 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/storage/pack.h
+-rw-r--r--   0 david     (1000) david     (1000)     2289 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/storage/storage.h
+-rw-r--r--   0 david     (1000) david     (1000)    10031 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/storage/typed_index.h
+-rw-r--r--   0 david     (1000) david     (1000)    10673 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/storage/typed_value.h
+-rw-r--r--   0 david     (1000) david     (1000)     8556 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/storage/typed_vector.h
+-rw-r--r--   0 david     (1000) david     (1000)     1232 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/taco_tensor_t.h
+-rw-r--r--   0 david     (1000) david     (1000)     1386 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/target.h
+-rw-r--r--   0 david     (1000) david     (1000)    47778 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/tensor.h
+-rw-r--r--   0 david     (1000) david     (1000)     7001 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/type.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.446375 tensora-0.0.8/src/taco/include/taco/util/
+-rw-r--r--   0 david     (1000) david     (1000)    10527 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/collections.h
+-rw-r--r--   0 david     (1000) david     (1000)     1056 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/comparable.h
+-rw-r--r--   0 david     (1000) david     (1000)     2072 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/env.h
+-rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/files.h
+-rw-r--r--   0 david     (1000) david     (1000)     9333 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/fill.h
+-rw-r--r--   0 david     (1000) david     (1000)      523 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/functions.h
+-rw-r--r--   0 david     (1000) david     (1000)     3183 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/intrusive_ptr.h
+-rw-r--r--   0 david     (1000) david     (1000)      483 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/name_generator.h
+-rw-r--r--   0 david     (1000) david     (1000)      352 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/printable.h
+-rw-r--r--   0 david     (1000) david     (1000)     1874 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/scopedmap.h
+-rw-r--r--   0 david     (1000) david     (1000)     1124 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/scopedset.h
+-rw-r--r--   0 david     (1000) david     (1000)      339 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/singleton.h
+-rw-r--r--   0 david     (1000) david     (1000)     2598 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/strings.h
+-rw-r--r--   0 david     (1000) david     (1000)     4597 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/timers.h
+-rw-r--r--   0 david     (1000) david     (1000)      300 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/include/taco/util/uncopyable.h
+-rw-r--r--   0 david     (1000) david     (1000)     2886 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/util/variadic.h
+-rw-r--r--   0 david     (1000) david     (1000)      884 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco/version.h.in
+-rw-r--r--   0 david     (1000) david     (1000)      196 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/include/taco.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.446375 tensora-0.0.8/src/taco/misc/
+-rw-r--r--   0 david     (1000) david     (1000)      523 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/misc/mainpage.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.446375 tensora-0.0.8/src/taco/python_bindings/
+-rw-r--r--   0 david     (1000) david     (1000)     1333 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)      584 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/Makefile
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.446375 tensora-0.0.8/src/taco/python_bindings/include/
+-rw-r--r--   0 david     (1000) david     (1000)      342 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyDatatypes.h
+-rw-r--r--   0 david     (1000) david     (1000)      372 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyFormat.h
+-rw-r--r--   0 david     (1000) david     (1000)      269 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyIndexNotation.h
+-rw-r--r--   0 david     (1000) david     (1000)      288 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyParsers.h
+-rw-r--r--   0 david     (1000) david     (1000)      242 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyTensor.h
+-rw-r--r--   0 david     (1000) david     (1000)      247 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyTensorIO.h
+-rw-r--r--   0 david     (1000) david     (1000)      168 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/include/pyeinsum.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.450374 tensora-0.0.8/src/taco/python_bindings/pybind11/
+-rw-rw-r--   0 david     (1000) david     (1000)     1304 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.appveyor.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      523 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.clang-format
+-rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.clang-tidy
+-rw-rw-r--   0 david     (1000) david     (1000)     2196 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.git
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.450374 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/
+-rw-rw-r--   0 david     (1000) david     (1000)    14415 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/CONTRIBUTING.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.450374 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 david     (1000) david     (1000)     1270 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      669 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-rw-r--   0 david     (1000) david     (1000)     1180 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/question.md
+-rw-rw-r--   0 david     (1000) david     (1000)      559 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/dependabot.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      116 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/labeler.yml
+-rw-rw-r--   0 david     (1000) david     (1000)       50 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/labeler_merged.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/pull_request_template.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.450374 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/
+-rw-rw-r--   0 david     (1000) david     (1000)    24549 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/ci.yml
+-rw-rw-r--   0 david     (1000) david     (1000)     2117 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/configure.yml
+-rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/format.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      333 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/labeler.yml
+-rw-rw-r--   0 david     (1000) david     (1000)     2497 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/pip.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      452 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.gitignore
+-rw-rw-r--   0 david     (1000) david     (1000)     2460 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 david     (1000) david     (1000)       62 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/.readthedocs.yml
+-rw-rw-r--   0 david     (1000) david     (1000)    10364 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     1684 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      256 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     8064 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.454374 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)      705 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/Doxyfile
+-rw-rw-r--   0 david     (1000) david     (1000)     7417 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/Makefile
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.454374 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/_static/
+-rw-rw-r--   0 david     (1000) david     (1000)      254 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/_static/theme_overrides.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.454374 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.458374 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/
+-rw-rw-r--   0 david     (1000) david     (1000)     3937 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/chrono.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3398 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/custom.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    14288 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/eigen.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3889 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/functional.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     1556 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    11680 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/overview.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     9703 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/stl.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     9372 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/strings.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    45877 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/classes.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     8420 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/embedding.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    14171 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/exceptions.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    25078 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/functions.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    12444 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/misc.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.458374 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    16538 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     7878 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/object.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     5125 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     6366 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/smart_ptrs.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     9369 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/basics.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     2974 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/benchmark.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3168 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/benchmark.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    73677 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/changelog.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    16122 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/classes.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.458374 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/cmake/
+-rw-rw-r--   0 david     (1000) david     (1000)      273 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/cmake/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    25511 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/compiling.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    12095 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/conf.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14592 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/faq.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      613 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3277 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/installing.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     3062 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/limitations.rst
+-rw-rw-r--   0 david     (1000) david     (1000)    58510 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11-logo.png
+-rw-rw-r--   0 david     (1000) david     (1000)    44653 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-rw-r--   0 david     (1000) david     (1000)    87708 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-rw-r--   0 david     (1000) david     (1000)    41121 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-rw-r--   0 david     (1000) david     (1000)    85853 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-rw-r--   0 david     (1000) david     (1000)     2113 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/reference.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     4028 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/release.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      168 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)    21940 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/docs/upgrade.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.430374 tensora-0.0.8/src/taco/python_bindings/pybind11/include/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.458374 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/
+-rw-rw-r--   0 david     (1000) david     (1000)    21412 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 david     (1000) david     (1000)     6118 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 david     (1000) david     (1000)    95557 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 david     (1000) david     (1000)     8185 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 david     (1000) david     (1000)      120 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 david     (1000) david     (1000)     2037 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.458374 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 david     (1000) david     (1000)    27823 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 david     (1000) david     (1000)    40452 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 david     (1000) david     (1000)     3602 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 david     (1000) david     (1000)    16397 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 david     (1000) david     (1000)    16375 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 david     (1000) david     (1000)     1486 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-r--   0 david     (1000) david     (1000)    29086 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 david     (1000) david     (1000)     7843 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 david     (1000) david     (1000)     5079 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 david     (1000) david     (1000)     3709 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 david     (1000) david     (1000)     6084 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 david     (1000) david     (1000)    69310 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 david     (1000) david     (1000)     9085 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 david     (1000) david     (1000)     2049 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 david     (1000) david     (1000)   111558 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 david     (1000) david     (1000)    66118 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/pytypes.h
+-rw-rw-r--   0 david     (1000) david     (1000)    14136 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 david     (1000) david     (1000)    23912 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.462374 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/
+-rw-rw-r--   0 david     (1000) david     (1000)      217 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/__main__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      202 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/_version.py
+-rw-rw-r--   0 david     (1000) david     (1000)      137 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/_version.pyi
+-rw-rw-r--   0 david     (1000) david     (1000)      663 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/commands.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/py.typed
+-rw-rw-r--   0 david     (1000) david     (1000)    15110 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/setup_helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1899 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/setup_helpers.pyi
+-rw-rw-r--   0 david     (1000) david     (1000)      118 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     2185 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     3499 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)    15362 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     4841 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/conftest.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11157 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/constructor_stats.h
+-rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/cross_module_gil_utils.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      376 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/env.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_python_package/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_python_package/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)     7074 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_python_package/test_files.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_setuptools/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_setuptools/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)     2581 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2144 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/local_bindings.h
+-rw-rw-r--   0 david     (1000) david     (1000)     5389 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/object.h
+-rw-rw-r--   0 david     (1000) david     (1000)     5285 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     3647 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pybind11_tests.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     2733 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pybind11_tests.h
+-rw-rw-r--   0 david     (1000) david     (1000)      626 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pytest.ini
+-rw-rw-r--   0 david     (1000) david     (1000)      736 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      864 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_async.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      558 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_async.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8048 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_buffers.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4946 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_buffers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13475 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_builtin_casters.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    17214 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_builtin_casters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3702 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_call_policies.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     5728 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_call_policies.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6600 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_callbacks.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4405 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_callbacks.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3406 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_chrono.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     6276 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_chrono.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21623 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_class.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    14273 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_class.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 david     (1000) david     (1000)     2639 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      656 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/embed.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 david     (1000) david     (1000)     1175 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 david     (1000) david     (1000)     1259 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.470374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 david     (1000) david     (1000)     1653 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      152 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/main.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 david     (1000) david     (1000)     1357 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 david     (1000) david     (1000)     1333 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      166 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/test.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5346 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1522 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9629 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_copy_move.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4645 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_copy_move.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5513 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4015 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_docstring_options.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1630 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_docstring_options.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16867 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eigen.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    28282 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eigen.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/
+-rw-rw-r--   0 david     (1000) david     (1000)     1758 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/CMakeLists.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      637 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/catch.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      554 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/external_module.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    10209 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2610 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_enum.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     7694 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_enum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2628 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eval.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      768 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eval.py
+-rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eval_call.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7862 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_exceptions.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     6753 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16562 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_factory_constructors.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    16637 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_factory_constructors.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1760 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_gil_scoped.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     3128 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_gil_scoped.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3381 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_iostream.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     5799 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_iostream.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6489 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    10048 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4333 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_local_bindings.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     8102 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_local_bindings.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19446 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    17310 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3742 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_modules.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     2841 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_modules.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8863 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     9495 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17781 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_array.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    18647 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_array.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17721 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    13484 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3832 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     9709 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2731 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_opaque_types.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1906 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_opaque_types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8431 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_operator_overloading.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     4136 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_operator_overloading.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4945 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pickling.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pickling.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13347 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pytypes.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    13720 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pytypes.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13120 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     5966 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17913 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_smart_ptr.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     9620 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_smart_ptr.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12793 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     8557 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4403 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl_binders.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)     7182 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl_binders.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4458 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      765 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.py
+-rw-rw-r--   0 david     (1000) david     (1000)      603 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_union.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_union.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18454 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_virtual_functions.cpp
+-rw-rw-r--   0 david     (1000) david     (1000)    11646 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_virtual_functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2558 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-rw-r--   0 david     (1000) david     (1000)     3103 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tests/valgrind-python.supp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/
+-rw-rw-r--   0 david     (1000) david     (1000)     2295 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     3105 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     9977 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/FindPythonLibsNew.cmake
+-rwxrwxr-x   0 david     (1000) david     (1000)     1427 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/check-style.sh
+-rw-rw-r--   0 david     (1000) david     (1000)      952 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1121 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/libsize.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     1202 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14003 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     7010 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 david     (1000) david     (1000)     9172 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     1822 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/python_bindings/pybind11/tools/setup_main.py.in
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pytaco/
+-rw-r--r--   0 david     (1000) david     (1000)       57 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/pytaco/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1542 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/pytaco/numpy_license.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/pytaco/pytensor/
+-rw-r--r--   0 david     (1000) david     (1000)       51 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/pytaco/pytensor/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)   111090 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/pytaco/pytensor/taco_tensor.py
+-rw-r--r--   0 david     (1000) david     (1000)     2248 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/pytaco/pytensor/tensorIO.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.474374 tensora-0.0.8/src/taco/python_bindings/source/
+-rw-r--r--   0 david     (1000) david     (1000)     2526 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/conf.py
+-rw-r--r--   0 david     (1000) david     (1000)      480 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/index.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.478374 tensora-0.0.8/src/taco/python_bindings/source/rst_files/
+-rw-r--r--   0 david     (1000) david     (1000)      114 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/as_np_dt.rst
+-rw-r--r--   0 david     (1000) david     (1000)      102 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/datatype.rst
+-rw-r--r--   0 david     (1000) david     (1000)       87 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/dtype_object.rst
+-rw-r--r--   0 david     (1000) david     (1000)      458 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/expr_funcs.rst
+-rw-r--r--   0 david     (1000) david     (1000)      780 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/file_io.rst
+-rw-r--r--   0 david     (1000) david     (1000)      111 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/format.rst
+-rw-r--r--   0 david     (1000) david     (1000)       73 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/format_class.rst
+-rw-r--r--   0 david     (1000) david     (1000)       71 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/format_funcs.rst
+-rw-r--r--   0 david     (1000) david     (1000)       91 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/idx_exp_obj.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1028 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/index_expressions.rst
+-rw-r--r--   0 david     (1000) david     (1000)       79 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/index_vars.rst
+-rw-r--r--   0 david     (1000) david     (1000)      131 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/iv_funcs.rst
+-rw-r--r--   0 david     (1000) david     (1000)       71 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/mode_format.rst
+-rw-r--r--   0 david     (1000) david     (1000)      152 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/parsers.rst
+-rw-r--r--   0 david     (1000) david     (1000)      199 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/sched.rst
+-rw-r--r--   0 david     (1000) david     (1000)       62 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/tensor_class.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1233 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/tensor_info.rst
+-rw-r--r--   0 david     (1000) david     (1000)       63 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/tensors.rst
+-rw-r--r--   0 david     (1000) david     (1000)      312 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/source/rst_files/udfs.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.478374 tensora-0.0.8/src/taco/python_bindings/src/
+-rw-r--r--   0 david     (1000) david     (1000)     4505 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pyDatatypes.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11285 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pyFormat.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    34934 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pyIndexNotation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3194 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pyParsers.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    18175 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pyTensor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      805 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pyTensorIO.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4379 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/src/pytaco.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    10971 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/python_bindings/unit_tests.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.478374 tensora-0.0.8/src/taco/src/
+-rw-r--r--   0 david     (1000) david     (1000)     1031 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/CMakeLists.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.478374 tensora-0.0.8/src/taco/src/codegen/
+-rw-r--r--   0 david     (1000) david     (1000)    19006 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/codegen.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3120 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/codegen.h
+-rw-r--r--   0 david     (1000) david     (1000)    17904 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/codegen_c.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1454 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/codegen_c.h
+-rw-r--r--   0 david     (1000) david     (1000)    49177 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/codegen_cuda.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3090 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/codegen_cuda.h
+-rw-r--r--   0 david     (1000) david     (1000)     5739 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/codegen/module.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1925 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/cuda.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.478374 tensora-0.0.8/src/taco/src/error/
+-rw-r--r--   0 david     (1000) david     (1000)     5070 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/error/error_checks.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      902 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/error/error_checks.h
+-rw-r--r--   0 david     (1000) david     (1000)     1309 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/error/error_messages.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1730 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/error.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11646 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/format.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.482374 tensora-0.0.8/src/taco/src/index_notation/
+-rw-r--r--   0 david     (1000) david     (1000)      356 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/index_notation/README.md
+-rw-r--r--   0 david     (1000) david     (1000)   116223 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/index_notation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2791 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/index_notation_nodes.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1049 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/index_notation/index_notation_nodes_abstract.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7250 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/index_notation_printer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11661 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/index_notation_rewriter.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2942 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/index_notation_visitor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    40775 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/index_notation/intrinsic.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     8065 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/iteration_algebra.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1309 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/iteration_algebra_printer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4292 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/index_notation/kernel.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4914 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/properties.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3423 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/property_pointers.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    58668 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/provenance_graph.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1424 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/index_notation/schedule.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4853 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/tensor_operator.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    74399 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/index_notation/transformations.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.482374 tensora-0.0.8/src/taco/src/ir/
+-rw-r--r--   0 david     (1000) david     (1000)      239 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/ir/README.md
+-rw-r--r--   0 david     (1000) david     (1000)    26833 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/ir.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1805 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/ir_generators.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    15742 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/ir_printer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    10832 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/ir_rewriter.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     8912 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/ir_verifier.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4411 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/ir_visitor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    19916 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/simplify.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2669 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir/workspace_rewriter.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      573 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/ir_tags.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.486374 tensora-0.0.8/src/taco/src/lower/
+-rw-r--r--   0 david     (1000) david     (1000)      260 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     7225 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/expr_tools.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      870 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/expr_tools.h
+-rw-r--r--   0 david     (1000) david     (1000)     6683 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/iteration_forest.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1020 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/iteration_forest.h
+-rw-r--r--   0 david     (1000) david     (1000)     8081 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/iteration_graph.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2945 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/iteration_graph.h
+-rw-r--r--   0 david     (1000) david     (1000)    23959 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/iterator.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2021 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/lower.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3152 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/lowerer_impl.cpp
+-rw-r--r--   0 david     (1000) david     (1000)   170132 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/lowerer_impl_imperative.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    49768 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/merge_lattice.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2880 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/mode.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      879 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/mode_access.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      819 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/mode_access.h
+-rw-r--r--   0 david     (1000) david     (1000)    11956 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/mode_format_compressed.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2878 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/mode_format_dense.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     8358 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/mode_format_impl.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     6169 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/lower/mode_format_singleton.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2930 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/tensor_path.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2200 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/lower/tensor_path.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.486374 tensora-0.0.8/src/taco/src/parser/
+-rw-r--r--   0 david     (1000) david     (1000)      293 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/parser/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     9758 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/parser/einsum_parser.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3565 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/parser/lexer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11905 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/parser/parser.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7141 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/parser/schedule_parser.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.486374 tensora-0.0.8/src/taco/src/storage/
+-rw-r--r--   0 david     (1000) david     (1000)      152 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/storage/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     5348 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/storage/array.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    12244 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/storage/file_io_mtx.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13141 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/storage/file_io_rb.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     4661 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/storage/file_io_tns.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3551 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/storage/index.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7948 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/storage/pack.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     6004 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/storage/storage.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    18028 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/storage/typed_index.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    23635 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/storage/typed_value.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2366 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/taco_tensor_t.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1904 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/target.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    47292 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/tensor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     9240 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/type.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.486374 tensora-0.0.8/src/taco/src/util/
+-rw-r--r--   0 david     (1000) david     (1000)      635 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/util/env.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      512 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/util/files.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      880 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/src/util/name_generator.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1062 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/src/util/strings.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.490374 tensora-0.0.8/src/taco/test/
+-rw-r--r--   0 david     (1000) david     (1000)      931 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)     3773 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/README_testing.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/
+-rw-rw-r--   0 david     (1000) david     (1000)      546 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.appveyor.yml
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/.devcontainer/
+-rw-rw-r--   0 david     (1000) david     (1000)      519 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.devcontainer/Dockerfile
+-rw-rw-r--   0 david     (1000) david     (1000)       83 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.devcontainer/devcontainer.json
+-rw-rw-r--   0 david     (1000) david     (1000)      687 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.editorconfig
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-06-15 20:50:05.000000 tensora-0.0.8/src/taco/test/bats/.git
+-rwxrwxr-x   0 david     (1000) david     (1000)       41 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.gitattributes
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.gitignore
+-rw-rw-r--   0 david     (1000) david     (1000)      800 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/.travis.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/AUTHORS
+-rw-rw-r--   0 david     (1000) david     (1000)      386 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/Dockerfile
+-rw-rw-r--   0 david     (1000) david     (1000)     2535 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/LICENSE.md
+-rw-rw-r--   0 david     (1000) david     (1000)    23464 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/bin/
+-rwxrwxr-x   0 david     (1000) david     (1000)     1675 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/bin/bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/contrib/
+-rwxrwxr-x   0 david     (1000) david     (1000)     3795 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/contrib/release.sh
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/contrib/rpm/
+-rw-rw-r--   0 david     (1000) david     (1000)     1575 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/contrib/rpm/bats.spec
+-rwxrwxr-x   0 david     (1000) david     (1000)     7973 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/contrib/semver
+-rw-rw-r--   0 david     (1000) david     (1000)      147 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docker-compose.override.dist
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docker-compose.yml
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)     7042 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)      211 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/CODEOWNERS
+-rw-rw-r--   0 david     (1000) david     (1000)     3643 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 david     (1000) david     (1000)    17557 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/CONTRIBUTING.md
+-rw-rw-r--   0 david     (1000) david     (1000)      317 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/docs/examples/
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/examples/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      604 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/examples/package-tarball
+-rwxrwxr-x   0 david     (1000) david     (1000)      869 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/examples/package-tarball.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     3979 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/releasing.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2338 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/usage.md
+-rw-rw-r--   0 david     (1000) david     (1000)      287 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/docs/versions.md
+-rwxrwxr-x   0 david     (1000) david     (1000)      627 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/install.sh
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.430374 tensora-0.0.8/src/taco/test/bats/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/lib/bats-core/
+-rw-rw-r--   0 david     (1000) david     (1000)      827 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/lib/bats-core/preprocessing.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     2646 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/lib/bats-core/test_functions.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     4197 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/lib/bats-core/tracing.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     1002 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/lib/bats-core/validator.bash
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.430374 tensora-0.0.8/src/taco/test/bats/libexec/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/
+-rwxrwxr-x   0 david     (1000) david     (1000)     5567 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats
+-rwxrwxr-x   0 david     (1000) david     (1000)     5654 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-exec-file
+-rwxrwxr-x   0 david     (1000) david     (1000)     2386 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-exec-suite
+-rwxrwxr-x   0 david     (1000) david     (1000)     4762 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-exec-test
+-rwxrwxr-x   0 david     (1000) david     (1000)     3436 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-format-junit
+-rwxrwxr-x   0 david     (1000) david     (1000)     4421 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-format-pretty
+-rwxrwxr-x   0 david     (1000) david     (1000)       32 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-format-tap
+-rwxrwxr-x   0 david     (1000) david     (1000)     1308 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-preprocess
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.494374 tensora-0.0.8/src/taco/test/bats/man/
+-rw-rw-r--   0 david     (1000) david     (1000)      427 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/man/Makefile
+-rw-rw-r--   0 david     (1000) david     (1000)      253 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/man/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)     3836 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/man/bats.1
+-rw-rw-r--   0 david     (1000) david     (1000)     3544 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/man/bats.1.ronn
+-rw-rw-r--   0 david     (1000) david     (1000)     4928 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/man/bats.7
+-rw-rw-r--   0 david     (1000) david     (1000)     4510 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/man/bats.7.ronn
+-rw-rw-r--   0 david     (1000) david     (1000)      641 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/package.json
+-rwxrwxr-x   0 david     (1000) david     (1000)      277 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/shellcheck.sh
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.498374 tensora-0.0.8/src/taco/test/bats/test/
+-rwxrwxr-x   0 david     (1000) david     (1000)    20307 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/bats.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     7356 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/file_setup_teardown.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.430374 tensora-0.0.8/src/taco/test/bats/test/fixtures/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.502374 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/
+-rw-rw-r--   0 david     (1000) david     (1000)      171 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/ambiguous
+-rw-rw-r--   0 david     (1000) david     (1000)      179 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/ambiguous.bash
+-rwxrwxr-x   0 david     (1000) david     (1000)      295 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/cmd_using_stdin.bash
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/dos_line.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      233 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/duplicate-tests.bats
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/empty.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      138 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/environment.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/expand_var_in_test_name.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      104 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/exported_function.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     1186 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/external_function_calls.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       72 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/failing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/failing_and_passing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       80 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/failing_helper.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/failing_setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       83 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/failing_teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/intact.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      118 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/load.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      239 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/loop_keep_IFS.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/no-final-newline.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      331 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/output.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/parallel.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/passing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/passing_and_failing.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/passing_and_skipping.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      106 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/passing_failing_and_skipping.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      109 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/quoted_and_unquoted_test_names.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      501 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/read_from_stdin.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       81 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      179 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter_in_setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/reference_unset_parameter_in_teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      266 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/single_line.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/skipped.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/skipped_with_parens.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       72 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file_in_setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      104 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/source_nonexistent_file_in_teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      169 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      267 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/test_helper.bash
+-rw-rw-r--   0 david     (1000) david     (1000)      331 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/unbound_variable.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       50 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/unofficial_bash_strict_mode.bash
+-rw-rw-r--   0 david     (1000) david     (1000)       92 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/unofficial_bash_strict_mode.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      593 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/whitespace.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       24 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/without_trailing_newline.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/no_setup_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       26 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/no_teardown_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      317 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       91 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_does_not_leak_env.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       69 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_does_not_leak_env2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      125 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_even_if_all_tests_are_skipped.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       84 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_failed.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       71 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/setup_file_halfway_error.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      117 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      117 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       96 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_after_failing_test.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      152 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_after_long_test.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      108 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_does_not_leak.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_does_not_leak2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      160 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_even_if_all_tests_are_skipped.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       57 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_failed.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/file_setup_teardown/teardown_file_halfway_error.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/
+-rw-rw-r--   0 david     (1000) david     (1000)      191 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/parallel-preserve-environment.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/parallel.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/setup_file/
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file1.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/setup_file/setup_file3.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/suite/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/suite/parallel1.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/suite/parallel2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/suite/parallel3.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/parallel/suite/parallel4.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.434374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/empty/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/empty/.gitkeep
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/filter/
+-rw-rw-r--   0 david     (1000) david     (1000)       65 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/filter/a.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       66 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/filter/b.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       68 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/filter/c.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/multiple/
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/multiple/a.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       73 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/multiple/b.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/recursive/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/recursive/subsuite/
+-rw-rw-r--   0 david     (1000) david     (1000)       40 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/recursive/subsuite/test2.bats
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/recursive/test.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/single/
+-rw-rw-r--   0 david     (1000) david     (1000)       34 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/single/test.bats
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/skip/
+-rw-rw-r--   0 david     (1000) david     (1000)      319 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/skip/skip-in-setup-and-teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      194 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/skip/skip-in-setup.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      158 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/skip/skip-in-teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      245 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/skip/skip-in-test-and-teardown.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      131 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/fixtures/suite/skip/skip-in-test.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     2116 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/install.bats
+-rw-rw-r--   0 david     (1000) david     (1000)      583 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/junit-formatter.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     2323 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/parallell.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/root.bats
+-rwxrwxr-x   0 david     (1000) david     (1000)     4913 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/suite.bats
+-rw-rw-r--   0 david     (1000) david     (1000)     1034 2023-06-15 20:50:06.000000 tensora-0.0.8/src/taco/test/bats/test/test_helper.bash
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/data/
+-rw-r--r--   0 david     (1000) david     (1000)      119 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/2tensor.mtx
+-rw-r--r--   0 david     (1000) david     (1000)       36 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/3tensor.tns
+-rw-r--r--   0 david     (1000) david     (1000)      267 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/d33.mtx
+-rw-r--r--   0 david     (1000) david     (1000)       66 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/d33.ttx
+-rw-r--r--   0 david     (1000) david     (1000)      136 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/d432.ttx
+-rw-r--r--   0 david     (1000) david     (1000)       88 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/d567.ttx
+-rw-r--r--   0 david     (1000) david     (1000)      268 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/ds33.mtx
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.506374 tensora-0.0.8/src/taco/test/data/qcd/
+-rw-r--r--   0 david     (1000) david     (1000)    11615 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/qcd/theta.ttx
+-rw-r--r--   0 david     (1000) david     (1000)       64 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/qcd/theta_simple.ttx
+-rw-r--r--   0 david     (1000) david     (1000)      555 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/qcd/z.ttx
+-rw-r--r--   0 david     (1000) david     (1000)       52 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/qcd/z_simple.ttx
+-rw-r--r--   0 david     (1000) david     (1000)     1487 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/rua_32.mtx
+-rw-r--r--   0 david     (1000) david     (1000)     1986 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/data/rua_32.rb
+-rw-r--r--   0 david     (1000) david     (1000)     4650 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/expr_factory.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2589 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/expr_factory.h
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.510374 tensora-0.0.8/src/taco/test/gtest/
+-rw-r--r--   0 david     (1000) david     (1000)     1475 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/gtest/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      155 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/gtest/README.TAC
+-rw-r--r--   0 david     (1000) david     (1000)   365644 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/gtest/gtest-all.cc
+-rw-r--r--   0 david     (1000) david     (1000)   849134 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/gtest/gtest.h
+-rw-r--r--   0 david     (1000) david     (1000)     4788 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/op_factory.h
+-rwxr-xr-x   0 david     (1000) david     (1000)    12555 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/taco-cli-test.bats
+-rw-r--r--   0 david     (1000) david     (1000)     7165 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test-iteration_algebra.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1110 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test-typedcomponent-memory.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1897 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3618 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test.h
+-rw-r--r--   0 david     (1000) david     (1000)     3125 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test_properties.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    11493 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test_tensors.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     5687 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/test_tensors.h
+-rw-r--r--   0 david     (1000) david     (1000)    12251 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-api.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2561 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-copyprop.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1310 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-error.cpp
+-rw-r--r--   0 david     (1000) david     (1000)      493 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-expr-reduction.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     5044 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-expr.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    43783 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-expr_storage.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3200 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-format-mm-permute.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2112 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-format.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1044 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-index.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13133 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-index_notation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2306 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-indexexpr.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     2918 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-indexstmt.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3609 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-io.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    55894 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-lower.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    59718 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-merge_lattice.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7101 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-parafac.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     1837 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-qcd.cpp
+-rw-r--r--   0 david     (1000) david     (1000)       68 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-regression.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3602 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-schedule-parser.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    76554 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-scheduling-eval.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    32561 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-scheduling.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    14078 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-storage.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3573 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-storage_alloc.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13383 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-tensor.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    13605 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-tensor_types.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    14092 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-transformation.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3574 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-transpose.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     3576 2020-07-08 22:41:29.000000 tensora-0.0.8/src/taco/test/tests-type.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    19463 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-windowing.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    17609 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/test/tests-workspaces.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.510374 tensora-0.0.8/src/taco/tools/
+-rw-r--r--   0 david     (1000) david     (1000)      490 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/tools/CMakeLists.txt
+-rw-r--r--   0 david     (1000) david     (1000)    52311 2023-01-16 18:11:38.000000 tensora-0.0.8/src/taco/tools/taco.cpp
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.510374 tensora-0.0.8/src/tensora/
+-rw-rw-r--   0 david     (1000) david     (1000)      148 2020-07-08 11:47:39.000000 tensora-0.0.8/src/tensora/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19747 2023-01-16 18:11:03.000000 tensora-0.0.8/src/tensora/compile.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.510374 tensora-0.0.8/src/tensora/expression/
+-rw-rw-r--   0 david     (1000) david     (1000)       93 2023-06-15 20:57:19.000000 tensora-0.0.8/src/tensora/expression/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5267 2020-07-08 11:47:39.000000 tensora-0.0.8/src/tensora/expression/ast.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1676 2023-06-15 20:57:23.000000 tensora-0.0.8/src/tensora/expression/parser.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.510374 tensora-0.0.8/src/tensora/format/
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2020-07-08 11:47:39.000000 tensora-0.0.8/src/tensora/format/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1305 2020-07-08 11:47:39.000000 tensora-0.0.8/src/tensora/format/format.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1502 2023-06-16 10:05:44.000000 tensora-0.0.8/src/tensora/format/parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7052 2023-06-15 20:57:23.000000 tensora-0.0.8/src/tensora/function.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23902 2023-06-15 20:57:23.000000 tensora-0.0.8/src/tensora/tensor.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.510374 tensora-0.0.8/src/tensora.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     9253 2023-06-27 10:40:05.000000 tensora-0.0.8/src/tensora.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    33517 2023-06-27 10:40:05.000000 tensora-0.0.8/src/tensora.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-27 10:40:05.000000 tensora-0.0.8/src/tensora.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-16 11:43:57.000000 tensora-0.0.8/src/tensora.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-06-27 10:40:05.000000 tensora-0.0.8/src/tensora.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-06-27 10:40:05.000000 tensora-0.0.8/src/tensora.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 10:40:05.514374 tensora-0.0.8/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     4741 2023-06-15 20:57:19.000000 tensora-0.0.8/tests/test_combinatorically.py
+-rw-r--r--   0 david     (1000) david     (1000)     2852 2023-01-16 18:11:03.000000 tensora-0.0.8/tests/test_compile.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2685 2023-06-15 20:57:23.000000 tensora-0.0.8/tests/test_expression.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1686 2023-06-15 20:57:23.000000 tensora-0.0.8/tests/test_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9370 2020-07-08 11:47:39.000000 tensora-0.0.8/tests/test_from_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2901 2023-01-16 18:11:03.000000 tensora-0.0.8/tests/test_function.py
+-rw-r--r--   0 david     (1000) david     (1000)      583 2023-01-16 18:11:03.000000 tensora-0.0.8/tests/test_numpy.py
+-rw-rw-r--   0 david     (1000) david     (1000)      668 2020-07-08 11:47:39.000000 tensora-0.0.8/tests/test_operators.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10193 2023-01-16 18:11:03.000000 tensora-0.0.8/tests/test_tensor.py
```

### Comparing `tensora-0.0.7/LICENSE` & `tensora-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/PKG-INFO` & `tensora-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensora
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for dense and sparse tensors built on the tensor algebra compiler.
 Home-page: https://github.com/drhagen/tensora
 Author: David Hagen
 Author-email: david@drhagen.com
 License: MIT
 Keywords: tensor sparse matrix array
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tensora-0.0.7/README.md` & `tensora-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/setup.py` & `tensora-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         # Ensure that platform tag is included because binaries are platform-specific
         self.root_is_pure = False
 
 
 setup(
     name='tensora',
-    version='0.0.7',
+    version='0.0.8',
 
     description='Library for dense and sparse tensors built on the tensor algebra compiler.',
     long_description=Path('README.md').read_text(encoding='utf-8'),
     long_description_content_type='text/markdown',
     keywords='tensor sparse matrix array',
 
     author='David Hagen',
```

### Comparing `tensora-0.0.7/src/taco/.github/workflows/buildandtest.yml` & `tensora-0.0.8/src/taco/.github/workflows/buildandtest.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/.github/workflows/cuda-test-manual.yml` & `tensora-0.0.8/src/taco/.github/workflows/cuda-test-manual.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/CMakeLists.txt` & `tensora-0.0.8/src/taco/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/Doxyfile` & `tensora-0.0.8/src/taco/Doxyfile`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/LICENSE` & `tensora-0.0.8/src/taco/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/README.md` & `tensora-0.0.8/src/taco/README.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/apps/tensor_times_vector/CMakeLists.txt` & `tensora-0.0.8/src/taco/apps/tensor_times_vector/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/ci/test-pr.md` & `tensora-0.0.8/src/taco/ci/test-pr.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/ci/test-pr.py` & `tensora-0.0.8/src/taco/ci/test-pr.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/codegen/module.h` & `tensora-0.0.8/src/taco/include/taco/codegen/module.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/component.h` & `tensora-0.0.8/src/taco/include/taco/component.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/coordinate.h` & `tensora-0.0.8/src/taco/include/taco/coordinate.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/cuda.h` & `tensora-0.0.8/src/taco/include/taco/cuda.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/error/error_messages.h` & `tensora-0.0.8/src/taco/include/taco/error/error_messages.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/error.h` & `tensora-0.0.8/src/taco/include/taco/error.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/format.h` & `tensora-0.0.8/src/taco/include/taco/format.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/README.md` & `tensora-0.0.8/src/taco/include/taco/index_notation/README.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/index_notation.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_nodes.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_nodes_abstract.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_printer.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_printer.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_rewriter.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_rewriter.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/index_notation_visitor.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/index_notation_visitor.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/intrinsic.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/intrinsic.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/iteration_algebra.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/iteration_algebra.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/iteration_algebra_printer.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/iteration_algebra_printer.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/kernel.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/kernel.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/properties.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/properties.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/property_pointers.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/property_pointers.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/provenance_graph.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/provenance_graph.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/schedule.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/schedule.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/tensor_operator.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/tensor_operator.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/index_notation/transformations.h` & `tensora-0.0.8/src/taco/include/taco/index_notation/transformations.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir/ir.h` & `tensora-0.0.8/src/taco/include/taco/ir/ir.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir/ir_generators.h` & `tensora-0.0.8/src/taco/include/taco/ir/ir_generators.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir/ir_printer.h` & `tensora-0.0.8/src/taco/include/taco/ir/ir_printer.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir/ir_rewriter.h` & `tensora-0.0.8/src/taco/include/taco/ir/ir_rewriter.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir/ir_visitor.h` & `tensora-0.0.8/src/taco/include/taco/ir/ir_visitor.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir/workspace_rewriter.h` & `tensora-0.0.8/src/taco/include/taco/ir/workspace_rewriter.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/ir_tags.h` & `tensora-0.0.8/src/taco/include/taco/ir_tags.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/iterator.h` & `tensora-0.0.8/src/taco/include/taco/lower/iterator.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/lower.h` & `tensora-0.0.8/src/taco/include/taco/lower/lower.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/lowerer_impl.h` & `tensora-0.0.8/src/taco/include/taco/lower/lowerer_impl.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/lowerer_impl_imperative.h` & `tensora-0.0.8/src/taco/include/taco/lower/lowerer_impl_imperative.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/merge_lattice.h` & `tensora-0.0.8/src/taco/include/taco/lower/merge_lattice.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/mode.h` & `tensora-0.0.8/src/taco/include/taco/lower/mode.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/mode_format_compressed.h` & `tensora-0.0.8/src/taco/include/taco/lower/mode_format_compressed.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/mode_format_dense.h` & `tensora-0.0.8/src/taco/include/taco/lower/mode_format_dense.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/mode_format_impl.h` & `tensora-0.0.8/src/taco/include/taco/lower/mode_format_impl.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/lower/mode_format_singleton.h` & `tensora-0.0.8/src/taco/include/taco/lower/mode_format_singleton.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/parser/einsum_parser.h` & `tensora-0.0.8/src/taco/include/taco/parser/einsum_parser.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/parser/lexer.h` & `tensora-0.0.8/src/taco/include/taco/parser/lexer.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/parser/parser.h` & `tensora-0.0.8/src/taco/include/taco/parser/parser.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/parser/schedule_parser.h` & `tensora-0.0.8/src/taco/include/taco/parser/schedule_parser.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/array.h` & `tensora-0.0.8/src/taco/include/taco/storage/array.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/coordinate.h` & `tensora-0.0.8/src/taco/include/taco/storage/coordinate.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/file_io_mtx.h` & `tensora-0.0.8/src/taco/include/taco/storage/file_io_mtx.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/file_io_rb.h` & `tensora-0.0.8/src/taco/include/taco/storage/file_io_rb.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/file_io_tns.h` & `tensora-0.0.8/src/taco/include/taco/storage/file_io_tns.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/index.h` & `tensora-0.0.8/src/taco/include/taco/storage/index.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/pack.h` & `tensora-0.0.8/src/taco/include/taco/storage/pack.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/storage.h` & `tensora-0.0.8/src/taco/include/taco/storage/storage.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/typed_index.h` & `tensora-0.0.8/src/taco/include/taco/storage/typed_index.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/typed_value.h` & `tensora-0.0.8/src/taco/include/taco/storage/typed_value.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/storage/typed_vector.h` & `tensora-0.0.8/src/taco/include/taco/storage/typed_vector.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/taco_tensor_t.h` & `tensora-0.0.8/src/taco/include/taco/taco_tensor_t.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/target.h` & `tensora-0.0.8/src/taco/include/taco/target.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/tensor.h` & `tensora-0.0.8/src/taco/include/taco/tensor.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/type.h` & `tensora-0.0.8/src/taco/include/taco/type.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/collections.h` & `tensora-0.0.8/src/taco/include/taco/util/collections.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/comparable.h` & `tensora-0.0.8/src/taco/include/taco/util/comparable.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/env.h` & `tensora-0.0.8/src/taco/include/taco/util/env.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/fill.h` & `tensora-0.0.8/src/taco/include/taco/util/fill.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/functions.h` & `tensora-0.0.8/src/taco/include/taco/util/functions.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/intrusive_ptr.h` & `tensora-0.0.8/src/taco/include/taco/util/intrusive_ptr.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/scopedmap.h` & `tensora-0.0.8/src/taco/include/taco/util/scopedmap.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/scopedset.h` & `tensora-0.0.8/src/taco/include/taco/util/scopedset.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/strings.h` & `tensora-0.0.8/src/taco/include/taco/util/strings.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/timers.h` & `tensora-0.0.8/src/taco/include/taco/util/timers.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/util/variadic.h` & `tensora-0.0.8/src/taco/include/taco/util/variadic.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/include/taco/version.h.in` & `tensora-0.0.8/src/taco/include/taco/version.h.in`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/misc/mainpage.h` & `tensora-0.0.8/src/taco/misc/mainpage.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/Makefile` & `tensora-0.0.8/src/taco/python_bindings/Makefile`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.appveyor.yml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.clang-format` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.cmake-format.yaml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/CONTRIBUTING.md` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/bug-report.md` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/feature-request.md` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/question.md` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/dependabot.yml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/ci.yml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/configure.yml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/format.yml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.github/workflows/pip.yml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/.pre-commit-config.yaml` & `tensora-0.0.8/src/taco/python_bindings/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/LICENSE` & `tensora-0.0.8/src/taco/python_bindings/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/README.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/Doxyfile` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/Makefile` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/chrono.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/custom.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/eigen.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/functional.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/index.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/overview.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/stl.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/cast/strings.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/classes.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/embedding.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/exceptions.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/functions.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/misc.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/numpy.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/object.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/pycpp/utilities.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/advanced/smart_ptrs.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/basics.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/benchmark.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/benchmark.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/changelog.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/classes.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/compiling.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/conf.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/faq.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/index.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/installing.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/limitations.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11-logo.png` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.png` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.svg` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.png` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.svg` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/reference.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/release.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/docs/upgrade.rst` & `tensora-0.0.8/src/taco/python_bindings/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/attr.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/buffer_info.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/cast.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/chrono.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/complex.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/class.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/common.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/descr.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/init.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/internals.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/detail/typeid.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/eigen.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/embed.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/eval.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/functional.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/iostream.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/numpy.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/operators.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/options.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/pybind11.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/pytypes.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/stl.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/include/pybind11/stl_bind.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/__main__.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/commands.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/setup_helpers.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/pybind11/setup_helpers.pyi` & `tensora-0.0.8/src/taco/python_bindings/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/setup.cfg` & `tensora-0.0.8/src/taco/python_bindings/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/setup.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/conftest.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/constructor_stats.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/cross_module_gil_utils.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_python_package/test_files.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/extra_setuptools/test_setuphelper.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/local_bindings.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/object.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_cross_module_tests.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_tests.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pybind11_tests.h` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/pytest.ini` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/requirements.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_async.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_async.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_buffers.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_buffers.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_builtin_casters.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_builtin_casters.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_call_policies.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_call_policies.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_callbacks.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_callbacks.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_chrono.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_chrono.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_class.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_class.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/embed.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_copy_move.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_copy_move.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_docstring_options.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_docstring_options.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eigen.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eigen.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/CMakeLists.txt` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/catch.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/external_module.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_enum.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_enum.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_eval.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_exceptions.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_exceptions.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_factory_constructors.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_factory_constructors.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_gil_scoped.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_gil_scoped.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_iostream.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_iostream.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_local_bindings.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_local_bindings.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_modules.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_modules.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_array.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_array.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_opaque_types.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_opaque_types.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_operator_overloading.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_operator_overloading.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pickling.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pickling.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pytypes.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_pytypes.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_smart_ptr.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_smart_ptr.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl_binders.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_stl_binders.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_union.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_virtual_functions.cpp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/test_virtual_functions.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/valgrind-numpy-scipy.supp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tests/valgrind-python.supp` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindCatch.cmake` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindEigen3.cmake` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/FindPythonLibsNew.cmake` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/check-style.sh` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/cmake_uninstall.cmake.in` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/libsize.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/make_changelog.py` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Common.cmake` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Config.cmake.in` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11NewTools.cmake` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/pybind11Tools.cmake` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/setup_global.py.in` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pybind11/tools/setup_main.py.in` & `tensora-0.0.8/src/taco/python_bindings/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pytaco/numpy_license.txt` & `tensora-0.0.8/src/taco/python_bindings/pytaco/numpy_license.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/taco_tensor.py` & `tensora-0.0.8/src/taco/python_bindings/pytaco/pytensor/taco_tensor.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/pytaco/pytensor/tensorIO.py` & `tensora-0.0.8/src/taco/python_bindings/pytaco/pytensor/tensorIO.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/source/conf.py` & `tensora-0.0.8/src/taco/python_bindings/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/source/rst_files/file_io.rst` & `tensora-0.0.8/src/taco/python_bindings/source/rst_files/file_io.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/source/rst_files/index_expressions.rst` & `tensora-0.0.8/src/taco/python_bindings/source/rst_files/index_expressions.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/source/rst_files/tensor_info.rst` & `tensora-0.0.8/src/taco/python_bindings/source/rst_files/tensor_info.rst`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pyDatatypes.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pyDatatypes.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pyFormat.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pyFormat.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pyIndexNotation.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pyIndexNotation.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pyParsers.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pyParsers.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pyTensor.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pyTensor.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pyTensorIO.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pyTensorIO.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/src/pytaco.cpp` & `tensora-0.0.8/src/taco/python_bindings/src/pytaco.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/python_bindings/unit_tests.py` & `tensora-0.0.8/src/taco/python_bindings/unit_tests.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/CMakeLists.txt` & `tensora-0.0.8/src/taco/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/codegen.cpp` & `tensora-0.0.8/src/taco/src/codegen/codegen.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/codegen.h` & `tensora-0.0.8/src/taco/src/codegen/codegen.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/codegen_c.cpp` & `tensora-0.0.8/src/taco/src/codegen/codegen_c.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/codegen_c.h` & `tensora-0.0.8/src/taco/src/codegen/codegen_c.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/codegen_cuda.cpp` & `tensora-0.0.8/src/taco/src/codegen/codegen_cuda.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/codegen_cuda.h` & `tensora-0.0.8/src/taco/src/codegen/codegen_cuda.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/codegen/module.cpp` & `tensora-0.0.8/src/taco/src/codegen/module.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/cuda.cpp` & `tensora-0.0.8/src/taco/src/cuda.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/error/error_checks.cpp` & `tensora-0.0.8/src/taco/src/error/error_checks.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/error/error_checks.h` & `tensora-0.0.8/src/taco/src/error/error_checks.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/error/error_messages.cpp` & `tensora-0.0.8/src/taco/src/error/error_messages.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/error.cpp` & `tensora-0.0.8/src/taco/src/error.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/format.cpp` & `tensora-0.0.8/src/taco/src/format.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/index_notation.cpp` & `tensora-0.0.8/src/taco/src/index_notation/index_notation.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes.cpp` & `tensora-0.0.8/src/taco/src/index_notation/index_notation_nodes.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/index_notation_nodes_abstract.cpp` & `tensora-0.0.8/src/taco/src/index_notation/index_notation_nodes_abstract.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/index_notation_printer.cpp` & `tensora-0.0.8/src/taco/src/index_notation/index_notation_printer.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/index_notation_rewriter.cpp` & `tensora-0.0.8/src/taco/src/index_notation/index_notation_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/index_notation_visitor.cpp` & `tensora-0.0.8/src/taco/src/index_notation/index_notation_visitor.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/intrinsic.cpp` & `tensora-0.0.8/src/taco/src/index_notation/intrinsic.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/iteration_algebra.cpp` & `tensora-0.0.8/src/taco/src/index_notation/iteration_algebra.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/iteration_algebra_printer.cpp` & `tensora-0.0.8/src/taco/src/index_notation/iteration_algebra_printer.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/kernel.cpp` & `tensora-0.0.8/src/taco/src/index_notation/kernel.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/properties.cpp` & `tensora-0.0.8/src/taco/src/index_notation/properties.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/property_pointers.cpp` & `tensora-0.0.8/src/taco/src/index_notation/property_pointers.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/provenance_graph.cpp` & `tensora-0.0.8/src/taco/src/index_notation/provenance_graph.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/schedule.cpp` & `tensora-0.0.8/src/taco/src/index_notation/schedule.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/tensor_operator.cpp` & `tensora-0.0.8/src/taco/src/index_notation/tensor_operator.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/index_notation/transformations.cpp` & `tensora-0.0.8/src/taco/src/index_notation/transformations.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/ir.cpp` & `tensora-0.0.8/src/taco/src/ir/ir.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/ir_generators.cpp` & `tensora-0.0.8/src/taco/src/ir/ir_generators.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/ir_printer.cpp` & `tensora-0.0.8/src/taco/src/ir/ir_printer.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/ir_rewriter.cpp` & `tensora-0.0.8/src/taco/src/ir/ir_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/ir_verifier.cpp` & `tensora-0.0.8/src/taco/src/ir/ir_verifier.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/ir_visitor.cpp` & `tensora-0.0.8/src/taco/src/ir/ir_visitor.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/simplify.cpp` & `tensora-0.0.8/src/taco/src/ir/simplify.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir/workspace_rewriter.cpp` & `tensora-0.0.8/src/taco/src/ir/workspace_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/ir_tags.cpp` & `tensora-0.0.8/src/taco/src/ir_tags.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/expr_tools.cpp` & `tensora-0.0.8/src/taco/src/lower/expr_tools.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/expr_tools.h` & `tensora-0.0.8/src/taco/src/lower/expr_tools.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/iteration_forest.cpp` & `tensora-0.0.8/src/taco/src/lower/iteration_forest.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/iteration_forest.h` & `tensora-0.0.8/src/taco/src/lower/iteration_forest.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/iteration_graph.cpp` & `tensora-0.0.8/src/taco/src/lower/iteration_graph.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/iteration_graph.h` & `tensora-0.0.8/src/taco/src/lower/iteration_graph.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/iterator.cpp` & `tensora-0.0.8/src/taco/src/lower/iterator.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/lower.cpp` & `tensora-0.0.8/src/taco/src/lower/lower.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/lowerer_impl.cpp` & `tensora-0.0.8/src/taco/src/lower/lowerer_impl.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/lowerer_impl_imperative.cpp` & `tensora-0.0.8/src/taco/src/lower/lowerer_impl_imperative.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/merge_lattice.cpp` & `tensora-0.0.8/src/taco/src/lower/merge_lattice.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode.cpp` & `tensora-0.0.8/src/taco/src/lower/mode.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode_access.cpp` & `tensora-0.0.8/src/taco/src/lower/mode_access.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode_access.h` & `tensora-0.0.8/src/taco/src/lower/mode_access.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode_format_compressed.cpp` & `tensora-0.0.8/src/taco/src/lower/mode_format_compressed.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode_format_dense.cpp` & `tensora-0.0.8/src/taco/src/lower/mode_format_dense.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode_format_impl.cpp` & `tensora-0.0.8/src/taco/src/lower/mode_format_impl.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/mode_format_singleton.cpp` & `tensora-0.0.8/src/taco/src/lower/mode_format_singleton.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/tensor_path.cpp` & `tensora-0.0.8/src/taco/src/lower/tensor_path.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/lower/tensor_path.h` & `tensora-0.0.8/src/taco/src/lower/tensor_path.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/parser/einsum_parser.cpp` & `tensora-0.0.8/src/taco/src/parser/einsum_parser.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/parser/lexer.cpp` & `tensora-0.0.8/src/taco/src/parser/lexer.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/parser/parser.cpp` & `tensora-0.0.8/src/taco/src/parser/parser.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/parser/schedule_parser.cpp` & `tensora-0.0.8/src/taco/src/parser/schedule_parser.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/array.cpp` & `tensora-0.0.8/src/taco/src/storage/array.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/file_io_mtx.cpp` & `tensora-0.0.8/src/taco/src/storage/file_io_mtx.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/file_io_rb.cpp` & `tensora-0.0.8/src/taco/src/storage/file_io_rb.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/file_io_tns.cpp` & `tensora-0.0.8/src/taco/src/storage/file_io_tns.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/index.cpp` & `tensora-0.0.8/src/taco/src/storage/index.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/pack.cpp` & `tensora-0.0.8/src/taco/src/storage/pack.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/storage.cpp` & `tensora-0.0.8/src/taco/src/storage/storage.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/typed_index.cpp` & `tensora-0.0.8/src/taco/src/storage/typed_index.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/storage/typed_value.cpp` & `tensora-0.0.8/src/taco/src/storage/typed_value.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/taco_tensor_t.cpp` & `tensora-0.0.8/src/taco/src/taco_tensor_t.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/target.cpp` & `tensora-0.0.8/src/taco/src/target.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/tensor.cpp` & `tensora-0.0.8/src/taco/src/tensor.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/type.cpp` & `tensora-0.0.8/src/taco/src/type.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/util/env.cpp` & `tensora-0.0.8/src/taco/src/util/env.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/util/files.cpp` & `tensora-0.0.8/src/taco/src/util/files.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/util/name_generator.cpp` & `tensora-0.0.8/src/taco/src/util/name_generator.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/src/util/strings.cpp` & `tensora-0.0.8/src/taco/src/util/strings.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/CMakeLists.txt` & `tensora-0.0.8/src/taco/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/README_testing.md` & `tensora-0.0.8/src/taco/test/README_testing.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/.appveyor.yml` & `tensora-0.0.8/src/taco/test/bats/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/.devcontainer/Dockerfile` & `tensora-0.0.8/src/taco/test/bats/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/.editorconfig` & `tensora-0.0.8/src/taco/test/bats/.editorconfig`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/.travis.yml` & `tensora-0.0.8/src/taco/test/bats/.travis.yml`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/LICENSE.md` & `tensora-0.0.8/src/taco/test/bats/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/README.md` & `tensora-0.0.8/src/taco/test/bats/README.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/bin/bats` & `tensora-0.0.8/src/taco/test/bats/bin/bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/contrib/release.sh` & `tensora-0.0.8/src/taco/test/bats/contrib/release.sh`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/contrib/rpm/bats.spec` & `tensora-0.0.8/src/taco/test/bats/contrib/rpm/bats.spec`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/contrib/semver` & `tensora-0.0.8/src/taco/test/bats/contrib/semver`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/CHANGELOG.md` & `tensora-0.0.8/src/taco/test/bats/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/CODE_OF_CONDUCT.md` & `tensora-0.0.8/src/taco/test/bats/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/CONTRIBUTING.md` & `tensora-0.0.8/src/taco/test/bats/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/examples/package-tarball` & `tensora-0.0.8/src/taco/test/bats/docs/examples/package-tarball`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/examples/package-tarball.bats` & `tensora-0.0.8/src/taco/test/bats/docs/examples/package-tarball.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/releasing.md` & `tensora-0.0.8/src/taco/test/bats/docs/releasing.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/docs/usage.md` & `tensora-0.0.8/src/taco/test/bats/docs/usage.md`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/install.sh` & `tensora-0.0.8/src/taco/test/bats/install.sh`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/lib/bats-core/preprocessing.bash` & `tensora-0.0.8/src/taco/test/bats/lib/bats-core/preprocessing.bash`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/lib/bats-core/test_functions.bash` & `tensora-0.0.8/src/taco/test/bats/lib/bats-core/test_functions.bash`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/lib/bats-core/tracing.bash` & `tensora-0.0.8/src/taco/test/bats/lib/bats-core/tracing.bash`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/lib/bats-core/validator.bash` & `tensora-0.0.8/src/taco/test/bats/lib/bats-core/validator.bash`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-file` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-exec-file`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-suite` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-exec-suite`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-exec-test` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-exec-test`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-junit` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-format-junit`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-format-pretty` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-format-pretty`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/libexec/bats-core/bats-preprocess` & `tensora-0.0.8/src/taco/test/bats/libexec/bats-core/bats-preprocess`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/man/bats.1` & `tensora-0.0.8/src/taco/test/bats/man/bats.1`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/man/bats.1.ronn` & `tensora-0.0.8/src/taco/test/bats/man/bats.1.ronn`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/man/bats.7` & `tensora-0.0.8/src/taco/test/bats/man/bats.7`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/man/bats.7.ronn` & `tensora-0.0.8/src/taco/test/bats/man/bats.7.ronn`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/package.json` & `tensora-0.0.8/src/taco/test/bats/package.json`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/bats.bats` & `tensora-0.0.8/src/taco/test/bats/test/bats.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/file_setup_teardown.bats` & `tensora-0.0.8/src/taco/test/bats/test/file_setup_teardown.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/external_function_calls.bats` & `tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/external_function_calls.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/fixtures/bats/whitespace.bats` & `tensora-0.0.8/src/taco/test/bats/test/fixtures/bats/whitespace.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/install.bats` & `tensora-0.0.8/src/taco/test/bats/test/install.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/junit-formatter.bats` & `tensora-0.0.8/src/taco/test/bats/test/junit-formatter.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/parallell.bats` & `tensora-0.0.8/src/taco/test/bats/test/parallell.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/root.bats` & `tensora-0.0.8/src/taco/test/bats/test/root.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/suite.bats` & `tensora-0.0.8/src/taco/test/bats/test/suite.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/bats/test/test_helper.bash` & `tensora-0.0.8/src/taco/test/bats/test/test_helper.bash`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/data/qcd/theta.ttx` & `tensora-0.0.8/src/taco/test/data/qcd/theta.ttx`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/data/qcd/z.ttx` & `tensora-0.0.8/src/taco/test/data/qcd/z.ttx`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/data/rua_32.mtx` & `tensora-0.0.8/src/taco/test/data/rua_32.mtx`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/data/rua_32.rb` & `tensora-0.0.8/src/taco/test/data/rua_32.rb`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/expr_factory.cpp` & `tensora-0.0.8/src/taco/test/expr_factory.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/expr_factory.h` & `tensora-0.0.8/src/taco/test/expr_factory.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/gtest/LICENSE` & `tensora-0.0.8/src/taco/test/gtest/LICENSE`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/gtest/gtest-all.cc` & `tensora-0.0.8/src/taco/test/gtest/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/gtest/gtest.h` & `tensora-0.0.8/src/taco/test/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/op_factory.h` & `tensora-0.0.8/src/taco/test/op_factory.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/taco-cli-test.bats` & `tensora-0.0.8/src/taco/test/taco-cli-test.bats`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test-iteration_algebra.cpp` & `tensora-0.0.8/src/taco/test/test-iteration_algebra.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test-typedcomponent-memory.cpp` & `tensora-0.0.8/src/taco/test/test-typedcomponent-memory.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test.cpp` & `tensora-0.0.8/src/taco/test/test.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test.h` & `tensora-0.0.8/src/taco/test/test.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test_properties.cpp` & `tensora-0.0.8/src/taco/test/test_properties.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test_tensors.cpp` & `tensora-0.0.8/src/taco/test/test_tensors.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/test_tensors.h` & `tensora-0.0.8/src/taco/test/test_tensors.h`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-api.cpp` & `tensora-0.0.8/src/taco/test/tests-api.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-copyprop.cpp` & `tensora-0.0.8/src/taco/test/tests-copyprop.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-error.cpp` & `tensora-0.0.8/src/taco/test/tests-error.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-expr.cpp` & `tensora-0.0.8/src/taco/test/tests-expr.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-expr_storage.cpp` & `tensora-0.0.8/src/taco/test/tests-expr_storage.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-format-mm-permute.cpp` & `tensora-0.0.8/src/taco/test/tests-format-mm-permute.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-format.cpp` & `tensora-0.0.8/src/taco/test/tests-format.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-index.cpp` & `tensora-0.0.8/src/taco/test/tests-index.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-index_notation.cpp` & `tensora-0.0.8/src/taco/test/tests-index_notation.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-indexexpr.cpp` & `tensora-0.0.8/src/taco/test/tests-indexexpr.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-indexstmt.cpp` & `tensora-0.0.8/src/taco/test/tests-indexstmt.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-io.cpp` & `tensora-0.0.8/src/taco/test/tests-io.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-lower.cpp` & `tensora-0.0.8/src/taco/test/tests-lower.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-merge_lattice.cpp` & `tensora-0.0.8/src/taco/test/tests-merge_lattice.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-parafac.cpp` & `tensora-0.0.8/src/taco/test/tests-parafac.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-qcd.cpp` & `tensora-0.0.8/src/taco/test/tests-qcd.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-schedule-parser.cpp` & `tensora-0.0.8/src/taco/test/tests-schedule-parser.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-scheduling-eval.cpp` & `tensora-0.0.8/src/taco/test/tests-scheduling-eval.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-scheduling.cpp` & `tensora-0.0.8/src/taco/test/tests-scheduling.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-storage.cpp` & `tensora-0.0.8/src/taco/test/tests-storage.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-storage_alloc.cpp` & `tensora-0.0.8/src/taco/test/tests-storage_alloc.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-tensor.cpp` & `tensora-0.0.8/src/taco/test/tests-tensor.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-tensor_types.cpp` & `tensora-0.0.8/src/taco/test/tests-tensor_types.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-transformation.cpp` & `tensora-0.0.8/src/taco/test/tests-transformation.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-transpose.cpp` & `tensora-0.0.8/src/taco/test/tests-transpose.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-type.cpp` & `tensora-0.0.8/src/taco/test/tests-type.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-windowing.cpp` & `tensora-0.0.8/src/taco/test/tests-windowing.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/test/tests-workspaces.cpp` & `tensora-0.0.8/src/taco/test/tests-workspaces.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/taco/tools/taco.cpp` & `tensora-0.0.8/src/taco/tools/taco.cpp`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/compile.py` & `tensora-0.0.8/src/tensora/compile.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/expression/ast.py` & `tensora-0.0.8/src/tensora/expression/ast.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/expression/parser.py` & `tensora-0.0.8/src/tensora/expression/parser.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/format/format.py` & `tensora-0.0.8/src/tensora/format/format.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/format/parser.py` & `tensora-0.0.8/src/tensora/format/parser.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/function.py` & `tensora-0.0.8/src/tensora/function.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora/tensor.py` & `tensora-0.0.8/src/tensora/tensor.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/src/tensora.egg-info/PKG-INFO` & `tensora-0.0.8/src/tensora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensora
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for dense and sparse tensors built on the tensor algebra compiler.
 Home-page: https://github.com/drhagen/tensora
 Author: David Hagen
 Author-email: david@drhagen.com
 License: MIT
 Keywords: tensor sparse matrix array
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tensora-0.0.7/src/tensora.egg-info/SOURCES.txt` & `tensora-0.0.8/src/tensora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_combinatorically.py` & `tensora-0.0.8/tests/test_combinatorically.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_compile.py` & `tensora-0.0.8/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_expression.py` & `tensora-0.0.8/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_format.py` & `tensora-0.0.8/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_from_data.py` & `tensora-0.0.8/tests/test_from_data.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_function.py` & `tensora-0.0.8/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_numpy.py` & `tensora-0.0.8/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_operators.py` & `tensora-0.0.8/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `tensora-0.0.7/tests/test_tensor.py` & `tensora-0.0.8/tests/test_tensor.py`

 * *Files identical despite different names*

