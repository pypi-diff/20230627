# Comparing `tmp/pinard-0.9.7.tar.gz` & `tmp/pinard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinard-0.9.7.tar", last modified: Mon Nov 28 15:29:57 2022, max compression
+gzip compressed data, was "pinard-1.0.0.tar", last modified: Tue Jun 27 09:40:13 2023, max compression
```

## Comparing `pinard-0.9.7.tar` & `pinard-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.097585 pinard-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)    21864 2022-11-28 15:29:43.000000 pinard-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2022-11-28 15:29:57.097585 pinard-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2022-11-28 15:29:43.000000 pinard-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.089585 pinard-0.9.7/pinard/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.093585 pinard-0.9.7/pinard/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/augmentation/_random_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/augmentation/_spline_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/augmentation/augmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.093585 pinard-0.9.7/pinard/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/model_selection/_data_driven_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/model_selection/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/model_selection/_nirs_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/model_selection/_random_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.093585 pinard-0.9.7/pinard/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/preprocessing/_nirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/preprocessing/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/preprocessing/_standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.093585 pinard-0.9.7/pinard/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/sklearn/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/sklearn/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2022-11-28 15:29:43.000000 pinard-0.9.7/pinard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.093585 pinard-0.9.7/pinard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2022-11-28 15:29:57.000000 pinard-0.9.7/pinard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2022-11-28 15:29:57.000000 pinard-0.9.7/pinard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 15:29:57.000000 pinard-0.9.7/pinard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-11-28 15:29:57.000000 pinard-0.9.7/pinard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-11-28 15:29:57.000000 pinard-0.9.7/pinard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-11-28 15:29:57.000000 pinard-0.9.7/pinard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-28 15:29:57.097585 pinard-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2022-11-28 15:29:43.000000 pinard-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:57.097585 pinard-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/test_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2022-11-28 15:29:43.000000 pinard-0.9.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    21467 2023-06-27 09:40:03.000000 pinard-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-27 09:40:13.437826 pinard-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-27 09:40:03.000000 pinard-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/_random_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/_spline_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/augmentation/augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_data_driven_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_nirs_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/model_selection/_random_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/pinard/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/_nirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/preprocessing/_standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/pinard/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/sklearn/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/sklearn/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-27 09:40:03.000000 pinard-1.0.0/pinard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.433826 pinard-1.0.0/pinard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 09:40:13.000000 pinard-1.0.0/pinard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:40:13.437826 pinard-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-27 09:40:03.000000 pinard-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:13.437826 pinard-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 09:40:03.000000 pinard-1.0.0/tests/test_utils.py
```

### Comparing `pinard-0.9.7/LICENSE` & `pinard-1.0.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,517 +1,217 @@
+Cea Cnrs Inria Logiciel Libre License, version 2.1 (CECILL-2.1)
 
-CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
+Version 2.1 dated 2013-06-21
 
+Notice
 
-    Notice
+This Agreement is a Free Software license agreement that is the result of discussions between its authors in order to ensure compliance with the two main principles guiding its drafting:
 
-This Agreement is a Free Software license agreement that is the result
-of discussions between its authors in order to ensure compliance with
-the two main principles guiding its drafting:
+    firstly, compliance with the principles governing the distribution of Free Software: access to source code, broad rights granted to users,
+    secondly, the election of a governing law, French law, with which it is conformant, both as regards the law of torts and intellectual property law, and the protection that it offers to both authors and holders of the economic rights over software.
 
-    * firstly, compliance with the principles governing the distribution
-      of Free Software: access to source code, broad rights granted to
-      users,
-    * secondly, the election of a governing law, French law, with which
-      it is conformant, both as regards the law of torts and
-      intellectual property law, and the protection that it offers to
-      both authors and holders of the economic rights over software.
+The authors of the CeCILL (for Ce[a] C[nrs] I[nria] L[ogiciel] L[ibre]) license are:
 
-The authors of the CeCILL-C (for Ce[a] C[nrs] I[nria] L[ogiciel] L[ibre])
-license are:
+Commissariat à l’énergie atomique et aux énergies – CEA, a public scientific, technical and industrial research establishment, having its principal place of business at 25 rue Leblanc, immeuble Le Ponant D, 75015 Paris, France.
 
-Commissariat à l'Energie Atomique - CEA, a public scientific, technical
-and industrial research establishment, having its principal place of
-business at 25 rue Leblanc, immeuble Le Ponant D, 75015 Paris, France.
+Centre National de la Recherche Scientifique – CNRS, a public scientific and technological establishment, having its principal place of business at 3 rue Michel-Ange, 75794 Paris cedex 16, France.
 
-Centre National de la Recherche Scientifique - CNRS, a public scientific
-and technological establishment, having its principal place of business
-at 3 rue Michel-Ange, 75794 Paris cedex 16, France.
+Institut National de Recherche en Informatique et en Automatique – Inria, a public scientific and technological establishment, having its principal place of business at Domaine de Voluceau, Rocquencourt, BP 105, 78153 Le Chesnay cedex, France.
+Preamble
 
-Institut National de Recherche en Informatique et en Automatique -
-INRIA, a public scientific and technological establishment, having its
-principal place of business at Domaine de Voluceau, Rocquencourt, BP
-105, 78153 Le Chesnay cedex, France.
+The purpose of this Free Software license agreement is to grant users the right to modify and redistribute the software governed by this license within the framework of an open source distribution model.
 
+The exercising of this right is conditional upon certain obligations for users so as to preserve this status for all subsequent redistributions.
 
-    Preamble
+In consideration of access to the source code and the rights to copy, modify and redistribute granted by the license, users are provided only with a limited warranty and the software’s author, the holder of the economic rights, and the successive licensors only have limited liability.
 
-The purpose of this Free Software license agreement is to grant users
-the right to modify and re-use the software governed by this license.
+In this respect, the risks associated with loading, using, modifying and/or developing or reproducing the software by the user are brought to the user’s attention, given its Free Software status, which may make it complicated to use, with the result that its use is reserved for developers and experienced professionals having in-depth computer knowledge. Users are therefore encouraged to load and test the suitability of the software as regards their requirements in conditions enabling the security of their systems and/or data to be ensured and, more generally, to use and operate it in the same conditions of security. This Agreement may be freely reproduced and published, provided it is not altered, and that no provisions are either added or removed herefrom.
 
-The exercising of this right is conditional upon the obligation to make
-available to the community the modifications made to the source code of
-the software so as to contribute to its evolution.
+This Agreement may apply to any or all software for which the holder of the economic rights decides to submit the use thereof to its provisions.
 
