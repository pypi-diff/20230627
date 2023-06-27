# Comparing `tmp/matminer-0.8.0.tar.gz` & `tmp/matminer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matminer-0.8.0.tar", last modified: Fri Nov 11 00:18:39 2022, max compression
+gzip compressed data, was "matminer-0.9.0.tar", last modified: Tue Jun 27 15:44:39 2023, max compression
```

## Comparing `matminer-0.8.0.tar` & `matminer-0.9.0.tar`

### file list

```diff
@@ -1,573 +1,572 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.561413 matminer-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.493412 matminer-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-11 00:13:13.000000 matminer-0.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-11 00:13:13.000000 matminer-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.493412 matminer-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-11-11 00:13:13.000000 matminer-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3566 2022-11-11 00:13:13.000000 matminer-0.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3749 2022-11-11 00:13:13.000000 matminer-0.8.0/.github/workflows/upgrade-dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-11-11 00:13:13.000000 matminer-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-11-11 00:13:13.000000 matminer-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-11 00:13:13.000000 matminer-0.8.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-11-11 00:13:13.000000 matminer-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)   111284 2022-11-11 00:13:13.000000 matminer-0.8.0/Flowchart.png
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-11-11 00:13:13.000000 matminer-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-11-11 00:13:13.000000 matminer-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-11-11 00:18:39.561413 matminer-0.8.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     2088 2022-11-11 00:13:13.000000 matminer-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.489412 matminer-0.8.0/dev_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.493412 matminer-0.8.0/dev_scripts/dataset_management/
--rw-r--r--   0 runner    (1001) docker     (121)    10192 2022-11-11 00:13:13.000000 matminer-0.8.0/dev_scripts/dataset_management/generate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     8463 2022-11-11 00:13:13.000000 matminer-0.8.0/dev_scripts/dataset_management/modify_dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    56843 2022-11-11 00:13:13.000000 matminer-0.8.0/dev_scripts/dataset_management/prep_dataset_for_figshare.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.497412 matminer-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.501412 matminer-0.8.0/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (121)   267829 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/Flowchart.png
--rw-r--r--   0 runner    (1001) docker     (121)   233051 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/example_bulkmod.png
--rw-r--r--   0 runner    (1001) docker     (121)   201518 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/example_bulkmod_feats.png
--rw-r--r--   0 runner    (1001) docker     (121)   116774 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/example_bulkmod_rf.png
--rw-r--r--   0 runner    (1001) docker     (121)   453119 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/featurizer_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.513413 matminer-0.8.0/docs/_images/math/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/01caff91ea974c5cc0c133c5b4a560d433ff589b.png
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/0239bb38c93a6213c5ac6ba1dabd3e0a003ed371.png
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/02d98909b5d6acd6a7ff927d4d42790bdd407d58.png
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/045fae7cfacaf28d29d6bdb81ab5ef61b1b07808.png
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/0467e0003559a763cbcd16dcd0bf3c33f9c65901.png
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/06dfe124bb57b08106d4043aea4218b309454d8d.png
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/074903764bb5a464b7c346e84f43cba2174f3ab0.png
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/079ba1f3373823268ba0e33b400423434ca7c0a6.png
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/083b5d48a524b6f7a39570bbe0d51d474cb588e6.png
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/08e21b3be44ad4aac8ed231afc369152e9c8539c.png
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/0b21f31621e4f0f2b3b5faa10af80dc999f9ffdf.png
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/0b7c1e16a3a8a849bb8ffdcdbf86f65fd1f30438.png
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/0c9c2dac2bd7f86735f42ef4184918c37425d67a.png
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/0ee4480fa3fe2856c28f74b0aa03fde5e83cfb0a.png
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/12249dbb3a129598bfef9a4f490147c6a4537213.png
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/182c7d0771b253a55441383d191fce92f3d58e02.png
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/18711f8217158b267749b882e02ef2f9f17431c0.png
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/18a48ac390a7070c05a265edbfa13f1322d47daf.png
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/18f11bbc89febc978169289978481f64a403be7e.png
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/192c5eb5f76c194be10ed549a12e8cae7e9f4e37.png
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/1947a1c371cf018ebfcdf1fee66dacce40b9ab4c.png
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/1b1fd12d69ea533588e033d255888cb6a17cdca6.png
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/1c7982e9bed52596de46d839a5334f537de1c35d.png
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/1ebe654cc7b8f2a0d8100aa5825cf2b9021adbbc.png
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/1fbee781f84569077719a167b64e12064360fac1.png
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/20380591afec1e5625f65892e5af51719381bf91.png
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/22a57909899e26fbb172500446c43f2ba7ebd563.png
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/240509feeacaad2b6744f49f69502b84f78f1fef.png
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/298204ab1b85022412ad261503dcab8bd14fb321.png
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2aa528e29c4df6e3a7e44783f02f45e46012b948.png
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2c79776b8b888d73f48a6a996815a078713a2a78.png
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2ede365ad144ab396916ec60458da03860803078.png
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2fc0510f783f8ce42baa1c4ac6b86d94a6382093.png
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2fe13d18c90531495ad5a8b7976e2a7bda67ae7e.png
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2fe6d1d220a6eb68148f55432fd2234ca529685c.png
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/2ff684758d53878ad22e0ebaa7f34d709cc1b6a4.png
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/30634b08f5df289a7acab4963cb6a3e6b99aba0f.png
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/30d9a509980f1622c5d182d9b846afd31019bb05.png
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/31880c4812286affe8e1e36fce7bdc56e8e28458.png
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/31fdf41b39df23c95e52c5aef07f59d9adf82f3c.png
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/326c6fcc3609b0c2183f6a9e23d4aa1d4b141ea2.png
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/35bab58b40a77a2e24ecb9f58898f1813de64459.png
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/3af01b3f850c53aa06a7ef9878392efada5f2e71.png
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/3c6c50508e2411873e8aec04b9b0d0b026227dad.png
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/3fd88e5561f4bce2bf17dc50624a4756051bf38a.png
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/413f8a8e40062a9090d9d50b88bc7b551b314c26.png
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/44a53fd8bbb2f72416882129ccc4cf64e49fc3df.png
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/44b79d2c935cf226fc2707938207c023c1351cb0.png
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/496867ca68c428fa123f26f0f73997632e61e116.png
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/4fbce1d9d579dd5c678c54ab9967433263dbeaa2.png
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5183ea9096ac86aff6e13dd3d4389ae47617b059.png
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5247131b3b1b9cc457d29a9b08a19c2062ed3d16.png
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/532f3248d6552e7ac6b785bd935f404ad593e6a9.png
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5635a7c34414599c2452d72430811e816b460335.png
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/56e23ea8dd42fdbfc2b216f54b730114ec8acfd8.png
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/59dc9a44d175aae008c18691b9f662270e36ef5d.png
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5a53aff7886e588bf17ff209a8fa05351cda8798.png
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5a939c5280da7202ca4531f175a7780ad5e1f80a.png
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5aa339d4daf45a810dda332e3c80a0698e526e04.png
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5bd39cc00b680a56dad487c2aa31394db3e90140.png
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5d5ac3af39ca1a97abbb4a0deccbb8c64a72d831.png
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5df994acd5cadc81c38f1a28e4ea3f8281b6c4cb.png
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5fa6513bef00e529069be708641fcce5a1535803.png
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/5faf686e0e8426c21ae030d783d5624321d18476.png
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/60b74287bf19e27bc5a3e755457326add30fc669.png
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/625e23c6d74cc842c0521cce76baa0d254b52926.png
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/66343a54ffb585a31a82fe441ee9fc3cd8eb4368.png
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/66b30555c6212f4bfbe96c9a9dfceb59d818aef6.png
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/6996f78ce1c5e71c67956260100a4a672b511de5.png
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/6b21e0b0899a0d2879d3b8019087fa630bab4ea2.png
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/6f63a2c6be03f660db3b46fdb09e3e5bbc9c0b83.png
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/717a514d7c39628ccc8ab9dc5b3b822017d413fc.png
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/71a383cae1bb3f6d73faeea9e3241486d863dbc9.png
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/7358fb1b6031c815b8f99086409882bf1980148f.png
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/774df2c68904c92b7c0db636d12ca2ca6ee21263.png
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/775308689ec82d24ee08490a702181d1ccbe59d8.png
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/78eabc361f3a54daeed501fff0d3353b946504ae.png
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/79a3d439d28652c547386f39b555d90d3aaf102d.png
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/7c4a5c45c86c3c6a4b3d73c5a58b549b14d201df.png
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/86ec1edb070ffe9216097a80189ee3434c9b5f20.png
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/879aee5829f6469733f819b01853c5205ecc88b6.png
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/889fc7f9c8e35e08413407d53c89909849345138.png
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/8968e4fd6ebe2d668010ed37e2172340daaefa2d.png
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/89bf47a4edaa04f32146a8079e6564a0146d6c92.png
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/8ec4bad22a4dd149e5658ab17c4358b3dbc8dc1e.png
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/8f3c6b529aaa515fdbc6c51b4fc4f73293dbfc09.png
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/9172efc523d7488d4c3ed299d0be813de01503b8.png
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/953bde2ab2fca30897f66185e5b37b73747b8b46.png
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/95cd8c0e712982ebb308efa59408cf9962067b3c.png
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/9630132210b904754c9ab272b61cb527d12263ca.png
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/97c27bd34a0b3f4f9b760f06500e50eb3e4b75f1.png
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/97db043c7cba573ac389b71add78b048077e8a13.png
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/99caa835285abdbc99536106ff1d075a870c2650.png
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/9c175e2552d4e2d9c682055a2ce7d1fbb538116d.png
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/9d2e3563d506091cb1a66a8405841ef4728fbd43.png
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/a25e560325b732d03aa5e9a69521f2bfa67e5f4e.png
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/a581f053bbfa5115f42c13094857cdd12a37ec49.png
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/a6c088a730612710750ee31f9cc780d5f94f9989.png
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/a9bb86de6492860286fd9038b2070f5870e63cb6.png
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/abdaecd41a1558846f03b71ab3d99436de6faf0d.png
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ac5b8bd01421ff3a8f1a464013ce05b7a4373141.png
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/b16ff7ad79d632da6d242820aa5676c989057de9.png
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/b1eee4055960efed015bee32bb3353501988dadd.png
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/b4111b2fd8976378ce69e158f8d25467da391510.png
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/b7fdf13f2e4d24f9f2d55a77dcebbf52c8ad19c7.png
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/b851d3a5fb872ad82d61f964772ca1cc2520a590.png
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/b988975be41fd13b4d091c10202ba19374643586.png
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ba11027b67a5958f16fb1495fba3b5fb7eadcaee.png
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ba1dc665bd30a53d02b5a623c6c1b7f3a52a3bff.png
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/c279824074ed8acc9cd963e930735f542462edec.png
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/c833e66a1aa68dba7be89cbcaed7e749967ab5c9.png
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/c9c2aeea32459ab854f099f25fd5310801d90ab2.png
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/cb5448c62c69431617901ff76ecf95172e07d606.png
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/cce73c20b14f5d57454e0ad66f02dd004d949e0c.png
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/cfca9af3a86afde1b9efe235bfc3e48f90890d82.png
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/d0081e53ec3772333006e7b8b488993ff712fe36.png
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/d188c978e0d95e667be9c33955b35c80ec4c786f.png
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/d32c78b759903e3f4bd4fd2ce0b86358f7500c5d.png
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/da96c58cf8c1bcc132a2252a23859c4ceaadf9f9.png
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/dbc4c429b48dd94e41ee866e1edbf0abededae3a.png
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/de47a77e2e05505f7581a4dcf8ae4f7750fe53ad.png
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/de784b45b336cd590561fbd176b9b0a250440e72.png
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/df0deb143e5ac127f00bd248ee8001ecae572adc.png
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e030043610306028604a08f8ced75f5cd780b96c.png
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e11f2701c4a39c7fe543a6c4150b421d50f1c159.png
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e1aaac0305e1b00c3c08173dd3e8402b6320c110.png
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e37b8a88ae16543f49591bf090bf9bd2fe5088da.png
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e3fc28292267f066fee7718c64f4bbfece521f24.png
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e7ab49f222c2489a65240601adcf9cc994535f01.png
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e8c0d853d9741d1d80356648c449808dd3fdeb3c.png
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/e9203da50e1059455123460d4e716c9c7f440cc3.png
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/eaa6ad49a7f78fe5a13b486690163bf2dc7e3e60.png
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/eda67b6e5103620f15dda4926fbd244c38024373.png
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ee29958a93bd815ef9f3e2508e54fa1871d0d111.png
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ee3eabc3b00202e0691a94570f869fa53a66c04d.png
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ee97899107420cf7a24b2532c2c7c09a023be431.png
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/eec83a497511513e0bfa38139255e53b02d0bd21.png
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/f02d0c0a7c4871d2d796585dcb779de3a8861f9b.png
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/f0d949c29370cd898ed70f8f32a09349764a1ebb.png
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/f761880e192d4bc7f9a3b7c5b0c495177b219bba.png
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/f7d483a2293790337ad1ba440b6430f82ad420d6.png
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/f81750957860f8838122955a5d011e73e7962d55.png
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/fa34489cf430b7630b30f28b2eb050e2489e3523.png
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/fcd0c45a70da7d2399b3fb666759b02c5edd251e.png
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/math/ff90a5f025d9fd305aac19c8dd64fa15f0c789a1.png
--rw-r--r--   0 runner    (1001) docker     (121)    36756 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_images/matminer_logo_small.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.513413 matminer-0.8.0/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (121)    15182 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/changelog.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/contributions.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/contributors.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10986 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/dataset_addition_guide.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)   148796 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/dataset_summary.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/example_bulkmod.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15477 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/featurizer_summary.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14983 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/installation.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.data_retrieval.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.data_retrieval.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.datasets.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.datasets.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.composition.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.composition.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.site.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.site.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.structure.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.structure.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.featurizers.utils.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.figrecipes.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.figrecipes.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.utils.data_files.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/matminer.utils.tests.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_sources/modules.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.525412 matminer-0.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   267829 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/Flowchart.png
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (121)    14810 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (121)  2486665 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/bulk_shear_moduli.html
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/comment-bright.png
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/comment-close.png
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/comment.png
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/down-pressed.png
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/down.png
--rw-r--r--   0 runner    (1001) docker     (121)   233051 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/example_bulkmod.png
--rw-r--r--   0 runner    (1001) docker     (121)   201518 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/example_bulkmod_feats.png
--rw-r--r--   0 runner    (1001) docker     (121)   116774 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/example_bulkmod_rf.png
--rw-r--r--   0 runner    (1001) docker     (121)   116774 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/examples_bulkmod_rf.png
--rw-r--r--   0 runner    (1001) docker     (121)   453119 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/featurizer_diagram.png
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (121)   263767 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/jquery-3.1.0.js
--rw-r--r--   0 runner    (1001) docker     (121)   268039 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/jquery-3.2.1.js
--rw-r--r--   0 runner    (1001) docker     (121)   287630 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (121)   288580 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (121)    89501 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (121)    36756 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/matminer_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (121)     4498 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/nature.css
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (121)    18215 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (121)     4712 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (121)    68420 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (121)    35168 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/underscore-1.3.1.js
--rw-r--r--   0 runner    (1001) docker     (121)    19530 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/underscore.js
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/up-pressed.png
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/up.png
--rw-r--r--   0 runner    (1001) docker     (121)    25355 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/_static/websupport.js
--rw-r--r--   0 runner    (1001) docker     (121)    24995 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/changelog.html
--rw-r--r--   0 runner    (1001) docker     (121)     6918 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/contributors.html
--rw-r--r--   0 runner    (1001) docker     (121)    26513 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/dataset_addition_guide.html
--rw-r--r--   0 runner    (1001) docker     (121)   229099 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/dataset_summary.html
--rw-r--r--   0 runner    (1001) docker     (121)    42193 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/example_bulkmod.html
--rw-r--r--   0 runner    (1001) docker     (121)    42827 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/featurizer_summary.html
--rw-r--r--   0 runner    (1001) docker     (121)   268477 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (121)    29760 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     7892 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/installation.html
--rw-r--r--   0 runner    (1001) docker     (121)    95405 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.data_retrieval.html
--rw-r--r--   0 runner    (1001) docker     (121)    27745 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.data_retrieval.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)    79126 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.datasets.html
--rw-r--r--   0 runner    (1001) docker     (121)    52354 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.datasets.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)   183284 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.composition.html
--rw-r--r--   0 runner    (1001) docker     (121)    39470 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.composition.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)   395510 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.html
--rw-r--r--   0 runner    (1001) docker     (121)   202396 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.site.html
--rw-r--r--   0 runner    (1001) docker     (121)    33386 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.site.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)   250624 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.structure.html
--rw-r--r--   0 runner    (1001) docker     (121)    45631 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.structure.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)    86307 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)    57345 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.utils.html
--rw-r--r--   0 runner    (1001) docker     (121)    23048 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.featurizers.utils.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.figrecipes.html
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.figrecipes.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)    96941 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.html
--rw-r--r--   0 runner    (1001) docker     (121)     5066 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.utils.data_files.html
--rw-r--r--   0 runner    (1001) docker     (121)    81617 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.utils.html
--rw-r--r--   0 runner    (1001) docker     (121)    33144 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/matminer.utils.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)     9827 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/modules.html
--rw-r--r--   0 runner    (1001) docker     (121)     9129 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)    33944 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (121)     3601 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (121)   366517 2022-11-11 00:13:13.000000 matminer-0.8.0/docs/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.525412 matminer-0.8.0/docs_rst/
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.533413 matminer-0.8.0/docs_rst/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   267829 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/Flowchart.png
--rw-r--r--   0 runner    (1001) docker     (121)  2486665 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/bulk_shear_moduli.html
--rw-r--r--   0 runner    (1001) docker     (121)   233051 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/example_bulkmod.png
--rw-r--r--   0 runner    (1001) docker     (121)   201518 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/example_bulkmod_feats.png
--rw-r--r--   0 runner    (1001) docker     (121)   116774 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/example_bulkmod_rf.png
--rw-r--r--   0 runner    (1001) docker     (121)   453119 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/featurizer_diagram.png
--rw-r--r--   0 runner    (1001) docker     (121)    36756 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/matminer_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (121)     4498 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_static/nature.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.533413 matminer-0.8.0/docs_rst/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)    15182 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9740 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10986 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/dataset_addition_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3230 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)   148796 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/dataset_summary.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/example_bulkmod.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5201 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/featurizer_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)    15477 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/featurizer_summary.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14983 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.data_retrieval.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.data_retrieval.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.datasets.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.datasets.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.composition.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.composition.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.site.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.site.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.structure.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.structure.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.featurizers.utils.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.figrecipes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.figrecipes.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.rst
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.utils.data_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/matminer.utils.tests.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-11 00:13:13.000000 matminer-0.8.0/docs_rst/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.533413 matminer-0.8.0/matminer/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.533413 matminer-0.8.0/matminer/data_retrieval/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9965 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_AFLOW.py
--rw-r--r--   0 runner    (1001) docker     (121)    13425 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_Citrine.py
--rw-r--r--   0 runner    (1001) docker     (121)     6877 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_MDF.py
--rw-r--r--   0 runner    (1001) docker     (121)     7041 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_MP.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10997 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_MPDS.py
--rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_MongoDB.py
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/retrieve_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.537413 matminer-0.8.0/matminer/data_retrieval/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_AFLOW.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_Citrine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MDF.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MP.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1377 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MPDS.py
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MongoDB.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.537413 matminer-0.8.0/matminer/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17143 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/convenience_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)   141785 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/dataset_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)     8164 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/dataset_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.537413 matminer-0.8.0/matminer/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/tests/test_convenience_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/tests/test_dataset_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (121)    21391 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6139 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.541413 matminer-0.8.0/matminer/featurizers/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12036 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (121)    30183 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.541413 matminer-0.8.0/matminer/featurizers/composition/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36872 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/alloy.py
--rw-r--r--   0 runner    (1001) docker     (121)    13074 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     7359 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/element.py
--rw-r--r--   0 runner    (1001) docker     (121)    14825 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/ion.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/orbital.py
--rw-r--r--   0 runner    (1001) docker     (121)    13096 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/packing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.541413 matminer-0.8.0/matminer/featurizers/composition/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9232 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_alloy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4755 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     3432 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_ion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_orbital.py
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5857 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/composition/thermo.py
--rw-r--r--   0 runner    (1001) docker     (121)    28685 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    27361 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/dos.py
--rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.545413 matminer-0.8.0/matminer/featurizers/site/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11557 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/bonding.py
--rw-r--r--   0 runner    (1001) docker     (121)    20936 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/chemical.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/cn_target_motif_op.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8299 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/external.py
--rw-r--r--   0 runner    (1001) docker     (121)    35232 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (121)    17259 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    20515 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.545413 matminer-0.8.0/matminer/featurizers/site/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/test_bonding.py
--rw-r--r--   0 runner    (1001) docker     (121)     5933 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/test_chemical.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/test_external.py
--rw-r--r--   0 runner    (1001) docker     (121)    13829 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/test_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7684 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/site/tests/test_rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.545413 matminer-0.8.0/matminer/featurizers/structure/
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    50941 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/bonding.py
--rw-r--r--   0 runner    (1001) docker     (121)    24060 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/composite.py
--rw-r--r--   0 runner    (1001) docker     (121)    18703 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10379 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/order.py
--rw-r--r--   0 runner    (1001) docker     (121)    13895 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    13990 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/sites.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.545413 matminer-0.8.0/matminer/featurizers/structure/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/Cs2CeN5O17_mp-1198000_computed.cif
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/Dy2HfS5_mp-1198001_computed.cif
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/JarvisCFID_problem_file.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_bonding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     9775 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/structure/tests/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.549413 matminer-0.8.0/matminer/featurizers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    80462 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/VBr2_971787_bandstructure.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   159299 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/nb3sn_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)    28605 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/si_bandstructure_line.json
--rw-r--r--   0 runner    (1001) docker     (121)   996960 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/si_bandstructure_uniform.json
--rw-r--r--   0 runner    (1001) docker     (121)   108978 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/si_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/si_structure.json
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/test_bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (121)    20996 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14230 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/test_dos.py
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/tests/test_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.549413 matminer-0.8.0/matminer/featurizers/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5119 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/grdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/oxidation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11384 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.549413 matminer-0.8.0/matminer/featurizers/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/tests/test_grdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/tests/test_oxidation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/featurizers/utils/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.549413 matminer-0.8.0/matminer/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)    20920 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.553413 matminer-0.8.0/matminer/utils/data_files/
--rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/Miedema.csv
--rw-r--r--   0 runner    (1001) docker     (121)    29088 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/MiedemaLiquidDeltaHf.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    94450 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/bvparm2016.cif
--rw-r--r--   0 runner    (1001) docker     (121)    96339 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/bvparm2020.cif
--rw-r--r--   0 runner    (1001) docker     (121)    28392 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/cgcnn_atom_feature.json
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/cohesive_energies.json
--rw-r--r--   0 runner    (1001) docker     (121)    41715 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/deml_elementdata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.553413 matminer-0.8.0/matminer/utils/data_files/jarvis/
--rw-r--r--   0 runner    (1001) docker     (121)  1162701 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/jarvis/element_charges.json
--rw-r--r--   0 runner    (1001) docker     (121)  1515058 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/jarvis/element_chem.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.561413 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AllenElectronegativity.table
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AtomicRadius.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     2054 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AtomicVolume.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     1132 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AtomicWeight.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      624 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/BoilingT.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      893 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/BulkModulus.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      603 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Column.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      807 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/CovalentRadius.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      943 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Density.table
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/DipolePolarizability.table
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ElectronAffinity.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      870 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Electronegativity.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      851 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/FirstIonizationEnergy.table
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/FusionEnthalpy.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      636 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSbandgap.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     1696 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSenergy_pa.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     1337 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSestBCClatcnt.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     1337 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSestFCClatcnt.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      842 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSmagmom.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     1133 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSvolume_pa.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      794 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HHIp.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      792 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HHIr.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      716 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMass.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      737 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMolar.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      655 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatFusion.table
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatVaporization.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      669 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ICSDVolume.table
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IonizationEnergies.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IsAlkali.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IsDBlock.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IsFBlock.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IsMetal.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IsMetalloid.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IsNonmetal.table
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/LogThermalConductivity.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      958 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MeltingT.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      694 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MendeleevNumber.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      523 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MiracleRadius.table
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MolarVolume.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      568 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NUnfilled.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      618 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NValence.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NdUnfilled.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      587 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NdValence.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      566 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NfUnfilled.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      596 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NfValence.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NpUnfilled.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NpValence.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NsUnfilled.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NsValence.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      676 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Number.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      528 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/OxidationStates.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      617 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Polarizability.table
--rwxr-xr-x   0 runner    (1001) docker     (121)     8892 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      560 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Row.table
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/SecondIonizationEnergy.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      899 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ShearModulus.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      858 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/SpaceGroupNumber.table
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ThermalConductivity.table
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/VdWRadius.table
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_d.table
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_p.table
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_pi.table
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_s.table
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_sigma.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      939 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/n_ws^third.table
--rwxr-xr-x   0 runner    (1001) docker     (121)      912 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/phi.table
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/magpie_elementdata_feature_descriptions.txt
--rw-r--r--   0 runner    (1001) docker     (121)   449163 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/matscholar_els.json
--rw-r--r--   0 runner    (1001) docker     (121)    39056 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/data_files/megnet_elemental_embedding.json
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/flatten_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/kernels.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.561413 matminer-0.8.0/matminer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/dataframe.json
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/dataframe.json.bz2
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/test_flatten_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-11 00:13:13.000000 matminer-0.8.0/matminer/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.533413 matminer-0.8.0/matminer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-11-11 00:18:39.000000 matminer-0.8.0/matminer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25556 2022-11-11 00:18:39.000000 matminer-0.8.0/matminer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 00:18:39.000000 matminer-0.8.0/matminer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 00:18:27.000000 matminer-0.8.0/matminer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-11 00:18:39.000000 matminer-0.8.0/matminer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-11 00:18:39.000000 matminer-0.8.0/matminer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17848 2022-11-11 00:13:13.000000 matminer-0.8.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-11 00:13:13.000000 matminer-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 00:18:39.561413 matminer-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6451 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6198 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6452 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6345 2022-11-11 00:13:13.000000 matminer-0.8.0/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-11-11 00:18:39.565413 matminer-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2022-11-11 00:13:13.000000 matminer-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2022-11-11 00:13:13.000000 matminer-0.8.0/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.763196 matminer-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.659188 matminer-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 15:37:48.000000 matminer-0.9.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 15:37:48.000000 matminer-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.659188 matminer-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-27 15:37:48.000000 matminer-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-27 15:37:48.000000 matminer-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-27 15:37:48.000000 matminer-0.9.0/.github/workflows/upgrade-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-27 15:37:48.000000 matminer-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-27 15:37:48.000000 matminer-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 15:37:48.000000 matminer-0.9.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-27 15:37:48.000000 matminer-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)   111284 2023-06-27 15:37:48.000000 matminer-0.9.0/Flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-27 15:37:48.000000 matminer-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-27 15:37:48.000000 matminer-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-27 15:44:39.763196 matminer-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-06-27 15:37:48.000000 matminer-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.651188 matminer-0.9.0/dev_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.659188 matminer-0.9.0/dev_scripts/dataset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-27 15:37:48.000000 matminer-0.9.0/dev_scripts/dataset_management/generate_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-27 15:37:48.000000 matminer-0.9.0/dev_scripts/dataset_management/modify_dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56843 2023-06-27 15:37:48.000000 matminer-0.9.0/dev_scripts/dataset_management/prep_dataset_for_figshare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.667189 matminer-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.671189 matminer-0.9.0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   267829 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/Flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)   233051 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/example_bulkmod.png
+-rw-r--r--   0 runner    (1001) docker     (123)   201518 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/example_bulkmod_feats.png
+-rw-r--r--   0 runner    (1001) docker     (123)   116774 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/example_bulkmod_rf.png
+-rw-r--r--   0 runner    (1001) docker     (123)   453119 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/featurizer_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.691191 matminer-0.9.0/docs/_images/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/01caff91ea974c5cc0c133c5b4a560d433ff589b.png
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/0239bb38c93a6213c5ac6ba1dabd3e0a003ed371.png
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/02d98909b5d6acd6a7ff927d4d42790bdd407d58.png
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/045fae7cfacaf28d29d6bdb81ab5ef61b1b07808.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/0467e0003559a763cbcd16dcd0bf3c33f9c65901.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/06dfe124bb57b08106d4043aea4218b309454d8d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/074903764bb5a464b7c346e84f43cba2174f3ab0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/079ba1f3373823268ba0e33b400423434ca7c0a6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/083b5d48a524b6f7a39570bbe0d51d474cb588e6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/08e21b3be44ad4aac8ed231afc369152e9c8539c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/0b21f31621e4f0f2b3b5faa10af80dc999f9ffdf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/0b7c1e16a3a8a849bb8ffdcdbf86f65fd1f30438.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/0c9c2dac2bd7f86735f42ef4184918c37425d67a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/0ee4480fa3fe2856c28f74b0aa03fde5e83cfb0a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/12249dbb3a129598bfef9a4f490147c6a4537213.png
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/182c7d0771b253a55441383d191fce92f3d58e02.png
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/18711f8217158b267749b882e02ef2f9f17431c0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/18a48ac390a7070c05a265edbfa13f1322d47daf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/18f11bbc89febc978169289978481f64a403be7e.png
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/192c5eb5f76c194be10ed549a12e8cae7e9f4e37.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/1947a1c371cf018ebfcdf1fee66dacce40b9ab4c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/1b1fd12d69ea533588e033d255888cb6a17cdca6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/1c7982e9bed52596de46d839a5334f537de1c35d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/1ebe654cc7b8f2a0d8100aa5825cf2b9021adbbc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/1fbee781f84569077719a167b64e12064360fac1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/20380591afec1e5625f65892e5af51719381bf91.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/22a57909899e26fbb172500446c43f2ba7ebd563.png
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/240509feeacaad2b6744f49f69502b84f78f1fef.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/298204ab1b85022412ad261503dcab8bd14fb321.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2aa528e29c4df6e3a7e44783f02f45e46012b948.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2c79776b8b888d73f48a6a996815a078713a2a78.png
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2ede365ad144ab396916ec60458da03860803078.png
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2fc0510f783f8ce42baa1c4ac6b86d94a6382093.png
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2fe13d18c90531495ad5a8b7976e2a7bda67ae7e.png
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2fe6d1d220a6eb68148f55432fd2234ca529685c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/2ff684758d53878ad22e0ebaa7f34d709cc1b6a4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/30634b08f5df289a7acab4963cb6a3e6b99aba0f.png
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/30d9a509980f1622c5d182d9b846afd31019bb05.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/31880c4812286affe8e1e36fce7bdc56e8e28458.png
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/31fdf41b39df23c95e52c5aef07f59d9adf82f3c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/326c6fcc3609b0c2183f6a9e23d4aa1d4b141ea2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/35bab58b40a77a2e24ecb9f58898f1813de64459.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/3af01b3f850c53aa06a7ef9878392efada5f2e71.png
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/3c6c50508e2411873e8aec04b9b0d0b026227dad.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/3fd88e5561f4bce2bf17dc50624a4756051bf38a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/413f8a8e40062a9090d9d50b88bc7b551b314c26.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/44a53fd8bbb2f72416882129ccc4cf64e49fc3df.png
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/44b79d2c935cf226fc2707938207c023c1351cb0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/496867ca68c428fa123f26f0f73997632e61e116.png
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/4fbce1d9d579dd5c678c54ab9967433263dbeaa2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5183ea9096ac86aff6e13dd3d4389ae47617b059.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5247131b3b1b9cc457d29a9b08a19c2062ed3d16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/532f3248d6552e7ac6b785bd935f404ad593e6a9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5635a7c34414599c2452d72430811e816b460335.png
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/56e23ea8dd42fdbfc2b216f54b730114ec8acfd8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/59dc9a44d175aae008c18691b9f662270e36ef5d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5a53aff7886e588bf17ff209a8fa05351cda8798.png
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5a939c5280da7202ca4531f175a7780ad5e1f80a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5aa339d4daf45a810dda332e3c80a0698e526e04.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5bd39cc00b680a56dad487c2aa31394db3e90140.png
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5d5ac3af39ca1a97abbb4a0deccbb8c64a72d831.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5df994acd5cadc81c38f1a28e4ea3f8281b6c4cb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5fa6513bef00e529069be708641fcce5a1535803.png
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/5faf686e0e8426c21ae030d783d5624321d18476.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/60b74287bf19e27bc5a3e755457326add30fc669.png
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/625e23c6d74cc842c0521cce76baa0d254b52926.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/66343a54ffb585a31a82fe441ee9fc3cd8eb4368.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/66b30555c6212f4bfbe96c9a9dfceb59d818aef6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/6996f78ce1c5e71c67956260100a4a672b511de5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/6b21e0b0899a0d2879d3b8019087fa630bab4ea2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/6f63a2c6be03f660db3b46fdb09e3e5bbc9c0b83.png
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/717a514d7c39628ccc8ab9dc5b3b822017d413fc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/71a383cae1bb3f6d73faeea9e3241486d863dbc9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/7358fb1b6031c815b8f99086409882bf1980148f.png
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/774df2c68904c92b7c0db636d12ca2ca6ee21263.png
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/775308689ec82d24ee08490a702181d1ccbe59d8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/78eabc361f3a54daeed501fff0d3353b946504ae.png
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/79a3d439d28652c547386f39b555d90d3aaf102d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/7c4a5c45c86c3c6a4b3d73c5a58b549b14d201df.png
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/86ec1edb070ffe9216097a80189ee3434c9b5f20.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/879aee5829f6469733f819b01853c5205ecc88b6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/889fc7f9c8e35e08413407d53c89909849345138.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/8968e4fd6ebe2d668010ed37e2172340daaefa2d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/89bf47a4edaa04f32146a8079e6564a0146d6c92.png
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/8ec4bad22a4dd149e5658ab17c4358b3dbc8dc1e.png
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/8f3c6b529aaa515fdbc6c51b4fc4f73293dbfc09.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/9172efc523d7488d4c3ed299d0be813de01503b8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/953bde2ab2fca30897f66185e5b37b73747b8b46.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/95cd8c0e712982ebb308efa59408cf9962067b3c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/9630132210b904754c9ab272b61cb527d12263ca.png
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/97c27bd34a0b3f4f9b760f06500e50eb3e4b75f1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/97db043c7cba573ac389b71add78b048077e8a13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/99caa835285abdbc99536106ff1d075a870c2650.png
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/9c175e2552d4e2d9c682055a2ce7d1fbb538116d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/9d2e3563d506091cb1a66a8405841ef4728fbd43.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/a25e560325b732d03aa5e9a69521f2bfa67e5f4e.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/a581f053bbfa5115f42c13094857cdd12a37ec49.png
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/a6c088a730612710750ee31f9cc780d5f94f9989.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/a9bb86de6492860286fd9038b2070f5870e63cb6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/abdaecd41a1558846f03b71ab3d99436de6faf0d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ac5b8bd01421ff3a8f1a464013ce05b7a4373141.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/b16ff7ad79d632da6d242820aa5676c989057de9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/b1eee4055960efed015bee32bb3353501988dadd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/b4111b2fd8976378ce69e158f8d25467da391510.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/b7fdf13f2e4d24f9f2d55a77dcebbf52c8ad19c7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/b851d3a5fb872ad82d61f964772ca1cc2520a590.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/b988975be41fd13b4d091c10202ba19374643586.png
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ba11027b67a5958f16fb1495fba3b5fb7eadcaee.png
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ba1dc665bd30a53d02b5a623c6c1b7f3a52a3bff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/c279824074ed8acc9cd963e930735f542462edec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/c833e66a1aa68dba7be89cbcaed7e749967ab5c9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/c9c2aeea32459ab854f099f25fd5310801d90ab2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/cb5448c62c69431617901ff76ecf95172e07d606.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/cce73c20b14f5d57454e0ad66f02dd004d949e0c.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/cfca9af3a86afde1b9efe235bfc3e48f90890d82.png
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/d0081e53ec3772333006e7b8b488993ff712fe36.png
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/d188c978e0d95e667be9c33955b35c80ec4c786f.png
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/d32c78b759903e3f4bd4fd2ce0b86358f7500c5d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/da96c58cf8c1bcc132a2252a23859c4ceaadf9f9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/dbc4c429b48dd94e41ee866e1edbf0abededae3a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/de47a77e2e05505f7581a4dcf8ae4f7750fe53ad.png
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/de784b45b336cd590561fbd176b9b0a250440e72.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/df0deb143e5ac127f00bd248ee8001ecae572adc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e030043610306028604a08f8ced75f5cd780b96c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e11f2701c4a39c7fe543a6c4150b421d50f1c159.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e1aaac0305e1b00c3c08173dd3e8402b6320c110.png
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e37b8a88ae16543f49591bf090bf9bd2fe5088da.png
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e3fc28292267f066fee7718c64f4bbfece521f24.png
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e7ab49f222c2489a65240601adcf9cc994535f01.png
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e8c0d853d9741d1d80356648c449808dd3fdeb3c.png
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/e9203da50e1059455123460d4e716c9c7f440cc3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/eaa6ad49a7f78fe5a13b486690163bf2dc7e3e60.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/eda67b6e5103620f15dda4926fbd244c38024373.png
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ee29958a93bd815ef9f3e2508e54fa1871d0d111.png
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ee3eabc3b00202e0691a94570f869fa53a66c04d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ee97899107420cf7a24b2532c2c7c09a023be431.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/eec83a497511513e0bfa38139255e53b02d0bd21.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/f02d0c0a7c4871d2d796585dcb779de3a8861f9b.png
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/f0d949c29370cd898ed70f8f32a09349764a1ebb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/f761880e192d4bc7f9a3b7c5b0c495177b219bba.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/f7d483a2293790337ad1ba440b6430f82ad420d6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/f81750957860f8838122955a5d011e73e7962d55.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/fa34489cf430b7630b30f28b2eb050e2489e3523.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/fcd0c45a70da7d2399b3fb666759b02c5edd251e.png
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/math/ff90a5f025d9fd305aac19c8dd64fa15f0c789a1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36756 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_images/matminer_logo_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.695191 matminer-0.9.0/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/contributions.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/contributors.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/dataset_addition_guide.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   148796 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/dataset_summary.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/example_bulkmod.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/featurizer_summary.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/installation.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.data_retrieval.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.data_retrieval.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.datasets.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.datasets.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.composition.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.composition.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.site.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.site.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.structure.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.structure.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.featurizers.utils.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.figrecipes.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.figrecipes.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.utils.data_files.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/matminer.utils.tests.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_sources/modules.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.711192 matminer-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   267829 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/Flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)  2486665 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/bulk_shear_moduli.html
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/comment-bright.png
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/comment-close.png
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/comment.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/down-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)   233051 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/example_bulkmod.png
+-rw-r--r--   0 runner    (1001) docker     (123)   201518 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/example_bulkmod_feats.png
+-rw-r--r--   0 runner    (1001) docker     (123)   116774 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/example_bulkmod_rf.png
+-rw-r--r--   0 runner    (1001) docker     (123)   116774 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/examples_bulkmod_rf.png
+-rw-r--r--   0 runner    (1001) docker     (123)   453119 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/featurizer_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)   263767 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/jquery-3.1.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   268039 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/jquery-3.2.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   287630 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36756 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/matminer_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/nature.css
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/underscore-1.3.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/underscore.js
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/up-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/up.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25355 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/_static/websupport.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24995 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/changelog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/contributors.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26513 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/dataset_addition_guide.html
+-rw-r--r--   0 runner    (1001) docker     (123)   229099 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/dataset_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42193 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/example_bulkmod.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42827 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/featurizer_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)   268477 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29760 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/installation.html
+-rw-r--r--   0 runner    (1001) docker     (123)    95405 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.data_retrieval.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.data_retrieval.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)    79126 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.datasets.html
+-rw-r--r--   0 runner    (1001) docker     (123)    52354 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.datasets.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)   183284 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.composition.html
+-rw-r--r--   0 runner    (1001) docker     (123)    39470 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.composition.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)   395510 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.html
+-rw-r--r--   0 runner    (1001) docker     (123)   202396 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.site.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33386 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.site.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)   250624 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.structure.html
+-rw-r--r--   0 runner    (1001) docker     (123)    45631 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.structure.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)    86307 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)    57345 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.featurizers.utils.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.figrecipes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.figrecipes.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)    96929 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.utils.data_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)    81617 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/matminer.utils.tests.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/modules.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)   366514 2023-06-27 15:37:48.000000 matminer-0.9.0/docs/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.715193 matminer-0.9.0/docs_rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.719193 matminer-0.9.0/docs_rst/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   267829 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/Flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2486665 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/bulk_shear_moduli.html
+-rw-r--r--   0 runner    (1001) docker     (123)   233051 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/example_bulkmod.png
+-rw-r--r--   0 runner    (1001) docker     (123)   201518 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/example_bulkmod_feats.png
+-rw-r--r--   0 runner    (1001) docker     (123)   116774 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/example_bulkmod_rf.png
+-rw-r--r--   0 runner    (1001) docker     (123)   453119 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/featurizer_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36756 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/matminer_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_static/nature.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.719193 matminer-0.9.0/docs_rst/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/dataset_addition_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148796 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/dataset_summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/example_bulkmod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/featurizer_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/featurizer_summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.data_retrieval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.data_retrieval.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.datasets.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.composition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.composition.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.site.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.site.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.structure.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.featurizers.utils.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.figrecipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.figrecipes.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.utils.data_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/matminer.utils.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 15:37:48.000000 matminer-0.9.0/docs_rst/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.719193 matminer-0.9.0/matminer/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.723193 matminer-0.9.0/matminer/data_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_AFLOW.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_Citrine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_MDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_MP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10997 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_MPDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_MongoDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/retrieve_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.723193 matminer-0.9.0/matminer/data_retrieval/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_AFLOW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_Citrine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MPDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MongoDB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.727193 matminer-0.9.0/matminer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/convenience_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141785 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/dataset_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/dataset_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.727193 matminer-0.9.0/matminer/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/tests/test_convenience_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/tests/test_dataset_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21371 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.727193 matminer-0.9.0/matminer/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30610 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.731194 matminer-0.9.0/matminer/featurizers/composition/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36872 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/alloy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/ion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/orbital.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/packing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.731194 matminer-0.9.0/matminer/featurizers/composition/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_alloy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_ion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/composition/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28767 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.731194 matminer-0.9.0/matminer/featurizers/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/chemical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/cn_target_motif_op.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20509 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.735194 matminer-0.9.0/matminer/featurizers/site/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/test_bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/test_chemical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/test_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/site/tests/test_rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.735194 matminer-0.9.0/matminer/featurizers/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50939 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.735194 matminer-0.9.0/matminer/featurizers/structure/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/Cs2CeN5O17_mp-1198000_computed.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/Dy2HfS5_mp-1198001_computed.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/JarvisCFID_problem_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/structure/tests/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.739194 matminer-0.9.0/matminer/featurizers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    80462 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/VBr2_971787_bandstructure.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159299 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/nb3sn_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28605 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/si_bandstructure_line.json
+-rw-r--r--   0 runner    (1001) docker     (123)   996960 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/si_bandstructure_uniform.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108978 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/si_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/si_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/test_bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20995 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/test_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/tests/test_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.739194 matminer-0.9.0/matminer/featurizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/grdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.743195 matminer-0.9.0/matminer/featurizers/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/tests/test_grdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/tests/test_oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/featurizers/utils/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.743195 matminer-0.9.0/matminer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.747195 matminer-0.9.0/matminer/utils/data_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/Miedema.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29088 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/MiedemaLiquidDeltaHf.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94450 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/bvparm2016.cif
+-rw-r--r--   0 runner    (1001) docker     (123)    96339 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/bvparm2020.cif
+-rw-r--r--   0 runner    (1001) docker     (123)    28392 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/cgcnn_atom_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/cohesive_energies.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41715 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/deml_elementdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.747195 matminer-0.9.0/matminer/utils/data_files/jarvis/
+-rw-r--r--   0 runner    (1001) docker     (123)  1162701 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/jarvis/element_charges.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1515058 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/jarvis/element_chem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.759196 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AllenElectronegativity.table
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AtomicRadius.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2054 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AtomicVolume.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AtomicWeight.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/BoilingT.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/BulkModulus.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Column.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/CovalentRadius.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Density.table
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/DipolePolarizability.table
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ElectronAffinity.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      870 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Electronegativity.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/FirstIonizationEnergy.table
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/FusionEnthalpy.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSbandgap.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1696 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSenergy_pa.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSestBCClatcnt.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSestFCClatcnt.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSmagmom.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSvolume_pa.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HHIp.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HHIr.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMass.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMolar.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatFusion.table
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatVaporization.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ICSDVolume.table
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IonizationEnergies.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IsAlkali.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IsDBlock.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IsFBlock.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IsMetal.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IsMetalloid.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IsNonmetal.table
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/LogThermalConductivity.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MeltingT.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MendeleevNumber.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MiracleRadius.table
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MolarVolume.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NUnfilled.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NValence.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NdUnfilled.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NdValence.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NfUnfilled.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NfValence.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NpUnfilled.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NpValence.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NsUnfilled.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NsValence.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Number.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/OxidationStates.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Polarizability.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8892 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Row.table
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/SecondIonizationEnergy.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ShearModulus.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/SpaceGroupNumber.table
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ThermalConductivity.table
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/VdWRadius.table
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_d.table
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_p.table
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_pi.table
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_s.table
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_sigma.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      939 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/n_ws^third.table
+-rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/phi.table
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/magpie_elementdata_feature_descriptions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   449163 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/matscholar_els.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39056 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/data_files/megnet_elemental_embedding.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/flatten_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.759196 matminer-0.9.0/matminer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/dataframe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/dataframe.json.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/test_flatten_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-27 15:37:48.000000 matminer-0.9.0/matminer/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.723193 matminer-0.9.0/matminer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-27 15:44:39.000000 matminer-0.9.0/matminer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25547 2023-06-27 15:44:39.000000 matminer-0.9.0/matminer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:44:39.000000 matminer-0.9.0/matminer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:44:25.000000 matminer-0.9.0/matminer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-27 15:44:39.000000 matminer-0.9.0/matminer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 15:44:39.000000 matminer-0.9.0/matminer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-27 15:37:48.000000 matminer-0.9.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 15:37:48.000000 matminer-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:39.763196 matminer-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-27 15:37:48.000000 matminer-0.9.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-27 15:44:39.763196 matminer-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-27 15:37:48.000000 matminer-0.9.0/setup.py
```

### Comparing `matminer-0.8.0/.github/workflows/release.yml` & `matminer-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/.github/workflows/test.yml` & `matminer-0.9.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,90 +5,90 @@
 
 on:
   push:
     branches:
       - main
     paths:
       - matminer/**
+      - requirements/**
 
   pull_request:
     branches:
       - main
     paths:
       - matminer/**
+      - requirements/**
 
   workflow_dispatch:
     inputs:
       fullTest:
         description: "run full test"
         required: true
         default: false
         type: boolean
 
 jobs:
 
   test:
     strategy:
       matrix:
-        python-version: ["3.8", "3.9"]
+        python-version: ["3.8", "3.9", "3.10"]
         mongodb-version: ['4.0']
 
     runs-on: ubuntu-latest
 
     env:
       PMG_MAPI_KEY: ${{ secrets.PMG_MAPI_KEY }}
       MPDS_KEY: ${{ secrets.MPDS_KEY }}
       CITRINATION_API_KEY: ${{ secrets.CITRINATION_API_KEY }}
       RUNNING_ON_GHACTIONS: "True"
       MPLBACKEND: "Agg"
       MATMINER_DATASET_FULL_TEST: ${{ inputs.fullTest }}
 
+    services:
+      mongo:
+        image: mongo:4
+        ports:
+          - 27017:27017
+
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: "pip"
         cache-dependency-path: '**/setup.py'
 
