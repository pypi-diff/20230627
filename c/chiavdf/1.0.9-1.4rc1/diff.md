# Comparing `tmp/chiavdf-1.0.9.tar.gz` & `tmp/chiavdf-1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiavdf-1.0.9.tar", last modified: Tue Jun 27 19:33:02 2023, max compression
+gzip compressed data, was "chiavdf-1.4rc1.tar", last modified: Sun Jan  9 02:29:35 2022, max compression
```

## Comparing `chiavdf-1.0.9.tar` & `chiavdf-1.4rc1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 19:32:48.000000 chiavdf-1.0.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.506926 chiavdf-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.510926 chiavdf-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-06-27 19:32:48.000000 chiavdf-1.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-27 19:32:48.000000 chiavdf-1.0.9/.github/workflows/codeql-analysis.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-06-27 19:32:48.000000 chiavdf-1.0.9/.github/workflows/stale-issue.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-06-27 19:32:48.000000 chiavdf-1.0.9/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-27 19:32:48.000000 chiavdf-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 19:32:48.000000 chiavdf-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-06-27 19:33:02.522926 chiavdf-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-06-27 19:32:48.000000 chiavdf-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-27 19:32:48.000000 chiavdf-1.0.9/README_AVX512.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.510926 chiavdf-1.0.9/chiavdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-06-27 19:33:02.000000 chiavdf-1.0.9/chiavdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-27 19:33:02.000000 chiavdf-1.0.9/chiavdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:33:02.000000 chiavdf-1.0.9/chiavdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:33:02.000000 chiavdf-1.0.9/chiavdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 19:33:02.000000 chiavdf-1.0.9/chiavdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   464444 2023-06-27 19:32:48.000000 chiavdf-1.0.9/classgroups.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-27 19:32:48.000000 chiavdf-1.0.9/comparenweso.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 19:32:48.000000 chiavdf-1.0.9/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 19:32:48.000000 chiavdf-1.0.9/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-27 19:32:48.000000 chiavdf-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:33:02.522926 chiavdf-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-27 19:32:48.000000 chiavdf-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.518926 chiavdf-1.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/1weso_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/2weso_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/ClassGroup.h
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/Makefile.vdf-client
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/Reducer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/alloc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    29480 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_avx512_ifma.h
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_base.h
--rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_gcd_128.h
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_gcd_base_continued_fractions.h
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_gcd_base_divide_table.h
--rw-r--r--   0 runner    (1001) docker     (123)    29721 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_gcd_unsigned.h
--rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_main.h
--rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/asm_vm.h
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/avx512_integer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/avx512_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/bit_manipulation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/bqfc.c
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/bqfc.h
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/callback.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.518926 chiavdf-1.0.9/src/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/cmake/FindGMP.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/cmake/FindGMPXX.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/compile_asm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/create_discriminant.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/double_utility.h
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/fast_storage.h
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gcd_128.h
--rw-r--r--   0 runner    (1001) docker     (123)    25108 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gcd_base_continued_fractions.h
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gcd_base_divide_table.h
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gcd_unsigned.h
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/generic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/generic_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gpu_integer.h
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gpu_integer_divide.h
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/gpu_integer_gcd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/include.h
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/integer.h
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/integer_common.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.506926 chiavdf-1.0.9/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.518926 chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/compat.c
--rw-r--r--   0 runner    (1001) docker     (123)    85426 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/longlong.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/mpz/
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/mpz/inp_raw.c
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/nucomp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/parameters.h
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/picosha2.h
--rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/pprods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/primetest.h
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/proof_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/prover_slow.h
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/prover_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/provers.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/src/python_bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/python_bindings/fastvdf.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/src/refcode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/refcode/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/refcode/lzcnt.c
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/threading.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/src/uint128_t/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/uint128_t.build
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/uint128_t.h
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/uint128_t.include
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/uint128_t/uint128_t_config.include
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/util.h
--rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_bench.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34151 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_fast.h
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_new.h
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_original.h
--rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/vdf_test.h
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/verifier.h
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/verifier_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-27 19:32:48.000000 chiavdf-1.0.9/src/xgcd_partial.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-27 19:32:48.000000 chiavdf-1.0.9/tests/test_n_weso_verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-27 19:32:48.000000 chiavdf-1.0.9/tests/test_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:33:02.522926 chiavdf-1.0.9/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-06-27 19:32:48.000000 chiavdf-1.0.9/tools/gen_pprods.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.020844 chiavdf-1.4rc1/
+-rw-r--r--   0 runner     (501) staff       (20)       95 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.flake8
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:34.971515 chiavdf-1.4rc1/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:34.982780 chiavdf-1.4rc1/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     3329 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.github/workflows/build-aarch64.yml
+-rw-r--r--   0 runner     (501) staff       (20)     3488 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.github/workflows/build-m1-wheel.yml
+-rw-r--r--   0 runner     (501) staff       (20)     5457 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.github/workflows/build.yml
+-rwxr-xr-x   0 runner     (501) staff       (20)     1330 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.github/workflows/stale-issue.yml
+-rwxr-xr-x   0 runner     (501) staff       (20)     2077 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.github/workflows/test.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      532 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      102 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/.gitmodules
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    20647 2022-01-09 02:29:35.020206 chiavdf-1.4rc1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    20318 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     5837 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/README_AVX512.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:34.985131 chiavdf-1.4rc1/chiavdf.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    20647 2022-01-09 02:29:34.000000 chiavdf-1.4rc1/chiavdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2031 2022-01-09 02:29:34.000000 chiavdf-1.4rc1/chiavdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-01-09 02:29:34.000000 chiavdf-1.4rc1/chiavdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-01-09 02:29:34.000000 chiavdf-1.4rc1/chiavdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        8 2022-01-09 02:29:34.000000 chiavdf-1.4rc1/chiavdf.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)   464444 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/classgroups.pdf
+-rw-r--r--   0 runner     (501) staff       (20)     7851 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/comparenweso.py
+-rw-r--r--   0 runner     (501) staff       (20)      343 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/lgtm.yml
+-rw-r--r--   0 runner     (501) staff       (20)       37 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/mypi.ini
+-rw-r--r--   0 runner     (501) staff       (20)      194 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-01-09 02:29:35.020971 chiavdf-1.4rc1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     8475 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.011750 chiavdf-1.4rc1/src/
+-rw-r--r--   0 runner     (501) staff       (20)     2057 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/1weso_test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2597 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/2weso_test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1131 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1952 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/ClassGroup.h
+-rw-r--r--   0 runner     (501) staff       (20)     1348 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/Makefile.vdf-client
+-rw-r--r--   0 runner     (501) staff       (20)     6410 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/Reducer.h
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/alloc.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    29480 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_avx512_ifma.h
+-rw-r--r--   0 runner     (501) staff       (20)     4487 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_base.h
+-rw-r--r--   0 runner     (501) staff       (20)    25992 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_gcd_128.h
+-rw-r--r--   0 runner     (501) staff       (20)    14791 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_gcd_base_continued_fractions.h
+-rw-r--r--   0 runner     (501) staff       (20)     6847 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_gcd_base_divide_table.h
+-rw-r--r--   0 runner     (501) staff       (20)    29734 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_gcd_unsigned.h
+-rw-r--r--   0 runner     (501) staff       (20)    15548 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_main.h
+-rw-r--r--   0 runner     (501) staff       (20)    17155 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_types.h
+-rw-r--r--   0 runner     (501) staff       (20)     4559 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/asm_vm.h
+-rw-r--r--   0 runner     (501) staff       (20)     5123 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/avx512_integer.h
+-rw-r--r--   0 runner     (501) staff       (20)     4279 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/avx512_test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1244 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/bit_manipulation.h
+-rw-r--r--   0 runner     (501) staff       (20)     7183 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/bqfc.c
+-rw-r--r--   0 runner     (501) staff       (20)      820 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/bqfc.h
+-rw-r--r--   0 runner     (501) staff       (20)     6868 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/callback.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.012673 chiavdf-1.4rc1/src/cmake/
+-rw-r--r--   0 runner     (501) staff       (20)     2909 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/cmake/FindGMP.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      921 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/cmake/FindGMPXX.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     1515 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/compile_asm.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      272 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/create_discriminant.h
+-rw-r--r--   0 runner     (501) staff       (20)     3043 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/double_utility.h
+-rw-r--r--   0 runner     (501) staff       (20)     4591 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/fast_storage.h
+-rw-r--r--   0 runner     (501) staff       (20)     8192 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gcd_128.h
+-rw-r--r--   0 runner     (501) staff       (20)    25108 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gcd_base_continued_fractions.h
+-rw-r--r--   0 runner     (501) staff       (20)     5576 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gcd_base_divide_table.h
+-rw-r--r--   0 runner     (501) staff       (20)    12852 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gcd_unsigned.h
+-rw-r--r--   0 runner     (501) staff       (20)     9926 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/generic.h
+-rw-r--r--   0 runner     (501) staff       (20)     1180 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/generic_macros.h
+-rw-r--r--   0 runner     (501) staff       (20)    19274 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gpu_integer.h
+-rw-r--r--   0 runner     (501) staff       (20)    10344 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gpu_integer_divide.h
+-rw-r--r--   0 runner     (501) staff       (20)     3257 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/gpu_integer_gcd.h
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/include.h
+-rw-r--r--   0 runner     (501) staff       (20)     1122 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/integer.h
+-rw-r--r--   0 runner     (501) staff       (20)    10216 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/integer_common.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:34.972586 chiavdf-1.4rc1/src/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.013504 chiavdf-1.4rc1/src/lib/gmp-patch-6.2.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1955 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/lib/gmp-patch-6.2.1/compat.c
+-rw-r--r--   0 runner     (501) staff       (20)    85426 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/lib/gmp-patch-6.2.1/longlong.h
+-rw-r--r--   0 runner     (501) staff       (20)     8764 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/nucomp.h
+-rw-r--r--   0 runner     (501) staff       (20)     9406 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/parameters.h
+-rw-r--r--   0 runner     (501) staff       (20)    13016 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/picosha2.h
+-rw-r--r--   0 runner     (501) staff       (20)    19946 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/pprods.h
+-rw-r--r--   0 runner     (501) staff       (20)     4543 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/primetest.h
+-rw-r--r--   0 runner     (501) staff       (20)     4016 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/proof_common.h
+-rw-r--r--   0 runner     (501) staff       (20)     3474 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/prover_slow.h
+-rw-r--r--   0 runner     (501) staff       (20)     2548 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/prover_test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7554 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/provers.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.014200 chiavdf-1.4rc1/src/python_bindings/
+-rw-r--r--   0 runner     (501) staff       (20)     4427 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/python_bindings/fastvdf.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.015069 chiavdf-1.4rc1/src/refcode/
+-rw-r--r--   0 runner     (501) staff       (20)     2755 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/refcode/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    17395 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/refcode/lzcnt.c
+-rw-r--r--   0 runner     (501) staff       (20)    22775 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/threading.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.018265 chiavdf-1.4rc1/src/uint128_t/
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     1385 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      203 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/uint128_t.build
+-rw-r--r--   0 runner     (501) staff       (20)    13370 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      180 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/uint128_t.h
+-rw-r--r--   0 runner     (501) staff       (20)    19142 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/uint128_t.include
+-rw-r--r--   0 runner     (501) staff       (20)      644 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/uint128_t/uint128_t_config.include
+-rw-r--r--   0 runner     (501) staff       (20)     3758 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/util.h
+-rw-r--r--   0 runner     (501) staff       (20)    29475 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf.h
+-rw-r--r--   0 runner     (501) staff       (20)     3455 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_bench.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    12994 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_client.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    34151 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_fast.h
+-rw-r--r--   0 runner     (501) staff       (20)    12711 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_new.h
+-rw-r--r--   0 runner     (501) staff       (20)     8212 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_original.h
+-rw-r--r--   0 runner     (501) staff       (20)    15641 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    10966 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/vdf_test.h
+-rw-r--r--   0 runner     (501) staff       (20)     4495 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/verifier.h
+-rw-r--r--   0 runner     (501) staff       (20)     3844 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/verifier_test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3684 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/src/xgcd_partial.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.019113 chiavdf-1.4rc1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     4622 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/tests/test_n_weso_verifier.py
+-rw-r--r--   0 runner     (501) staff       (20)     1280 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/tests/test_verifier.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:29:35.019528 chiavdf-1.4rc1/tools/
+-rwxr-xr-x   0 runner     (501) staff       (20)     1890 2022-01-09 02:29:08.000000 chiavdf-1.4rc1/tools/gen_pprods.py
```

### Comparing `chiavdf-1.0.9/.github/workflows/stale-issue.yml` & `chiavdf-1.4rc1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/.github/workflows/test.yaml` & `chiavdf-1.4rc1/.github/workflows/test.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 name: Test Prover and vdf_client
 