-In consideration of access to the source code and the rights to copy,
-modify and redistribute granted by the license, users are provided only
-with a limited warranty and the software's author, the holder of the
-economic rights, and the successive licensors only have limited liability.
+Frequently asked questions can be found on the official website of the CeCILL licenses family (http://www.cecill.info/index.en.html) for any necessary clarification.
+Article 1 – DEFINITIONS
 
-In this respect, the risks associated with loading, using, modifying
-and/or developing or reproducing the software by the user are brought to
-the user's attention, given its Free Software status, which may make it
-complicated to use, with the result that its use is reserved for
-developers and experienced professionals having in-depth computer
-knowledge. Users are therefore encouraged to load and test the
-suitability of the software as regards their requirements in conditions
-enabling the security of their systems and/or data to be ensured and,
-more generally, to use and operate it in the same conditions of
-security. This Agreement may be freely reproduced and published,
-provided it is not altered, and that no provisions are either added or
-removed herefrom.
+For the purpose of this Agreement, when the following expressions commence with a capital letter, they shall have the following meaning:
 
-This Agreement may apply to any or all software for which the holder of
-the economic rights decides to submit the use thereof to its provisions.
+Agreement: means this license agreement, and its possible subsequent versions and annexes.
 
+Software: means the software in its Object Code and/or Source Code form and, where applicable, its documentation, “as is” when the Licensee accepts the Agreement.
 
-    Article 1 - DEFINITIONS
+Initial Software: means the Software in its Source Code and possibly its Object Code form and, where applicable, its documentation, “as is” when it is first distributed under the terms and conditions of the Agreement.
 
-For the purpose of this Agreement, when the following expressions
-commence with a capital letter, they shall have the following meaning:
+Modified Software: means the Software modified by at least one Contribution.
 
-Agreement: means this license agreement, and its possible subsequent
-versions and annexes.
+Source Code: means all the Software’s instructions and program lines to which access is required so as to modify the Software.
 
-Software: means the software in its Object Code and/or Source Code form
-and, where applicable, its documentation, "as is" when the Licensee
-accepts the Agreement.
+Object Code: means the binary files originating from the compilation of the Source Code.
 
-Initial Software: means the Software in its Source Code and possibly its
-Object Code form and, where applicable, its documentation, "as is" when
-it is first distributed under the terms and conditions of the Agreement.
-
-Modified Software: means the Software modified by at least one
-Integrated Contribution.
-
-Source Code: means all the Software's instructions and program lines to
-which access is required so as to modify the Software.
-
-Object Code: means the binary files originating from the compilation of
-the Source Code.
-
-Holder: means the holder(s) of the economic rights over the Initial
-Software.
+Holder: means the holder(s) of the economic rights over the Initial Software.
 
 Licensee: means the Software user(s) having accepted the Agreement.
 
-Contributor: means a Licensee having made at least one Integrated
-Contribution.
-
-Licensor: means the Holder, or any other individual or legal entity, who
-distributes the Software under the Agreement.
-
-Integrated Contribution: means any or all modifications, corrections,
-translations, adaptations and/or new functions integrated into the
-Source Code by any or all Contributors.
-
-Related Module: means a set of sources files including their
-documentation that, without modification to the Source Code, enables
-supplementary functions or services in addition to those offered by the
-Software.
-
-Derivative Software: means any combination of the Software, modified or
-not, and of a Related Module.
-
-Parties: mean both the Licensee and the Licensor.
-
-These expressions may be used both in singular and plural form.
-
-
-    Article 2 - PURPOSE
-
-The purpose of the Agreement is the grant by the Licensor to the
-Licensee of a non-exclusive, transferable and worldwide license for the
-Software as set forth in Article 5 hereinafter for the whole term of the
-protection granted by the rights over said Software. 
-
-
-    Article 3 - ACCEPTANCE
-
-3.1 The Licensee shall be deemed as having accepted the terms and
-conditions of this Agreement upon the occurrence of the first of the
-following events:
+Contributor: means a Licensee having made at least one Contribution.
 
-    * (i) loading the Software by any or all means, notably, by
-      downloading from a remote server, or by loading from a physical
-      medium;
-    * (ii) the first time the Licensee exercises any of the rights
-      granted hereunder.
+Licensor: means the Holder, or any other individual or legal entity, who distributes the Software under the Agreement.
 
-3.2 One copy of the Agreement, containing a notice relating to the
-characteristics of the Software, to the limited warranty, and to the
-fact that its use is restricted to experienced users has been provided
-to the Licensee prior to its acceptance as set forth in Article 3.1
-hereinabove, and the Licensee hereby acknowledges that it has read and
-understood it.
+Contribution: means any or all modifications, corrections, translations, adaptations and/or new functions integrated into the Software by any or all Contributors, as well as any or all Internal Modules.
 
+Module: means a set of sources files including their documentation that enables supplementary functions or services in addition to those offered by the Software.
 
-    Article 4 - EFFECTIVE DATE AND TERM
+External Module: means any or all Modules, not derived from the Software, so that this Module and the Software run in separate address spaces, with one calling the other when they are run.
 
+Internal Module: means any or all Module, connected to the Software so that they both execute in the same address space.
 
-      4.1 EFFECTIVE DATE
+GNU GPL: means the GNU General Public License version 2 or any subsequent version, as published by the Free Software Foundation Inc.
 
-The Agreement shall become effective on the date when it is accepted by
-the Licensee as set forth in Article 3.1.
+GNU Affero GPL: means the GNU Affero General Public License version 3 or any subsequent version, as published by the Free Software Foundation Inc.
 
+EUPL: means the European Union Public License version 1.1 or any subsequent version, as published by the European Commission.
 
-      4.2 TERM
-
-The Agreement shall remain in force for the entire legal term of
-protection of the economic rights over the Software.
+Parties: mean both the Licensee and the Licensor.
 
+These expressions may be used both in singular and plural form.
+Article 2 – PURPOSE
 
-    Article 5 - SCOPE OF RIGHTS GRANTED
+The purpose of the Agreement is the grant by the Licensor to the Licensee of a non-exclusive, transferable and worldwide license for the Software as set forth in Article 5 hereinafter for the whole term of the protection granted by the rights over said Software.
+Article 3 – ACCEPTANCE
 
-The Licensor hereby grants to the Licensee, who accepts, the following
-rights over the Software for any or all use, and for the term of the
-Agreement, on the basis of the terms and conditions set forth hereinafter.
+3.1 The Licensee shall be deemed as having accepted the terms and conditions of this Agreement upon the occurrence of the first of the following events:
 
-Besides, if the Licensor owns or comes to own one or more patents
-protecting all or part of the functions of the Software or of its
-components, the Licensor undertakes not to enforce the rights granted by
-these patents against successive Licensees using, exploiting or
-modifying the Software. If these patents are transferred, the Licensor
-undertakes to have the transferees subscribe to the obligations set
-forth in this paragraph.
+    (i) loading the Software by any or all means, notably, by downloading from a remote server, or by loading from a physical medium;
+    (ii) the first time the Licensee exercises any of the rights granted hereunder.
 
+3.2 One copy of the Agreement, containing a notice relating to the characteristics of the Software, to the limited warranty, and to the fact that its use is restricted to experienced users has been provided to the Licensee prior to its acceptance as set forth in Article 3.1 hereinabove, and the Licensee hereby acknowledges that it has read and understood it.
+Article 4 – EFFECTIVE DATE AND TERM
+4.1 EFFECTIVE DATE
 
-      5.1 RIGHT OF USE
+The Agreement shall become effective on the date when it is accepted by the Licensee as set forth in Article 3.1.
+4.2 TERM
 
-The Licensee is authorized to use the Software, without any limitation
-as to its fields of application, with it being hereinafter specified
-that this comprises:
+The Agreement shall remain in force for the entire legal term of protection of the economic rights over the Software.
+Article 5 – SCOPE OF RIGHTS GRANTED
 
-   1. permanent or temporary reproduction of all or part of the Software
-      by any or all means and in any or all form.
+The Licensor hereby grants to the Licensee, who accepts, the following rights over the Software for any or all use, and for the term of the Agreement, on the basis of the terms and conditions set forth hereinafter.
 
-   2. loading, displaying, running, or storing the Software on any or
-      all medium.
+Besides, if the Licensor owns or comes to own one or more patents protecting all or part of the functions of the Software or of its components, the Licensor undertakes not to enforce the rights granted by these patents against successive Licensees using, exploiting or modifying the Software. If these patents are transferred, the Licensor undertakes to have the transferees subscribe to the obligations set forth in this paragraph.
+5.1 RIGHT OF USE
 
-   3. entitlement to observe, study or test its operation so as to
-      determine the ideas and principles behind any or all constituent
-      elements of said Software. This shall apply when the Licensee
-      carries out any or all loading, displaying, running, transmission
-      or storage operation as regards the Software, that it is entitled
-      to carry out hereunder.
+The Licensee is authorized to use the Software, without any limitation as to its fields of application, with it being hereinafter specified that this comprises:
 
+    permanent or temporary reproduction of all or part of the Software by any or all means and in any or all form.
+    loading, displaying, running, or storing the Software on any or all medium.
+    entitlement to observe, study or test its operation so as to determine the ideas and principles behind any or all constituent elements of said Software. This shall apply when the Licensee carries out any or all loading, displaying, running, transmission or storage operation as regards the Software, that it is entitled to carry out hereunder.
 
-      5.2 RIGHT OF MODIFICATION
+5.2 ENTITLEMENT TO MAKE CONTRIBUTIONS
 
-The right of modification includes the right to translate, adapt,
-arrange, or make any or all modifications to the Software, and the right
-to reproduce the resulting software. It includes, in particular, the
-right to create a Derivative Software.
+The right to make Contributions includes the right to translate, adapt, arrange, or make any or all modifications to the Software, and the right to reproduce the resulting software.
 
-The Licensee is authorized to make any or all modification to the
-Software provided that it includes an explicit notice that it is the
-author of said modification and indicates the date of the creation thereof.
+The Licensee is authorized to make any or all Contributions to the Software provided that it includes an explicit notice that it is the author of said Contribution and indicates the date of the creation thereof.
+5.3 RIGHT OF DISTRIBUTION
 
+In particular, the right of distribution includes the right to publish, transmit and communicate the Software to the general public on any or all medium, and by any or all means, and the right to market, either in consideration of a fee, or free of charge, one or more copies of the Software by any means.
 
-      5.3 RIGHT OF DISTRIBUTION
+The Licensee is further authorized to distribute copies of the modified or unmodified Software to third parties according to the terms and conditions set forth hereinafter.
+5.3.1 DISTRIBUTION OF SOFTWARE WITHOUT MODIFICATION
 
-In particular, the right of distribution includes the right to publish,
-transmit and communicate the Software to the general public on any or
-all medium, and by any or all means, and the right to market, either in
-consideration of a fee, or free of charge, one or more copies of the
-Software by any means.
+The Licensee is authorized to distribute true copies of the Software in Source Code or Object Code form, provided that said distribution complies with all the provisions of the Agreement and is accompanied by:
 
-The Licensee is further authorized to distribute copies of the modified
-or unmodified Software to third parties according to the terms and
-conditions set forth hereinafter.
+    a copy of the Agreement,
+    a notice relating to the limitation of both the Licensor’s warranty and liability as set forth in Articles 8 and 9,
 
+and that, in the event that only the Object Code of the Software is redistributed, the Licensee allows effective access to the full Source Code of the Software for a period of at least three years from the distribution of the Software, it being understood that the additional acquisition cost of the Source Code shall not exceed the cost of the data transfer.
+5.3.2 DISTRIBUTION OF MODIFIED SOFTWARE
 
-        5.3.1 DISTRIBUTION OF SOFTWARE WITHOUT MODIFICATION
+When the Licensee makes a Contribution to the Software, the terms and conditions for the distribution of the resulting Modified Software become subject to all the provisions of this Agreement.
 
-The Licensee is authorized to distribute true copies of the Software in
-Source Code or Object Code form, provided that said distribution
-complies with all the provisions of the Agreement and is accompanied by:
+The Licensee is authorized to distribute the Modified Software, in source code or object code form, provided that said distribution complies with all the provisions of the Agreement and is accompanied by:
 
-   1. a copy of the Agreement,
+    a copy of the Agreement,
+    a notice relating to the limitation of both the Licensor’s warranty and liability as set forth in Articles 8 and 9,
 
-   2. a notice relating to the limitation of both the Licensor's
-      warranty and liability as set forth in Articles 8 and 9,
+and, in the event that only the object code of the Modified Software is redistributed,
 
-and that, in the event that only the Object Code of the Software is
-redistributed, the Licensee allows effective access to the full Source
-Code of the Software at a minimum during the entire period of its
-distribution of the Software, it being understood that the additional
-cost of acquiring the Source Code shall not exceed the cost of
-transferring the data.
+    a note stating the conditions of effective access to the full source code of the Modified Software for a period of at least three years from the distribution of the Modified Software, it being understood that the additional acquisition cost of the source code shall not exceed the cost of the data transfer.
 
+5.3.3 DISTRIBUTION OF EXTERNAL MODULES
 
-        5.3.2 DISTRIBUTION OF MODIFIED SOFTWARE
+When the Licensee has developed an External Module, the terms and conditions of this Agreement do not apply to said External Module, that may be distributed under a separate license agreement.
+5.3.4 COMPATIBILITY WITH OTHER LICENSES
 
-When the Licensee makes an Integrated Contribution to the Software, the
-terms and conditions for the distribution of the resulting Modified
-Software become subject to all the provisions of this Agreement.
+The Licensee can include a code that is subject to the provisions of one of the versions of the GNU GPL, GNU Affero GPL and/or EUPL in the Modified or unmodified Software, and distribute that entire code under the terms of the same version of the GNU GPL, GNU Affero GPL and/or EUPL.
 
-The Licensee is authorized to distribute the Modified Software, in
-source code or object code form, provided that said distribution
-complies with all the provisions of the Agreement and is accompanied by:
+The Licensee can include the Modified or unmodified Software in a code that is subject to the provisions of one of the versions of the GNU GPL, GNU Affero GPL and/or EUPL and distribute that entire code under the terms of the same version of the GNU GPL, GNU Affero GPL and/or EUPL.
+Article 6 – INTELLECTUAL PROPERTY
+6.1 OVER THE INITIAL SOFTWARE
 
-   1. a copy of the Agreement,
+The Holder owns the economic rights over the Initial Software. Any or all use of the Initial Software is subject to compliance with the terms and conditions under which the Holder has elected to distribute its work and no one shall be entitled to modify the terms and conditions for the distribution of said Initial Software.
 
-   2. a notice relating to the limitation of both the Licensor's
-      warranty and liability as set forth in Articles 8 and 9,
+The Holder undertakes that the Initial Software will remain ruled at least by this Agreement, for the duration set forth in Article 4.2.
+6.2 OVER THE CONTRIBUTIONS
 
-and that, in the event that only the object code of the Modified
-Software is redistributed, the Licensee allows effective access to the
-full source code of the Modified Software at a minimum during the entire
-period of its distribution of the Modified Software, it being understood
-that the additional cost of acquiring the source code shall not exceed
-the cost of transferring the data.
+The Licensee who develops a Contribution is the owner of the intellectual property rights over this Contribution as defined by applicable law.
+6.3 OVER THE EXTERNAL MODULES
 
+The Licensee who develops an External Module is the owner of the intellectual property rights over this External Module as defined by applicable law and is free to choose the type of agreement that shall govern its distribution.
+6.4 JOINT PROVISIONS
 
-        5.3.3 DISTRIBUTION OF DERIVATIVE SOFTWARE
+The Licensee expressly undertakes:
 
-When the Licensee creates Derivative Software, this Derivative Software
-may be distributed under a license agreement other than this Agreement,
-subject to compliance with the requirement to include a notice
-concerning the rights over the Software as defined in Article 6.4.
-In the event the creation of the Derivative Software required modification 
-of the Source Code, the Licensee undertakes that:
+    not to remove, or modify, in any manner, the intellectual property notices attached to the Software;
+    to reproduce said notices, in an identical manner, in the copies of the Software modified or not.
 
-   1. the resulting Modified Software will be governed by this Agreement,
-   2. the Integrated Contributions in the resulting Modified Software
-      will be clearly identified and documented,
-   3. the Licensee will allow effective access to the source code of the
-      Modified Software, at a minimum during the entire period of
-      distribution of the Derivative Software, such that such
-      modifications may be carried over in a subsequent version of the
-      Software; it being understood that the additional cost of
-      purchasing the source code of the Modified Software shall not
-      exceed the cost of transferring the data.
+The Licensee undertakes not to directly or indirectly infringe the intellectual property rights on the Software of the Holder and/or Contributors, and to take, where applicable, vis-à-vis its staff, any and all measures required to ensure respect of said intellectual property rights of the Holder and/or Contributors.
+Article 7 – RELATED SERVICES
 
+7.1 Under no circumstances shall the Agreement oblige the Licensor to provide technical assistance or maintenance services for the Software.
 
-        5.3.4 COMPATIBILITY WITH THE CeCILL LICENSE
+However, the Licensor is entitled to offer this type of services. The terms and conditions of such technical assistance, and/or such maintenance, shall be set forth in a separate instrument. Only the Licensor offering said maintenance and/or technical assistance services shall incur liability therefor.
 
-When a Modified Software contains an Integrated Contribution subject to
-the CeCILL license agreement, or when a Derivative Software contains a
-Related Module subject to the CeCILL license agreement, the provisions
-set forth in the third item of Article 6.4 are optional.
+7.2 Similarly, any Licensor is entitled to offer to its licensees, under its sole responsibility, a warranty, that shall only be binding upon itself, for the redistribution of the Software and/or the Modified Software, under terms and conditions that it is free to decide. Said warranty, and the financial terms and conditions of its application, shall be subject of a separate instrument executed between the Licensor and the Licensee.
+Article 8 – LIABILITY
 
+8.1 Subject to the provisions of Article 8.2, the Licensee shall be entitled to claim compensation for any direct loss it may have suffered from the Software as a result of a fault on the part of the relevant Licensor, subject to providing evidence thereof.
 
-    Article 6 - INTELLECTUAL PROPERTY
+8.2 The Licensor’s liability is limited to the commitments made under this Agreement and shall not be incurred as a result of in particular: (i) loss due the Licensee’s total or partial failure to fulfill its obligations, (ii) direct or consequential loss that is suffered by the Licensee due to the use or performance of the Software, and (iii) more generally, any consequential loss. In particular the Parties expressly agree that any or all pecuniary or business loss (i.e. loss of data, loss of profits, operating loss, loss of customers or orders, opportunity cost, any disturbance to business activities) or any or all legal proceedings instituted against the Licensee by a third party, shall constitute consequential loss and shall not provide entitlement to any or all compensation from the Licensor.
+Article 9 – WARRANTY
 
+9.1 The Licensee acknowledges that the scientific and technical state-of-the-art when the Software was distributed did not enable all possible uses to be tested and verified, nor for the presence of possible defects to be detected. In this respect, the Licensee’s attention has been drawn to the risks associated with loading, using, modifying and/or developing and reproducing the Software which are reserved for experienced users.
 
-      6.1 OVER THE INITIAL SOFTWARE
+The Licensee shall be responsible for verifying, by any or all means, the suitability of the product for its requirements, its good working order, and for ensuring that it shall not cause damage to either persons or properties.
 
-The Holder owns the economic rights over the Initial Software. Any or
-all use of the Initial Software is subject to compliance with the terms
-and conditions under which the Holder has elected to distribute its work
-and no one shall be entitled to modify the terms and conditions for the
-distribution of said Initial Software.
+9.2 The Licensor hereby represents, in good faith, that it is entitled to grant all the rights over the Software (including in particular the rights set forth in Article 5).
 
-The Holder undertakes that the Initial Software will remain ruled at
-least by this Agreement, for the duration set forth in Article 4.2.
+9.3 The Licensee acknowledges that the Software is supplied “as is” by the Licensor without any other express or tacit warranty, other than that provided for in Article 9.2 and, in particular, without any warranty as to its commercial value, its secured, safe, innovative or relevant nature.
 
+Specifically, the Licensor does not warrant that the Software is free from any error, that it will operate without interruption, that it will be compatible with the Licensee’s own equipment and software configuration, nor that it will meet the Licensee’s requirements.
 
-      6.2 OVER THE INTEGRATED CONTRIBUTIONS
+9.4 The Licensor does not either expressly or tacitly warrant that the Software does not infringe any third party intellectual property right relating to a patent, software or any other property right. Therefore, the Licensor disclaims any and all liability towards the Licensee arising out of any or all proceedings for infringement that may be instituted in respect of the use, modification and redistribution of the Software. Nevertheless, should such proceedings be instituted against the Licensee, the Licensor shall provide it with technical and legal expertise for its defense. Such technical and legal expertise shall be decided on a case-by-case basis between the relevant Licensor and the Licensee pursuant to a memorandum of understanding. The Licensor disclaims any and all liability as regards the Licensee’s use of the name of the Software. No warranty is given as regards the existence of prior rights over the name of the Software or as regards the existence of a trademark.
+Article 10 – TERMINATION
 
-The Licensee who develops an Integrated Contribution is the owner of the
-intellectual property rights over this Contribution as defined by
-applicable law.
+10.1 In the event of a breach by the Licensee of its obligations hereunder, the Licensor may automatically terminate this Agreement thirty (30) days after notice has been sent to the Licensee and has remained ineffective.
 
+10.2 A Licensee whose Agreement is terminated shall no longer be authorized to use, modify or distribute the Software. However, any licenses that it may have granted prior to termination of the Agreement shall remain valid subject to their having been granted in compliance with the terms and conditions hereof.
+Article 11 – MISCELLANEOUS
+11.1 EXCUSABLE EVENTS
 
-      6.3 OVER THE RELATED MODULES
+Neither Party shall be liable for any or all delay, or failure to perform the Agreement, that may be attributable to an event of force majeure, an act of God or an outside cause, such as defective functioning or interruptions of the electricity or telecommunications networks, network paralysis following a virus attack, intervention by government authorities, natural disasters, water damage, earthquakes, fire, explosions, strikes and labor unrest, war, etc.
 
-The Licensee who develops a Related Module is the owner of the
-intellectual property rights over this Related Module as defined by
-applicable law and is free to choose the type of agreement that shall
-govern its distribution under the conditions defined in Article 5.3.3.
+11.2 Any failure by either Party, on one or more occasions, to invoke one or more of the provisions hereof, shall under no circumstances be interpreted as being a waiver by the interested Party of its right to invoke said provision(s) subsequently.
 
+11.3 The Agreement cancels and replaces any or all previous agreements, whether written or oral, between the Parties and having the same purpose, and constitutes the entirety of the agreement between said Parties concerning said purpose. No supplement or modification to the terms and conditions hereof shall be effective as between the Parties unless it is made in writing and signed by their duly authorized representatives.
 
-      6.4 NOTICE OF RIGHTS
+11.4 In the event that one or more of the provisions hereof were to conflict with a current or future applicable act or legislative text, said act or legislative text shall prevail, and the Parties shall make the necessary amendments so as to comply with said act or legislative text. All other provisions shall remain effective. Similarly, invalidity of a provision of the Agreement, for any reason whatsoever, shall not cause the Agreement as a whole to be invalid.
+11.5 LANGUAGE
 
-The Licensee expressly undertakes:
+The Agreement is drafted in both French and English and both versions are deemed authentic.
+Article 12 – NEW VERSIONS OF THE AGREEMENT
 
-   1. not to remove, or modify, in any manner, the intellectual property
-      notices attached to the Software;
+12.1 Any person is authorized to duplicate and distribute copies of this Agreement.
 
-   2. to reproduce said notices, in an identical manner, in the copies
-      of the Software modified or not;
+12.2 So as to ensure coherence, the wording of this Agreement is protected and may only be modified by the authors of the License, who reserve the right to periodically publish updates or new versions of the Agreement, each with a separate number. These subsequent versions may address new issues encountered by Free Software.
 
-   3. to ensure that use of the Software, its intellectual property
-      notices and the fact that it is governed by the Agreement is
-      indicated in a text that is easily accessible, specifically from
-      the interface of any Derivative Software.
-
-The Licensee undertakes not to directly or indirectly infringe the
-intellectual property rights of the Holder and/or Contributors on the
-Software and to take, where applicable, vis-à-vis its staff, any and all
-measures required to ensure respect of said intellectual property rights
-of the Holder and/or Contributors.
-
-
-    Article 7 - RELATED SERVICES
-
-7.1 Under no circumstances shall the Agreement oblige the Licensor to
-provide technical assistance or maintenance services for the Software.
-
-However, the Licensor is entitled to offer this type of services. The
-terms and conditions of such technical assistance, and/or such
-maintenance, shall be set forth in a separate instrument. Only the
-Licensor offering said maintenance and/or technical assistance services
-shall incur liability therefor.
-
-7.2 Similarly, any Licensor is entitled to offer to its licensees, under
-its sole responsibility, a warranty, that shall only be binding upon
-itself, for the redistribution of the Software and/or the Modified
-Software, under terms and conditions that it is free to decide. Said
-warranty, and the financial terms and conditions of its application,
-shall be subject of a separate instrument executed between the Licensor
-and the Licensee.
-
-
-    Article 8 - LIABILITY
-
-8.1 Subject to the provisions of Article 8.2, the Licensee shall be
-entitled to claim compensation for any direct loss it may have suffered
-from the Software as a result of a fault on the part of the relevant
-Licensor, subject to providing evidence thereof.
-
-8.2 The Licensor's liability is limited to the commitments made under
-this Agreement and shall not be incurred as a result of in particular:
-(i) loss due the Licensee's total or partial failure to fulfill its
-obligations, (ii) direct or consequential loss that is suffered by the
-Licensee due to the use or performance of the Software, and (iii) more
-generally, any consequential loss. In particular the Parties expressly
-agree that any or all pecuniary or business loss (i.e. loss of data,
-loss of profits, operating loss, loss of customers or orders,
-opportunity cost, any disturbance to business activities) or any or all
-legal proceedings instituted against the Licensee by a third party,
-shall constitute consequential loss and shall not provide entitlement to
-any or all compensation from the Licensor.
-
-
-    Article 9 - WARRANTY
-
-9.1 The Licensee acknowledges that the scientific and technical
-state-of-the-art when the Software was distributed did not enable all
-possible uses to be tested and verified, nor for the presence of
-possible defects to be detected. In this respect, the Licensee's
-attention has been drawn to the risks associated with loading, using,
-modifying and/or developing and reproducing the Software which are
-reserved for experienced users.
-
-The Licensee shall be responsible for verifying, by any or all means,
-the suitability of the product for its requirements, its good working
-order, and for ensuring that it shall not cause damage to either persons
-or properties.
-
-9.2 The Licensor hereby represents, in good faith, that it is entitled
-to grant all the rights over the Software (including in particular the
-rights set forth in Article 5).
-
-9.3 The Licensee acknowledges that the Software is supplied "as is" by
-the Licensor without any other express or tacit warranty, other than
-that provided for in Article 9.2 and, in particular, without any warranty
-as to its commercial value, its secured, safe, innovative or relevant
-nature.
-
-Specifically, the Licensor does not warrant that the Software is free
-from any error, that it will operate without interruption, that it will
-be compatible with the Licensee's own equipment and software
-configuration, nor that it will meet the Licensee's requirements.
-
-9.4 The Licensor does not either expressly or tacitly warrant that the
-Software does not infringe any third party intellectual property right
-relating to a patent, software or any other property right. Therefore,
-the Licensor disclaims any and all liability towards the Licensee
-arising out of any or all proceedings for infringement that may be
-instituted in respect of the use, modification and redistribution of the
-Software. Nevertheless, should such proceedings be instituted against
-the Licensee, the Licensor shall provide it with technical and legal
-assistance for its defense. Such technical and legal assistance shall be
-decided on a case-by-case basis between the relevant Licensor and the
-Licensee pursuant to a memorandum of understanding. The Licensor
-disclaims any and all liability as regards the Licensee's use of the
-name of the Software. No warranty is given as regards the existence of
-prior rights over the name of the Software or as regards the existence
-of a trademark.
-
-
-    Article 10 - TERMINATION
-
-10.1 In the event of a breach by the Licensee of its obligations
-hereunder, the Licensor may automatically terminate this Agreement
-thirty (30) days after notice has been sent to the Licensee and has
-remained ineffective.
-
-10.2 A Licensee whose Agreement is terminated shall no longer be
-authorized to use, modify or distribute the Software. However, any
-licenses that it may have granted prior to termination of the Agreement
-shall remain valid subject to their having been granted in compliance
-with the terms and conditions hereof.
-
-
-    Article 11 - MISCELLANEOUS
-
-
-      11.1 EXCUSABLE EVENTS
-
-Neither Party shall be liable for any or all delay, or failure to
-perform the Agreement, that may be attributable to an event of force
-majeure, an act of God or an outside cause, such as defective
-functioning or interruptions of the electricity or telecommunications
-networks, network paralysis following a virus attack, intervention by
-government authorities, natural disasters, water damage, earthquakes,
-fire, explosions, strikes and labor unrest, war, etc.
-
-11.2 Any failure by either Party, on one or more occasions, to invoke
-one or more of the provisions hereof, shall under no circumstances be
-interpreted as being a waiver by the interested Party of its right to
-invoke said provision(s) subsequently.
-
-11.3 The Agreement cancels and replaces any or all previous agreements,
-whether written or oral, between the Parties and having the same
-purpose, and constitutes the entirety of the agreement between said
-Parties concerning said purpose. No supplement or modification to the
-terms and conditions hereof shall be effective as between the Parties
-unless it is made in writing and signed by their duly authorized
-representatives.
-
-11.4 In the event that one or more of the provisions hereof were to
-conflict with a current or future applicable act or legislative text,
-said act or legislative text shall prevail, and the Parties shall make
-the necessary amendments so as to comply with said act or legislative
-text. All other provisions shall remain effective. Similarly, invalidity
-of a provision of the Agreement, for any reason whatsoever, shall not
-cause the Agreement as a whole to be invalid.
-
-
-      11.5 LANGUAGE
-
-The Agreement is drafted in both French and English and both versions
-are deemed authentic.
-
-
-    Article 12 - NEW VERSIONS OF THE AGREEMENT
-
-12.1 Any person is authorized to duplicate and distribute copies of this
-Agreement.
-
-12.2 So as to ensure coherence, the wording of this Agreement is
-protected and may only be modified by the authors of the License, who
-reserve the right to periodically publish updates or new versions of the
-Agreement, each with a separate number. These subsequent versions may
-address new issues encountered by Free Software.
-
-12.3 Any Software distributed under a given version of the Agreement may
-only be subsequently distributed under the same version of the Agreement
-or a subsequent version.
-
-
-    Article 13 - GOVERNING LAW AND JURISDICTION
-
-13.1 The Agreement is governed by French law. The Parties agree to
-endeavor to seek an amicable solution to any disagreements or disputes
-that may arise during the performance of the Agreement.
-
-13.2 Failing an amicable solution within two (2) months as from their
-occurrence, and unless emergency proceedings are necessary, the
-disagreements or disputes shall be referred to the Paris Courts having
-jurisdiction, by the more diligent Party.
+12.3 Any Software distributed under a given version of the Agreement may only be subsequently distributed under the same version of the Agreement or a subsequent version, subject to the provisions of Article 5.3.4.
+Article 13 – GOVERNING LAW AND JURISDICTION
 
+13.1 The Agreement is governed by French law. The Parties agree to endeavor to seek an amicable solution to any disagreements or disputes that may arise during the performance of the Agreement.
 
-Version 1.0 dated 2006-09-05.
+13.2 Failing an amicable solution within two (2) months as from their occurrence, and unless emergency proceedings are necessary, the disagreements or disputes shall be referred to the Paris Courts having jurisdiction, by the more diligent Party.
```

### Comparing `pinard-0.9.7/pinard/augmentation/__init__.py` & `pinard-1.0.0/pinard/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/pinard/preprocessing/__init__.py` & `pinard-1.0.0/pinard/preprocessing/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 The :mod:`pinard.preprocessing` module includes savitzky golay, baseline, haar, 
 gaussian, etc. TransformerMixins to preprocess NIR spectra.
 """
 from sklearn.preprocessing import FunctionTransformer as IdentityTransformer
 from sklearn.preprocessing import RobustScaler as RobustNormalVariate
 from sklearn.preprocessing import StandardScaler as StandardNormalVariate
 
-from ._nirs import (Haar, MultiplicativeScatterCorrection, SavitzkyGolay,
-                    Wavelet, msc, savgol, wavelet_transform)
-from ._scaler import (Derivate, Normalize, SimpleScale, derivate, norml,
-                      spl_norml)
+from ._nirs import (Haar, MultiplicativeScatterCorrection, SavitzkyGolay, Wavelet, msc, savgol, wavelet_transform)
+from ._scaler import (Derivate, Normalize, SimpleScale, derivate, norml, spl_norml)
 from ._standard import Baseline, Detrend, Gaussian, baseline, detrend, gaussian
 
 __all__ = [
     "IdentityTransformer",  # sklearn.preprocessing.FunctionTransformer alias
     "Baseline",
     "StandardNormalVariate",  # sklearn.preprocessing.StandardScaler alias
     "RobustNormalVariate",  # sklearn.preprocessing.RobusScaler alias
```

### Comparing `pinard-0.9.7/pinard/preprocessing/_nirs.py` & `pinard-1.0.0/pinard/preprocessing/_nirs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,232 @@
 import numpy as np
 import pywt
-from scipy import signal, sparse
+import scipy
+from scipy import signal
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import StandardScaler, scale
 from sklearn.utils import check_array
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted
 
 
-# mode: ['zero', 'constant', 'symmetric', 'periodic', 'smooth', 'periodization',
-# 'reflect', 'antisymmetric', 'antireflect']
-# wavelet: ['haar', 'db', 'sym', 'coif', 'bior', 'rbio', 'dmey', 'gaus', 'mexh', 'morl',
-# 'cgau', 'shan', 'fbsp', 'cmor']
-def wavelet_transform(spectra, wavelet, mode="periodization"):
-    """Computes transform using pywavelet transform.
+def wavelet_transform(spectra: np.ndarray, wavelet: str, mode: str = "periodization") -> np.ndarray:
+    """
+    Computes transform using pywavelet transform.
+
     Args:
-        spectra < numpy.ndarray > : NIRS data matrix.
-        wavelet < str > : wavelet family transformation
-        mode < str > : signal extension mode
+        spectra (numpy.ndarray): NIRS data matrix.
+        wavelet (str): wavelet family transformation.
+        mode (str): signal extension mode.
+
     Returns:
-        spectra < numpy.ndarray > : wavelet and resampled spectra.
+        numpy.ndarray: wavelet and resampled spectra.
     """
     _, wt_coeffs = pywt.dwt(spectra, wavelet=wavelet, mode=mode)
     if len(wt_coeffs[0]) != len(spectra[0]):
         return signal.resample(wt_coeffs, len(spectra[0]), axis=1)
     else:
         return wt_coeffs
 
 
 class Wavelet(TransformerMixin, BaseEstimator):
-    """Single level Discrete Wavelet Transform.
+    """
+    Single level Discrete Wavelet Transform.
 
     Performs a discrete wavelet transform on `data`, using a `wavelet` function.
-    see: https://pywavelets.readthedocs.io
 
     Parameters
-    --  --  --  --  --
-    wavelet : Wavelet object or name, default = 'haar'
+    ----------
+    wavelet : Wavelet object or name, default='haar'
         Wavelet to use: ['Haar', 'Daubechies', 'Symlets', 'Coiflets', 'Biorthogonal',
         'Reverse biorthogonal', 'Discrete Meyer (FIR Approximation)'...]
-        see: https://www.pybytes.com/pywavelets/ref/wavelets.html#wavelet-families
+    mode : str, optional, default='periodization'
+        Signal extension mode.
 
-    mode : str, optional, default = 'periodization'
-        Signal extension mode.add
-        ['zero', 'constant', 'symmetric', 'periodic', 'smooth', 'periodization',
-         'reflect', 'antisymmetric', 'antireflect']
-        see: https://pywavelets.readthedocs.io/en/latest/ref/signal-extension-modes.html#ref-modes
     """
 
-    def __init__(self, wavelet="haar", mode="periodization", *, copy=True):
+    def __init__(self, wavelet: str = "haar", mode: str = "periodization", *, copy: bool = True):
         self.copy = copy
         self.wavelet = wavelet
         self.mode = mode
 
     def _reset(self):
         pass
 
     def fit(self, X, y=None):
-        """Verify the X data compliance with wavelet transform
+        """
+        Verify the X data compliance with wavelet transform.
 
         Parameters
-        --  --  --  --  --
-        X: array-like, spectra
+        ----------
+        X : array-like, spectra
             The data to transform.
-        y: (None) - Ignored
+        y : None
+            Ignored.
 
-        Raises:
-            ValueError: _description_
-
-        Returns:
-            _type_: _description_
+        Raises
+        ------
+        ValueError
+            If the input X is a sparse matrix.
+
+        Returns
+        -------
+        Wavelet
+            The fitted object.
         """
-        if sparse.issparse(X):
-            raise ValueError("Wavelets does not support sparse input")
+        if scipy.sparse.issparse(X):
+            raise ValueError("Wavelets does not support scipy.sparse input")
         return self
 
     def transform(self, X, copy=None):
-        if sparse.issparse(X):
+        """
+        Apply wavelet transform to the data X.
+
+        Parameters
+        ----------
+        X : array-like
+            The data to transform.
+        copy : bool or None, optional
+            Whether to copy the input data.
+
+        Returns
+        -------
+        numpy.ndarray
+            The transformed data.
+        """
+        if scipy.sparse.issparse(X):
             raise ValueError('Sparse matrices not supported!"')
 
         X = self._validate_data(
             X, reset=False, copy=self.copy, dtype=FLOAT_DTYPES, estimator=self
         )
 
         return wavelet_transform(X, self.wavelet, mode=self.mode)
 
     def _more_tags(self):
         return {"allow_nan": False}
 
 
 class Haar(Wavelet):
-    """Shortcut to the Wavelet haar transform"""
+    """
+    Shortcut to the Wavelet haar transform.
+    """
 
-    def __init__(self, *, copy=True):
+    def __init__(self, *, copy: bool = True):
         super().__init__("haar", "periodization", copy=copy)
 
 
-def savgol(spectra, window_length=11, polyorder=3, deriv=0, delta=1.0):
-    """Perform Savitzky–Golay filtering on the data (also calculates derivatives). 
+def savgol(
+    spectra: np.ndarray,
+    window_length: int = 11,
+    polyorder: int = 3,
+    deriv: int = 0,
+    delta: float = 1.0,
+) -> np.ndarray:
+    """
+    Perform Savitzky–Golay filtering on the data (also calculates derivatives).
     This function is a wrapper for scipy.signal.savgol_filter.
+
     Args:
-        spectra < numpy.ndarray > : NIRS data matrix.
-        filter_win < int > : Size of the filter window in samples (default 11).
-        polyorder < int > : Order of the polynomial estimation (default 3).
-        deriv < int > : Order of the derivation (default 0).
+        spectra (numpy.ndarray): NIRS data matrix.
+        window_length (int): Size of the filter window in samples (default 11).
+        polyorder (int): Order of the polynomial estimation (default 3).
+        deriv (int): Order of the derivation (default 0).
+        delta (float): Sampling distance of the data.
+
     Returns:
-        spectra < numpy.ndarray > : NIRS data smoothed with Savitzky-Golay filtering
+        numpy.ndarray: NIRS data smoothed with Savitzky-Golay filtering.
     """
     return signal.savgol_filter(spectra, window_length, polyorder, deriv, delta=delta)
 
 
 class SavitzkyGolay(TransformerMixin, BaseEstimator):
-    def __init__(self, window_length=11, polyorder=3, deriv=0, delta=1.0, *, copy=True):
+    """
+    A class for smoothing and differentiating data using the Savitzky-Golay filter.
+
+    Parameters:
+    -----------
+    window_length : int, optional (default=11)
+        The length of the window used for smoothing.
+    polyorder : int, optional (default=3)
+        The order of the polynomial used for fitting the samples within the window.
+    deriv : int, optional (default=0)
+        The order of the derivative to compute.
+    delta : float, optional (default=1.0)
+        The sampling distance of the data.
+    copy : bool, optional (default=True)
+        Whether to copy the input data.
+
+    Methods:
+    --------
+    fit(X, y=None)
+        Fits the transformer to the data X.
+    transform(X, copy=None)
+        Applies the Savitzky-Golay filter to the data X.
+    """
+
+    def __init__(
+        self,
+        window_length: int = 11,
+        polyorder: int = 3,
+        deriv: int = 0,
+        delta: float = 1.0,
+        *,
+        copy: bool = True
+    ):
         self.copy = copy
         self.window_length = window_length
         self.polyorder = polyorder
         self.deriv = deriv
         self.delta = delta
 
     def _reset(self):
         pass
 
     def fit(self, X, y=None):
-        if sparse.issparse(X):
-            raise ValueError("SavitzkyGolay does not support sparse input")
+        """
+        Verify the X data compliance with Savitzky-Golay filter.
+
+        Parameters
+        ----------
+        X : array-like
+            The data to transform.
+        y : None
+            Ignored.
+
+        Raises
+        ------
+        ValueError
+            If the input X is a sparse matrix.
+
+        Returns
+        -------
+        SavitzkyGolay
+            The fitted object.
+        """
+        if scipy.sparse.issparse(X):
+            raise ValueError("SavitzkyGolay does not support scipy.sparse input")
         return self
 
     def transform(self, X, copy=None):
-        if sparse.issparse(X):
+        """
+        Apply the Savitzky-Golay filter to the data X.
+
+        Parameters
+        ----------
+        X : array-like
+            The data to transform.
+        copy : bool or None, optional
+            Whether to copy the input data.
+
+        Returns
+        -------
+        numpy.ndarray
+            The transformed data.
+        """
+        if scipy.sparse.issparse(X):
             raise ValueError('Sparse matrices not supported!"')
 
         X = self._validate_data(
             X, reset=False, copy=self.copy, dtype=FLOAT_DTYPES, estimator=self
         )
 
         return savgol(
@@ -157,16 +253,16 @@
             del self.b_
 
     def fit(self, X, y=None):
         self._reset()
         return self.partial_fit(X, y)
 
     def partial_fit(self, X, y=None):
-        if sparse.issparse(X):
-            raise TypeError("Normalization does not support sparse input")
+        if scipy.sparse.issparse(X):
+            raise TypeError("Normalization does not support scipy.sparse input")
 
         first_pass = not hasattr(self, "mean_")
         X = self._validate_data(X, reset=first_pass, dtype=FLOAT_DTYPES, estimator=self)
 
         tmp_x = X
         if self.scale:
             scaler = StandardScaler(with_std=False)
@@ -231,18 +327,21 @@
 
     def _more_tags(self):
         return {"allow_nan": False}
 
 
 def msc(spectra, scaled=True):
     """Performs multiplicative scatter correction to the mean.
+
     Args:
-        spectra < numpy.ndarray > : NIRS data matrix.
+        spectra (numpy.ndarray): NIRS data matrix.
+        scaled (bool): Whether to scale the data. Defaults to True.
+
     Returns:
-        spectra < numpy.ndarray > : Scatter corrected NIR spectra.
+        numpy.ndarray: Scatter-corrected NIR spectra.
     """
     if scaled:
         spectra = scale(spectra, with_std=False, axis=0)  # StandardScaler / demean
 
     reference = np.mean(spectra, axis=1)
 
     for col in range(spectra.shape[1]):
```

### Comparing `pinard-0.9.7/pinard/preprocessing/_scaler.py` & `pinard-1.0.0/pinard/preprocessing/_scaler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from sklearn.utils.validation import check_array, check_is_fitted
 import warnings
 
 import numpy as np
-from scipy import sparse
+import scipy
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import FunctionTransformer as IdentityTransformer
 from sklearn.preprocessing import RobustScaler as RobustNormalVariate
 from sklearn.preprocessing import StandardScaler as StandardNormalVariate
 from sklearn.utils import check_array
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted
 
@@ -15,14 +16,15 @@
 
     Parameters
     ----------
     feature_range : tuple (min, max), default=(-1, -1)
         Desired range of transformed data. If range min and max equals -1, linalg
         normalization is applied, otherwise user defined normalization
         is applied
+
     copy : bool, default=True
         Set to False to perform inplace row normalization and avoid a
         copy (if the input is already a numpy array).
 
     """
 
     def __init__(self, feature_range=(-1, 1), *, copy=True):
@@ -36,33 +38,63 @@
             del self.max_
             del self.f_
 
         if hasattr(self, "linalg_norm_"):
             del self.linalg_norm_
 
     def fit(self, X, y=None):
+        """Fit the Normalize transformer on the training data.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The training data.
+
+        y : None
+            Ignored variable.
+
+        Returns
+        -------
+        self : object
+            Returns the instance itself.
+        """
         self._reset()
         return self.partial_fit(X, y)
 
     def partial_fit(self, X, y=None):
+        """Perform incremental fit on the training data.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The training data.
+
+        y : None
+            Ignored variable.
+
+        Returns
+        -------
+        self : object
+            Returns the instance itself.
+        """
         feature_range = self.feature_range
         if self.user_defined and feature_range[0] >= feature_range[1]:
             warnings.warn(
                 "Minimum of desired feature range should be smaller than "
                 "maximum. Got %s." % str(feature_range),
                 SyntaxWarning,
             )
 
         if self.user_defined and feature_range[0] == feature_range[1]:
             raise ValueError(
                 "Feature range is not correctly defined. Got %s." % str(feature_range)
             )
 
-        if sparse.issparse(X):
-            raise TypeError("Normalization does not support sparse input")
+        if scipy.sparse.issparse(X):
+            raise TypeError("Normalization does not support scipy.sparse input")
 
         first_pass = not hasattr(self, "min_")
         X = self._validate_data(X, reset=first_pass, dtype=FLOAT_DTYPES, estimator=self)
 
         if self.user_defined:
             self.min_ = np.min(X, axis=0)
             self.max_ = np.max(X, axis=0)
@@ -70,14 +102,26 @@
             imax = self.feature_range[1]
             self.f_ = (imax - imin) / (self.max_ - self.min_)
         else:
             self.linalg_norm_ = np.linalg.norm(X, axis=0)
         return self
 
     def transform(self, X):
+        """Transform the input data.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input data to be transformed.
+
+        Returns
+        -------
+        X : ndarray of shape (n_samples, n_features)
+            The transformed data.
+        """
         check_is_fitted(self)
 
         X = self._validate_data(
             X, reset=False, copy=self.copy, dtype=FLOAT_DTYPES, estimator=self
         )
 
         if self.user_defined:
@@ -91,14 +135,26 @@
                 arr = np.append(arr, [dnorm], axis=0)
             X = np.transpose(arr)
         else:
             X = X / self.linalg_norm_
         return X
 
     def inverse_transform(self, X):
+        """Transform the normalized data back to the original representation.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The normalized data to be transformed back.
+
+        Returns
+        -------
+        X : ndarray of shape (n_samples, n_features)
+            The inverse transformed data.
+        """
         check_is_fitted(self)
 
         X = check_array(X, copy=self.copy, dtype=FLOAT_DTYPES)
 
         if self.user_defined:
             imin = self.feature_range[0]
             f = self.f_
@@ -114,36 +170,43 @@
         return X
 
     def _more_tags(self):
         return {"allow_nan": False}
 
 
 def norml(spectra, feature_range=(-1, 1)):
-    """Perform spectral normalisation with user-defined limits. (numpy linalg)
-    Args:
-        spectra < numpy.ndarray > : NIRS data matrix.
-        feature_range : tuple (min, max), default=(-1, -1)
-            Desired range of transformed data. If range min and max equals -1, linalg
-            normalization is applied, otherwise user bounds defined normalization
-            is applied
-    Returns:
-        spectra < numpy.ndarray > : Normalized NIR spectra
     """
-    if feature_range[0] != -1 and feature_range[0] != -1:
+    Perform spectral normalization with user-defined limits.
+
+    Parameters
+    ----------
+    spectra : numpy.ndarray
+        NIRS data matrix.
+    feature_range : tuple (min, max), default=(-1, 1)
+        Desired range of transformed data. If range min and max equals -1, linalg
+        normalization is applied; otherwise, user bounds-defined normalization
+        is applied.
+
+    Returns
+    -------
+    spectra : numpy.ndarray
+        Normalized NIR spectra.
+    """
+    if feature_range[0] != -1 and feature_range[1] != -1:
         imin = feature_range[0]
         imax = feature_range[1]
         if imin >= imax:
             warnings.warn(
-                "Minimum of desired feature range should be smaller than maximum."
-                "Got %s." % str(feature_range),
+                "Minimum of desired feature range should be smaller than maximum. "
+                f"Got {feature_range}.",
                 SyntaxWarning,
             )
         if imin == imax:
             raise ValueError(
-                "Feature range is not correctly defined. Got %s." % str(feature_range)
+                f"Feature range is not correctly defined. Got {feature_range}."
             )
 
         f = (imax - imin) / (np.max(spectra) - np.min(spectra))
         n = spectra.shape
         arr = np.empty((0, n[0]), dtype=float)  # create empty array for spectra
         for i in range(0, n[1]):
             d = spectra[:, i]
@@ -151,29 +214,29 @@
             arr = np.append(arr, [dnorm], axis=0)
         return np.transpose(arr)
     else:
         return spectra / np.linalg.norm(spectra, axis=0)
 
 
 class Derivate(TransformerMixin, BaseEstimator):
-    def __init__(self, order=1, delta=1, *, copy=True):
+    def __init__(self, order=1, delta=1, copy=True):
         self.copy = copy
         self.order = order
         self.delta = delta
 
     def _reset(self):
         pass
 
     def fit(self, X, y=None):
-        if sparse.issparse(X):
-            raise ValueError("SavitzkyGolay does not support sparse input")
+        if scipy.sparse.issparse(X):
+            raise ValueError("SavitzkyGolay does not support scipy.sparse input")
         return self
 
     def transform(self, X, copy=None):
-        if sparse.issparse(X):
+        if scipy.sparse.issparse(X):
             raise ValueError('Sparse matrices not supported!"')
 
         X = self._validate_data(
             X, reset=False, copy=self.copy, dtype=FLOAT_DTYPES, estimator=self
         )
 
         for n in range(self.order):
@@ -182,43 +245,52 @@
         return X
 
     def _more_tags(self):
         return {"allow_nan": False}
 
 
 def derivate(spectra, order=1, delta=1):
-    """Computes Nth order derivates with the desired spacing using numpy.gradient.
-    Args:
-        spectra < numpy.ndarray > : NIRS data matrix.
-        order < float > : Order of the derivation.
-        delta < int > : Delta of the derivate (in samples).
-    Returns:
-        spectra < numpy.ndarray > : Derivated NIR spectra.
+    """
+    Computes Nth order derivatives with the desired spacing using numpy.gradient.
+
+    Parameters
+    ----------
+    spectra : numpy.ndarray
+        NIRS data matrix.
+    order : float, optional
+        Order of the derivation, by default 1.
+    delta : int, optional
+        Delta of the derivative (in samples), by default 1.
+
+    Returns
+    -------
+    spectra : numpy.ndarray
+        Derived NIR spectra.
     """
     for n in range(order):
         spectra = np.gradient(spectra, delta, axis=0)
     return spectra
 
 
 class SimpleScale(TransformerMixin, BaseEstimator):
-    def __init__(self, *, copy=True):
+    def __init__(self, copy=True):
         self.copy = copy
 
     def _reset(self):
         if hasattr(self, "min_"):
             del self.min_
             del self.max_
 
     def fit(self, X, y=None):
         self._reset()
         return self.partial_fit(X, y)
 
     def partial_fit(self, X, y=None):
-        if sparse.issparse(X):
-            raise TypeError("Normalization does not support sparse input")
+        if scipy.sparse.issparse(X):
+            raise TypeError("Normalization does not support scipy.sparse input")
 
         first_pass = not hasattr(self, "min_")
         X = self._validate_data(X, reset=first_pass, dtype=FLOAT_DTYPES, estimator=self)
 
         self.min_ = np.min(X, axis=0)
         self.max_ = np.max(X, axis=0)
         return self
@@ -245,16 +317,23 @@
         return X
 
     def _more_tags(self):
         return {"allow_nan": False}
 
 
 def spl_norml(spectra):
-    """Perform simple spectral normalisation. (manual algo)
-    Args:
-        spectra < numpy.ndarray > : NIRS data matrix.
-    Returns:
-        spectra < numpy.ndarray > : Normalized NIR spectra
+    """
+    Perform simple spectral normalization.
+
+    Parameters
+    ----------
+    spectra : numpy.ndarray
+        NIRS data matrix.
+
+    Returns
+    -------
+    spectra : numpy.ndarray
+        Normalized NIR spectra.
     """
     min_ = np.min(spectra, axis=0)
     max_ = np.max(spectra, axis=0)
     return (spectra - min_) / (max_ - min_)
```

### Comparing `pinard-0.9.7/pinard/sklearn/_pipeline.py` & `pinard-1.0.0/pinard/sklearn/_pipeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -42,34 +42,56 @@
             # All transformers are None
             return np.zeros((X.shape[0], 0))
         Xs = np.swapaxes(Xs, 0, 1)
         Xs = np.swapaxes(Xs, 1, 2)
         return Xs
 
 
-# def _transform_one(transformer, X, y, weight, **fit_params):
-#     res = transformer.transform(X)
-#     # if we have a weight for this transformer, multiply output
-#     if weight is None:
-#         return res
-#     return res * weight
+class SampleAugmentation(FeatureUnion):
+    """Applies multiple feature extraction mechanisms to the same input data and concatenates the results.
 
+    Inherits from the `FeatureUnion` class of the `sklearn.pipeline` module.
 
-# def _transform_one_xy(transformer, X, y, weight, **fit_params):
-#     resX, resY = transformer.transform(X, y)
-#     # if we have a weight for this transformer, multiply output
-#     if weight is None:
-#         return resX, resY
-#     return resX * weight, resY
+    Parameters
+    ----------
+    transformer_list : list of (str, transformer) or (int, str, transformer) tuples
+        List of transformer tuples to be applied to the data. Each tuple contains either two or three elements.
+        If the tuple has two elements, it is a (str, transformer) tuple where the first element is the name of the transformer and the second element is the transformer object.
+        If the tuple has three elements, it is an (int, str, transformer) tuple where the first element is the count of augmentations for that transformer, the second element is the name of the transformer and the third element is the transformer object.
+    n_jobs : int or None, optional (default=None)
+        The number of jobs to run in parallel. `None` means 1 unless in a `joblib.parallel_backend` context. `-1` means using all processors.
+    transformer_weights : dict or None, optional (default=None)
+        Multiplicative weights for features per transformer. Keys are transformer names, values are weights.
+    verbose : bool, optional (default=False)
+        If True, the time elapsed while fitting each transformer will be printed as it is completed.
+
+    Attributes
+    ----------
+    transformer_list : list of (str, transformer) tuples
+        List of (name, trans) tuples specifying the transformer objects to be applied to the data.
+    """
 
+    def __init__(self, transformer_list, *, n_jobs=None, transformer_weights=None, verbose=False):
+        """
+        This is the constructor for a class that initializes a list of transformers with optional
+        parameters.
 
-class SampleAugmentation(FeatureUnion):
-    def __init__(
-        self, transformer_list, *, n_jobs=None, transformer_weights=None, verbose=False
-    ):
+        :param transformer_list: A list of tuples where each tuple represents a transformer to be
+        applied to the data. The tuple can have either two or three elements. If it has two elements,
+        the first element is the transformer object and the second element is the name of the
+        transformer. If it has three elements, the first element
+        :param n_jobs: The number of CPU cores to use for parallel processing. If set to None, all
+        available cores will be used
+        :param transformer_weights: A dictionary of weights assigned to each transformer. These weights
+        are used to compute the weighted average of the transformed features. If not provided, all
+        transformers are assumed to have equal weight
+        :param verbose: A boolean parameter that controls whether or not progress messages are printed
+        to the console during the fitting process. If set to True, progress messages will be printed. If
+        set to False, no progress messages will be printed, defaults to False (optional)
+        """
         transformer_origin_list = []
         self.augmentation_count = []
         self.total_count = 0
         for tpl in transformer_list:
             if len(tpl) == 2:
                 transformer_origin_list.append(tpl)
                 self.augmentation_count.append(1)
@@ -129,14 +151,30 @@
 
         Xs = np.concatenate(Xs, axis=0)
         Ys = np.repeat(y, self.total_count, axis=0)
 
         return Xs, Ys
 
 
+# def _transform_one(transformer, X, y, weight, **fit_params):
+#     res = transformer.transform(X)
+#     # if we have a weight for this transformer, multiply output
+#     if weight is None:
+#         return res
+#     return res * weight
+
+
+# def _transform_one_xy(transformer, X, y, weight, **fit_params):
+#     resX, resY = transformer.transform(X, y)
+#     # if we have a weight for this transformer, multiply output
+#     if weight is None:
+#         return resX, resY
+#     return resX * weight, resY
+
+
 # class Pipeline_XY(Pipeline):
 #     def _validate_steps(self):
 #         pass
 #         # names, estimators = zip(*self.steps)
 
 #         # # validate names
 #         # self._validate_names(names)
```

### Comparing `pinard-0.9.7/pinard/sklearn/_utils.py` & `pinard-1.0.0/pinard/sklearn/_utils.py`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/pinard/utils.py` & `pinard-1.0.0/pinard/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 
 def load_csv(
     x_fname,
     y_fname=None,
     y_cols=0,
     *,
-    sep=";",
+    sep=None,
     x_hdr=None,
     y_hdr=None,
     x_index_col=None,
     y_index_col=None,
-    remove_na=False
+    autoremove_na=False
 ):
     """Helper to load a NIRS dataset from csv file(s) using pandas and numpy:
     The data can be either in one file (y_path set to None) or in two files
     for x and y data.
     Rows with NaN or str values are automatically removed.
 
     Parameters
@@ -57,52 +57,59 @@
         Automatically removed from the dataset.
         Default: None.
     y_index_col : int, str, sequence of int / str, or False, optional
         Column(s) to use as the row labels of the y data, either given as string name
         or column index.
         Automatically removed from the dataset.
         Default: None.
-    remove_na: bool
+    autoremove_na: bool
         The behavior with NA value. 
         If False, raises error if NA values are detected.
         If True, remove rows containing NA values.
         Default: False
 
     Returns
     -------
     np.array, ,np.array
         Returns x and y data as np.array containing np.float32.
     """
     assert y_fname is not None or y_cols is not None
     # TODO - add assert/exceptions on non-numerical columns
+    # TODO - better management of NaN and Null (esp exception msg)
 
     x_df = pd.read_csv(x_fname, sep=sep, header=x_hdr, index_col=x_index_col)
     x_df = x_df.apply(pd.to_numeric, args=("coerce",))
-    if remove_na:
-        x_df = x_df.dropna()
-    elif x_df.isna().values.any():
-        raise WrongFormatError(x_df, None)
 
     x_data = x_df.astype(np.float32).values
+    x_rows_del = []
+    if autoremove_na:
+        if np.isnan(x_data).any():
+            x_rows_del, _ = np.where(np.isnan(x_data))
+            x_data = np.delete(x_data, x_rows_del, axis=0)
+
     if len(x_data.shape) != 2 or len(x_data) == 0:
         raise WrongFormatError(x_data, None)
 
     y_data = None
     if y_fname is None:
         y_data = x_data[:, y_cols]
         x_data = np.delete(x_data, y_cols, axis=1)
     else:
         y_df = pd.read_csv(y_fname, sep=sep, header=y_hdr, index_col=y_index_col)
         y_df = y_df.apply(pd.to_numeric, args=("coerce",))
-        if remove_na:
-            y_df = y_df.dropna()
-        elif y_df.isna().values.any():
-            raise WrongFormatError(None, x_df)
-            
+
         y_data = y_df.astype(np.float32).values
+        if autoremove_na:
+            if len(x_rows_del) > 0:
+                y_data = np.delete(y_data, x_rows_del, axis=0)
+
+            if np.isnan(y_data).any():
+                y_rows_del, _ = np.where(np.isnan(y_data))
+                y_data = np.delete(y_data, y_rows_del, axis=0)
+                x_data = np.delete(x_data, y_rows_del, axis=0)
 
         if len(y_data.shape) != 2:
             raise WrongFormatError(x_data, y_data)
 
         if y_cols != -1:
             y_data = y_data[:, y_cols]
```

### Comparing `pinard-0.9.7/pinard.egg-info/SOURCES.txt` & `pinard-1.0.0/pinard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/setup.py` & `pinard-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/tests/conftest.py` & `pinard-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/tests/test_preprocessing.py` & `pinard-1.0.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/tests/test_selection.py` & `pinard-1.0.0/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `pinard-0.9.7/tests/test_utils.py` & `pinard-1.0.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def test_single_file_load(simple_data):
     x, y = utils.load_csv(simple_data, y_cols=[0, 1], x_hdr=0, x_index_col=[0, 1])
     assert x.shape == (6, 3)
     assert x[0, 1] == 2
 
 
 def test_single_file_load_na(simple_data_na):
-    x, y = utils.load_csv(simple_data_na, y_cols=[0, 1], x_hdr=0, x_index_col=[0, 1], remove_na=True)
+    x, y = utils.load_csv(simple_data_na, y_cols=[0, 1], x_hdr=0, x_index_col=[0, 1], autoremove_na=True)
     assert x.shape == (4, 3)
     assert x[0, 1] == 2
 
 
 def test_double_file_load(simple_data, simple_data_na):
     x, y = utils.load_csv(
         simple_data,
@@ -28,19 +28,12 @@
     assert x[0, 1] == 2
     assert y[0, 1] == 2
 
 
 def test_double_file_load_na(simple_data, simple_data_na):
     try:
         x, y = utils.load_csv(
-            simple_data,
-            simple_data_na,
-            y_cols=[0, 1],
-            x_hdr=0,
-            y_hdr=0,
-            x_index_col=[0, 1, 2, 3],
-            y_index_col=[0, 1],
-            remove_na=True
+            simple_data, simple_data_na, y_cols=[0, 1], x_hdr=0, y_hdr=0, x_index_col=[0, 1, 2, 3], y_index_col=[0, 1], autoremove_na=True
         )
     except utils.WrongFormatError as error:
         assert error.x.shape == (6, 3)
         assert error.y.shape == (4, 2)
```