-    #- name: Install Python dependencies
-    #  run: |
-    #    python${{ matrix.python-version }} -m pip install --upgrade pip pip-tools setuptools setuptools_scm
-    #    python${{ matrix.python-version }} -m piptools sync --user requirements/ubuntu-latest_py${{ matrix.python-version }}_extras.txt
-    #    # Using non-editable install for testing building of MANIFEST files
-    #    python${{ matrix.python-version }} -m pip install --no-deps .
-
-    #- name: linting
-    #  run: |
-    #    black --version
-    #    black --check --diff --color matminer
-    #    flake8 --version
-    #    flake8 --count --show-source --statistics matminer
-    #    # exit-zero treats all errors as warnings.
-    #    flake8 --count --exit-zero --max-complexity=20 --statistics matminer
-    #    # mypy --version
-    #    # rm -rf .mypy_cache
-    #    # mypy matminer
-    #    # pydocstyle --count matminer
-    #    # pylint matminer
-
-    #- name: Start MongoDB
-    #  uses: supercharge/mongodb-github-action@1.6.0
-    #  with:
-    #    mongodb-version: ${{ matrix.mongodb-version }}
-
-    #- name: Run tests
-    #  run: |
-    #    # Sleeping to allow mongo a bit more time to boot, avoiding connect errors
-    #    sleep 10
-    #    mongo localhost/admin --eval 'db.createUser({user: "admin",pwd: "password",roles: [ { role: "root", db: "admin" } ]})'
-    #    python${{ matrix.python-version }} -m pytest --cov=matminer matminer
+    - name: Install Python dependencies
+      run: |
+        python${{ matrix.python-version }} -m pip install --upgrade pip pip-tools setuptools setuptools_scm
+        python${{ matrix.python-version }} -m piptools sync --user requirements/ubuntu-latest_py${{ matrix.python-version }}_extras.txt
+        # Using non-editable install for testing building of MANIFEST files
+        python${{ matrix.python-version }} -m pip install --no-deps .
+
+    - name: linting
+      run: |
+        black --version
+        black --check --diff --color matminer
+        flake8 --version
+        flake8 --count --show-source --statistics matminer
+        # exit-zero treats all errors as warnings.
+        flake8 --count --exit-zero --max-complexity=20 --statistics matminer
+        # mypy --version
+        # rm -rf .mypy_cache
+        # mypy matminer
+        # pydocstyle --count matminer
+        # pylint matminer
+
+    - name: Run tests
+      run: |
+        python${{ matrix.python-version }} -m pytest --cov=matminer matminer --durations=0 --timeout=360
 
     - name: Build package
       if: matrix.python-version == 3.9
       run: |
         python${{ matrix.python-version }} -m pip install --upgrade pip build setuptools setuptools_scm wheel
         python${{ matrix.python-version }} -m build