-on:
-  push:
-    branches:
-      - main
-    tags:
-      - '**'
-  pull_request:
-    branches:
-      - '**'
+on: [push, pull_request]
 
 jobs:
   test:
     name: Test ${{ matrix.config }} ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
         config: [ optimized=1, TSAN=1, ASAN=1]
 
     steps:
     - name: Checkout code
-      uses: actions/checkout@v3
+      uses: actions/checkout@v2
 
     - name: Build vdf-client on Ubuntu
       if: startsWith(matrix.os, 'ubuntu')
       run: |
-        sudo apt-get install libgmp-dev libboost-python-dev libpython3-dev libboost-system-dev build-essential -y
+        sudo apt-get install libgmp-dev libboost-python-dev libpython3.8-dev libboost-system-dev build-essential -y
+        sudo fallocate -l 16G /swapfile
+        sudo chmod 600 /swapfile
+        sudo mkswap /swapfile
+        sudo swapon /swapfile
+        swapon -s
         cd src
         make ${{ matrix.config }} -f Makefile.vdf-client
 
     - name: Build vdf-client on Mac
       if: startsWith(matrix.os, 'mac')
       run: |
         brew install boost
```

### Comparing `chiavdf-1.0.9/.gitignore` & `chiavdf-1.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/LICENSE` & `chiavdf-1.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/PKG-INFO` & `chiavdf-1.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: chiavdf
-Version: 1.0.9
+Version: 1.4rc1
 Summary: Chia vdf verification (wraps C++)
 Home-page: https://github.com/Chia-Network/chiavdf
 Author: Florin Chirica
 Author-email: florin@chia.net
 License: Apache License
+Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chia VDF
 
 ![Build](https://github.com/Chia-Network/chiavdf/workflows/Build/badge.svg)
@@ -213,7 +214,9 @@
 ### Intermediates storage
 
 In order to finish segments, some intermediate values need to be stored for each segment. For each different possible segment length, we use a sliding window of length 20 to store those. Hence, for each segment length, we'll store only the intermediates values needed for the last 20 segments produced by the main VDF loop. Since finishing segments is faster than producing them by the main VDF loop, we assume the segment threads won't be behind by more than 20 segments from the main VDF loop, for each segment length. Thanks to the sliding window technique, the memory used will always be constant.
 
 Generally, the main VDF loop performs all the storing, after computing a form we're interested in. However, since storing is very frequent and expensive (GMP operations), this will slow down the main VDF loop.
 
 For the machines having at least 16 concurrent threads, an optimization is provided: the main VDF loop does only repeated squaring, without storing any form. After each 2^15 steps are performed, a new thread starts redoing the work for 2^15 more steps, this time storing the intermediate values as well. All the intermediates threads and the main VDF loop will work in parallel. The only purpose of the main VDF loop becomes now to produce the starting values for the intermediate threads, as fast as possible. The squarings used in the intermediates threads will be 2 times slower than the ones used in the main VDF loop. It's expected the intermediates will only lag behind the main VDF loop by 2^15 iterations, at any point: after 2^16 iterations are done by the main VDF loop, the first thread doing the first 2^15 intermediate values is already finished. Also, at that point, half of the work of the second thread doing the last 2^15 intermediates values should be already done.
+
+
```

### Comparing `chiavdf-1.0.9/README.md` & `chiavdf-1.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/README_AVX512.md` & `chiavdf-1.4rc1/README_AVX512.md`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/chiavdf.egg-info/PKG-INFO` & `chiavdf-1.4rc1/chiavdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: chiavdf
-Version: 1.0.9
+Version: 1.4rc1
 Summary: Chia vdf verification (wraps C++)
 Home-page: https://github.com/Chia-Network/chiavdf
 Author: Florin Chirica
 Author-email: florin@chia.net
 License: Apache License
+Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chia VDF
 
 ![Build](https://github.com/Chia-Network/chiavdf/workflows/Build/badge.svg)
@@ -213,7 +214,9 @@
 ### Intermediates storage
 
 In order to finish segments, some intermediate values need to be stored for each segment. For each different possible segment length, we use a sliding window of length 20 to store those. Hence, for each segment length, we'll store only the intermediates values needed for the last 20 segments produced by the main VDF loop. Since finishing segments is faster than producing them by the main VDF loop, we assume the segment threads won't be behind by more than 20 segments from the main VDF loop, for each segment length. Thanks to the sliding window technique, the memory used will always be constant.
 
 Generally, the main VDF loop performs all the storing, after computing a form we're interested in. However, since storing is very frequent and expensive (GMP operations), this will slow down the main VDF loop.
 
 For the machines having at least 16 concurrent threads, an optimization is provided: the main VDF loop does only repeated squaring, without storing any form. After each 2^15 steps are performed, a new thread starts redoing the work for 2^15 more steps, this time storing the intermediate values as well. All the intermediates threads and the main VDF loop will work in parallel. The only purpose of the main VDF loop becomes now to produce the starting values for the intermediate threads, as fast as possible. The squarings used in the intermediates threads will be 2 times slower than the ones used in the main VDF loop. It's expected the intermediates will only lag behind the main VDF loop by 2^15 iterations, at any point: after 2^16 iterations are done by the main VDF loop, the first thread doing the first 2^15 intermediate values is already finished. Also, at that point, half of the work of the second thread doing the last 2^15 intermediates values should be already done.
+
+
```

### Comparing `chiavdf-1.0.9/chiavdf.egg-info/SOURCES.txt` & `chiavdf-1.4rc1/chiavdf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 .flake8
 .gitignore
+.gitmodules
 LICENSE
 README.md
 README_AVX512.md
 classgroups.pdf
 comparenweso.py
 lgtm.yml
 mypi.ini
 pyproject.toml
 setup.py
 ./
+.github/workflows/build-aarch64.yml
+.github/workflows/build-m1-wheel.yml
 .github/workflows/build.yml
-.github/workflows/codeql-analysis.yml
 .github/workflows/stale-issue.yml
 .github/workflows/test.yaml
 chiavdf.egg-info/PKG-INFO
 chiavdf.egg-info/SOURCES.txt
 chiavdf.egg-info/dependency_links.txt
 chiavdf.egg-info/not-zip-safe
 chiavdf.egg-info/top_level.txt
@@ -79,15 +81,14 @@
 src/verifier.h
 src/verifier_test.cpp
 src/xgcd_partial.c
 src/cmake/FindGMP.cmake
 src/cmake/FindGMPXX.cmake
 src/lib/gmp-patch-6.2.1/compat.c
 src/lib/gmp-patch-6.2.1/longlong.h
-src/lib/gmp-patch-6.2.1/mpz/inp_raw.c
 src/python_bindings/fastvdf.cpp
 src/refcode/README.md
 src/refcode/lzcnt.c
 src/uint128_t/LICENSE
 src/uint128_t/README.md
 src/uint128_t/uint128_t.build
 src/uint128_t/uint128_t.cpp
```

### Comparing `chiavdf-1.0.9/classgroups.pdf` & `chiavdf-1.4rc1/classgroups.pdf`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/comparenweso.py` & `chiavdf-1.4rc1/comparenweso.py`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/setup.py` & `chiavdf-1.4rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
+from distutils.command.build import build  # type: ignore
 from distutils.command.install import install
 from distutils.version import LooseVersion
 
 from setuptools import Command, Extension, setup, setuptools
-from setuptools.command.build import build
 from setuptools.command.build_ext import build_ext
 
 BUILD_HOOKS = []
 INSTALL_HOOKS = []
 
 
 def add_install_hook(hook):
@@ -249,18 +249,20 @@
         author="Mariano Sorgente",
         author_email="mariano@chia.net",
         description="Chia vdf verification (wraps C++)",
         license="Apache License",
         python_requires=">=3.7",
         long_description=open("README.md").read(),
         long_description_content_type="text/markdown",
+        build_requires=["pybind11"],
         url="https://github.com/Chia-Network/chiavdf",
         ext_modules=ext_modules,
         cmdclass={"build_ext": BuildExt},
         zip_safe=False,
+        use_scm_version={"fallback_version": "unknown-no-.git-directory"},
     )
 else:
     build.sub_commands.append(("build_hook", lambda x: True))  # type: ignore
     install.sub_commands.append(("install_hook", lambda x: True))
 
     setup(
         name="chiavdf",
@@ -268,13 +270,15 @@
         author_email="florin@chia.net",
         description="Chia vdf verification (wraps C++)",
         license="Apache License",
         python_requires=">=3.7",
         long_description=open("README.md").read(),
         long_description_content_type="text/markdown",
         url="https://github.com/Chia-Network/chiavdf",
+        setup_requires=["pybind11>=2.5.0"],
         ext_modules=[CMakeExtension("chiavdf", "src")],
         cmdclass=dict(
             build_ext=CMakeBuild, install_hook=install_hook, build_hook=build_hook
         ),
         zip_safe=False,
+        use_scm_version={"fallback_version": "unknown-no-.git-directory"},
     )
```

### Comparing `chiavdf-1.0.9/src/1weso_test.cpp` & `chiavdf-1.4rc1/src/1weso_test.cpp`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/2weso_test.cpp` & `chiavdf-1.4rc1/src/2weso_test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 int gcd_128_max_iter=3;
 
 void CheckProof(integer& D, Proof& proof, uint64_t iteration) {
     form x = form::generator(D);
     std::vector<unsigned char> bytes;
     bytes.insert(bytes.end(), proof.y.begin(), proof.y.end());
     bytes.insert(bytes.end(), proof.proof.begin(), proof.proof.end());
-    if (CheckProofOfTimeNWesolowski(D, DEFAULT_ELEMENT, bytes.data(), bytes.size(), iteration, 1024, proof.witness_type)) {
+    if (CheckProofOfTimeNWesolowski(D, DEFAULT_ELEMENT, bytes.data(), bytes.size(), iteration, proof.witness_type)) {
         std::cout << "Correct proof\n";
     } else {
         std::cout << "Incorrect proof\n";
         throw std::runtime_error("incorrect proof");
     }
 }
```

### Comparing `chiavdf-1.0.9/src/CMakeLists.txt` & `chiavdf-1.4rc1/src/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # CMake 3.14+
 include(FetchContent)
 
 FetchContent_Declare(
   pybind11-src
   GIT_REPOSITORY https://github.com/pybind/pybind11.git
-  GIT_TAG        v2.10.0
+  GIT_TAG        v2.6.2
 )
 FetchContent_MakeAvailable(pybind11-src)
 
 pybind11_add_module(chiavdf
   ${CMAKE_CURRENT_SOURCE_DIR}/python_bindings/fastvdf.cpp
   ${CMAKE_CURRENT_SOURCE_DIR}/refcode/lzcnt.c
 )
```

### Comparing `chiavdf-1.0.9/src/ClassGroup.h` & `chiavdf-1.4rc1/src/ClassGroup.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/Makefile.vdf-client` & `chiavdf-1.4rc1/src/Makefile.vdf-client`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/Reducer.h` & `chiavdf-1.4rc1/src/Reducer.h`

 * *Files 1% similar despite different names*

```diff
@@ -41,33 +41,33 @@
 unsigned int lzcnt64_hard(unsigned long long x) WEAK;
 }
 
 /** constants utilized in reduction algorithm */
 namespace {
 const int_fast64_t THRESH{1ul << 31};
 const int_fast64_t EXP_THRESH{31};
-}
+} 
 
 /**
- * @brief The Reducer class that does custom reduce operation for VDF
+ * @brief The Reducer class that does custom reduce operation for VDF 
  * repeated squaring algorithm. The implementation is based on
  * Akashnil VDF competition entry and further optimized for speed.
  */
 class alignas(64) Reducer {
 public:
   /**
    * @brief Reducer - constructs by using reference into cg context.
-   */
+   */  
   Reducer(ClassGroupContext &ctx_) : ctx(ctx_) {}
 
   ~Reducer() {}
 
   /**
    * @brief run - runs reduction algorithm for cg context params
-   */
+   */  
   inline void run() {
     while (!isReduced()) {
       int_fast64_t a, b, c;
       {
         int_fast64_t a_exp, b_exp, c_exp;
         mpz_get_si_2exp(a, a_exp, ctx.a);
         mpz_get_si_2exp(b, b_exp, ctx.b);
@@ -136,15 +136,15 @@
     uint_fast64_t last(mpz_getlimbn(op, (size - 1)));
 
     if(!bLZCChecked)
     {
         bLZCHasHW=has_lzcnt_hard();
         bLZCChecked=true;
     }
-
+    
     int_fast64_t lg2;
 
     if(bLZCHasHW)
         lg2 = exp = ((63 - lzcnt64_hard(last)) + 1);
     else
         lg2 = exp = ((63 - lzcnt64_soft(last)) + 1);
```

### Comparing `chiavdf-1.0.9/src/alloc.hpp` & `chiavdf-1.4rc1/src/alloc.hpp`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_avx512_ifma.h` & `chiavdf-1.4rc1/src/asm_avx512_ifma.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_base.h` & `chiavdf-1.4rc1/src/asm_base.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_gcd_128.h` & `chiavdf-1.4rc1/src/asm_gcd_128.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_gcd_base_continued_fractions.h` & `chiavdf-1.4rc1/src/asm_gcd_base_continued_fractions.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_gcd_base_divide_table.h` & `chiavdf-1.4rc1/src/asm_gcd_base_divide_table.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_gcd_unsigned.h` & `chiavdf-1.4rc1/src/asm_gcd_unsigned.h`

 * *Files 0% similar despite different names*

```diff
@@ -466,16 +466,16 @@
             APPEND_M(str( "CMP `tmp, #", size ));
 
             APPEND_M(str( "JE ")+asmprefix+str("multiply_uv_size_#", mapped_size ));
         }
 #else
         for (int end_index=0;end_index<int_size;++end_index) {
             int size=end_index+1;
-
-            int mapped_size=size;
+            
+            int mapped_size=size; 
             while (mapped_size==0 || mapped_size%4!=0) {
                 ++mapped_size;
             }
 
             APPEND_M(str( ".quad ")+asmprefix+str("multiply_uv_size_#", mapped_size ));
         }
         APPEND_M(str( ".text" ));
```

### Comparing `chiavdf-1.0.9/src/asm_main.h` & `chiavdf-1.4rc1/src/asm_main.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_types.h` & `chiavdf-1.4rc1/src/asm_types.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/asm_vm.h` & `chiavdf-1.4rc1/src/asm_vm.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/avx512_integer.h` & `chiavdf-1.4rc1/src/avx512_integer.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/avx512_test.cpp` & `chiavdf-1.4rc1/src/avx512_test.cpp`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/bit_manipulation.h` & `chiavdf-1.4rc1/src/bit_manipulation.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/bqfc.c` & `chiavdf-1.4rc1/src/bqfc.c`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,14 @@
 
     if (mpz_sgn(c->t) < 0) {
         mpz_add(t, c->t, c->a);
     } else {
         mpz_set(t, c->t);
     }
 