```

### Comparing `matminer-0.8.0/.github/workflows/upgrade-dependencies.yml` & `matminer-0.9.0/.github/workflows/upgrade-dependencies.yml`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/.gitignore` & `matminer-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/.pre-commit-config.yaml` & `matminer-0.9.0/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,57 @@
 exclude: ^(docs|.*test_files|cmd_line|dev_scripts)
 
-default_language_version:
-  python: python3
-
 ci:
   autoupdate_schedule: monthly
   skip: [flake8, mypy, pylint]
 
 repos:
 
   - repo: https://github.com/myint/autoflake
-    rev: v1.4
+    rev: v1.7.7
     hooks:
       - id: autoflake
-        args:
-          - --in-place
-          - --remove-unused-variables
-          - --remove-all-unused-imports
-          - --expand-star-imports
-          - --ignore-init-module-imports
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.0
+    rev: v3.2.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.3.0
     hooks:
       - id: check-yaml
         exclude: pymatgen/analysis/vesta_cutoffs.yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.10.1
     hooks:
       - id: isort
-        args: ["--profile", "black"]
+        args: [--profile, black]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 22.10.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 5.0.4
     hooks:
       - id: flake8
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.950
+    rev: v0.991
     hooks:
       - id: mypy
 
   - repo: local
     hooks:
       - id: pylint
         name: pylint
         entry: pylint
         language: python
         types: [python]
-        args:
-          [
-            "-sn",
-            "--rcfile=pylintrc",
-          ]
+        args: [-sn, --rcfile=pylintrc]
         additional_dependencies: [pylint]
```

### Comparing `matminer-0.8.0/CONTRIBUTING.md` & `matminer-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/Flowchart.png` & `matminer-0.9.0/Flowchart.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/LICENSE` & `matminer-0.9.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 choose to make your Enhancements available either publicly, or
 directly to Lawrence Berkeley National Laboratory or its
 contributors, without imposing a separate written license agreement
 for such Enhancements, then you hereby grant the following license:
 a  non-exclusive, royalty-free perpetual license to install, use,
 modify, prepare derivative works, incorporate into other computer
 software, distribute, and sublicense such enhancements or derivative
-works thereof, in binary and source code form.
+works thereof, in binary and source code form.
```

### Comparing `matminer-0.8.0/MANIFEST.in` & `matminer-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/PKG-INFO` & `matminer-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: matminer
-Version: 0.8.0
+Version: 0.9.0
 Summary: matminer is a library that contains tools for data mining in Materials Science
 Home-page: https://github.com/hackingmaterials/matminer
 Author: Anubhav Jain
 Author-email: anubhavster@gmail.com
 License: modified BSD
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
 Provides-Extra: mpds
 Provides-Extra: dscribe
 Provides-Extra: mdfforge
 Provides-Extra: aflow
 Provides-Extra: citrine
 Provides-Extra: dev