-    if (mpz_sgn(c->a) == 0) {
-        ret = -1;
-        goto out;
-    }
     mpz_gcdext(tmp, t_inv, NULL, t, c->a);
     if (mpz_cmp_ui(tmp, 1)) {
         ret = -1;
         goto out;
     }
     if (mpz_sgn(t_inv) < 0) {
         mpz_add(t_inv, t_inv, c->a);
```

### Comparing `chiavdf-1.0.9/src/bqfc.h` & `chiavdf-1.4rc1/src/bqfc.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/callback.h` & `chiavdf-1.4rc1/src/callback.h`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         uint64_t space_needed = wanted_iter / (k * l) + 100;
         forms.reset(new form[space_needed]);
         forms[0] = f;
     }
 
     void OnIteration(int type, void *data, uint64_t iteration) {
         iteration++;
-        if (iteration > wanted_iter)
+        if (iteration > wanted_iter) 
             return ;
 
         if (iteration % kl == 0) {
             uint64_t pos = iteration / kl;
             form* mulf = &forms[pos];
             SetForm(type, data, mulf);
         }
@@ -185,15 +185,15 @@
     }
 
     form *GetForm(uint64_t exponent, int bucket) {
         uint64_t pos = GetPosition(exponent, bucket);
         return &(forms[pos]);
     }
 
-    // We need to store:
+    // We need to store: 
     // 2^16 * k + 10 * l
     // 2^(18 + 2*m) * k + 12 * 2^(2*m) * l
     void OnIteration(int type, void *data, uint64_t iteration) {
         iteration++;
         if (multi_proc_machine) {
             if (iteration % (1 << 15) == 0) {
                 SetForm(type, data, &y_ret);
```

### Comparing `chiavdf-1.0.9/src/cmake/FindGMP.cmake` & `chiavdf-1.4rc1/src/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/cmake/FindGMPXX.cmake` & `chiavdf-1.4rc1/src/cmake/FindGMPXX.cmake`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/compile_asm.cpp` & `chiavdf-1.4rc1/src/compile_asm.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 #include "asm_main.h"
 
 int main(int argc, char** argv) {
     set_rounding_mode();
 
     string filename="asm_compiled.s";
-
+    
     bool compile_avx512=false;
 
     if((argc==2)&&(strcmp(argv[1],"avx2")==0))
     {
        use_divide_table=true;
        gcd_base_bits=63;
        gcd_128_max_iter=2;
```

### Comparing `chiavdf-1.0.9/src/double_utility.h` & `chiavdf-1.4rc1/src/double_utility.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/fast_storage.h` & `chiavdf-1.4rc1/src/fast_storage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-// If 'FAST_MACHINE' is set to 1, the machine needs to have a high number
+// If 'FAST_MACHINE' is set to 1, the machine needs to have a high number 
 // of CPUs. This will optimize the runtime,
 // by not storing any intermediate values in main VDF worker loop.
 // Other threads will come back and redo the work, this
 // time storing the intermediates as well.
 // For machines with small numbers of CPU, setting this to 1 will slow
 // down everything, possible even stall.
 #ifndef FAST_STORAGE_H
@@ -76,15 +76,15 @@
                 if ((iteration % power_2) % kl == 0) {
                     if (stopped) return;
                     form* mulf = weso->GetForm(iteration, i);
                     weso->SetForm(NL_FORM, &y, mulf, /*reduced=*/false);
                 }
             }
             nudupl_form(y, y, D, L);
-            reducer.reduce(y);
+            reducer.reduce(y);   
         }
         AddIntermediates(iter_begin);
     }
 
     void SubmitCheckpoint(form y_ret, uint64_t iteration) {
         {
             std::lock_guard<std::mutex> lk(intermediates_mutex);
@@ -95,15 +95,15 @@
 
     uint64_t GetFinishedSegment() {
         while (intermediates_stored[2 * (intermediates_iter / (1 << 16))] == true &&
                intermediates_stored[2 * (intermediates_iter / (1 << 16)) + 1] == true) {
                     intermediates_iter += (1 << 16);
                 }
         return intermediates_iter;
-    }
+    } 
 
     void CalculateIntermediatesThread() {
         while (!stopped) {
             {
                 std::unique_lock<std::mutex> lk(intermediates_mutex);
                 intermediates_cv.wait(lk, [&] {
                     return (!pending_intermediates.empty() || stopped);
```

### Comparing `chiavdf-1.0.9/src/gcd_128.h` & `chiavdf-1.4rc1/src/gcd_128.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/gcd_base_continued_fractions.h` & `chiavdf-1.4rc1/src/gcd_base_continued_fractions.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/gcd_base_divide_table.h` & `chiavdf-1.4rc1/src/gcd_base_divide_table.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/gcd_unsigned.h` & `chiavdf-1.4rc1/src/gcd_unsigned.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/generic.h` & `chiavdf-1.4rc1/src/generic.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/generic_macros.h` & `chiavdf-1.4rc1/src/generic_macros.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/gpu_integer.h` & `chiavdf-1.4rc1/src/gpu_integer.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/gpu_integer_divide.h` & `chiavdf-1.4rc1/src/gpu_integer_divide.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/gpu_integer_gcd.h` & `chiavdf-1.4rc1/src/gpu_integer_gcd.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/include.h` & `chiavdf-1.4rc1/src/include.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/integer.h` & `chiavdf-1.4rc1/src/integer.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/integer_common.h` & `chiavdf-1.4rc1/src/integer_common.h`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         //get rid of the null terminator and everything after it
         return res_string.c_str();
     }
 
     string to_string_dec() const {
         string res_string;
         res_string.resize(mpz_sizeinbase(impl, 10));
-
+        
         mpz_get_str(&(res_string[0]), 10, impl);
 
         return res_string.c_str();
     }
 
     integer& operator+=(const integer& t) {
         mpz_add(impl, impl, t.impl);
```

### Comparing `chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/compat.c` & `chiavdf-1.4rc1/src/lib/gmp-patch-6.2.1/compat.c`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/lib/gmp-patch-6.2.1/longlong.h` & `chiavdf-1.4rc1/src/lib/gmp-patch-6.2.1/longlong.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/nucomp.h` & `chiavdf-1.4rc1/src/nucomp.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#ifndef NUCOMP_H
-#define NUCOMP_H
+#ifndef VDF_NEW_H
+#define VDF_NEW_H
 
 /**
     Copyright (C) 2012 William Hart
-
+    
     Permission is hereby granted, free of charge, to any person obtaining a copy of this
-    software and associated documentation files (the "Software"), to deal in the Software
-    without restriction, including without limitation the rights to use, copy, modify, merge,
-    publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons
+    software and associated documentation files (the "Software"), to deal in the Software 
+    without restriction, including without limitation the rights to use, copy, modify, merge, 
+    publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons 
     to whom the Software is furnished to do so, subject to the following conditions:
     The above copyright notice and this permission notice shall be included in all copies or
     substantial portions of the Software.
-
+    
     THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
     INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
     PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
     FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
     OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
     DEALINGS IN THE SOFTWARE.
-
+    
     MIT licensing permission obtained January 13, 2020 by Chia Network Inc. from William Hart
 
 Copyright 2020 Chia Network Inc
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
@@ -47,15 +47,15 @@
     mpz_t b;
     mpz_t c;
 } qfb;
 
 typedef qfb qfb_t[1];
 
 // From Antic using Flint (works!)
-void qfb_nucomp(qfb_t r, const qfb_t f, const qfb_t g, mpz_t const& D, mpz_t const& L)
+void qfb_nucomp(qfb_t r, const qfb_t f, const qfb_t g, mpz_t& D, mpz_t& L)
 {
    mpz_t a1, a2, c2, ca, cb, cc, k, s, sp, ss, m, t, u2, v1, v2;
 
    if (mpz_cmp(f->a, g->a) > 0)
    {
       qfb_nucomp(r, g, f, D, L);
       return;
@@ -85,19 +85,19 @@
       mpz_set_ui(v1, 0);
       mpz_set(sp, a1);
    } else
       mpz_gcdext(sp, v1, NULL, t, a1);
 
    mpz_mul(k, m, v1);
    mpz_fdiv_r(k, k, a1);
-
+ 
    if (mpz_cmp_ui(sp, 1))
    {
       mpz_gcdext(s, v2, u2, ss, sp);
-
+ 
       /* k = k*u2 - v2*c2 */
       mpz_mul(k, k, u2);
       mpz_mul(t, v2, c2);
       mpz_sub(k, k, t);
 
       if (mpz_cmp_ui(s, 1))
       {
@@ -159,15 +159,15 @@
       mpz_mul(cb, ca, co2);
       mpz_sub(cb, t, cb);
       mpz_mul_2exp(cb, cb, 1);
       mpz_divexact(cb, cb, co1);
       mpz_sub(cb, cb, g->b);
       mpz_mul_2exp(temp, ca, 1);
       mpz_fdiv_r(cb, cb, temp);
-
+ 
       /* cc = (cb*cb - D) / (4*ca) */
       mpz_mul(cc, cb, cb);
       mpz_sub(cc, cc, D);
       mpz_divexact(cc, cc, ca);
       mpz_fdiv_q_2exp(cc, cc, 2);
 
       if (mpz_sgn(ca) < 0)
@@ -188,15 +188,15 @@
    mpz_clear(k); mpz_clear(m);
    mpz_clear(s); mpz_clear(sp); mpz_clear(ss);
    mpz_clear(t); mpz_clear(u2); mpz_clear(v1); mpz_clear(v2);
    mpz_clear(a1); mpz_clear(a2); mpz_clear(c2);
 }
 
 // a = b * c
-void nucomp_form(form &a, form const& b, form const& c, integer const& D, integer const& L) {
+void nucomp_form(form &a, form &b, form &c, integer &D, integer &L) {
     qfb fr, fr2, fr3;
 
     *fr.a = *a.a.impl;
     *fr.b = *a.b.impl;
     *fr.c = *a.c.impl;
     *fr2.a = *b.a.impl;
     *fr2.b = *b.b.impl;
@@ -339,8 +339,8 @@
     qfb_nudupl(&fr, &fr2, D.impl, L.impl);
 
     *a.a.impl = *fr.a;
     *a.b.impl = *fr.b;
     *a.c.impl = *fr.c;
 }
 
-#endif // NUCOMP_H
+#endif // VDF_NEW_H
```

### Comparing `chiavdf-1.0.9/src/parameters.h` & `chiavdf-1.4rc1/src/parameters.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/picosha2.h` & `chiavdf-1.4rc1/src/picosha2.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/pprods.h` & `chiavdf-1.4rc1/src/pprods.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/primetest.h` & `chiavdf-1.4rc1/src/primetest.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/proof_common.h` & `chiavdf-1.4rc1/src/proof_common.h`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,14 @@
         throw std::runtime_error("Form is not reduced");
     }
     return f;
 }
 
 integer FastPow(uint64_t a, uint64_t b, integer& c) {
     integer res, a1 = integer(a);
-    if (mpz_sgn(c.impl) == 0) {
-        throw std::runtime_error("Division by 0");
-    }
     mpz_powm_ui(res.impl, a1.impl, b, c.impl);
     return res;
 }
 
 integer GetB(const integer& D, form &x, form& y) {
     int d_bits = D.num_bits();
     std::vector<unsigned char> serialization = SerializeForm(x, d_bits);
```

### Comparing `chiavdf-1.0.9/src/prover_slow.h` & `chiavdf-1.4rc1/src/prover_slow.h`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     integer res = FastPow(2, T - k * (i + 1), B);
     mpz_mul_2exp(res.impl, res.impl, k);
     res = res / B;
     auto res_vector = res.to_vector();
     return res_vector[0];
 }
 
-form GenerateWesolowski(form &y, form &x_init,
-                        integer &D, PulmarkReducer& reducer,
-                        std::vector<form> const& intermediates,
-                        uint64_t num_iterations,
+form GenerateWesolowski(form &y, form &x_init, 
+                        integer &D, PulmarkReducer& reducer, 
+                        std::vector<form>& intermediates,
+                        uint64_t num_iterations, 
                         uint64_t k, uint64_t l) {
     integer B = GetB(D, x_init, y);
     integer L=root(-D, 4);
 
     uint64_t k1 = k / 2;
     uint64_t k0 = k - k1;
     assert(k > 0);
@@ -78,33 +78,27 @@
     return x;
 }
 
 std::vector<uint8_t> ProveSlow(integer& D, form& x, uint64_t num_iterations) {
     integer L = root(-D, 4);
     PulmarkReducer reducer;
     form y = form::from_abd(x.a, x.b, D);
+    std::vector<form> intermediates;
+    int k, l;
     int d_bits = D.num_bits();
 
-    int k, l;
     ApproximateParameters(num_iterations, l, k);
     if (k <= 0) k = 1;
     if (l <= 0) l = 1;
-    int const kl = k * l;
-
-    uint64_t const size_vec = (num_iterations + kl - 1) / kl;
-    std::vector<form> intermediates(size_vec);
-    form* cursor = intermediates.data();
-    for (uint64_t i = 0; i < num_iterations; i++) {
-        if (i % kl == 0) {
-            *cursor = y;
-            ++cursor;
+    for (int i = 0; i < num_iterations; i++) {
+        if (i % (k * l) == 0) {
+            intermediates.push_back(y);
         }
         nudupl_form(y, y, D, L);
         reducer.reduce(y);
-    }
-
+    } 
     form proof = GenerateWesolowski(y, x, D, reducer, intermediates, num_iterations, k, l);
     std::vector<uint8_t> result = SerializeForm(y, d_bits);
     std::vector<uint8_t> proof_bytes = SerializeForm(proof, d_bits);
     result.insert(result.end(), proof_bytes.begin(), proof_bytes.end());
     return result;
 }
```

### Comparing `chiavdf-1.0.9/src/prover_test.cpp` & `chiavdf-1.4rc1/src/prover_test.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Proof CreateProof(integer D, ProverManager& pm, uint64_t iteration) {
     Proof proof = pm.Prove(iteration);
     if (!stop_signal) {
         form x = form::generator(D);
         std::vector<unsigned char> bytes;
         bytes.insert(bytes.end(), proof.y.begin(), proof.y.end());
         bytes.insert(bytes.end(), proof.proof.begin(), proof.proof.end());
-        if (CheckProofOfTimeNWesolowski(D, DEFAULT_ELEMENT, bytes.data(), bytes.size(), iteration, 1024, proof.witness_type)) {
+        if (CheckProofOfTimeNWesolowski(D, DEFAULT_ELEMENT, bytes.data(), bytes.size(), iteration, proof.witness_type)) {
             std::cout << "Correct proof";
         } else {
             std::cout << "Incorrect proof\n";
             std::exit(1);
         }
         std::cout << " (iteration: " << iteration << ").\n";
     }
```

### Comparing `chiavdf-1.0.9/src/provers.h` & `chiavdf-1.4rc1/src/provers.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/python_bindings/fastvdf.cpp` & `chiavdf-1.4rc1/src/python_bindings/fastvdf.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 
 PYBIND11_MODULE(chiavdf, m) {
     m.doc() = "Chia proof of time";
 
     // Creates discriminant.
     m.def("create_discriminant", [] (const py::bytes& challenge_hash, int discriminant_size_bits) {
         std::string challenge_hash_str(challenge_hash);
-        py::gil_scoped_release release;
         auto challenge_hash_bits = std::vector<uint8_t>(challenge_hash_str.begin(), challenge_hash_str.end());
         integer D = CreateDiscriminant(
             challenge_hash_bits,
             discriminant_size_bits
         );
         return D.to_string();
     });
 
     // Checks a simple wesolowski proof.
     m.def("verify_wesolowski", [] (const string& discriminant,
                                    const string& x_s, const string& y_s,
                                    const string& proof_s,
                                    uint64_t num_iterations) {
-        py::gil_scoped_release release;
         integer D(discriminant);
         form x = DeserializeForm(D, (const uint8_t *)x_s.data(), x_s.size());
         form y = DeserializeForm(D, (const uint8_t *)y_s.data(), y_s.size());
         form proof = DeserializeForm(D, (const uint8_t *)proof_s.data(), proof_s.size());
 
         bool is_valid = false;
         VerifyWesolowskiProof(D, x, y, proof, num_iterations, is_valid);
@@ -37,63 +35,54 @@
     });
 
     // Checks an N wesolowski proof.
     m.def("verify_n_wesolowski", [] (const string& discriminant,
                                    const string& x_s,
                                    const string& proof_blob,
                                    const uint64_t num_iterations, const uint64_t disc_size_bits, const uint64_t recursion) {
-        py::gil_scoped_release release;
         std::string proof_blob_str(proof_blob);
         uint8_t *proof_blob_ptr = reinterpret_cast<uint8_t *>(proof_blob_str.data());
         int proof_blob_size = proof_blob.size();
 
-        return CheckProofOfTimeNWesolowski(integer(discriminant), (const uint8_t *)x_s.data(), proof_blob_ptr, proof_blob_size, num_iterations, disc_size_bits, recursion);
-    });
-
-    m.def("prove", [] (const py::bytes& challenge_hash, const string& x_s, int discriminant_size_bits, uint64_t num_iterations) {
-        std::string challenge_hash_str(challenge_hash);
-        std::vector<uint8_t> result;
-        {
-            py::gil_scoped_release release;
-            std::vector<uint8_t> challenge_hash_bytes(challenge_hash_str.begin(), challenge_hash_str.end());
-            integer D = CreateDiscriminant(
-                    challenge_hash_bytes,
-                    discriminant_size_bits
-            );
-            form x = DeserializeForm(D, (const uint8_t *) x_s.data(), x_s.size());
-            result = ProveSlow(D, x, num_iterations);
-        }
-        py::bytes ret = py::bytes(reinterpret_cast<char*>(result.data()), result.size());
-        return ret;
+        return CheckProofOfTimeNWesolowski(integer(discriminant), (const uint8_t *)x_s.data(), proof_blob_ptr, proof_blob_size, num_iterations, recursion);
     });
 
     // Checks an N wesolowski proof, given y is given by 'GetB()' instead of a form.
     m.def("verify_n_wesolowski_with_b", [] (const string& discriminant,
                                    const string& B,
                                    const string& x_s,
                                    const string& proof_blob,
                                    const uint64_t num_iterations, const uint64_t recursion) {
+        std::string proof_blob_str(proof_blob);
+        uint8_t *proof_blob_ptr = reinterpret_cast<uint8_t *>(proof_blob_str.data());
+        int proof_blob_size = proof_blob.size();
         std::pair<bool, std::vector<uint8_t>> result;
-        {
-            py::gil_scoped_release release;
-            std::string proof_blob_str(proof_blob);
-            uint8_t *proof_blob_ptr = reinterpret_cast<uint8_t *>(proof_blob_str.data());
-            int proof_blob_size = proof_blob.size();
-            result = CheckProofOfTimeNWesolowskiWithB(integer(discriminant), integer(B), (const uint8_t *)x_s.data(), proof_blob_ptr, proof_blob_size, num_iterations, recursion);
-        }
+        result = CheckProofOfTimeNWesolowskiWithB(integer(discriminant), integer(B), (const uint8_t *)x_s.data(), proof_blob_ptr, proof_blob_size, num_iterations, recursion);
         py::bytes res_bytes = py::bytes(reinterpret_cast<char*>(result.second.data()), result.second.size());
         py::tuple res_tuple = py::make_tuple(result.first, res_bytes);
         return res_tuple;
     });
 
     m.def("get_b_from_n_wesolowski", [] (const string& discriminant,
                                    const string& x_s,
                                    const string& proof_blob,
                                    const uint64_t num_iterations, const uint64_t recursion) {
-        py::gil_scoped_release release;
         std::string proof_blob_str(proof_blob);
         uint8_t *proof_blob_ptr = reinterpret_cast<uint8_t *>(proof_blob_str.data());
         int proof_blob_size = proof_blob.size();
         integer B = GetBFromProof(integer(discriminant), (const uint8_t *)x_s.data(), proof_blob_ptr, proof_blob_size, num_iterations, recursion);
         return B.to_string();
     });
+
+    m.def("prove", [] (const py::bytes& challenge_hash, const string& x_s, int discriminant_size_bits, uint64_t num_iterations) {
+        std::string challenge_hash_str(challenge_hash);
+        std::vector<uint8_t> challenge_hash_bytes(challenge_hash_str.begin(), challenge_hash_str.end());
+        integer D = CreateDiscriminant(
+                challenge_hash_bytes,
+                discriminant_size_bits
+        );
+        form x = DeserializeForm(D, (const uint8_t *)x_s.data(), x_s.size());
+        auto result = ProveSlow(D, x, num_iterations);
+        py::bytes ret = py::bytes(reinterpret_cast<char*>(result.data()), result.size());
+        return ret;
+    });
 }
```

### Comparing `chiavdf-1.0.9/src/refcode/README.md` & `chiavdf-1.4rc1/src/refcode/README.md`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/refcode/lzcnt.c` & `chiavdf-1.4rc1/src/refcode/lzcnt.c`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/threading.h` & `chiavdf-1.4rc1/src/threading.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/uint128_t/LICENSE` & `chiavdf-1.4rc1/src/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/uint128_t/README.md` & `chiavdf-1.4rc1/src/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/uint128_t/uint128_t.cpp` & `chiavdf-1.4rc1/src/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/uint128_t/uint128_t.include` & `chiavdf-1.4rc1/src/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/uint128_t/uint128_t_config.include` & `chiavdf-1.4rc1/src/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/util.h` & `chiavdf-1.4rc1/src/util.h`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     form proof;
     bool is_empty;
 
     Segment() {
         is_empty = true;
     }
 
-    Segment(uint64_t start, uint64_t length, form& x, form& y) {
+    Segment(uint64_t start, uint64_t length, form& x, form& y) {        
         this->start = start;
         this->length = length;
         this->x = x;
         this->y = y;
         is_empty = false;
     }
 
@@ -58,15 +58,15 @@
         if (is_empty) {
             if (!other.is_empty)
                 return true;
             return false;
         }
         if (length > other.length)
             return true;
-        if (length < other.length)
+        if (length < other.length)  
             return false;
         return start > other.start;
     }
 
     int GetSegmentBucket() {
         uint64_t c_length = length;
         length >>= 16;
```

### Comparing `chiavdf-1.0.9/src/vdf.h` & `chiavdf-1.4rc1/src/vdf.h`

 * *Files 0% similar despite different names*

```diff
@@ -238,19 +238,17 @@
         print( "fast iterations per slow iteration", double(num_iterations_fast)/double(num_iterations_slow) );
     #endif
 }
 
 Proof ProveOneWesolowski(uint64_t iters, integer& D, form f, OneWesolowskiCallback* weso,
     std::atomic<bool>& stopped)
 {
-    while (!stopped && weso->iterations < iters) {
+    while (weso->iterations < iters) {
         this_thread::sleep_for(1s);
     }
-    if (stopped)
-        return Proof();
     Segment sg(
         /*start=*/0,
         /*length=*/iters,
         /*x=*/f,
         /*y=*/weso->result
     );
     OneWesolowskiProver prover(sg, D, weso->forms.get(), stopped);
@@ -449,15 +447,15 @@
             last_segment = sg;
         }
         uint64_t proved_iters = 0;
         bool valid_proof = false;
         while (!valid_proof && !stopped) {
             std::unique_lock<std::mutex> lk(proof_mutex);
             proof_cv.wait(lk, [this, iteration] {
-                if (max_proving_iteration >= iteration - iteration % (1 << 16))
+                if (max_proving_iteration >= iteration - iteration % (1 << 16)) 
                     return true;
                 return stopped.load();
             });
             if (stopped)
                 return Proof();
             int blobs = 0;
             for (int i = segment_count - 1; i >= 0; i--) {
@@ -560,24 +558,24 @@
                 std::lock_guard<std::mutex> lk(proof_mutex);
                 bool new_small_segment = false;
                 // Check if some provers finished.
                 for (int i = 0; i < provers.size(); i++) {
                     if (provers[i].first->IsFinished()) {
                         provers[i].second.proof = provers[i].first->GetProof();
                         if (debug_mode) {
-                            std::cout << "Done segment: [" << provers[i].second.start
-                                      << ", " << provers[i].second.start + provers[i].second.length
+                            std::cout << "Done segment: [" << provers[i].second.start 
+                                      << ", " << provers[i].second.start + provers[i].second.length 
                                       << "]. Bucket: " << provers[i].second.GetSegmentBucket() << ".\n";
                         }
                         if (provers[i].second.length == (1 << 16)) {
                             new_small_segment = true;
                         }
                         int index = provers[i].second.GetSegmentBucket();
                         int position = provers[i].second.start / provers[i].second.length;
-                        while (done_segments[index].size() <= position)
+                        while (done_segments[index].size() <= position)  
                             done_segments[index].emplace_back(Segment());
                         done_segments[index][position] = provers[i].second;
                         if (provers[i].first->IsFullyFinished()) {
                             provers.erase(provers.begin() + i);
                             i--;
                         }
                     }
@@ -586,15 +584,15 @@
                 // We can advance the proving iterations only when a new 2^16 segment is done.
                 if (new_small_segment) {
                     uint64_t expected_proving_iters = 0;
                     if (done_segments[0].size() > 0) {
                         expected_proving_iters = done_segments[0][done_segments[0].size() - 1].start +
                                                  done_segments[0][done_segments[0].size() - 1].length;
                     }
-
+                    
                     if (pending_iters.size() > 0)
                         best_pending_iter = *pending_iters.begin();
                     if (pending_iters.size() > 0 && expected_proving_iters >= best_pending_iter - best_pending_iter % (1 << 16)) {
                         // Calculate the real number of iters we can prove.
                         // It needs to stick to 64-wesolowski limit.
                         // In some cases, the last 2^16 segment might be slightly inaccurate,
                         // so calculate the real number.
@@ -687,15 +685,15 @@
                 if (active_provers < max_proving_threads) {
                     spawn_best = true;
                     active_provers++;
                 } else {
                     // Otherwise, pause one already running segment, if candidate is better.
                     Segment worst_running;
                     int worst_index;
-                    for (int i = 0; i < provers.size(); i++)
+                    for (int i = 0; i < provers.size(); i++) 
                         if (provers[i].first->IsRunning()) {
                             if (worst_running.is_empty == true || provers[i].second.IsWorseThan(worst_running)) {
                                 worst_running = provers[i].second;
                                 worst_index = i;
                             }
                         }
                     // If the candidate is better than worst running, stop worst running and spawn candidate.
```

### Comparing `chiavdf-1.0.9/src/vdf_bench.cpp` & `chiavdf-1.4rc1/src/vdf_bench.cpp`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/vdf_client.cpp` & `chiavdf-1.4rc1/src/vdf_client.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 int gcd_128_max_iter=3;
 
 int main(int argc, char* argv[]) try
 {
     init_gmp();
     if (argc != 4)
     {
-      std::cerr << "Usage: ./vdf_client <host> <port> <counter>\n";
+      std::cerr << "Usage: ./vdf_client <host> <port>\n";
       return 1;
     }
 
     if(hasAVX2())
     {
       gcd_base_bits=63;
       gcd_128_max_iter=2;
```

### Comparing `chiavdf-1.0.9/src/vdf_fast.h` & `chiavdf-1.4rc1/src/vdf_fast.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/vdf_new.h` & `chiavdf-1.4rc1/src/vdf_new.h`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     static form identity(const integer& d) {
         return from_abd(integer(1), integer(1), d);
     }
 
     static form generator(const integer& d) {
         return from_abd(integer(2), integer(1), d);
     }
-
+    
     void reduce() {
         ::reduce(a, b, c);
     }
 
     bool is_reduced() {
         int a_cmp_c = mpz_cmp(a.impl, c.impl);
```

### Comparing `chiavdf-1.0.9/src/vdf_original.h` & `chiavdf-1.4rc1/src/vdf_original.h`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ***/
 
 class vdf_original
 {
 public:
-
+    
     struct form {
         // y = ax^2 + bxy + y^2
         mpz_t a;
         mpz_t b;
         mpz_t c;
 
         //mpz_t d; // discriminant
@@ -317,10 +317,10 @@
         mpz_inits(negative_a, r, denom, old_a, old_b, ra, s, x, g, d, e, q, w, m,
                 u, a, b, k, mu, v, sigma, lambda, f3.a, f3.b, f3.c, //f3.d,
                 NULL);
     }
 
     ~vdf_original() {
         mpz_clears(negative_a, r, denom, old_a, old_b, ra, s, x, g, d, e, q, w, m,
-                   u, a, b, k, mu, v, sigma, lambda, f3.a, f3.b, f3.c, NULL); //,);
+                   u, a, b, k, mu, v, sigma, lambda, f3.a, f3.b, f3.c, NULL); //,); 
     }
 };
```

### Comparing `chiavdf-1.0.9/src/vdf_test.cpp` & `chiavdf-1.4rc1/src/vdf_test.cpp`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/vdf_test.h` & `chiavdf-1.4rc1/src/vdf_test.h`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/src/verifier.h` & `chiavdf-1.4rc1/src/verifier.h`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 #include "picosha2.h"
 #include "nucomp.h"
 #include "proof_common.h"
 #include "create_discriminant.h"
 
 const uint8_t DEFAULT_ELEMENT[] = { 0x08 };
 
-int VerifyWesoSegment(integer &D, form x, form proof, integer &B, uint64_t iters, form &out_y)
+int VerifyWesoSegment(integer &D, form x, form proof, integer &B, uint64_t iters, bool skip_check, form &out_y)
 {
     PulmarkReducer reducer;
     integer L = root(-D, 4);
     integer r = FastPow(2, iters, B);
     form f1 = FastPowFormNucomp(proof, D, B, L, reducer);
     form f2 = FastPowFormNucomp(x, D, r, L, reducer);
     out_y = f1 * f2;
-
+    // Optimize to only get `out_y` without verification, when not needed.
+    if (skip_check) {
+        return 0;
+    }
     return B == GetB(D, x, out_y) ? 0 : -1;
 }
 
 void VerifyWesolowskiProof(integer &D, form x, form y, form proof, uint64_t iters, bool &is_valid)
 {
     PulmarkReducer reducer;
     integer L = root(-D, 4);
@@ -37,95 +40,70 @@
     }
     else
     {
         is_valid = false;
     }
 }
 
-bool CheckProofOfTimeNWesolowski(integer D, const uint8_t* x_s, const uint8_t* proof_blob, int32_t proof_blob_len, uint64_t iterations, uint64 disc_size_bits, int32_t depth)
-{
+bool CheckProofOfTimeNWesolowskiCommon(integer& D, form& x, const uint8_t* proof_blob, int32_t proof_blob_len, uint64_t& iterations, int last_segment, bool skip_check = false) {
     int form_size = BQFC_FORM_SIZE;
     int segment_len = 8 + B_bytes + form_size;
     int i = proof_blob_len - segment_len;
-    form x = DeserializeForm(D, x_s, form_size);
 
-    if (proof_blob_len != 2 * form_size + depth * segment_len)
-        return false;
-
-    // Loop depth times
-    bool is_valid = false;
-    for (; i >= 2 * form_size; i -= segment_len) {
+    for (; i >= last_segment; i -= segment_len) {
         uint64_t segment_iters = BytesToInt64(&proof_blob[i]);
         form proof = DeserializeForm(D, &proof_blob[i + 8 + B_bytes], form_size);
         integer B(&proof_blob[i + 8], B_bytes);
         form xnew;
-        if (VerifyWesoSegment(D, x, proof, B, segment_iters, xnew))
+        if (VerifyWesoSegment(D, x, proof, B, segment_iters, skip_check, xnew))
             return false;
 
         x = xnew;
         if (segment_iters > iterations) {
             return false;
         }
         iterations -= segment_iters;
     }
+    return true;
+}
 
+bool CheckProofOfTimeNWesolowski(integer D, const uint8_t* x_s, const uint8_t* proof_blob, int32_t proof_blob_len, uint64_t iterations, int32_t depth) {
+    int form_size = BQFC_FORM_SIZE;
+    int segment_len = 8 + B_bytes + form_size;
+    form x = DeserializeForm(D, x_s, form_size);
+    if (proof_blob_len != 2 * form_size + depth * segment_len) {
+        return false;
+    }
+    bool is_valid = CheckProofOfTimeNWesolowskiCommon(D, x, proof_blob, proof_blob_len, iterations, 2 * form_size);
+    if (is_valid == false) {
+        return false;
+    }
     VerifyWesolowskiProof(D, x,
         DeserializeForm(D, proof_blob, form_size),
         DeserializeForm(D, &proof_blob[form_size], form_size),
         iterations, is_valid);
 
     return is_valid;
 }
 
-bool CheckProofOfTimeNWesolowskiCommon(integer& D, form& x, const uint8_t* proof_blob, int32_t proof_blob_len, uint64_t& iterations, int last_segment, bool skip_check = false) {
-    int form_size = BQFC_FORM_SIZE;
-    int segment_len = 8 + B_bytes + form_size;
-    int i = proof_blob_len - segment_len;
-    PulmarkReducer reducer;
-
-    for (; i >= last_segment; i -= segment_len) {
-        uint64_t segment_iters = BytesToInt64(&proof_blob[i]);
-        form proof = DeserializeForm(D, &proof_blob[i + 8 + B_bytes], form_size);
-        integer B(&proof_blob[i + 8], B_bytes);
-        form xnew;
-        if (!skip_check) {
-            if (VerifyWesoSegment(D, x, proof, B, segment_iters, xnew))
-                return false;
-        } else {
-            integer L = root(-D, 4);
-            integer r = FastPow(2, segment_iters, B);
-            form f1 = FastPowFormNucomp(proof, D, B, L, reducer);
-            form f2 = FastPowFormNucomp(x, D, r, L, reducer);
-            xnew = f1 * f2;
-        }
-
-        x = xnew;
-        if (segment_iters > iterations) {
-            return false;
-        }
-        iterations -= segment_iters;
-    }
-    return true;
-}
-
 std::pair<bool, std::vector<uint8_t>> CheckProofOfTimeNWesolowskiWithB(integer D, integer B, const uint8_t* x_s, const uint8_t* proof_blob, int32_t proof_blob_len, uint64_t iterations, int32_t depth) {
     int form_size = BQFC_FORM_SIZE;
     int segment_len = 8 + B_bytes + form_size;
     form x = DeserializeForm(D, x_s, form_size);
     std::vector<uint8_t> result;
     if (proof_blob_len != form_size + depth * segment_len) {
         return {false, result};
     }
     bool is_valid = CheckProofOfTimeNWesolowskiCommon(D, x, proof_blob, proof_blob_len, iterations, form_size);
     if (is_valid == false) {
         return {false, result};
     }
     form proof = DeserializeForm(D, proof_blob, form_size);
     form y_result;
-    if (VerifyWesoSegment(D, x, proof, B, iterations, y_result) == -1) {
+    if (VerifyWesoSegment(D, x, proof, B, iterations, /*skip_check=*/false, y_result) == -1) {
         return {false, result};
     }
     int d_bits = D.num_bits();
     result = SerializeForm(y_result, d_bits);
     return {true, result};
 }
```

### Comparing `chiavdf-1.0.9/src/verifier_test.cpp` & `chiavdf-1.4rc1/src/verifier_test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
         bool is_valid = CheckProofOfTimeNWesolowski(
             integer("-131653324254138636653163861414331698305531090221496467927360326686715180966094250598321899621249972220387687148397451395672779897144571112116763666653213748473909547482437246405018707472153290116227072825447643324530509016778432769802300913461285128339119844239772697652504835780459732685000796733645621728639"),
             DEFAULT_ELEMENT,
             arr,
             result.size(),
             33554432,
-            1024,
             2);
 
     auto challenge_hash1 = HexToBytes(string("a4bb1461ade74ac602e9ae511af68bb254dfe65d61b7faf9fab82d0b4364a30b").data());
     auto challenge_hash2 = HexToBytes(string("1633f29c0ca0597258507bc7d323a8bd485d5f059da56340a2c616081fb05b7f").data());
     auto challenge_hash3 = HexToBytes(string("6aa2451d1469e1213e50f114a49744f96073fedbe53921c8294a303779baa32d").data());
 
     // Create Discriminant tests
```

### Comparing `chiavdf-1.0.9/src/xgcd_partial.c` & `chiavdf-1.4rc1/src/xgcd_partial.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
     Copyright (C) 2012 William Hart
 
     Permission is hereby granted, free of charge, to any person obtaining a copy of this
-    software and associated documentation files (the "Software"), to deal in the Software
-    without restriction, including without limitation the rights to use, copy, modify, merge,
-    publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons
+    software and associated documentation files (the "Software"), to deal in the Software 
+    without restriction, including without limitation the rights to use, copy, modify, merge, 
+    publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons 
     to whom the Software is furnished to do so, subject to the following conditions:
 
     The above copyright notice and this permission notice shall be included in all copies or
     substantial portions of the Software.
 
     THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
     INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
     PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
     FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
     OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
     DEALINGS IN THE SOFTWARE.
-
+    
     MIT licensing permission obtained January 13, 2020 by Chia Network Inc. from William Hart
     */
 
 #ifndef _XGCD_PARTIAL
 #define _XGCD_PARTIAL
 
 #include <gmp.h>
@@ -29,47 +29,47 @@
                                     mpz_t r2, mpz_t r1, const mpz_t L)
 {
    mpz_t q, r;
    mp_limb_signed_t aa2, aa1, bb2, bb1, rr1, rr2, qq, bb, t1, t2, t3, i;
    mp_limb_signed_t bits, bits1, bits2;
 
    mpz_init(q); mpz_init(r);
-
+   
    mpz_set_ui(co2, 0);
    mpz_set_si(co1, -1);
-
+  
    while (mpz_cmp_ui(r1, 0) && mpz_cmp(r1, L) > 0)
    {
       bits2 = mpz_sizeinbase(r2, 2);
       bits1 = mpz_sizeinbase(r1, 2);
       bits = __GMP_MAX(bits2, bits1) - GMP_LIMB_BITS + 1;
       if (bits < 0) bits = 0;
-
+      
       mpz_tdiv_q_2exp(r, r2, bits);
       rr2 = mpz_get_ui(r);
       mpz_tdiv_q_2exp(r, r1, bits);
       rr1 = mpz_get_ui(r);
       mpz_tdiv_q_2exp(r, L, bits);
       bb = mpz_get_ui(r);
 
       aa2 = 0; aa1 = 1;
       bb2 = 1; bb1 = 0;
 
       for (i = 0; rr1 != 0 && rr1 > bb; i++)
       {
          qq = rr2 / rr1;
 
-         t1 = rr2 - qq*rr1;
-         t2 = aa2 - qq*aa1;
-         t3 = bb2 - qq*bb1;
+         t1 = rr2 - qq*rr1; 
+         t2 = aa2 - qq*aa1; 
+         t3 = bb2 - qq*bb1; 
 
          if (i & 1)
          {
             if (t1 < -t3 || rr1 - t1 < t2 - aa1) break;
-         } else
+         } else 
          {
             if (t1 < -t2 || rr1 - t1 < t3 - bb1) break;
          }
 
          rr2 = rr1; rr1 = t1;
          aa2 = aa1; aa1 = t2;
          bb2 = bb1; bb1 = t3;
@@ -110,15 +110,15 @@
 
          if (mpz_sgn(r1) < 0) { mpz_neg(co1, co1); mpz_neg(r1, r1); }
          if (mpz_sgn(r2) < 0) { mpz_neg(co2, co2); mpz_neg(r2, r2); }
       }
    }
 
    if (mpz_sgn(r2) < 0)
-   {
+   { 
       mpz_neg(co2, co2); mpz_neg(co1, co1);
       mpz_neg(r2, r2);
    }
 
    mpz_clear(q); mpz_clear(r);
 }
 #endif /* _XGCD_PARTIAL */
```

### Comparing `chiavdf-1.0.9/tests/test_n_weso_verifier.py` & `chiavdf-1.4rc1/tests/test_n_weso_verifier.py`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/tests/test_verifier.py` & `chiavdf-1.4rc1/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `chiavdf-1.0.9/tools/gen_pprods.py` & `chiavdf-1.4rc1/tools/gen_pprods.py`

 * *Files identical despite different names*