+Provides-Extra: tests
 License-File: LICENSE
 
 # <img alt="matminer" src="docs_rst/_static/matminer_logo_small.png" width="300">
 
 matminer is a library for performing data mining in the field of materials science.
 
 - **[Website (including documentation)](https://hackingmaterials.github.io/matminer/)**
-- **[Examples Repository](https://github.com/hackingmaterials/matminer_examples)** 
-- **[Help/Support Forum](https://matsci.org/c/matminer/16)** 
-- **[Source Repository](https://github.com/hackingmaterials/matminer)** 
+- **[Examples Repository](https://github.com/hackingmaterials/matminer_examples)**
+- **[Help/Support Forum](https://matsci.org/c/matminer/16)**
+- **[Source Repository](https://github.com/hackingmaterials/matminer)**
 
 matminer supports Python 3.8+.
 
 #### Related packages:
 
 - If you like matminer, you might also try [automatminer](https://github.com/hackingmaterials/automatminer).
 - If you are interested in furthering development of datasets in matminer, you may be interested in [matbench](https://github.com/hackingmaterials/matbench).
@@ -51,8 +53,8 @@
 materials data mining. Comput. Mater. Sci. 152, 60-69 (2018).
 ```
 
 Matminer helps users apply methods and data sets developed by the community. Please also cite the original sources, as this will add clarity to your article and credit the original authors:
 
 - If you use one or more **datasets** accessed through matminer, check the dataset metadata info for relevant citations on the original datasets.
 - If you use one or more **data retrieval methods**, check ``citations()`` method of the data retrieval class. This method will provide a list of BibTeX-formatted citations for that featurizer, making it easy to keep track of and cite the original publications.
-- If you use one or more **featurizers**, please take advantage of the ```citations()``` function present for every featurizer in matminer. 
+- If you use one or more **featurizers**, please take advantage of the ```citations()``` function present for every featurizer in matminer.
```

### Comparing `matminer-0.8.0/README.md` & `matminer-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # <img alt="matminer" src="docs_rst/_static/matminer_logo_small.png" width="300">
 
 matminer is a library for performing data mining in the field of materials science.
 
 - **[Website (including documentation)](https://hackingmaterials.github.io/matminer/)**
-- **[Examples Repository](https://github.com/hackingmaterials/matminer_examples)** 
-- **[Help/Support Forum](https://matsci.org/c/matminer/16)** 
-- **[Source Repository](https://github.com/hackingmaterials/matminer)** 
+- **[Examples Repository](https://github.com/hackingmaterials/matminer_examples)**
+- **[Help/Support Forum](https://matsci.org/c/matminer/16)**
+- **[Source Repository](https://github.com/hackingmaterials/matminer)**
 
 matminer supports Python 3.8+.
 
 #### Related packages:
 
 - If you like matminer, you might also try [automatminer](https://github.com/hackingmaterials/automatminer).
 - If you are interested in furthering development of datasets in matminer, you may be interested in [matbench](https://github.com/hackingmaterials/matbench).
@@ -26,8 +26,8 @@
 materials data mining. Comput. Mater. Sci. 152, 60-69 (2018).
 ```
 
 Matminer helps users apply methods and data sets developed by the community. Please also cite the original sources, as this will add clarity to your article and credit the original authors:
 
 - If you use one or more **datasets** accessed through matminer, check the dataset metadata info for relevant citations on the original datasets.
 - If you use one or more **data retrieval methods**, check ``citations()`` method of the data retrieval class. This method will provide a list of BibTeX-formatted citations for that featurizer, making it easy to keep track of and cite the original publications.
-- If you use one or more **featurizers**, please take advantage of the ```citations()``` function present for every featurizer in matminer. 
+- If you use one or more **featurizers**, please take advantage of the ```citations()``` function present for every featurizer in matminer.
```

### Comparing `matminer-0.8.0/dev_scripts/dataset_management/generate_datasets.py` & `matminer-0.9.0/dev_scripts/dataset_management/generate_datasets.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/dev_scripts/dataset_management/modify_dataset_metadata.py` & `matminer-0.9.0/dev_scripts/dataset_management/modify_dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/dev_scripts/dataset_management/prep_dataset_for_figshare.py` & `matminer-0.9.0/dev_scripts/dataset_management/prep_dataset_for_figshare.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/Flowchart.png` & `matminer-0.9.0/docs/_images/Flowchart.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/example_bulkmod.png` & `matminer-0.9.0/docs/_images/example_bulkmod.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/example_bulkmod_feats.png` & `matminer-0.9.0/docs/_images/example_bulkmod_feats.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/example_bulkmod_rf.png` & `matminer-0.9.0/docs/_images/example_bulkmod_rf.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/featurizer_diagram.png` & `matminer-0.9.0/docs/_images/featurizer_diagram.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/06dfe124bb57b08106d4043aea4218b309454d8d.png` & `matminer-0.9.0/docs/_images/math/06dfe124bb57b08106d4043aea4218b309454d8d.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/0b21f31621e4f0f2b3b5faa10af80dc999f9ffdf.png` & `matminer-0.9.0/docs/_images/math/0b21f31621e4f0f2b3b5faa10af80dc999f9ffdf.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/2fc0510f783f8ce42baa1c4ac6b86d94a6382093.png` & `matminer-0.9.0/docs/_images/math/2fc0510f783f8ce42baa1c4ac6b86d94a6382093.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/30d9a509980f1622c5d182d9b846afd31019bb05.png` & `matminer-0.9.0/docs/_images/math/30d9a509980f1622c5d182d9b846afd31019bb05.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/326c6fcc3609b0c2183f6a9e23d4aa1d4b141ea2.png` & `matminer-0.9.0/docs/_images/math/326c6fcc3609b0c2183f6a9e23d4aa1d4b141ea2.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/6f63a2c6be03f660db3b46fdb09e3e5bbc9c0b83.png` & `matminer-0.9.0/docs/_images/math/6f63a2c6be03f660db3b46fdb09e3e5bbc9c0b83.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/71a383cae1bb3f6d73faeea9e3241486d863dbc9.png` & `matminer-0.9.0/docs/_images/math/71a383cae1bb3f6d73faeea9e3241486d863dbc9.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/7358fb1b6031c815b8f99086409882bf1980148f.png` & `matminer-0.9.0/docs/_images/math/7358fb1b6031c815b8f99086409882bf1980148f.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/78eabc361f3a54daeed501fff0d3353b946504ae.png` & `matminer-0.9.0/docs/_images/math/78eabc361f3a54daeed501fff0d3353b946504ae.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/97c27bd34a0b3f4f9b760f06500e50eb3e4b75f1.png` & `matminer-0.9.0/docs/_images/math/97c27bd34a0b3f4f9b760f06500e50eb3e4b75f1.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/9c175e2552d4e2d9c682055a2ce7d1fbb538116d.png` & `matminer-0.9.0/docs/_images/math/9c175e2552d4e2d9c682055a2ce7d1fbb538116d.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/b4111b2fd8976378ce69e158f8d25467da391510.png` & `matminer-0.9.0/docs/_images/math/b4111b2fd8976378ce69e158f8d25467da391510.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/b7fdf13f2e4d24f9f2d55a77dcebbf52c8ad19c7.png` & `matminer-0.9.0/docs/_images/math/b7fdf13f2e4d24f9f2d55a77dcebbf52c8ad19c7.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/b851d3a5fb872ad82d61f964772ca1cc2520a590.png` & `matminer-0.9.0/docs/_images/math/b851d3a5fb872ad82d61f964772ca1cc2520a590.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/ba11027b67a5958f16fb1495fba3b5fb7eadcaee.png` & `matminer-0.9.0/docs/_images/math/ba11027b67a5958f16fb1495fba3b5fb7eadcaee.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/c833e66a1aa68dba7be89cbcaed7e749967ab5c9.png` & `matminer-0.9.0/docs/_images/math/c833e66a1aa68dba7be89cbcaed7e749967ab5c9.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/cfca9af3a86afde1b9efe235bfc3e48f90890d82.png` & `matminer-0.9.0/docs/_images/math/cfca9af3a86afde1b9efe235bfc3e48f90890d82.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/d188c978e0d95e667be9c33955b35c80ec4c786f.png` & `matminer-0.9.0/docs/_images/math/d188c978e0d95e667be9c33955b35c80ec4c786f.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/de47a77e2e05505f7581a4dcf8ae4f7750fe53ad.png` & `matminer-0.9.0/docs/_images/math/de47a77e2e05505f7581a4dcf8ae4f7750fe53ad.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/e8c0d853d9741d1d80356648c449808dd3fdeb3c.png` & `matminer-0.9.0/docs/_images/math/e8c0d853d9741d1d80356648c449808dd3fdeb3c.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/ee3eabc3b00202e0691a94570f869fa53a66c04d.png` & `matminer-0.9.0/docs/_images/math/ee3eabc3b00202e0691a94570f869fa53a66c04d.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/ee97899107420cf7a24b2532c2c7c09a023be431.png` & `matminer-0.9.0/docs/_images/math/ee97899107420cf7a24b2532c2c7c09a023be431.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/math/eec83a497511513e0bfa38139255e53b02d0bd21.png` & `matminer-0.9.0/docs/_images/math/eec83a497511513e0bfa38139255e53b02d0bd21.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_images/matminer_logo_small.png` & `matminer-0.9.0/docs/_images/matminer_logo_small.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/changelog.rst.txt` & `matminer-0.9.0/docs_rst/changelog.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/contributors.rst.txt` & `matminer-0.9.0/docs/_sources/contributors.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/dataset_addition_guide.rst.txt` & `matminer-0.9.0/docs/_sources/dataset_addition_guide.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/dataset_summary.rst.txt` & `matminer-0.9.0/docs/_sources/dataset_summary.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/example_bulkmod.rst.txt` & `matminer-0.9.0/docs/_sources/example_bulkmod.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/featurizer_summary.rst.txt` & `matminer-0.9.0/docs/_sources/featurizer_summary.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/index.rst.txt` & `matminer-0.9.0/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/installation.rst.txt` & `matminer-0.9.0/docs/_sources/installation.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 ----
 
 * Make sure you are using Python 3.6 or higher
 * If you have trouble with the installation of a component library (sympy, pymatgen, mdf-forge, etc.), you can try to run ``pip install <<component>>`` or (if you are using `Anaconda <https://www.anaconda.com/distribution/>`_) ``conda install <<component>>`` first, and then re-try the installation.
 
     - For example, installing pymatgen on a Windows platform is easiest with Anaconda via ``conda install -c conda-forge pymatgen``.
 
-* If you still have trouble, open up a a ticket on our `forum <https://discuss.matsci.org/c/matminer>`_  describing your problem in full (including your system specifications, Python version information, and input/output log). There is a good likelihood that someone else is running into the same issue, and by posting it on the forum we can help make the documentation clearer and smoother.
+* If you still have trouble, open up a ticket on our `forum <https://discuss.matsci.org/c/matminer>`_  describing your problem in full (including your system specifications, Python version information, and input/output log). There is a good likelihood that someone else is running into the same issue, and by posting it on the forum we can help make the documentation clearer and smoother.
```

### Comparing `matminer-0.8.0/docs/_sources/matminer.data_retrieval.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.data_retrieval.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.data_retrieval.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.data_retrieval.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.datasets.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.datasets.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.datasets.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.datasets.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.composition.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.composition.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.composition.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.composition.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.site.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.site.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.site.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.site.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.structure.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.structure.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.structure.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.structure.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.utils.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.featurizers.utils.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.featurizers.utils.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.utils.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_sources/matminer.utils.tests.rst.txt` & `matminer-0.9.0/docs/_sources/matminer.utils.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/Flowchart.png` & `matminer-0.9.0/docs/_static/Flowchart.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/_sphinx_javascript_frameworks_compat.js` & `matminer-0.9.0/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/ajax-loader.gif` & `matminer-0.9.0/docs/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/basic.css` & `matminer-0.9.0/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/bulk_shear_moduli.html` & `matminer-0.9.0/docs/_static/bulk_shear_moduli.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/comment-bright.png` & `matminer-0.9.0/docs/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/comment-close.png` & `matminer-0.9.0/docs/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/comment.png` & `matminer-0.9.0/docs/_static/comment.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/doctools.js` & `matminer-0.9.0/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/example_bulkmod.png` & `matminer-0.9.0/docs/_static/example_bulkmod.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/example_bulkmod_feats.png` & `matminer-0.9.0/docs/_static/example_bulkmod_feats.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/example_bulkmod_rf.png` & `matminer-0.9.0/docs/_static/example_bulkmod_rf.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/examples_bulkmod_rf.png` & `matminer-0.9.0/docs/_static/examples_bulkmod_rf.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/featurizer_diagram.png` & `matminer-0.9.0/docs/_static/featurizer_diagram.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/jquery-3.1.0.js` & `matminer-0.9.0/docs/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/jquery-3.2.1.js` & `matminer-0.9.0/docs/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/jquery-3.5.1.js` & `matminer-0.9.0/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/jquery-3.6.0.js` & `matminer-0.9.0/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/jquery.js` & `matminer-0.9.0/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/language_data.js` & `matminer-0.9.0/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/matminer_logo_small.png` & `matminer-0.9.0/docs/_static/matminer_logo_small.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/nature.css` & `matminer-0.9.0/docs/_static/nature.css`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/pygments.css` & `matminer-0.9.0/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/searchtools.js` & `matminer-0.9.0/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/sphinx_highlight.js` & `matminer-0.9.0/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/underscore-1.13.1.js` & `matminer-0.9.0/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/underscore-1.3.1.js` & `matminer-0.9.0/docs/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/underscore.js` & `matminer-0.9.0/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/_static/websupport.js` & `matminer-0.9.0/docs/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/changelog.html` & `matminer-0.9.0/docs/changelog.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/contributors.html` & `matminer-0.9.0/docs/contributors.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/dataset_addition_guide.html` & `matminer-0.9.0/docs/dataset_addition_guide.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/dataset_summary.html` & `matminer-0.9.0/docs/dataset_summary.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/example_bulkmod.html` & `matminer-0.9.0/docs/example_bulkmod.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/featurizer_summary.html` & `matminer-0.9.0/docs/featurizer_summary.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/genindex.html` & `matminer-0.9.0/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/index.html` & `matminer-0.9.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/installation.html` & `matminer-0.9.0/docs/installation.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.data_retrieval.html` & `matminer-0.9.0/docs/matminer.data_retrieval.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.data_retrieval.tests.html` & `matminer-0.9.0/docs/matminer.data_retrieval.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.datasets.html` & `matminer-0.9.0/docs/matminer.datasets.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.datasets.tests.html` & `matminer-0.9.0/docs/matminer.datasets.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.composition.html` & `matminer-0.9.0/docs/matminer.featurizers.composition.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.composition.tests.html` & `matminer-0.9.0/docs/matminer.featurizers.composition.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.html` & `matminer-0.9.0/docs/matminer.featurizers.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.site.html` & `matminer-0.9.0/docs/matminer.featurizers.site.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.site.tests.html` & `matminer-0.9.0/docs/matminer.featurizers.site.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.structure.html` & `matminer-0.9.0/docs/matminer.featurizers.structure.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.structure.tests.html` & `matminer-0.9.0/docs/matminer.featurizers.structure.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.tests.html` & `matminer-0.9.0/docs/matminer.featurizers.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.utils.html` & `matminer-0.9.0/docs/matminer.featurizers.utils.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.featurizers.utils.tests.html` & `matminer-0.9.0/docs/matminer.featurizers.utils.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.figrecipes.html` & `matminer-0.9.0/docs/matminer.figrecipes.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.figrecipes.tests.html` & `matminer-0.9.0/docs/matminer.figrecipes.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.html` & `matminer-0.9.0/docs/matminer.html`

 * *Files 0% similar despite different names*

```diff
@@ -612,15 +612,15 @@
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="module-matminer">
 <span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-matminer" title="Permalink to this heading">¶</a></h2>
-<p>library for data mining materials properties</p>
+<p>data mining materials properties</p>
 </section>
 </section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
```

#### html2text {}

```diff
@@ -415,15 +415,15 @@
                       # ItemSelector.fit()
                       # ItemSelector.transform()
           o matminer.utils.utils_module
                 # homogenize_multiindex()
           o Module_contents
 
 ***** Module contentsÂ¶ *****
-library for data mining materials properties
+data mining materials properties
 
 **** Table_of_Contents ****
     * matminer_package
           o Subpackages
           o Module_contents
 **** This Page ****
     * Show_Source
```

### Comparing `matminer-0.8.0/docs/matminer.utils.data_files.html` & `matminer-0.9.0/docs/matminer.utils.data_files.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.utils.html` & `matminer-0.9.0/docs/matminer.utils.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/matminer.utils.tests.html` & `matminer-0.9.0/docs/matminer.utils.tests.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/modules.html` & `matminer-0.9.0/docs/modules.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/objects.inv` & `matminer-0.9.0/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/py-modindex.html` & `matminer-0.9.0/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/search.html` & `matminer-0.9.0/docs/search.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs/searchindex.js` & `matminer-0.9.0/docs/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2319,15 +2319,15 @@
         "futur": [3, 13, 14, 20],
         "activ": 3,
         "area": [3, 6, 16, 18],
         "minut": 4,
         "retrieve_mp": [4, 6, 8, 28],
         "popul": 4,
         "scikit": [4, 6, 13, 25],
-        "librari": [4, 5, 6, 7, 8, 9, 13, 16, 25],
+        "librari": [4, 5, 6, 7, 9, 13, 16, 25],
         "displai": [4, 13],
         "warn": [4, 9, 13, 14, 18, 20],
         "filterwarn": 4,
         "numpi": [4, 13, 16, 18, 21],
         "np": [4, 13, 16, 18, 21],
         "view": 4,
         "set_opt": 4,
```

### Comparing `matminer-0.8.0/docs_rst/Makefile` & `matminer-0.9.0/docs_rst/Makefile`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/Flowchart.png` & `matminer-0.9.0/docs_rst/_static/Flowchart.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/bulk_shear_moduli.html` & `matminer-0.9.0/docs_rst/_static/bulk_shear_moduli.html`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/example_bulkmod.png` & `matminer-0.9.0/docs_rst/_static/example_bulkmod.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/example_bulkmod_feats.png` & `matminer-0.9.0/docs_rst/_static/example_bulkmod_feats.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/example_bulkmod_rf.png` & `matminer-0.9.0/docs_rst/_static/example_bulkmod_rf.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/featurizer_diagram.png` & `matminer-0.9.0/docs_rst/_static/featurizer_diagram.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/matminer_logo_small.png` & `matminer-0.9.0/docs_rst/_static/matminer_logo_small.png`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/_static/nature.css` & `matminer-0.9.0/docs_rst/_static/nature.css`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/changelog.rst` & `matminer-0.9.0/docs/_sources/changelog.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 * More intuitive input arguments for featurize_many (L. Ward)
 * Bugfixes for BOOP features (L. Ward, A. Thompson)
 
 **v0.4.0**
 
 * Progressbar for featurizers (A. Dunn)
 * Add BOOP features (L. Ward)
-* Add Seko features, including more lookuip tables for MagpieData and elemental property site features + covariance, skew, kurtosis (L. Ward)
+* Add Seko features, including more lookup tables for MagpieData and elemental property site features + covariance, skew, kurtosis (L. Ward)
 * New scheme for GRDF/AFS bin functions (L. Ward)
 * misc fixes (A. Dunn., L. Ward)
 
 **v0.3.9**
 
 * BandEdge renamed to Hybridization, gives smoother featurizations (M. Dylla, A. Faghaninia)
 * Add hoverinfo option for many plots (A. Dunn)
```

### Comparing `matminer-0.8.0/docs_rst/conf.py` & `matminer-0.9.0/docs_rst/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,44 +14,49 @@
 import sys
 
 from matminer import __version__
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.append(os.path.abspath('..'))
+sys.path.append(os.path.abspath(".."))
 # print sys.path
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest',
-              'sphinx.ext.intersphinx', 'sphinx.ext.todo',
-              'sphinx.ext.coverage', 'sphinx.ext.imgmath',
-              'sphinx.ext.ifconfig']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.imgmath",
+    "sphinx.ext.ifconfig",
+]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'matminer'
-copyright = '2015, Anubhav Jain'
+project = "matminer"
+copyright = "2015, Anubhav Jain"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = __version__
@@ -66,15 +71,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
@@ -83,25 +88,25 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'nature'
+html_theme = "nature"
 
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
@@ -123,15 +128,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -167,34 +172,31 @@
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'FireWorksdoc'
+htmlhelp_basename = "FireWorksdoc"
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ('index', 'FireWorks.tex', 'FireWorks Documentation',
-     'Anubhav Jain', 'manual'),
+    ("index", "FireWorks.tex", "FireWorks Documentation", "Anubhav Jain", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -214,33 +216,34 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    ('index', 'fireworks', 'FireWorks Documentation',
-     ['Anubhav Jain'], 1)
-]
+man_pages = [("index", "fireworks", "FireWorks Documentation", ["Anubhav Jain"], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'matminer', 'matminer Documentation',
-     'Anubhav Jain',
-     'matminer is a library for machine learning in materials science',
-     'Miscellaneous'),
+    (
+        "index",
+        "matminer",
+        "matminer Documentation",
+        "Anubhav Jain",
+        "matminer is a library for machine learning in materials science",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
@@ -248,18 +251,18 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
 
 # -- Options for Epub output ---------------------------------------------------
 
 # Bibliographic Dublin Core info.
-epub_title = 'matminer'
-epub_author = 'Anubhav Jain'
-epub_publisher = 'Anubhav Jain'
-epub_copyright = '2015, Anubhav Jain'
+epub_title = "matminer"
+epub_author = "Anubhav Jain"
+epub_publisher = "Anubhav Jain"
+epub_copyright = "2015, Anubhav Jain"
 
 # The language of the text. It defaults to the language option
 # or en if the language is not set.
 # epub_language = ''
 
 # The scheme of the identifier. Typical schemes are ISBN or URL.
 # epub_scheme = ''
@@ -274,30 +277,30 @@
 # A tuple containing the cover image and cover page html template filenames.
 # epub_cover = ()
 
 # HTML files that should be inserted before the pages created by sphinx.
 # The format is a list of tuples containing the path and title.
 # epub_pre_files = []
 
-# HTML files shat should be inserted after the pages created by sphinx.
+# HTML files that should be inserted after the pages created by sphinx.
 # The format is a list of tuples containing the path and title.
 # epub_post_files = []
 
 # A list of files that should not be packed into the epub file.
 # epub_exclude_files = []
 
 # The depth of the table of contents in toc.ncx.
 # epub_tocdepth = 3
 
 # Allow duplicate toc entries.
 # epub_tocdup = True
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+intersphinx_mapping = {"http://docs.python.org/": None}
 
 
 # AJ: a hack found online to get __init__ to show up in docs
 def skip(app, what, name, obj, skip, options):
     if name == "__init__":
         return False
     return skip
```

### Comparing `matminer-0.8.0/docs_rst/contributors.rst` & `matminer-0.9.0/docs_rst/contributors.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/dataset_addition_guide.rst` & `matminer-0.9.0/docs_rst/dataset_addition_guide.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/dataset_summary.py` & `matminer-0.9.0/docs_rst/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/dataset_summary.rst` & `matminer-0.9.0/docs_rst/dataset_summary.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/example_bulkmod.rst` & `matminer-0.9.0/docs_rst/example_bulkmod.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/featurizer_summary.py` & `matminer-0.9.0/docs_rst/featurizer_summary.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/featurizer_summary.rst` & `matminer-0.9.0/docs_rst/featurizer_summary.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/index.rst` & `matminer-0.9.0/docs_rst/index.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/installation.rst` & `matminer-0.9.0/docs_rst/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 ----
 
 * Make sure you are using Python 3.6 or higher
 * If you have trouble with the installation of a component library (sympy, pymatgen, mdf-forge, etc.), you can try to run ``pip install <<component>>`` or (if you are using `Anaconda <https://www.anaconda.com/distribution/>`_) ``conda install <<component>>`` first, and then re-try the installation.
 
     - For example, installing pymatgen on a Windows platform is easiest with Anaconda via ``conda install -c conda-forge pymatgen``.
 
-* If you still have trouble, open up a a ticket on our `forum <https://discuss.matsci.org/c/matminer>`_  describing your problem in full (including your system specifications, Python version information, and input/output log). There is a good likelihood that someone else is running into the same issue, and by posting it on the forum we can help make the documentation clearer and smoother.
+* If you still have trouble, open up a ticket on our `forum <https://discuss.matsci.org/c/matminer>`_  describing your problem in full (including your system specifications, Python version information, and input/output log). There is a good likelihood that someone else is running into the same issue, and by posting it on the forum we can help make the documentation clearer and smoother.
```

### Comparing `matminer-0.8.0/docs_rst/matminer.data_retrieval.rst` & `matminer-0.9.0/docs_rst/matminer.data_retrieval.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.data_retrieval.tests.rst` & `matminer-0.9.0/docs_rst/matminer.data_retrieval.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.datasets.rst` & `matminer-0.9.0/docs_rst/matminer.datasets.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.datasets.tests.rst` & `matminer-0.9.0/docs_rst/matminer.datasets.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.composition.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.composition.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.composition.tests.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.composition.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.site.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.site.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.site.tests.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.site.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.structure.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.structure.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.structure.tests.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.structure.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.tests.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.utils.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.utils.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.featurizers.utils.tests.rst` & `matminer-0.9.0/docs_rst/matminer.featurizers.utils.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.utils.rst` & `matminer-0.9.0/docs_rst/matminer.utils.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/docs_rst/matminer.utils.tests.rst` & `matminer-0.9.0/docs_rst/matminer.utils.tests.rst`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_AFLOW.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_AFLOW.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,21 +214,19 @@
 
         Args:
             pymongo_query: (dict) Pymongo-like query operator. See the
                 AFLOWDataRetrieval.get_dataframe method for more details
         """
 
         for str_property, value in pymongo_query.items():
-
             # converts str representation of property to aflow.Keyword
             keyword = getattr(K, str_property)
 
             if isinstance(value, dict):  # handles special operators
                 for inner_key, inner_value in value.items():
-
                     if inner_key == "$in":
                         self.filter(
                             reduce(
                                 lambda x, y: (x | y),
                                 map(lambda z: (keyword == z), inner_value),
                             )
                         )
```

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_Citrine.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_Citrine.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             api_key = os.environ["CITRINATION_API_KEY"]
         elif "CITRINE_KEY" in os.environ:
             api_key = os.environ["CITRINE_KEY"]
         else:
             raise AttributeError(
                 """Citrine API key not found.
 
-            You need to get an API key from Citrination, and either supply it as an argument to 
+            You need to get an API key from Citrination, and either supply it as an argument to
             this class or set it as the value of the CITRINATION_API_KEY environment variable
 
             See https://citrineinformatics.github.io/api-documentation/quickstart/index.html
             for details on how to get an API key"""
             )
 
         self.client = CitrinationClient(api_key, "https://citrination.com")
```

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_MDF.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_MDF.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_MP.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_MP.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
     def __init__(self, api_key=None):
         """
         Args:
             api_key: (str) Your Materials Project API key, or None if you've
                 set up your pymatgen config.
         """
-        self.mprester = MPRester(api_key=api_key)
+        if api_key:
+            self.mprester = MPRester(api_key=api_key)
+        else:
+            self.mprester = MPRester()
 
     def api_link(self):
         return "https://materialsproject.org/wiki/index.php/The_Materials_API"
 
     def get_dataframe(self, criteria, properties, index_mpid=True, **kwargs):
         """
         Gets data from MP in a dataframe format. See api_link for more details.
```

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_MPDS.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_MPDS.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_MongoDB.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_MongoDB.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/retrieve_base.py` & `matminer-0.9.0/matminer/data_retrieval/retrieve_base.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_AFLOW.py` & `matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_AFLOW.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import unittest
+import os
 
 import numpy as np
 from pymatgen.core.structure import Structure
 
 from matminer.data_retrieval.retrieve_AFLOW import AFLOWDataRetrieval
+from matminer.data_retrieval.tests.base import on_ci
 
 
+@unittest.skipIf(on_ci.upper() == "TRUE", "Bad AFLOW-GHActions pipeline")
 class AFLOWDataRetrievalTest(unittest.TestCase):
     def setUp(self):
         self.aflowdr = AFLOWDataRetrieval()
 
     def test_get_data(self):
         df = self.aflowdr.get_dataframe(
-            criteria={"auid": "aflow:a17a2da2f3d3953a"},
+            criteria={"auid": {"$in": ["aflow:a17a2da2f3d3953a"]}},
             properties=["density", "enthalpy_formation_atom", "positions_fractional"],
             files=["structure"],
         )
 
         # ensures that only one result is returned for a single auid
         self.assertEqual(len(df["aurl"]), 1)
```

### Comparing `matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_Citrine.py` & `matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_Citrine.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MDF.py` & `matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MDF.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MP.py` & `matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MP.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MPDS.py` & `matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MPDS.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
         self.schema = json.loads(content)
         Draft4Validator.check_schema(self.schema)
 
     @unittest.skipIf(on_ci.upper() == "TRUE", "Bad Datasource-GHActions pipeline")
     @unittest.skipIf("MPDS_KEY" not in os.environ, "MPDS_KEY env var not set")
     def test_valid_answer(self):
-
         client = MPDSDataRetrieval()
         answer = client.get_data(self.test_request, fields={})
 
         try:
             validate(answer, self.schema)
         except ValidationError as e:
             self.fail(f"The item: \r\n\r\n {e.instance} \r\n\r\n has an issue: \r\n\r\n {e.context}")
```

### Comparing `matminer-0.8.0/matminer/data_retrieval/tests/test_retrieve_MongoDB.py` & `matminer-0.9.0/matminer/data_retrieval/tests/test_retrieve_MongoDB.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def test_remove_ints(self):
         self.assertEqual(remove_ints("a.1"), "a")
         self.assertEqual(remove_ints("a.1.x"), "a.x")
 
     @unittest.skipIf(not on_ci, "MongoDataRetrievalTest configured only to run on CI by default")
     def test_get_dataframe(self):
-        db = MongoClient("localhost", 27017, username="admin", password="password").test_db
+        db = MongoClient("localhost", 27017).test_db
         c = db.test_collection
         docs = [
             {
                 "some": {"nested": {"result": 14.5}},
                 "other": "notnestedresult",
                 "final": 16.938475 + i,
                 "array": [1.4, 5.6, 11.2, 1.1],
```

### Comparing `matminer-0.8.0/matminer/datasets/convenience_loaders.py` & `matminer-0.9.0/matminer/datasets/convenience_loaders.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/dataset_metadata.json` & `matminer-0.9.0/matminer/datasets/dataset_metadata.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/dataset_retrieval.py` & `matminer-0.9.0/matminer/datasets/dataset_retrieval.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/tests/base.py` & `matminer-0.9.0/matminer/datasets/tests/base.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/tests/test_convenience_loaders.py` & `matminer-0.9.0/matminer/datasets/tests/test_convenience_loaders.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/tests/test_dataset_retrieval.py` & `matminer-0.9.0/matminer/datasets/tests/test_dataset_retrieval.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/tests/test_datasets.py` & `matminer-0.9.0/matminer/datasets/tests/test_datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         self,
         dataset_name,
         object_headers=None,
         numeric_headers=None,
         bool_headers=None,
         test_func=None,
     ):
-
         # "Hard" integrity checks that take a long time.
         # These tests only run if the MATMINER_DATASET_FULL_TEST
         # environment variable is set to True
         if do_complete_test:
             # Get rid of dataset if it's on the disk already
             data_path = os.path.join(
                 self.dataset_dir,
@@ -110,22 +109,22 @@
             "K_VRH",
             "K_Voigt",
             "poisson_ratio",
             "kpoint_density",
         ]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
             tensor_headers = [
                 "compliance_tensor",
                 "elastic_tensor",
                 "elastic_tensor_original",
             ]
             for c in tensor_headers:
-                self.assertEqual(type(df[c][0]), np.ndarray)
+                self.assertIsInstance(df[c][0], np.ndarray)
 
         self.universal_dataset_check(
             "elastic_tensor_2015",
             object_headers,
             numeric_headers,
             test_func=_unique_tests,
         )
@@ -142,16 +141,16 @@
             "meta",
             "poscar",
         ]
 
         numeric_headers = ["nsites", "space_group", "volume", "eij_max"]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
-            self.assertEqual(type(df["piezoelectric_tensor"][0]), np.ndarray)
+            self.assertIsInstance(df["structure"][0], Structure)
+            self.assertIsInstance(df["piezoelectric_tensor"][0], np.ndarray)
 
         self.universal_dataset_check(
             "piezoelectric_tensor",
             object_headers,
             numeric_headers,
             test_func=_unique_tests,
         )
@@ -177,15 +176,15 @@
             "poly_electronic",
             "poly_total",
         ]
 
         bool_headers = ["pot_ferroelectric"]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
 
         self.universal_dataset_check(
             "dielectric_constant",
             object_headers,
             numeric_headers,
             bool_headers,
             test_func=_unique_tests,
@@ -198,15 +197,15 @@
             "e_above_hull",
             "nsites",
             "formation_energy",
             "formation_energy_per_atom",
         ]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
 
         self.universal_dataset_check("flla", object_headers, numeric_headers, test_func=_unique_tests)
 
     def test_castelli_perovskites(self):
         object_headers = ["structure", "formula"]
 
         numeric_headers = [
@@ -218,15 +217,15 @@
             "cbm",
             "gap gllbsc",
         ]
 
         bool_headers = ["gap is direct"]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
 
         self.universal_dataset_check(
             "castelli_perovskites",
             object_headers,
             numeric_headers,
             bool_headers=bool_headers,
             test_func=_unique_tests,
@@ -234,25 +233,25 @@
 
     def test_boltztrap_mp(self):
         object_headers = ["structure", "formula", "mpid"]
 
         numeric_headers = ["pf_n", "pf_p", "s_n", "s_p", "m_n", "m_p"]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
 
         self.universal_dataset_check("boltztrap_mp", object_headers, numeric_headers, test_func=_unique_tests)
 
     def test_phonon_dielectric_mp(self):
         object_headers = ["structure", "formula", "mpid"]
 
         numeric_headers = ["eps_electronic", "eps_total", "last phdos peak"]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
 
         self.universal_dataset_check(
             "phonon_dielectric_mp",
             object_headers,
             numeric_headers,
             test_func=_unique_tests,
         )
@@ -300,15 +299,15 @@
             "elastic anisotropy",
             "bulk modulus",
             "shear modulus",
             "e_form",
         ]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
+            self.assertIsInstance(df["structure"][0], Structure)
 
         self.universal_dataset_check("mp_all_20181018", object_headers, numeric_headers, test_func=_unique_tests)
 
     def test_mp_nostruct_20181018(self):
         object_headers = ["mpid", "formula"]
 
         numeric_headers = [
@@ -425,16 +424,16 @@
             "epsilon_x tbmbj",
             "epsilon_y tbmbj",
             "epsilon_z tbmbj",
             "gap opt",
         ]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
-            self.assertEqual(type(df["composition"][0]), Composition)
+            self.assertIsInstance(df["structure"][0], Structure)
+            self.assertIsInstance(df["composition"][0], Composition)
 
         self.universal_dataset_check(
             "jarvis_ml_dft_training",
             object_headers,
             numeric_headers,
             test_func=_unique_tests,
         )
@@ -459,16 +458,16 @@
             "epsilon_x tbmbj",
             "epsilon_y tbmbj",
             "epsilon_z tbmbj",
             "gap opt",
         ]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
-            self.assertEqual(type(df["composition"][0]), Composition)
+            self.assertIsInstance(df["structure"][0], Structure)
+            self.assertIsInstance(df["composition"][0], Composition)
 
         self.universal_dataset_check("jarvis_dft_3d", object_headers, numeric_headers, test_func=_unique_tests)
 
     def test_jarvis_dft_2d(self):
         object_headers = [
             "jid",
             "mpid",
@@ -487,16 +486,16 @@
             "epsilon_x tbmbj",
             "epsilon_y tbmbj",
             "epsilon_z tbmbj",
             "gap opt",
         ]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
-            self.assertEqual(type(df["composition"][0]), Composition)
+            self.assertIsInstance(df["structure"][0], Structure)
+            self.assertIsInstance(df["composition"][0], Composition)
 
         self.universal_dataset_check("jarvis_dft_2d", object_headers, numeric_headers, test_func=_unique_tests)
 
     def test_glass_binary(self):
         object_headers = ["formula"]
 
         numeric_headers = ["gfa"]
@@ -554,16 +553,16 @@
         ]
 
         numeric_headers = ["shear_modulus", "bulk_modulus"]
 
         bool_headers = ["suspect_value"]
 
         def _unique_tests(df):
-            self.assertEqual(type(df["structure"][0]), Structure)
-            self.assertEqual(type(df["composition"][0]), Composition)
+            self.assertIsInstance(df["structure"][0], Structure)
+            self.assertIsInstance(df["composition"][0], Composition)
             self.assertTrue(isinstance(df["brgoch_feats"][0], dict))
 
         self.universal_dataset_check(
             "brgoch_superhard_training",
             object_headers,
             numeric_headers,
             bool_headers,
@@ -573,15 +572,14 @@
     def test_expt_gap_kingsbury(self):
         object_headers = ["formula", "likely_mpid"]
 
         numeric_headers = ["expt_gap"]
         self.universal_dataset_check("expt_gap_kingsbury", object_headers, numeric_headers)
 
     def test_expt_formation_enthalpy_kingsbury(self):
-
         object_headers = ["formula", "likely_mpid", "phaseinfo", "reference"]
 
         numeric_headers = ["expt_form_e", "uncertainty"]
 
         self.universal_dataset_check(
             "expt_formation_enthalpy_kingsbury",
             object_headers,
```

### Comparing `matminer-0.8.0/matminer/datasets/tests/test_utils.py` & `matminer-0.9.0/matminer/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/datasets/utils.py` & `matminer-0.9.0/matminer/datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
 import json
 import os
-import warnings
 import time
+import warnings
 
 import pandas as pd
 import requests
 import tqdm
 
 __author__ = "Daniel Dopp <dbdopp@lbl.gov>"
 
@@ -74,15 +74,14 @@
 
     if n_retries_allowed < 0:
         raise ValueError("Number of retries for download cannot be less than 0.")
 
     do_download = False
     # If the file doesn't exist, download it
     if not os.path.exists(data_path):
-
         # Ensure proper arguments for download
         if not download_if_missing:
             raise OSError("Data not found and download_if_missing set to False")
         elif url is None:
             raise ValueError("To download an external dataset, the url metadata must be provided")
 
         # Ensure storage location exists
```

### Comparing `matminer-0.8.0/matminer/featurizers/bandstructure.py` & `matminer-0.9.0/matminer/featurizers/bandstructure.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/base.py` & `matminer-0.9.0/matminer/featurizers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     Some featurizers require first calling the `fit` method before the
     featurization methods can function. Generally, you pass the dataset to
     fit to determine which features a featurizer should compute. For example,
     a featurizer that returns the partial radial distribution function
     may need to know which elements are present in a dataset.
 
-    You can can also use the `precheck` and `precheck_dataframe` methods to
+    You can also use the `precheck` and `precheck_dataframe` methods to
     ensure a featurizer is in scope for a given sample (or dataset) before
     featurizing.
 
     You can also employ the featurizer as part of a ScikitLearn Pipeline object.
     For these cases, ScikitLearn calls the `transform` function of the
     `BaseFeaturizer` which is a less-featured wrapper of `featurize_many`. You
     would then provide your input data as an array to the Pipeline, which would
@@ -134,16 +134,22 @@
     information for user to map a feature name what it means. The objective in
     this part is to allow people to understand what each column of their
     dataframe is without having to read the Python code. You do not need to
     explain all of the math/algorithms behind each feature for them to be able
     to reproduce the feature, just to get an idea what it is.
     """
 
-    def set_n_jobs(self, n_jobs):
-        """Set the number of threads for this."""
+    def set_n_jobs(self, n_jobs: int) -> None:
+        """Set the number of concurrent jobs to spawn during featurization.
+
+        Args:
+            n_jobs (int): Number of threads in multiprocessing pool.
+
+        Note: It seems multiprocessing can be the cause of out-of-memory (OOM) errors, especially when trying to featurize large structures on HPC nodes with strict memory limits. Using featurizer.set_n_jobs(1) has been known to help as a workaround.
+        """
         self._n_jobs = n_jobs
 
     @property
     def n_jobs(self):
         return self._n_jobs if hasattr(self, "_n_jobs") else cpu_count()
 
     def set_chunksize(self, chunksize):
@@ -434,15 +440,15 @@
             entries = entries.values
         elif isinstance(entries, pd.Series) or not isinstance(entries[0], (tuple, list, np.ndarray)):
             entries = zip(entries)
 
         # Add a progress bar
         if pbar:
             # list() required, tqdm has issues with memory if generator given
-            entries = tqdm(list(entries), desc=self.__class__.__name__)
+            entries = tqdm(list(entries), desc=self.__class__.__name__, **(pbar if isinstance(pbar, dict) else {}))
 
         # Run the actual featurization
         if self.n_jobs == 1:
             return [
                 self.featurize_wrapper(x, ignore_errors=ignore_errors, return_errors=return_errors) for x in entries
             ]
         else:
```

### Comparing `matminer-0.8.0/matminer/featurizers/composition/__init__.py` & `matminer-0.9.0/matminer/featurizers/composition/__init__.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/alloy.py` & `matminer-0.9.0/matminer/featurizers/composition/alloy.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/composite.py` & `matminer-0.9.0/matminer/featurizers/composition/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Features: Based on the statistics of the data_source chosen, computed
     by element stoichiometry. The format generally is:
 
     "{data source} {statistic} {property}"
 
     For example:
 
-    "PymetgenData range X"  # Range of electronegativity from Pymatgen data
+    "PymatgenData range X"  # Range of electronegativity from Pymatgen data
 
     For a list of all statistics, see the PropertyStats documentation; for a
     list of all attributes available for a given data_source, see the
     documentation for the data sources (e.g., PymatgenData, MagpieData,
     MatscholarElementData, etc.).
 
     Args:
```

### Comparing `matminer-0.8.0/matminer/featurizers/composition/element.py` & `matminer-0.9.0/matminer/featurizers/composition/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,17 @@
     """
     Estimation of absolute position of band center using electronegativity.
 
     Features
         - Band center
     """
 
+    magpie_data = MagpieData()
+    deml_data = DemlData()
+
     def featurize(self, comp):
         """
         (Rough) estimation of absolution position of band center using
         geometric mean of electronegativity.
 
         Args:
             comp (Composition).
@@ -218,16 +221,16 @@
         Returns:
             (float) band center.
 
         """
         gmean = 1.0
         sumamt = sum(comp.get_el_amt_dict().values())
         for el, amt in comp.get_el_amt_dict().items():
-            first_ioniz = DemlData().get_elemental_property(Element(el), "first_ioniz") / 1000
-            elec_aff = MagpieData().get_elemental_property(Element(el), "ElectronAffinity")
+            first_ioniz = self.deml_data.get_elemental_property(Element(el), "first_ioniz") / 1000
+            elec_aff = self.magpie_data.get_elemental_property(Element(el), "ElectronAffinity")
             gmean *= (0.5 * (first_ioniz + elec_aff) / 96.48) ** (amt / sumamt)
         return [gmean]
 
     def feature_labels(self):
         return ["band center"]
 
     def citations(self):
```

### Comparing `matminer-0.8.0/matminer/featurizers/composition/ion.py` & `matminer-0.9.0/matminer/featurizers/composition/ion.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/orbital.py` & `matminer-0.9.0/matminer/featurizers/composition/orbital.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/packing.py` & `matminer-0.9.0/matminer/featurizers/composition/packing.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         Return:
             (NearNeighbors): Tool to find nearby clusters in this system. None
                 if there are no efficiently-packed clusters for this combination of elements
         """
         elements = list(set(elements))
         return self._create_cluster_lookup_tool(tuple(sorted(elements)))
 
-    @lru_cache()
+    @lru_cache
     def _create_cluster_lookup_tool(self, elements):
         """
         Cached version of `create_cluster_lookup_tool`. Assumes that the
         elements are passed as sorted tuple with no duplicates
 
         Args:
             elements ([Element]): Elements in system
```

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/base.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/base.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_alloy.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_alloy.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_composite.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_element.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_ion.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_ion.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_orbital.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_orbital.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_packing.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 class PackingFeaturesTest(CompositionFeaturesTest):
     def test_ape(self):
         f = AtomicPackingEfficiency()
         ef = ElementFraction()
         ef.set_n_jobs(1)
+        f.set_n_jobs(1)
 
         # Test the APE calculation routines
         self.assertAlmostEqual(1.11632, f.get_ideal_radius_ratio(15))
         self.assertAlmostEqual(0.154701, f.get_ideal_radius_ratio(2))
         self.assertAlmostEqual(1.65915, f.get_ideal_radius_ratio(27))
         self.assertAlmostEqual(15, f.find_ideal_cluster_size(1.116)[0])
         self.assertAlmostEqual(3, f.find_ideal_cluster_size(0.1)[0])
```

### Comparing `matminer-0.8.0/matminer/featurizers/composition/tests/test_thermo.py` & `matminer-0.9.0/matminer/featurizers/composition/tests/test_thermo.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,22 +5,31 @@
 
 from matminer.featurizers.composition.tests.base import CompositionFeaturesTest
 from matminer.featurizers.composition.thermo import CohesiveEnergy, CohesiveEnergyMP
 
 
 class ThermoFeaturesTest(CompositionFeaturesTest):
     def test_cohesive_energy(self):
-        mpr = MPRester()
+        try:
+            mpr = MPRester()
+        except ValueError:
+            raise SkipTest("Materials Project API key not set; Skipping cohesive energy test")
+
         if not mpr.api_key:
             raise SkipTest("Materials Project API key not set; Skipping cohesive energy test")
+
         df_cohesive_energy = CohesiveEnergy().featurize_dataframe(self.df, col_id="composition")
         self.assertAlmostEqual(df_cohesive_energy["cohesive energy"][0], 5.179358342, 2)
 
     def test_cohesive_energy_mp(self):
-        mpr = MPRester()
+        try:
+            mpr = MPRester()
+        except ValueError:
+            raise SkipTest("Materials Project API key not set; Skipping cohesive energy test")
+
         if not mpr.api_key:
             raise SkipTest("Materials Project API key not set; Skipping cohesive energy test")
         ce = CohesiveEnergyMP()
         ce.set_n_jobs(1)
         df_cohesive_energy = ce.featurize_dataframe(self.df, col_id="composition")
         self.assertAlmostEqual(df_cohesive_energy["cohesive energy (MP)"][0], 5.778053364, 2)
```

### Comparing `matminer-0.8.0/matminer/featurizers/composition/thermo.py` & `matminer-0.9.0/matminer/featurizers/composition/thermo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Composition featurizers for thermodynamic properties.
 """
 
-from pymatgen.ext.matproj import MPRester
 
 from matminer.featurizers.base import BaseFeaturizer
 from matminer.utils.data import CohesiveEnergyData
 
 
 class CohesiveEnergy(BaseFeaturizer):
     """
@@ -36,16 +35,22 @@
         """
         comp = comp.reduced_composition
         el_amt_dict = comp.get_el_amt_dict()
 
         formation_energy_per_atom = formation_energy_per_atom or None
 
         if not formation_energy_per_atom:
+            from pymatgen.ext.matproj import MPRester
+
             # Get formation energy of most stable structure from MP
-            struct_lst = MPRester(self.mapi_key).get_data(comp.reduced_formula)
+            if self.mapi_key:
+                struct_lst = MPRester(self.mapi_key).get_data(comp.reduced_formula)
+            else:
+                struct_lst = MPRester().get_data(comp.reduced_formula)
+
             if len(struct_lst) > 0:
                 most_stable_entry = sorted(struct_lst, key=lambda e: e["energy_per_atom"])[0]
                 formation_energy_per_atom = most_stable_entry["formation_energy_per_atom"]
             else:
                 raise ValueError(f"No structure found in MP for {comp}")
 
         # Subtract elemental cohesive energies from formation energy
@@ -90,17 +95,18 @@
 
     def featurize(self, comp):
         """
 
         Args:
             comp: (str) compound composition, eg: "NaCl"
         """
+        from pymatgen.ext.matproj import MPRester
 
         # Get formation energy of most stable structure from MP
-        with MPRester(self.mapi_key) as mpr:
+        with MPRester(self.mapi_key) if self.mapi_key else MPRester() as mpr:
             struct_lst = mpr.get_data(comp.reduced_formula)
             if len(struct_lst) > 0:
                 most_stable_entry = sorted(struct_lst, key=lambda e: e["energy_per_atom"])[0]
                 try:
                     return [mpr.get_cohesive_energy(most_stable_entry["material_id"], per_atom=True)]
                 except Exception:
                     raise ValueError(
```

### Comparing `matminer-0.8.0/matminer/featurizers/conversions.py` & `matminer-0.9.0/matminer/featurizers/conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """
 
 import json
 
 from monty.json import MontyDecoder
 from pymatgen.core.composition import Composition
 from pymatgen.core.structure import IStructure
-from pymatgen.ext.matproj import MPRester
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from matminer.featurizers.base import BaseFeaturizer
 
 
 class ConversionFeaturizer(BaseFeaturizer):
     """
@@ -562,16 +561,22 @@
         overwrite_data (bool): Overwrite any data in `target_column` if it
             exists.
         map_key (str): Materials API key
 
     """
 
     def __init__(self, target_col_id="structure", overwrite_data=False, mapi_key=None):
+
+        from pymatgen.ext.matproj import MPRester
+
         super().__init__(target_col_id, overwrite_data)
-        self.mpr = MPRester(mapi_key)
+        if mapi_key:
+            self.mpr = MPRester(mapi_key)
+        else:
+            self.mpr = MPRester()
         self.set_n_jobs(1)
 
     def featurize(self, comp):
         """
         Get the most stable structure from Materials Project
         Args:
             comp (`pymatgen.core.composition.Composition`): A composition.
@@ -636,15 +641,14 @@
         target_col_id (str): Output column for the results. If not provided, the func name
             will be used.
         overwrite_data (bool): If True, will overwrite target_col_id even if there is
             data currently in that column
     """
 
     def __init__(self, func, func_args=None, func_kwargs=None, target_col_id=None, overwrite_data=False):
-
         if not callable(func):
             raise TypeError(f"Function {func} is not callable!")
 
         if not target_col_id:
             target_col_id = func.__name__
 
         super().__init__(target_col_id, overwrite_data)
```

### Comparing `matminer-0.8.0/matminer/featurizers/dos.py` & `matminer-0.9.0/matminer/featurizers/dos.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,15 +593,14 @@
     structure = dos.structure
     site = structure.sites[idx]
 
     # calculate s/p/d/f dos for cbm and vbm
     orbital_scores = {}
     proj = dos.get_site_spd_dos(site)
     for orb in proj:
-
         # smear dos for spin up and down
         smear_dos = proj[orb].get_smeared_densities(gaussian_smear)
         dos_up = smear_dos[Spin.up]
         dos_down = smear_dos[Spin.down] if Spin.down in smear_dos else smear_dos[Spin.up]
         dos_total = [sum(id) for id in zip(dos_up, dos_down)]
 
         # determine energy range to sample
```

### Comparing `matminer-0.8.0/matminer/featurizers/function.py` & `matminer-0.9.0/matminer/featurizers/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             representing a function of a single variable x, e. g.
             ["1 / x", "x ** 2"], defaults to the list above
         multi_feature_depth (int): how many features to include if using
             multiple fields for functionalization, e. g. 2 will
             include pairwise combined features
         postprocess (function or type): type to cast functional outputs
             to, if, for example, you want to include the possibility of
-            complex numbers in your outputs, use postprocess=np.complex,
+            complex numbers in your outputs, use postprocess=np.complex128,
             defaults to float
         combo_function (function): function to combine multi-features,
             defaults to np.prod (i.e. cumulative product of expressions),
             note that a combo function must cleanly process sympy
             expressions and **takes a list of arbitrary length as input**,
             other options include np.sum
         latexify_labels (bool): whether to render labels in latex,
@@ -80,15 +80,14 @@
         self,
         expressions=None,
         multi_feature_depth=1,
         postprocess=None,
         combo_function=None,
         latexify_labels=False,
     ):
-
         self.expressions = expressions or default_exps
         self.multi_feature_depth = multi_feature_depth
         self.combo_function = combo_function or np.prod
         self.latexify_labels = latexify_labels
         self.postprocess = postprocess or float
         self._feature_labels = None
```

### Comparing `matminer-0.8.0/matminer/featurizers/site/__init__.py` & `matminer-0.9.0/matminer/featurizers/site/__init__.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/bonding.py` & `matminer-0.9.0/matminer/featurizers/site/bonding.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/chemical.py` & `matminer-0.9.0/matminer/featurizers/site/chemical.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,19 @@
                                   np.array([[struct, site], [struct, site], …])
                             -Pandas dataframe:
                              e.g. df[['struct', 'site']]
             y : unused (added for consistency with overridden method signature)
         Returns:
             self
         """
+        if isinstance(X, (list, tuple)):
+            # Required for numpy 1.24 due to changes in the way numpy casts
+            # object arrays.
+            X = np.array(X, dtype=object)
+
         structs = np.atleast_2d(X)[:, 0]
         if not all([isinstance(struct, Structure) for struct in structs]):
             raise TypeError("This fit requires an array-like input of Pymatgen " "Structures and sites!")
 
         self.el_amt_dict_ = {}
         el_set_ = set()
         for s in structs:
```

### Comparing `matminer-0.8.0/matminer/featurizers/site/cn_target_motif_op.yaml` & `matminer-0.9.0/matminer/featurizers/site/cn_target_motif_op.yaml`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/external.py` & `matminer-0.9.0/matminer/featurizers/site/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,32 +144,32 @@
                 if e.Z not in elements:
                     elements.add(e.Z)
         self.elements_sorted = sorted(list(elements))
 
         self.atomic_numbers = elements
         self.soap = SOAP_dscribe(
             species=self.atomic_numbers,
-            rcut=self.rcut,
-            nmax=self.nmax,
-            lmax=self.lmax,
+            r_cut=self.rcut,
+            n_max=self.nmax,
+            l_max=self.lmax,
             sigma=self.sigma,
             rbf=self.rbf,
             periodic=self.periodic,
             crossover=self.crossover,
             average="off",
             sparse=False,
         )
 
         self.length = self.soap.get_number_of_features()
         return self
 
     def featurize(self, struct, idx):
         self._check_fitted()
         s_ase = self.adaptor.get_atoms(struct)
-        return self.soap.create(s_ase, positions=[idx], n_jobs=self.n_jobs).tolist()[0]
+        return self.soap.create(s_ase, centers=[idx], n_jobs=self.n_jobs).tolist()[0]
 
     def feature_labels(self):
         self._check_fitted()
         return [f"SOAP_{i}" for i in range(self.length)]
 
     def citations(self):
         return [
```

### Comparing `matminer-0.8.0/matminer/featurizers/site/fingerprint.py` & `matminer-0.9.0/matminer/featurizers/site/fingerprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,14 @@
         dr=0.1,
         ddr=0.01,
         ndr=1,
         dop=0.001,
         dist_exp=2,
         zero_ops=True,
     ):
-
         cn_target_motif_op = load_cn_target_motif_op()
         cn_motif_op_params = load_cn_motif_op_params()
 
         self.cn_target_motif_op = (
             copy.deepcopy(cn_target_motif_op) if target_motifs is None else copy.deepcopy(target_motifs)
         )
         self.dr = dr
@@ -417,15 +416,15 @@
         if chem_info is not None:
             self.chem_info = copy.deepcopy(chem_info)
             self.chem_props = list(chem_info.keys())
         else:
             self.chem_info = None
         cn_motif_op_params = load_cn_motif_op_params()
 
-        self.ops = {}  # load order parameter objects & paramaters
+        self.ops = {}  # load order parameter objects & parameters
         for cn, t_list in self.op_types.items():
             self.ops[cn] = []
             for t in t_list:
                 if t == "wt":
                     self.ops[cn].append(t)
                 else:
                     ot = t
```

### Comparing `matminer-0.8.0/matminer/featurizers/site/misc.py` & `matminer-0.9.0/matminer/featurizers/site/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         self.interstice_types = ["dist", "area", "vol"] if interstice_types is None else interstice_types
         if isinstance(self.interstice_types, str):
             self.interstice_types = [self.interstice_types]
         if all(t not in self.interstice_types for t in ["dist", "area", "vol"]):
             raise ValueError("interstice_types only support sub-list of " "['dist', 'area', 'vol']")
         self.stats = ["mean", "std_dev", "minimum", "maximum"] if stats is None else stats
         self.radius_type = radius_type
+        self.data_source = MagpieData()
 
     def featurize(self, struct, idx):
         """
         Get interstice distribution fingerprints of site with given index in
         input structure.
         Args:
             struct (Structure): Pymatgen Structure object.
@@ -74,17 +75,17 @@
 
         # Get the nearest neighbors using Voronoi tessellation
         n_w = VoronoiNN(cutoff=self.cutoff).get_voronoi_polyhedra(struct, idx).values()
 
         nn_coords = np.array([nn["site"].coords for nn in n_w])
 
         # Get center atom's radius and its nearest neighbors' radii
-        center_r = MagpieData().get_elemental_properties([struct[idx].specie], self.radius_type)[0] / 100
+        center_r = self.data_source.get_elemental_properties([struct[idx].specie], self.radius_type)[0] / 100
         nn_els = [nn["site"].specie for nn in n_w]
-        nn_rs = np.array(MagpieData().get_elemental_properties(nn_els, self.radius_type)) / 100
+        nn_rs = np.array(self.data_source.get_elemental_properties(nn_els, self.radius_type)) / 100
 
         # Get indices of atoms forming the simplices of convex hull
         convex_hull_simplices = ConvexHull(nn_coords).simplices
 
         if "dist" in self.interstice_types:
             nn_dists = [nn["face_dist"] * 2 for nn in n_w]
             interstice_dist_list = IntersticeDistribution.analyze_dist_interstices(center_r, nn_rs, nn_dists)
```

### Comparing `matminer-0.8.0/matminer/featurizers/site/rdf.py` & `matminer-0.9.0/matminer/featurizers/site/rdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
             (float) Gaussian angular symmetry function for all combinations of eta, zeta, gamma
         """
 
         output = np.zeros((len(etas) * len(zetas) * len(gammas),))
 
         # Loop over each neighbor j
         for j, neigh_j in enumerate(neigh_coords):
-
             # Compute the distance of each neighbor (k) to r
             r_ij = neigh_dist[j]
             d_jk = neigh_coords[(j + 1) :] - neigh_coords[j]
             r_jk = np.linalg.norm(d_jk, 2, axis=1)
             r_ik = neigh_dist[(j + 1) :]
 
             # Compute the cosine term
@@ -205,18 +204,18 @@
 
     1. GRDF: (recommended) - n_bins length vector
         In GRDF mode, The GRDF is computed by considering all sites around a
         central site (i.e., no sites are omitted when computing the GRDF). The
         features output from this mode will be vectors with length n_bins.
 
     2. pairwise GRDF: (advanced users) - n_bins x n_sites matrix
-        In this mode, GRDFs are are still computed around a central site, but
+        In this mode, GRDFs are still computed around a central site, but
         only one other site (and their translational equivalents) are used to
         compute a GRDF (e.g. site 1 with site 2 and the translational
-        equivalents of site 2). This results in a a n_sites x n_bins matrix of
+        equivalents of site 2). This results in a n_sites x n_bins matrix of
         features. Requires `fit` for determining the max number of sites for
 
     The GRDF is a generalization of the partial radial distribution function
     (PRDF). In contrast with the PRDF, the bins of the GRDF are not mutually-
     exclusive and need not carry a constant weight of 1. The PRDF is a case of
     the GRDF when the bins are rectangular functions. Examples of other
     functions to use with the GRDF are Gaussian, trig, and Bessel functions.
@@ -249,15 +248,15 @@
     def fit(self, X, y=None, **fit_kwargs):
         """
         Determine the maximum number of sites in X to assign correct feature
         labels
 
         Args:
             X - [list of tuples], training data
-                tuple values should be (struc, idx)
+                tuple values should be (struct, idx)
         Returns:
             self
         """
 
         max_sites = max(len(X[i][0]._sites) for i in range(len(X)))
         self.fit_labels = [f"site2 {i} {bin.name()}" for bin in self.bins for i in range(max_sites)]
         return self
```

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/base.py` & `matminer-0.9.0/matminer/featurizers/site/tests/base.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/test_bonding.py` & `matminer-0.9.0/matminer/featurizers/site/tests/test_bonding.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/test_chemical.py` & `matminer-0.9.0/matminer/featurizers/site/tests/test_chemical.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/test_external.py` & `matminer-0.9.0/matminer/featurizers/site/tests/test_external.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/test_fingerprint.py` & `matminer-0.9.0/matminer/featurizers/site/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/test_misc.py` & `matminer-0.9.0/matminer/featurizers/site/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/site/tests/test_rdf.py` & `matminer-0.9.0/matminer/featurizers/site/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/__init__.py` & `matminer-0.9.0/matminer/featurizers/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/bonding.py` & `matminer-0.9.0/matminer/featurizers/structure/bonding.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,14 @@
                 abonds_data[lb] += local_bonds[lb]
             else:
                 lbs = self._species_from_bondstr(lb)
 
                 nearest = []
                 d_min = None
                 for abss in abonds_species.keys():
-
                     # The distance between bonds is euclidean. To get a good
                     # measure of the coordinate between mendeleev numbers for
                     # each specie, we use the minimum difference. ie, for
                     # finding the distance between Na-O and O-Li, we would
                     # not want the distance between (Na and O) and (O and Li),
                     # we want the distance between (Na and Li) and (O and O).
 
@@ -711,15 +710,14 @@
     Features:
         The global instability index is the square root of the sum of squared
             differences of the bond valence sums from the formal valences
             averaged over all atoms in the unit cell.
     """
 
     def __init__(self, r_cut=4.0, disordered_pymatgen=False):
-
         bv = IUCrBondValenceData()
         self.bv_values = bv.params
         self.r_cut = r_cut
         self.disordered_pymatgen = disordered_pymatgen
 
     def precheck(self, struct):
         """
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/composite.py` & `matminer-0.9.0/matminer/featurizers/structure/composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         use_chem=True,
         use_chg=True,
         use_rdf=True,
         use_adf=True,
         use_ddf=True,
         use_nn=True,
     ):
-
         self.use_cell = use_cell
         self.use_chem = use_chem
         self.use_chg = use_chg
         self.use_adf = use_adf
         self.use_rdf = use_rdf
         self.use_ddf = use_ddf
         self.use_nn = use_nn
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/matrix.py` & `matminer-0.9.0/matminer/featurizers/structure/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             elif curr_shell[1] == "d":
                 l = 2
             elif curr_shell[1] == "f":
                 l = 3
             ohd[l][curr_shell[2]] = 1
             nume += curr_shell[2]
             shell_num += 1
-        my_ohv = np.zeros(self.size, np.int)
+        my_ohv = np.zeros(self.size, np.int32)
         k = 0
         for j in range(4):
             for i in range(2 * (2 * j + 1)):
                 my_ohv[k] = ohd[j][i + 1]
                 k += 1
         if period_tag:
             row = sp.row
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/misc.py` & `matminer-0.9.0/matminer/featurizers/structure/misc.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/order.py` & `matminer-0.9.0/matminer/featurizers/structure/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     def __init__(self, desired_features=None):
         """
         Args:
             desired_features: [str] - choose from "density", "vpa",
                 "packing fraction"
         """
+        self.desired_features = desired_features
         self.features = ["density", "vpa", "packing fraction"] if not desired_features else desired_features
 
     def precheck(self, s: Structure) -> bool:
         """
         Precheck a single entry. DensityFeatures does not work for disordered
         structures. To precheck an entire dataframe (qnd automatically gather
         the fraction of structures that will pass the precheck), please use
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/rdf.py` & `matminer-0.9.0/matminer/featurizers/structure/rdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 
         # Make structure primitive.
         struct = SpacegroupAnalyzer(s).find_primitive() or s
 
         # Add oxidation states.
         struct = ValenceIonicRadiusEvaluator(struct).structure
 
-        distribution = np.zeros(self.nbins, dtype=np.float)
+        distribution = np.zeros(self.nbins, dtype=np.float64)
 
         for site in struct.sites:
             this_charge = float(site.specie.oxi_state)
             neighbors = struct.get_neighbors(site, self.cutoff)
             for nnsite, dist, *_ in neighbors:
                 neigh_charge = float(nnsite.specie.oxi_state)
                 bin_index = int(dist / self.dr)
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/sites.py` & `matminer-0.9.0/matminer/featurizers/structure/sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class SiteStatsFingerprint(BaseFeaturizer):
     """
     Computes statistics of properties across all sites in a structure.
 
     This featurizer first uses a site featurizer class (see site.py for
     options) to compute features of each site in a structure, and then computes
     features of the entire structure by measuring statistics of each attribute.
-    Can optionally compute the the statistics of only sites with certain ranges
+    Can optionally compute the statistics of only sites with certain ranges
     of oxidation states (e.g., only anions).
 
     Features:
         - Returns each statistic of each site feature
     """
 
     def __init__(
@@ -51,15 +51,15 @@
             min_oxi (int): minimum site oxidation state for inclusion (e.g.,
                 zero means metals/cations only)
             max_oxi (int): maximum site oxidation state for inclusion
             covariance (bool): Whether to compute the covariance of site features
         """
 
         self.site_featurizer = site_featurizer
-        self.stats = tuple([stats]) if type(stats) == str else stats
+        self.stats = tuple([stats]) if isinstance(stats, str) else stats
         if self.stats and "_mode" in "".join(self.stats):
             nmodes = 0
             for stat in self.stats:
                 if "_mode" in stat and int(stat[0]) > nmodes:
                     nmodes = int(stat[0])
             self.nmodes = nmodes
 
@@ -326,15 +326,14 @@
         for e in self.elements_:
             pssf_stats = self.compute_pssf(s, e)
             output.append(pssf_stats)
 
         return np.hstack(output)
 
     def compute_pssf(self, s, e):
-
         # This code is extremely similar to super().featurize(). The key
         # difference is that only one specific element is analyzed.
 
         # Get each feature for each site
         vals = [[] for t in self._site_labels]
         for i, site in enumerate(s.sites):
             if site.specie.symbol == e:
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/symmetry.py` & `matminer-0.9.0/matminer/featurizers/structure/symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         "hexagonal": 2,
         "cubic": 1,
     }
 
     all_features = ["spacegroup_num", "crystal_system", "crystal_system_int", "is_centrosymmetric", "n_symmetry_ops"]
 
     def __init__(self, desired_features=None):
+        self.desired_features = desired_features
         self.features = desired_features if desired_features else self.all_features
 
     def featurize(self, s):
         sga = SpacegroupAnalyzer(s)
         output = []
 
         if "spacegroup_num" in self.features:
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/Cs2CeN5O17_mp-1198000_computed.cif` & `matminer-0.9.0/matminer/featurizers/structure/tests/Cs2CeN5O17_mp-1198000_computed.cif`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/Dy2HfS5_mp-1198001_computed.cif` & `matminer-0.9.0/matminer/featurizers/structure/tests/Dy2HfS5_mp-1198001_computed.cif`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/JarvisCFID_problem_file.json` & `matminer-0.9.0/matminer/featurizers/structure/tests/JarvisCFID_problem_file.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/base.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/base.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_bonding.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_bonding.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 )
 from matminer.featurizers.structure.matrix import CoulombMatrix, SineCoulombMatrix
 from matminer.featurizers.structure.tests.base import StructureFeaturesTest
 
 
 class BondingStructureTest(StructureFeaturesTest):
     def test_bondfractions(self):
-
         # Test individual structures with featurize
         bf_md = BondFractions.from_preset("MinimumDistanceNN")
         bf_md.no_oxi = True
         bf_md.fit([self.diamond_no_oxi])
         self.assertArrayEqual(bf_md.featurize(self.diamond), [1.0])
         self.assertArrayEqual(bf_md.featurize(self.diamond_no_oxi), [1.0])
 
@@ -58,15 +57,14 @@
         df = bf_voronoi.featurize_dataframe(df, "s")
         self.assertArrayEqual(df["C - C bond frac."].to_numpy(), [1.0, 0.0])
         self.assertArrayEqual(df["Al - Ni bond frac."].to_numpy(), [0.0, 0.5])
         self.assertArrayEqual(df["Al - Al bond frac."].to_numpy(), [0.0, 0.0])
         self.assertArrayEqual(df["Ni - Ni bond frac."].to_numpy(), [0.0, 0.5])
 
     def test_bob(self):
-
         # Test a single fit and featurization
         scm = SineCoulombMatrix(flatten=False)
         bob = BagofBonds(coulomb_matrix=scm, token=" - ")
         bob.fit([self.ni3al])
         truth1 = [
             235.74041833262768,
             1486.4464890775491,
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_composite.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_matrix.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_misc.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         self.assertArrayAlmostEqual(comp.featurize(self.nacl.composition), features)
 
         # Test the citations/implementors
         self.assertEqual(comp.citations(), f.citations())
         self.assertEqual(comp.implementors(), f.implementors())
 
     def test_xrd_powderPattern(self):
-
         # default settings test
         xpp = XRDPowderPattern()
         pattern = xpp.featurize(self.diamond)
         self.assertAlmostEqual(pattern[44], 0.19378, places=2)
         self.assertEqual(len(pattern), 128)
 
         # reduced range
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_order.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_rdf.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_sites.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_sites.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 
 from matminer.featurizers.site import SiteElementalProperty
 from matminer.featurizers.structure.sites import (
-    SiteStatsFingerprint,
     PartialsSiteStatsFingerprint,
+    SiteStatsFingerprint,
 )
 from matminer.featurizers.structure.tests.base import StructureFeaturesTest
 
 
 class StructureSitesFeaturesTest(StructureFeaturesTest):
     def test_sitestatsfingerprint(self):
         # Test matrix.
```

### Comparing `matminer-0.8.0/matminer/featurizers/structure/tests/test_symmetry.py` & `matminer-0.9.0/matminer/featurizers/structure/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/VBr2_971787_bandstructure.json` & `matminer-0.9.0/matminer/featurizers/tests/VBr2_971787_bandstructure.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/nb3sn_dos.json` & `matminer-0.9.0/matminer/featurizers/tests/nb3sn_dos.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/si_bandstructure_line.json` & `matminer-0.9.0/matminer/featurizers/tests/si_bandstructure_line.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/si_bandstructure_uniform.json` & `matminer-0.9.0/matminer/featurizers/tests/si_bandstructure_uniform.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/si_dos.json` & `matminer-0.9.0/matminer/featurizers/tests/si_dos.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/si_structure.json` & `matminer-0.9.0/matminer/featurizers/tests/si_structure.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/test_bandstructure.py` & `matminer-0.9.0/matminer/featurizers/tests/test_bandstructure.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/test_base.py` & `matminer-0.9.0/matminer/featurizers/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,14 @@
     def test_ignore_errors(self):
         # Make sure multiplefeaturizer returns the correct sub-featurizer multiindex keys
 
         # Iterate through many tests: single/parallel, returning errors or not,
         # multiindex or not, and interaction over entries/featurizers
 
         for mi, re, n, iter_entries in product([True, False], [True, False], [1, 2], [True, False]):
-
             mf = MultipleFeaturizer([self.multi, self.single], iterate_over_entries=iter_entries)
             # Make some test data that will cause errors
             data = pd.DataFrame({"x": ["a", 2, 3]})
 
             # Set the number of threads
             mf.set_n_jobs(n)
```

### Comparing `matminer-0.8.0/matminer/featurizers/tests/test_conversions.py` & `matminer-0.9.0/matminer/featurizers/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/tests/test_dos.py` & `matminer-0.9.0/matminer/featurizers/tests/test_dos.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         self.df = pd.DataFrame({"dos": [si_dos], "site": [0]})
 
         with open(os.path.join(test_dir, "nb3sn_dos.json")) as sDOS:
             nb3sn_dos = CompleteDos.from_dict(json.load(sDOS))
         self.nb3sn_df = pd.DataFrame({"dos": [nb3sn_dos]})
 
     def test_SiteDOS(self):
-
         dos = self.df["dos"][0]
 
         # ensure that both sites give same scores (expected behavior for si)
         features0 = SiteDOS(decay_length=0.1).featurize(dos, 0)
         features1 = SiteDOS(decay_length=0.1).featurize(dos, 1)
         self.assertArrayEqual(features0, features1)
```

### Comparing `matminer-0.8.0/matminer/featurizers/tests/test_function.py` & `matminer-0.9.0/matminer/featurizers/tests/test_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         ff = FunctionFeaturizer(expressions=expressions, multi_feature_depth=3)
         new_df = ff.fit_featurize_dataframe(self.test_df, ["a", "b", "c"], inplace=False)
         new_df = new_df.dropna()
         self.assertTrue(np.allclose(new_df["1/a"] * new_df["1/b"] * new_df["1/c"], new_df["1/(a*b*c)"]))
 
         # Test complex functionality
         expressions = ["sqrt(x)"]
-        ff = FunctionFeaturizer(expressions=expressions, postprocess=np.complex)
+        ff = FunctionFeaturizer(expressions=expressions, postprocess=np.complex128)
         new_df = ff.fit_featurize_dataframe(self.test_df, "a", inplace=False)
         self.assertEqual(new_df["sqrt(a)"][0], 1j)
 
         ff = FunctionFeaturizer(expressions=expressions, multi_feature_depth=2, combo_function=np.sum)
         new_df = ff.fit_featurize_dataframe(self.test_df, ["a", "b"], inplace=False)
         self.assertAlmostEqual(new_df["sqrt(a) + sqrt(b)"][2], 2.41421356)
```

### Comparing `matminer-0.8.0/matminer/featurizers/utils/grdf.py` & `matminer-0.9.0/matminer/featurizers/utils/grdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self.start = start
         self.width = width
 
     def __call__(self, r_ij):
         return np.logical_and(
             np.greater_equal(r_ij, self.start),
             np.less(r_ij, self.start + self.width),
-            dtype=np.float,
+            dtype=np.float64,
         )
 
     def volume(self, cutoff):
         return 4.0 / 3 * np.pi * (min(self.start + self.width, cutoff) ** 3 - self.start**3)
 
 
 class Gaussian(AbstractPairwise):
```

### Comparing `matminer-0.8.0/matminer/featurizers/utils/stats.py` & `matminer-0.9.0/matminer/featurizers/utils/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     computing the mean of a list looks like::
 
         x = [1, 2, 3]
         PropertyStats.calc_stat(x, 'mean') # Result is 2
         PropertyStats.calc_stat(x, 'mean', weights=[0, 0, 1]) # Result is 3
 
     Some of the statistics functions take options (e.g., Holder means). You can
-    pass them to the the statistics functions by adding them after the name and
+    pass them to the statistics functions by adding them after the name and
     two colons. For example, the 0th Holder mean would be::
 
         PropertyStats.calc_stat(x, 'holder_mean::0')
 
     You can, of course, call the statistical functions directly. All take at
     least two arguments.  The first is the data being assessed and the second,
     optional, argument is the weights.
```

### Comparing `matminer-0.8.0/matminer/featurizers/utils/tests/test_grdf.py` & `matminer-0.9.0/matminer/featurizers/utils/tests/test_grdf.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/featurizers/utils/tests/test_stats.py` & `matminer-0.9.0/matminer/featurizers/utils/tests/test_stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,21 @@
             statistic: name of statistic
             sample_1: float, expected value for statistic of sample 1 without weights
             sample_1_weighted: float, expected value for statistic of sample 1 with weights
             sample_2: float, expected value for statistic of sample 2 without weights
             sample_2_weighted: float, expected value for statistic of sample 2 with weights
         """
 
-        self.assertAlmostEqual(sample_1, PropertyStats.calc_stat(self.sample_1, statistic))
-        self.assertAlmostEqual(
+        np.testing.assert_almost_equal(sample_1, PropertyStats.calc_stat(self.sample_1, statistic))
+        np.testing.assert_almost_equal(
             sample_1_weighted,
             PropertyStats.calc_stat(self.sample_1, statistic, self.sample_1_weights),
         )
-        self.assertAlmostEqual(sample_2, PropertyStats.calc_stat(self.sample_2, statistic))
-        self.assertAlmostEqual(
+        np.testing.assert_almost_equal(sample_2, PropertyStats.calc_stat(self.sample_2, statistic))
+        np.testing.assert_almost_equal(
             sample_2_weighted,
             PropertyStats.calc_stat(self.sample_2, statistic, self.sample_2_weights),
         )
 
     def test_minimum(self):
         self._run_test("minimum", 1, 1, 0, 0)
 
@@ -50,18 +50,18 @@
     def test_avg_dev(self):
         self._run_test("avg_dev", 0, 0, 5.0 / 9, 0.448979592)
 
     def test_std_dev(self):
         self._run_test("std_dev", 0, 0, 0.623609564, 0.694365075)
 
     def test_skewness(self):
-        self._run_test("skewness", 0, 0, 0.38180177, 0.559451361)
+        self._run_test("skewness", np.nan, 0, 0.38180177, 0.559451361)
 
     def test_kurtosis(self):
-        self._run_test("kurtosis", 0, 0, 1.5, 1.9403292181)
+        self._run_test("kurtosis", np.nan, 0, 1.5, 1.9403292181)
 
     def test_mode(self):
         self._run_test("mode", 1, 1, 0, 0.5)
 
         # Additional tests
         self.assertAlmostEqual(0, PropertyStats.mode([0, 1, 2], [1, 1, 1]))
```

### Comparing `matminer-0.8.0/matminer/utils/caching.py` & `matminer-0.9.0/matminer/utils/caching.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data.py` & `matminer-0.9.0/matminer/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
         Args:
             elem - (Element) element to be assessed
             property_name - (str) property to be retrieved
         Returns:
             float, property of that element
         """
-        pass
 
     def get_elemental_properties(self, elems, property_name):
         """Get elemental properties for a list of elements
 
         Args:
             elems - ([Element]) list of elements
             property_name - (str) property to be retrieved
@@ -57,15 +56,14 @@
         """Retrieve the possible oxidation states of an element
 
         Args:
             elem - (Element), Target element
         Returns:
             [int] - oxidation states
         """
-        pass
 
 
 class OxidationStateDependentData(AbstractData):
     """Abstract class that also includes oxidation-state-dependent properties"""
 
     @abc.abstractmethod
     def get_charge_dependent_property(self, element, charge, property_name):
@@ -74,15 +72,14 @@
         Args:
             element - (Element), Target element
             charge - (int), Oxidation state
             property_name - (string), name of property
         Return:
             (float) - Value of property
         """
-        pass
 
     def get_charge_dependent_property_from_specie(self, specie, property_name):
         """Retrieve a oxidation-state dependent elemental property
 
         Args:
             specie - (Specie), Specie of interest
             property_name - (string), name of property
```

### Comparing `matminer-0.8.0/matminer/utils/data_files/Miedema.csv` & `matminer-0.9.0/matminer/utils/data_files/Miedema.csv`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/MiedemaLiquidDeltaHf.tsv` & `matminer-0.9.0/matminer/utils/data_files/MiedemaLiquidDeltaHf.tsv`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/bvparm2016.cif` & `matminer-0.9.0/matminer/utils/data_files/bvparm2016.cif`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/bvparm2020.cif` & `matminer-0.9.0/matminer/utils/data_files/bvparm2020.cif`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/cgcnn_atom_feature.json` & `matminer-0.9.0/matminer/utils/data_files/cgcnn_atom_feature.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/cohesive_energies.json` & `matminer-0.9.0/matminer/utils/data_files/cohesive_energies.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/deml_elementdata.py` & `matminer-0.9.0/matminer/utils/data_files/deml_elementdata.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/jarvis/element_charges.json` & `matminer-0.9.0/matminer/utils/data_files/jarvis/element_charges.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/jarvis/element_chem.json` & `matminer-0.9.0/matminer/utils/data_files/jarvis/element_chem.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AllenElectronegativity.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AllenElectronegativity.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AtomicVolume.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AtomicVolume.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/AtomicWeight.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/AtomicWeight.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/BoilingT.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/BoilingT.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/BulkModulus.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/BulkModulus.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Column.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Column.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/CovalentRadius.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/CovalentRadius.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Density.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Density.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/DipolePolarizability.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/DipolePolarizability.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ElectronAffinity.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ElectronAffinity.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Electronegativity.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Electronegativity.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/FirstIonizationEnergy.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/FirstIonizationEnergy.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/FusionEnthalpy.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/FusionEnthalpy.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSbandgap.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSbandgap.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSenergy_pa.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSenergy_pa.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSestBCClatcnt.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSestBCClatcnt.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSestFCClatcnt.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSestFCClatcnt.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSmagmom.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSmagmom.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/GSvolume_pa.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/GSvolume_pa.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HHIp.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HHIp.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HHIr.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HHIr.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMass.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMass.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMolar.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatCapacityMolar.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatFusion.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatFusion.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/HeatVaporization.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/HeatVaporization.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ICSDVolume.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ICSDVolume.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/IonizationEnergies.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/IonizationEnergies.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/LogThermalConductivity.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/LogThermalConductivity.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MeltingT.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MeltingT.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MendeleevNumber.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MendeleevNumber.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MiracleRadius.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MiracleRadius.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/MolarVolume.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/MolarVolume.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NUnfilled.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NUnfilled.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NValence.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NValence.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NdUnfilled.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NdUnfilled.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NdValence.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NdValence.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NfUnfilled.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NfUnfilled.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/NfValence.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/NfValence.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Number.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Number.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/OxidationStates.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/OxidationStates.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/Polarizability.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/Polarizability.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/README.txt` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/README.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/SecondIonizationEnergy.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/SecondIonizationEnergy.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ShearModulus.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ShearModulus.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/SpaceGroupNumber.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/SpaceGroupNumber.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ThermalConductivity.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ThermalConductivity.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_d.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_d.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_p.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_p.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_pi.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_pi.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_s.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_s.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_sigma.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/ZungerPP-r_sigma.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/n_ws^third.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/n_ws^third.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata/phi.table` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata/phi.table`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/magpie_elementdata_feature_descriptions.txt` & `matminer-0.9.0/matminer/utils/data_files/magpie_elementdata_feature_descriptions.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/matscholar_els.json` & `matminer-0.9.0/matminer/utils/data_files/matscholar_els.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/data_files/megnet_elemental_embedding.json` & `matminer-0.9.0/matminer/utils/data_files/megnet_elemental_embedding.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/flatten_dict.py` & `matminer-0.9.0/matminer/utils/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/io.py` & `matminer-0.9.0/matminer/utils/io.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/kernels.py` & `matminer-0.9.0/matminer/utils/kernels.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/pipeline.py` & `matminer-0.9.0/matminer/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/tests/dataframe.json` & `matminer-0.9.0/matminer/utils/tests/dataframe.json`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/tests/test_caching.py` & `matminer-0.9.0/matminer/utils/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/tests/test_data.py` & `matminer-0.9.0/matminer/utils/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/tests/test_flatten_dict.py` & `matminer-0.9.0/matminer/utils/tests/test_flatten_dict.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer/utils/tests/test_io.py` & `matminer-0.9.0/matminer/utils/tests/test_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
             to_unit_cell=False,
             coords_are_cartesian=True,
             site_properties=None,
         )
         self.df = pd.DataFrame(data={"structure": [self.diamond]})
 
     def test_store_dataframe_as_json(self):
-
         # check write produces correct file
         temp_file = os.path.join(self.temp_folder, "test_dataframe.json")
         test_file = os.path.join(test_dir, "dataframe.json")
         store_dataframe_as_json(self.df, temp_file)
 
         with zopen(temp_file, "rb") as f:
             temp_data = json.load(f)
@@ -117,15 +116,14 @@
 
         temp_data["data"][0][0].pop("@version")
         test_data["data"][0][0].pop("@version")
 
         self.assertDictsAlmostEqual(temp_data, test_data)
 
     def test_load_dataframe_from_json(self):
-
         df = load_dataframe_from_json(os.path.join(test_dir, "dataframe.json"))
         self.assertTrue(self.diamond == df["structure"][0], "Dataframe contents do not match")
 
         df = load_dataframe_from_json(os.path.join(test_dir, "dataframe.json.gz"))
         self.assertTrue(self.diamond == df["structure"][0], "Dataframe contents do not match")
 
         df = load_dataframe_from_json(os.path.join(test_dir, "dataframe.json.bz2"))
```

### Comparing `matminer-0.8.0/matminer/utils/utils.py` & `matminer-0.9.0/matminer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/matminer.egg-info/PKG-INFO` & `matminer-0.9.0/matminer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: matminer
-Version: 0.8.0
+Version: 0.9.0
 Summary: matminer is a library that contains tools for data mining in Materials Science
 Home-page: https://github.com/hackingmaterials/matminer
 Author: Anubhav Jain
 Author-email: anubhavster@gmail.com
 License: modified BSD
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
 Provides-Extra: mpds
 Provides-Extra: dscribe
 Provides-Extra: mdfforge
 Provides-Extra: aflow
 Provides-Extra: citrine
 Provides-Extra: dev
+Provides-Extra: tests
 License-File: LICENSE
 
 # <img alt="matminer" src="docs_rst/_static/matminer_logo_small.png" width="300">
 
 matminer is a library for performing data mining in the field of materials science.
 
 - **[Website (including documentation)](https://hackingmaterials.github.io/matminer/)**
-- **[Examples Repository](https://github.com/hackingmaterials/matminer_examples)** 
-- **[Help/Support Forum](https://matsci.org/c/matminer/16)** 
-- **[Source Repository](https://github.com/hackingmaterials/matminer)** 
+- **[Examples Repository](https://github.com/hackingmaterials/matminer_examples)**
+- **[Help/Support Forum](https://matsci.org/c/matminer/16)**
+- **[Source Repository](https://github.com/hackingmaterials/matminer)**
 
 matminer supports Python 3.8+.
 
 #### Related packages:
 
 - If you like matminer, you might also try [automatminer](https://github.com/hackingmaterials/automatminer).
 - If you are interested in furthering development of datasets in matminer, you may be interested in [matbench](https://github.com/hackingmaterials/matbench).
@@ -51,8 +53,8 @@
 materials data mining. Comput. Mater. Sci. 152, 60-69 (2018).
 ```
 
 Matminer helps users apply methods and data sets developed by the community. Please also cite the original sources, as this will add clarity to your article and credit the original authors:
 
 - If you use one or more **datasets** accessed through matminer, check the dataset metadata info for relevant citations on the original datasets.
 - If you use one or more **data retrieval methods**, check ``citations()`` method of the data retrieval class. This method will provide a list of BibTeX-formatted citations for that featurizer, making it easy to keep track of and cite the original publications.
-- If you use one or more **featurizers**, please take advantage of the ```citations()``` function present for every featurizer in matminer. 
+- If you use one or more **featurizers**, please take advantage of the ```citations()``` function present for every featurizer in matminer.
```

### Comparing `matminer-0.8.0/matminer.egg-info/SOURCES.txt` & `matminer-0.9.0/matminer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pylintrc
 pyproject.toml
 setup.cfg
 setup.py
-tasks.py
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/upgrade-dependencies.yml
 dev_scripts/dataset_management/generate_datasets.py
 dev_scripts/dataset_management/modify_dataset_metadata.py
```

### Comparing `matminer-0.8.0/pylintrc` & `matminer-0.9.0/pylintrc`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/macos-latest_py3.10.txt` & `matminer-0.9.0/requirements/macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/macos-latest_py3.10_extras.txt` & `matminer-0.9.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with python 3.10
 # To update, run:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 aflow==0.0.11
     # via matminer (setup.py)
 alabaster==0.7.12
     # via sphinx
 ase==3.22.1
     # via
@@ -54,15 +54,15 @@
     # via pylint
 dnspython==2.2.1
     # via pymongo
 docopt==0.6.2
     # via coveralls
 docutils==0.19
     # via sphinx
-dscribe==1.2.2
+dscribe==2.0.0
     # via matminer (setup.py)
 emmet-core==0.38.9
     # via mp-api
 exceptiongroup==1.0.1
     # via pytest
 fair-research-login==0.3.0
     # via mdf-toolbox
@@ -223,14 +223,16 @@
     # via jsonschema
 pytest==7.2.0
     # via
     #   matminer (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via matminer (setup.py)
+pytest-timeout==2.1.0
+    # via matminer (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
 pytz==2022.6
     # via
     #   babel
```

### Comparing `matminer-0.8.0/requirements/macos-latest_py3.8.txt` & `matminer-0.9.0/requirements/macos-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/macos-latest_py3.8_extras.txt` & `matminer-0.9.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     # via pylint
 dnspython==2.2.1
     # via pymongo
 docopt==0.6.2
     # via coveralls
 docutils==0.19
     # via sphinx
-dscribe==1.2.2
+dscribe==2.0.0
     # via matminer (setup.py)
 emmet-core==0.38.9
     # via mp-api
 exceptiongroup==1.0.1
     # via pytest
 fair-research-login==0.3.0
     # via mdf-toolbox
@@ -229,14 +229,16 @@
     # via jsonschema
 pytest==7.2.0
     # via
     #   matminer (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via matminer (setup.py)
+pytest-timeout==2.1.0
+    # via matminer (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
 pytz==2022.6
     # via
     #   babel
```

### Comparing `matminer-0.8.0/requirements/macos-latest_py3.9.txt` & `matminer-0.9.0/requirements/macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/macos-latest_py3.9_extras.txt` & `matminer-0.9.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     # via pylint
 dnspython==2.2.1
     # via pymongo
 docopt==0.6.2
     # via coveralls
 docutils==0.19
     # via sphinx
-dscribe==1.2.2
+dscribe==2.0.0
     # via matminer (setup.py)
 emmet-core==0.38.9
     # via mp-api
 exceptiongroup==1.0.1
     # via pytest
 fair-research-login==0.3.0
     # via mdf-toolbox
@@ -225,14 +225,16 @@
     # via jsonschema
 pytest==7.2.0
     # via
     #   matminer (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via matminer (setup.py)
+pytest-timeout==2.1.0
+    # via matminer (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
 pytz==2022.6
     # via
     #   babel
```

### Comparing `matminer-0.8.0/requirements/ubuntu-latest_py3.10.txt` & `matminer-0.9.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/ubuntu-latest_py3.10_extras.txt` & `matminer-0.9.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with python 3.10
 # To update, run:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
 #
 aflow==0.0.11
     # via matminer (setup.py)
 alabaster==0.7.12
     # via sphinx
 ase==3.22.1
     # via
@@ -54,15 +54,15 @@
     # via pylint
 dnspython==2.2.1
     # via pymongo
 docopt==0.6.2
     # via coveralls
 docutils==0.19
     # via sphinx
-dscribe==1.2.2
+dscribe==2.0.0
     # via matminer (setup.py)
 emmet-core==0.38.9
     # via mp-api
 exceptiongroup==1.0.1
     # via pytest
 fair-research-login==0.3.0
     # via mdf-toolbox
@@ -223,14 +223,16 @@
     # via jsonschema
 pytest==7.2.0
     # via
     #   matminer (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via matminer (setup.py)
+pytest-timeout==2.1.0
+    # via matminer (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
 pytz==2022.6
     # via
     #   babel
```

### Comparing `matminer-0.8.0/requirements/ubuntu-latest_py3.8.txt` & `matminer-0.9.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/ubuntu-latest_py3.8_extras.txt` & `matminer-0.9.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     # via pylint
 dnspython==2.2.1
     # via pymongo
 docopt==0.6.2
     # via coveralls
 docutils==0.19
     # via sphinx
-dscribe==1.2.2
+dscribe==2.0.0
     # via matminer (setup.py)
 emmet-core==0.38.9
     # via mp-api
 exceptiongroup==1.0.1
     # via pytest
 fair-research-login==0.3.0
     # via mdf-toolbox
@@ -229,14 +229,16 @@
     # via jsonschema
 pytest==7.2.0
     # via
     #   matminer (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via matminer (setup.py)
+pytest-timeout==2.1.0
+    # via matminer (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
 pytz==2022.6
     # via
     #   babel
```

### Comparing `matminer-0.8.0/requirements/ubuntu-latest_py3.9.txt` & `matminer-0.9.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `matminer-0.8.0/requirements/ubuntu-latest_py3.9_extras.txt` & `matminer-0.9.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     # via pylint
 dnspython==2.2.1
     # via pymongo
 docopt==0.6.2
     # via coveralls
 docutils==0.19
     # via sphinx
-dscribe==1.2.2
+dscribe==2.0.0
     # via matminer (setup.py)
 emmet-core==0.38.9
     # via mp-api
 exceptiongroup==1.0.1
     # via pytest
 fair-research-login==0.3.0
     # via mdf-toolbox
@@ -225,14 +225,16 @@
     # via jsonschema
 pytest==7.2.0
     # via
     #   matminer (setup.py)
     #   pytest-cov
 pytest-cov==4.0.0
     # via matminer (setup.py)
+pytest-timeout==2.1.0
+    # via matminer (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
 pytz==2022.6
     # via
     #   babel
```

### Comparing `matminer-0.8.0/setup.cfg` & `matminer-0.9.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 upload-dir = docs/_build/html
 
 [aliases]
 upload_docs = upload_docs --upload-dir=docs/_build/html
 release = register sdist upload
 
 [pycodestyle]
-count = True
+count = true
 ignore = E121,E123,E126,E133,E226,E241,E242,E704,W503,W504,W505,E741,W605,W293,W291,W292,E203,E231
 max-line-length = 120
-statistics = True
+statistics = true
 exclude = docs_rst/*.py
 
 [flake8]
 exclude = .git,__pycache__,docs_rst/conf.py,tests
 extend-ignore = E741,W291,W293,E501,E231,E203
 max-line-length = 120
 per-file-ignores = 
@@ -37,16 +37,23 @@
 	raise AssertionError
 	raise NotImplementedError
 	if 0:
 	if __name__ == .__main__.:
 	@deprecated
 
 [mypy]
-ignore_missing_imports = True
+ignore_missing_imports = true
 
 [isort]
 profile = black
 
+[autoflake]
+in-place = true
+remove-unused-variables = true
+remove-all-unused-imports = true
+expand-star-imports = true
+ignore-init-module-imports = true
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `matminer-0.8.0/setup.py` & `matminer-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,64 +10,74 @@
     return ""
 
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
 extras_require = {
     "mpds": ["ujson", "jmespath", "httplib2", "ase", "jsonschema"],
-    "dscribe": ["dscribe"],
+    "dscribe": ["dscribe~=2.0"],
     "mdfforge": ["mdf-forge"],
     "aflow": ["aflow"],
     "citrine": ["citrination-client"],
     "dev": [
-        "pytest", "pytest-cov", "coverage", "coveralls",
-        "flake8", "black", "pylint", "sphinx"
-    ]
+        "pytest",
+        "pytest-cov",
+        "pytest-timeout",
+        "coverage",
+        "coveralls",
+        "flake8",
+        "black",
+        "pylint",
+        "sphinx",
+    ],
 }
 tests_require = [r for v in extras_require.values() for r in v]
 
+extras_require["tests"] = tests_require
+
 if __name__ == "__main__":
     setup(
-        name='matminer',
+        name="matminer",
         use_scm_version={
             "root": ".",
             "relative_to": __file__,
             "local_scheme": local_version,
         },
         setup_requires=["setuptools_scm"],
-        description='matminer is a library that contains tools for data '
-                    'mining in Materials Science',
-        long_description=open(os.path.join(module_dir, 'README.md')).read(),
-        url='https://github.com/hackingmaterials/matminer',
-        author='Anubhav Jain',
-        author_email='anubhavster@gmail.com',
-        license='modified BSD',
+        description="matminer is a library that contains tools for data mining in Materials Science",
+        long_description=open(os.path.join(module_dir, "README.md")).read(),
+        url="https://github.com/hackingmaterials/matminer",
+        long_description_content_type="text/markdown",
+        author="Anubhav Jain",
+        author_email="anubhavster@gmail.com",
+        license="modified BSD",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         install_requires=[
             "numpy>=1.20.1",
             "requests",
-            "pandas",
+            "pandas~=1.5",
             "tqdm",
             "pymongo",
             "future",
             "scikit_learn",
             "sympy",
             "monty",
             "pymatgen",
         ],
         extras_require=extras_require,
         classifiers=[
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Development Status :: 4 - Beta',
-            'Intended Audience :: Science/Research',
-            'Intended Audience :: System Administrators',
-            'Intended Audience :: Information Technology',
-            'Operating System :: OS Independent',
-            'Topic :: Other/Nonlisted Topic',
-            'Topic :: Scientific/Engineering'],
-        test_suite='matminer',
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Development Status :: 4 - Beta",
+            "Intended Audience :: Science/Research",
+            "Intended Audience :: System Administrators",
+            "Intended Audience :: Information Technology",
+            "Operating System :: OS Independent",
+            "Topic :: Other/Nonlisted Topic",
+            "Topic :: Scientific/Engineering",
+        ],
+        test_suite="matminer",
         tests_require=tests_require,
-        scripts=[]
+        scripts=[],
     )
```

