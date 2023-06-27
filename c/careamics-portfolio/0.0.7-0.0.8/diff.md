# Comparing `tmp/careamics_portfolio-0.0.7.tar.gz` & `tmp/careamics_portfolio-0.0.8.tar.gz`

## Comparing `careamics_portfolio-0.0.7.tar` & `careamics_portfolio-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.copier-answers.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.github/PR_TEMPLATE/pull_request.md
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.github/workflows/datasets_ci.yml
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/examples/example.ipynb
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/scripts/download_and_examine.py
--rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/scripts/export_portfolio_to_json.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/scripts/export_portfolio_to_registry.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/__init__.py
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/denoiseg_datasets.py
--rw-r--r--   0        0        0     9429 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/denoising_datasets.py
--rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/portfolio.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/portfolio_entry.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/py.typed
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/datasets/datasets.json
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/datasets/registry.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/utils/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/utils/download_utils.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/src/careamics_portfolio/utils/pale_blue_dot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/test_denoiseg_datasets.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/test_denoising_datasets.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/test_download_utils.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/test_portfolio.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/test_portfolio_entry.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/tests/utils.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/LICENSE
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/README.md
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.copier-answers.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/PR_TEMPLATE/pull_request.md
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/workflows/datasets_ci.yml
+-rw-r--r--   0        0        0    12056 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/datasets/datasets.json
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/examples/example.ipynb
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/scripts/update_json.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/scripts/update_registry.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/__init__.py
+-rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/denoiseg_datasets.py
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/denoising_datasets.py
+-rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio_entry.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/py.typed
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/registry/registry.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/__init__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/download_utils.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot_zip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_denoiseg_datasets.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_denoising_datasets.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_download_utils.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_portfolio.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_portfolio_entry.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/utils.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/README.md
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/PKG-INFO
```

### Comparing `careamics_portfolio-0.0.7/.copier-answers.yml` & `careamics_portfolio-0.0.8/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/.pre-commit-config.yaml` & `careamics_portfolio-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/.github/PR_TEMPLATE/pull_request.md` & `careamics_portfolio-0.0.8/.github/PR_TEMPLATE/pull_request.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/.github/workflows/ci.yml` & `careamics_portfolio-0.0.8/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -90,34 +90,37 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - name: Build package
         run: python -m pip install .
 
+      # important to maintain the json summary
       - name: Run json export script
-        run: python scripts/export_portfolio_to_json.py
+        run: python scripts/update_json.py
 
+      # not sure that is useful since tests will not pass with the wrong registry
       - name: Run json export script
-        run: python scripts/export_portfolio_to_registry.py
+        run: python scripts/update_registry.py
 
       - name: Verify Changed files
-        uses: tj-actions/verify-changed-files@v15
+        uses: tj-actions/verify-changed-files@v16
         id: verify-changed-files
         with:
           files: |
-            src/careamics_portfolio/datasets/datasets.json
-            src/careamics_portfolio/datasets/registry.txt
+            datasets/datasets.json
+            src/careamics_portfolio/registry/registry.txt
 
       - name: Commit changes
         if: steps.verify-changed-files.outputs.files_changed == 'true'
         run: |
           git config user.name 'github-actions[bot]'
           git config user.email 'github-actions[bot]@users.noreply.github.com'  
-          git add src/careamics_portfolio/datasets/datasets.json
+          git add datasets/datasets.json
+          git add src/careamics_portfolio/registry/registry.txt
           git commit -m "Update datasets.json"
 
       - name: Push changes
         if: steps.verify-changed-files.outputs.files_changed == 'true'
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: git push
```

### Comparing `careamics_portfolio-0.0.7/.github/workflows/datasets_ci.yml` & `careamics_portfolio-0.0.8/.github/workflows/datasets_ci.yml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/examples/example.ipynb` & `careamics_portfolio-0.0.8/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/denoiseg_datasets.py` & `careamics_portfolio-0.0.8/src/careamics_portfolio/denoiseg_datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     """The 2018 Data Science Bowl dataset used by DenoiSeg.
 
     The dataset is available in three different noise levels: N0, N10 and N20.
 
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         noise_level (NoiseLevel): Noise level of the dataset.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self, noise_level: NoiseLevel = NoiseLevel.N0) -> None:
         """Initialize a DSB2018 instance.
 
         Parameters
@@ -79,18 +79,18 @@
             "Original data: "
             "https://www.kaggle.com/competitions/data-science-bowl-2018/data",
             license="GPL-3.0",
             citation="Caicedo, J.C., Goodman, A., Karhohs, K.W. et al. Nucleus "
             "segmentation across imaging experiments: the 2018 Data Science "
             "Bowl. Nat Methods 16, 1247-1253 (2019). "
             "https://doi.org/10.1038/s41592-019-0612-7",
-            files={
-                f"DSB2018_n{noise_level.value}/train": ["train_data.npz"],
-                f"DSB2018_n{noise_level.value}/test": ["test_data.npz"],
-            },
+            files=[
+                f"DSB2018_n{noise_level.value}/train/train_data.npz",
+                f"DSB2018_n{noise_level.value}/test/test_data.npz",
+            ],
             size=self._get_size(noise_level),
             tags=["denoising", "segmentation", "nuclei", "fluorescence"],
         )
 
     @staticmethod
     def _get_url(noise: NoiseLevel) -> str:
         if noise == NoiseLevel.N0:
@@ -123,26 +123,26 @@
     """Flywing dataset used by DenoiSeg.
 
     The dataset is available in three different noise levels: N0, N10 and N20.
 
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         noise_level (NoiseLevel): Noise level of the dataset.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self, noise_level: NoiseLevel = NoiseLevel.N0) -> None:
         """Initialize a Flywing instance.
 
         Parameters
@@ -160,18 +160,18 @@
             description="This dataset consist of 1428 training and 252 "
             "validation patches of a membrane labeled fly wing. The test set "
             "is comprised of 50 additional images.",
             license="CC BY-SA 4.0",
             citation="Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, "
             "F.: Denoiseg: joint denoising and segmentation. In: European "
             "Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
-            files={
-                f"Flywing_n{noise_level.value}/train": ["train_data.npz"],
-                f"Flywing_n{noise_level.value}/test": ["test_data.npz"],
-            },
+            files=[
+                f"Flywing_n{noise_level.value}/train/train_data.npz",
+                f"Flywing_n{noise_level.value}/test/test_data.npz",
+            ],
             size=self._get_size(noise_level),
             tags=["denoising", "segmentation", "membrane", "fluorescence"],
         )
 
     @staticmethod
     def _get_url(noise: NoiseLevel) -> str:
         if noise == NoiseLevel.N0:
@@ -204,26 +204,26 @@
     """Mouse nuclei dataset used by DenoiSeg.
 
     The dataset is available in three different noise levels: N0, N10 and N20.
 
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         noise_level (NoiseLevel): Noise level of the dataset.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self, noise_level: NoiseLevel = NoiseLevel.N0) -> None:
         """Initialize a MouseNuclei instance.
 
         Parameters
@@ -241,18 +241,18 @@
             description="A dataset depicting diverse and non-uniformly "
             "clustered nuclei in the mouse skull, consisting of 908 training "
             "and 160 validation patches. The test set counts 67 additional images",
             license="CC BY-SA 4.0",
             citation="Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, "
             "F.: Denoiseg: joint denoising and segmentation. In: European "
             "Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
-            files={
-                f"Mouse_n{noise_level.value}/train": ["train_data.npz"],
-                f"Mouse_n{noise_level.value}/test": ["test_data.npz"],
-            },
+            files=[
+                f"Mouse_n{noise_level.value}/train/train_data.npz",
+                f"Mouse_n{noise_level.value}/test/test_data.npz",
+            ],
             size=self._get_size(noise_level),
             tags=["denoising", "segmentation", "nuclei", "fluorescence"],
         )
 
     @staticmethod
     def _get_url(noise: NoiseLevel) -> str:
         if noise == NoiseLevel.N0:
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/denoising_datasets.py` & `careamics_portfolio-0.0.8/src/careamics_portfolio/denoising_datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 
 class N2V_BSD68(PortfolioEntry):
     """BSD68 dataset.
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self) -> None:
         super().__init__(
             portfolio=DENOISING,
             name="N2V_BSD68",
@@ -42,43 +42,41 @@
             citation='D. Martin, C. Fowlkes, D. Tal and J. Malik, "A database of '
             "human segmented natural images and its application to "
             "evaluating segmentation algorithms and measuring ecological "
             'statistics," Proceedings Eighth IEEE International '
             "Conference on Computer Vision. ICCV 2001, Vancouver, BC, "
             "Canada, 2001, pp. 416-423 vol.2, doi: "
             "10.1109/ICCV.2001.937655.",
-            files={
-                "BSD68_reproducibility_data/test": [
-                    "bsd68_gaussian25.npy",
-                    "bsd68_groundtruth.npy",
-                ],
-                "BSD68_reproducibility_data/train": ["DCNN400_train_gaussian25.npy"],
-                "BSD68_reproducibility_data/val": ["DCNN400_validation_gaussian25.npy"],
-            },
+            files=[
+                "BSD68_reproducibility_data/test/bsd68_gaussian25.npy",
+                "BSD68_reproducibility_data/test/bsd68_groundtruth.npy",
+                "BSD68_reproducibility_data/train/DCNN400_train_gaussian25.npy",
+                "BSD68_reproducibility_data/val/DCNN400_validation_gaussian25.npy",
+            ],
             size=875.0,
             tags=["denoising", "natural images"],
         )
 
 
 class N2V_SEM(PortfolioEntry):
     """SEM dataset.
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self) -> None:
         super().__init__(
             portfolio=DENOISING,
             name="N2V_SEM",
@@ -87,38 +85,36 @@
             sha256="7600a17c3dbd4992ea547be12458640c21e797eef6a9f776f36ba5890f26855d",
             description="Cropped images from a SEM dataset from T.-O. Buchholz et al "
             "(Methods Cell Biol, 2020).",
             license="CC-BY-4.0",
             citation="T.-O. Buchholz, A. Krull, R. Shahidi, G. Pigino, G. Jékely, "
             'F. Jug, "Content-aware image restoration for electron '
             'microscopy", Methods Cell Biol 152, 277-289',
-            files={
-                ".": ["train.tif", "validation.tif"],
-            },
+            files=["train.tif", "validation.tif"],
             size=13.0,
             tags=["denoising", "electron microscopy"],
         )
 
 
 class N2V_RGB(PortfolioEntry):
     """RGB dataset.
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self) -> None:
         super().__init__(
             portfolio=DENOISING,
             name="N2V_RGB",
@@ -127,38 +123,38 @@
             sha256="4c2010c6b5c253d3a580afe744cbff969d387617c9dde29fea4463636d285657",
             description="Banner of the CVPR 2019 conference with extra noise.",
             license="CC-BY-4.0",
             citation='A. Krull, T.-O. Buchholz and F. Jug, "Noise2Void - Learning '
             'Denoising From Single Noisy Images," 2019 IEEE/CVF '
             "Conference on Computer Vision and Pattern Recognition (CVPR),"
             " 2019, pp. 2124-2132",
-            files={
-                ".": ["longBeach.png"],
-            },
+            files=[
+                "longBeach.png",
+            ],
             size=10.4,
             tags=["denoising", "natural images", "RGB"],
         )
 
 
 class Flywing(PortfolioEntry):
     """Flywing dataset.
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the downloaded file.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self) -> None:
         super().__init__(
             portfolio=DENOISING,
             name="Flywing",
@@ -166,38 +162,38 @@
             file_name="flywing-data.zip",
             sha256="01106b6dc096c423babfca47ef27059a01c2ca053769da06e8649381089a559f",
             description="Image of a membrane-labeled fly wing (35x692x520 pixels).",
             license="CC-BY-4.0",
             citation="Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, "
             "F.: Denoiseg: joint denoising and segmentation. In: European "
             "Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
-            files={
-                ".": ["flywing.tif"],
-            },
+            files=[
+                "flywing.tif",
+            ],
             size=10.2,
             tags=["denoising", "membrane", "fluorescence"],
         )
 
 
 class Convallaria(PortfolioEntry):
     """Convallaria dataset.
 
     Attributes
     ----------
-        portfolio (str): Name of the portfolio to which the dataset.
+        portfolio (str): Name of the portfolio to which the dataset belong.
         name (str): Name of the dataset.
         url (str): URL of the dataset.
-        file_name (str): Name of the file to download.
-        hash (str): SHA256 hash of the downloaded file.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
-        files (dict): Dictionary containing the files to download.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self) -> None:
         super().__init__(
             portfolio=DENOISING,
             name="Convallaria",
@@ -207,16 +203,14 @@
             description="Image of a convallaria flower (35x692x520 pixels).\n"
             "The image also comes with a defocused image in order to allow \n"
             "estimating the noise distribution.",
             license="CC-BY-4.0",
             citation="Krull, A., Vičar, T., Prakash, M., Lalit, M., & Jug, F. (2020). "
             "Probabilistic noise2void: Unsupervised content-aware denoising. Frontiers"
             " in Computer Science, 2, 5.",
-            files={
-                "Convallaria_diaphragm": [
-                    "20190520_tl_25um_50msec_05pc_488_130EM_Conv.tif",
-                    "20190726_tl_50um_500msec_wf_130EM_FD.tif",
-                ],
-            },
+            files=[
+                "Convallaria_diaphragm/20190520_tl_25um_50msec_05pc_488_130EM_Conv.tif",
+                "Convallaria_diaphragm/20190726_tl_50um_500msec_wf_130EM_FD.tif",
+            ],
             size=344.0,
             tags=["denoising", "membrane", "fluorescence"],
         )
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/portfolio.py` & `careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     N2V_BSD68,
     N2V_RGB,
     N2V_SEM,
     Convallaria,
     Flywing,
 )
 from .portfolio_entry import PortfolioEntry
+from .utils.download_utils import get_registry_path
 from .utils.pale_blue_dot import PaleBlueDot
+from .utils.pale_blue_dot_zip import PaleBlueDotZip
 
 
 class IterablePortfolio:
     """Iterable portfolio class.
 
     Subclass this class and add PortfolioEntry objects as attributes.
 
@@ -104,18 +106,18 @@
         # for each attribute
         for attribute in vars(self).values():
             if isinstance(attribute, PortfolioEntry):
                 attributes.append(attribute.name)
 
         return attributes
 
-    def as_dict(self) -> dict[str, dict[str, str]]:
+    def as_dict(self) -> dict:
         """Dictionary representation of a portfolio.
 
-        Used to serialize the class to json, with friendly name as entries.
+        Used to serialize the class to json, with friendly names as entries.
 
         Returns
         -------
         dict[str]
             Dictionary representation of the DenoiSeg portfolio.
         """
         entries = {}
@@ -126,15 +128,17 @@
             if isinstance(attribute, PortfolioEntry):
                 # add the attribute to the entries dictionary
                 entries[attribute.name] = {
                     "URL": attribute.url,
                     "Description": attribute.description,
                     "Citation": attribute.citation,
                     "License": attribute.license,
+                    "Hash": attribute.hash,
                     "File size": f"{attribute.size} MB",
+                    "Tags": attribute.tags,
                 }
         return entries
 
     def __str__(self) -> str:
         """String representation of a portfolio.
 
         Returns
@@ -379,46 +383,47 @@
     denoising (Denoising): Denoising datasets.
     denoiseg (DenoiSeg): DenoiSeg datasets.
     """
 
     def __init__(self) -> None:
         self._denoising = Denoising()
         self._denoiseg = DenoiSeg()
+        # self._segmentation = Segmentation()
 
     @property
     def denoising(self) -> Denoising:
         """Denoising datasets.
 
         Returns
         -------
         Denoising
-        Denoising datasets.
+            Denoising datasets.
         """
         return self._denoising
 
     @property
     def denoiseg(self) -> DenoiSeg:
         """DenoiSeg datasets.
 
         Returns
         -------
         DenoiSeg
-        DenoiSeg datasets.
+            DenoiSeg datasets.
         """
         return self._denoiseg
 
     def __str__(self) -> str:
         """String representation of the portfolio.
 
         This method allows having a frendly representation of the portfolio as string.
 
         Returns
         -------
         str
-        String representation of the portfolio.
+            String representation of the portfolio.
         """
         return (
             f"Portfolio:\n"
             f"Denoising datasets: {self.denoising.list_datasets()}\n"
             f"DenoiSeg datasets: {self.denoiseg.list_datasets()}"
         )
 
@@ -460,21 +465,40 @@
         Parameters
         ----------
         path : str or Path
             Path to json file.
         """
         portfolios = self.as_dict()
         with open(path, "w") as file:
+            file.write("# Portfolio datasets - pooch registry\n")
+            file.write("# Generated by running " "scripts/update_registry.py\n\n")
+
+            # write each portfolio
             for key in portfolios.keys():
+                file.write(f"# {key} \n")
                 for entry in portfolios[key]:
                     file.write(
                         f"{entry.get_registry_name()} " f"{entry.hash} {entry.url}\n"
                     )
+                file.write("\n")
 
             # add pale blue dot for testing purposes
-            file.write("\n")
             file.write("# Test sample\n")
             pale_blue_dot = PaleBlueDot()
             file.write(
                 f"{pale_blue_dot.get_registry_name()} "
                 f"{pale_blue_dot.hash} {pale_blue_dot.url}\n"
             )
+            pale_blue_dot_zip = PaleBlueDotZip()
+            file.write(
+                f"{pale_blue_dot_zip.get_registry_name()} "
+                f"{pale_blue_dot_zip.hash} {pale_blue_dot_zip.url}\n"
+            )
+
+
+def update_registry(path: str | Path | None = None) -> None:
+    """Update the registry.txt file."""
+    if path is None:
+        path = get_registry_path()
+
+    portfolio = PortfolioManager()
+    portfolio.to_registry(path)
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/portfolio_entry.py` & `careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from pooch import Unzip
 
 from .utils import get_poochfolio
 
 
 class PortfolioEntry:
@@ -15,15 +15,15 @@
         name (str): Name of the dataset.
         url (str): URL of the dataset.
         description (str): Description of the dataset.
         license (str): License of the dataset.
         citation (str): Citation to use when referring to the dataset.
         file_name (str): Name of the downloaded file.
         hash (str): SHA256 hash of the downloaded file.
-        files (dict[str, list]): Dictionary of files in the dataset.
+        files (list[str]): List of files in the dataset.
         size (int): Size of the dataset in MB.
         tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(
         self,
@@ -31,15 +31,15 @@
         name: str,
         url: str,
         description: str,
         license: str,
         citation: str,
         file_name: str,
         sha256: str,
-        files: Dict[str, list],
+        files: List[str],
         size: float,
         tags: List[str],
         is_zip: bool = True,
         **kwargs: str,
     ) -> None:
         self._portfolio = portfolio
 
@@ -143,15 +143,15 @@
         -------
         str
             SHA256 hash of the downloaded file.
         """
         return self._hash
 
     @property
-    def files(self) -> Dict[str, list]:
+    def files(self) -> List[str]:
         """Dictionary of files in the dataset.
 
         Returns
         -------
         dict[str, list]
             Dictionary of files in the dataset.
         """
@@ -219,17 +219,18 @@
         return {
             "name": self.name,
             "url": self.url,
             "description": self.description,
             "license": self.license,
             "citation": self.citation,
             "file_name": self.file_name,
-            "md5_hash": self.hash,
+            "hash": self.hash,
             "files": self.files,
             "size": self.size,
+            "tags": self.tags,
         }
 
     def download(
         self,
         path: Optional[Union[str, Path]] = None,
     ) -> Union[List[str], Any]:
         """Download dataset in the specified path.
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/datasets/datasets.json` & `careamics_portfolio-0.0.8/datasets/datasets.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'denoiseg'": "{'DSB2018_n0': {'Hash': "*

 * *               "'729d7683ccfa1ad437f666256b23e73b3b3b3da6a8e47bb37303f0c64376a299', 'Tags': "*

 * *               "['denoising', 'segmentation', 'nuclei', 'fluorescence']}, 'DSB2018_n10': {'Hash': "*

 * *               "'a4cf731aa0652f8198275f8ce29fb98e0c76c391a96b6092d0792fe447e4103a', 'Tags': "*

 * *               "['denoising', 'segmentation', 'nuclei', 'fluorescence']}, 'DSB2018_n20': {'Hash': "*

 * *               "'6a732a12bf18fecc590230b1cd4df5e32acfa1b35ef2fca42db811cb8277c67c' […]*

```diff
@@ -1,104 +1,195 @@
 {
     "denoiseg": {
         "DSB2018_n0": {
             "Citation": "Caicedo, J.C., Goodman, A., Karhohs, K.W. et al. Nucleus segmentation across imaging experiments: the 2018 Data Science Bowl. Nat Methods 16, 1247-1253 (2019). https://doi.org/10.1038/s41592-019-0612-7",
             "Description": "From the Kaggle 2018 Data Science Bowl challenge, the training and validation sets consist of 3800 and 670 patches respectively, while the test set counts 50 images.\nOriginal data: https://www.kaggle.com/competitions/data-science-bowl-2018/data",
             "File size": "40.2 MB",
+            "Hash": "729d7683ccfa1ad437f666256b23e73b3b3b3da6a8e47bb37303f0c64376a299",
             "License": "GPL-3.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "nuclei",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5156969/files/DSB2018_n0.zip?download=1"
         },
         "DSB2018_n10": {
             "Citation": "Caicedo, J.C., Goodman, A., Karhohs, K.W. et al. Nucleus segmentation across imaging experiments: the 2018 Data Science Bowl. Nat Methods 16, 1247-1253 (2019). https://doi.org/10.1038/s41592-019-0612-7",
             "Description": "From the Kaggle 2018 Data Science Bowl challenge, the training and validation sets consist of 3800 and 670 patches respectively, while the test set counts 50 images.\nOriginal data: https://www.kaggle.com/competitions/data-science-bowl-2018/data",
             "File size": "366.0 MB",
+            "Hash": "a4cf731aa0652f8198275f8ce29fb98e0c76c391a96b6092d0792fe447e4103a",
             "License": "GPL-3.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "nuclei",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5156977/files/DSB2018_n10.zip?download=1"
         },
         "DSB2018_n20": {
             "Citation": "Caicedo, J.C., Goodman, A., Karhohs, K.W. et al. Nucleus segmentation across imaging experiments: the 2018 Data Science Bowl. Nat Methods 16, 1247-1253 (2019). https://doi.org/10.1038/s41592-019-0612-7",
             "Description": "From the Kaggle 2018 Data Science Bowl challenge, the training and validation sets consist of 3800 and 670 patches respectively, while the test set counts 50 images.\nOriginal data: https://www.kaggle.com/competitions/data-science-bowl-2018/data",
             "File size": "368.0 MB",
+            "Hash": "6a732a12bf18fecc590230b1cd4df5e32acfa1b35ef2fca42db811cb8277c67c",
             "License": "GPL-3.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "nuclei",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5156983/files/DSB2018_n20.zip?download=1"
         },
         "Flywing_n0": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "This dataset consist of 1428 training and 252 validation patches of a membrane labeled fly wing. The test set is comprised of 50 additional images.",
             "File size": "47.0 MB",
+            "Hash": "3fb49ba44e7e3e20b4fc3c77754f1bbff7184af7f343f23653f258d50e5d5aca",
             "License": "CC BY-SA 4.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "membrane",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5156991/files/Flywing_n0.zip?download=1"
         },
         "Flywing_n10": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "This dataset consist of 1428 training and 252 validation patches of a membrane labeled fly wing. The test set is comprised of 50 additional images.",
             "File size": "282.0 MB",
+            "Hash": "c599981b0900e6b43f0a742f84a5fde664373600dc5334f537b61a76a7be2a3c",
             "License": "CC BY-SA 4.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "membrane",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5156993/files/Flywing_n10.zip?download=1"
         },
         "Flywing_n20": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "This dataset consist of 1428 training and 252 validation patches of a membrane labeled fly wing. The test set is comprised of 50 additional images.",
             "File size": "293.0 MB",
+            "Hash": "604b3a3a081eaa57ee25d708bc9b76b85d05235ba09d7c2b25b171e201ea966f",
             "License": "CC BY-SA 4.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "membrane",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5156995/files/Flywing_n20.zip?download=1"
         },
         "MouseNuclei_n0": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "A dataset depicting diverse and non-uniformly clustered nuclei in the mouse skull, consisting of 908 training and 160 validation patches. The test set counts 67 additional images",
             "File size": "12.4 MB",
+            "Hash": "5d6fd2fc23ab991a8fde4bd0ec5e9fc9299f9a9ddc2a8acb7095f9b02ff3c9d7",
             "License": "CC BY-SA 4.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "nuclei",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5157001/files/Mouse_n0.zip?download=1"
         },
         "MouseNuclei_n10": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "A dataset depicting diverse and non-uniformly clustered nuclei in the mouse skull, consisting of 908 training and 160 validation patches. The test set counts 67 additional images",
             "File size": "161.0 MB",
+            "Hash": "de634496e3e46a4887907b713fe6f575e410c3006046054bce67ef9398523c2c",
             "License": "CC BY-SA 4.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "nuclei",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5157003/files/Mouse_n10.zip?download=1"
         },
         "MouseNuclei_n20": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "A dataset depicting diverse and non-uniformly clustered nuclei in the mouse skull, consisting of 908 training and 160 validation patches. The test set counts 67 additional images",
             "File size": "160.0 MB",
+            "Hash": "d3d1bf8c89bb97a673a0791874e5b75a6a516ccaaeece0244b4e1e0afe7ab3ec",
             "License": "CC BY-SA 4.0",
+            "Tags": [
+                "denoising",
+                "segmentation",
+                "nuclei",
+                "fluorescence"
+            ],
             "URL": "https://zenodo.org/record/5157008/files/Mouse_n20.zip?download=1"
         }
     },
     "denoising": {
         "Convallaria": {
             "Citation": "Krull, A., Vi\u010dar, T., Prakash, M., Lalit, M., & Jug, F. (2020). Probabilistic noise2void: Unsupervised content-aware denoising. Frontiers in Computer Science, 2, 5.",
             "Description": "Image of a convallaria flower (35x692x520 pixels).\nThe image also comes with a defocused image in order to allow \nestimating the noise distribution.",
             "File size": "344.0 MB",
+            "Hash": "8a2ac3e2792334c833ee8a3ca449fc14eada18145f9d56fa2cb40f462c2e8909",
             "License": "CC-BY-4.0",
+            "Tags": [
+                "denoising",
+                "membrane",
+                "fluorescence"
+            ],
             "URL": "https://cloud.mpi-cbg.de/index.php/s/BE8raMtHQlgLDF3/download"
         },
         "Flywing": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "Image of a membrane-labeled fly wing (35x692x520 pixels).",
             "File size": "10.2 MB",
+            "Hash": "01106b6dc096c423babfca47ef27059a01c2ca053769da06e8649381089a559f",
             "License": "CC-BY-4.0",
+            "Tags": [
+                "denoising",
+                "membrane",
+                "fluorescence"
+            ],
             "URL": "https://download.fht.org/jug/n2v/flywing-data.zip"
         },
         "N2V_BSD68": {
             "Citation": "D. Martin, C. Fowlkes, D. Tal and J. Malik, \"A database of human segmented natural images and its application to evaluating segmentation algorithms and measuring ecological statistics,\" Proceedings Eighth IEEE International Conference on Computer Vision. ICCV 2001, Vancouver, BC, Canada, 2001, pp. 416-423 vol.2, doi: 10.1109/ICCV.2001.937655.",
             "Description": "This dataset is taken from K. Zhang et al (TIP, 2017). \nIt consists of 400 gray-scale 180x180 images (cropped from the BSD dataset) and splitted between training and validation, and 68 gray-scale test images (BSD68).\nAll images were corrupted with Gaussian noise with standard deviation of 25 pixels. The test dataset contains the uncorrupted images as well.\nOriginal dataset: https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/",
             "File size": "875.0 MB",
+            "Hash": "e31d77060d4104d5a5ac14c11ad88e5e83636d396de8b80f294dd2033b4ba5a6",
             "License": "Unknown",
+            "Tags": [
+                "denoising",
+                "natural images"
+            ],
             "URL": "https://download.fht.org/jug/n2v/BSD68_reproducibility.zip"
         },
         "N2V_RGB": {
             "Citation": "A. Krull, T.-O. Buchholz and F. Jug, \"Noise2Void - Learning Denoising From Single Noisy Images,\" 2019 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2019, pp. 2124-2132",
             "Description": "Banner of the CVPR 2019 conference with extra noise.",
             "File size": "10.4 MB",
+            "Hash": "4c2010c6b5c253d3a580afe744cbff969d387617c9dde29fea4463636d285657",
             "License": "CC-BY-4.0",
+            "Tags": [
+                "denoising",
+                "natural images",
+                "RGB"
+            ],
             "URL": "https://download.fht.org/jug/n2v/RGB.zip"
         },
         "N2V_SEM": {
             "Citation": "T.-O. Buchholz, A. Krull, R. Shahidi, G. Pigino, G. J\u00e9kely, F. Jug, \"Content-aware image restoration for electron microscopy\", Methods Cell Biol 152, 277-289",
             "Description": "Cropped images from a SEM dataset from T.-O. Buchholz et al (Methods Cell Biol, 2020).",
             "File size": "13.0 MB",
+            "Hash": "7600a17c3dbd4992ea547be12458640c21e797eef6a9f776f36ba5890f26855d",
             "License": "CC-BY-4.0",
+            "Tags": [
+                "denoising",
+                "electron microscopy"
+            ],
             "URL": "https://download.fht.org/jug/n2v/SEM.zip"
         }
     }
 }
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/datasets/registry.txt` & `careamics_portfolio-0.0.8/src/careamics_portfolio/registry/registry.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+# Portfolio datasets - pooch registry
+# Generated by running scripts/update_registry.py
+
+# denoising 
 denoising-N2V_BSD68 e31d77060d4104d5a5ac14c11ad88e5e83636d396de8b80f294dd2033b4ba5a6 https://download.fht.org/jug/n2v/BSD68_reproducibility.zip
 denoising-N2V_SEM 7600a17c3dbd4992ea547be12458640c21e797eef6a9f776f36ba5890f26855d https://download.fht.org/jug/n2v/SEM.zip
 denoising-N2V_RGB 4c2010c6b5c253d3a580afe744cbff969d387617c9dde29fea4463636d285657 https://download.fht.org/jug/n2v/RGB.zip
 denoising-Flywing 01106b6dc096c423babfca47ef27059a01c2ca053769da06e8649381089a559f https://download.fht.org/jug/n2v/flywing-data.zip
 denoising-Convallaria 8a2ac3e2792334c833ee8a3ca449fc14eada18145f9d56fa2cb40f462c2e8909 https://cloud.mpi-cbg.de/index.php/s/BE8raMtHQlgLDF3/download
+
+# denoiseg 
 denoiseg-DSB2018_n0 729d7683ccfa1ad437f666256b23e73b3b3b3da6a8e47bb37303f0c64376a299 https://zenodo.org/record/5156969/files/DSB2018_n0.zip?download=1
 denoiseg-DSB2018_n10 a4cf731aa0652f8198275f8ce29fb98e0c76c391a96b6092d0792fe447e4103a https://zenodo.org/record/5156977/files/DSB2018_n10.zip?download=1
 denoiseg-DSB2018_n20 6a732a12bf18fecc590230b1cd4df5e32acfa1b35ef2fca42db811cb8277c67c https://zenodo.org/record/5156983/files/DSB2018_n20.zip?download=1
 denoiseg-Flywing_n0 3fb49ba44e7e3e20b4fc3c77754f1bbff7184af7f343f23653f258d50e5d5aca https://zenodo.org/record/5156991/files/Flywing_n0.zip?download=1
 denoiseg-Flywing_n10 c599981b0900e6b43f0a742f84a5fde664373600dc5334f537b61a76a7be2a3c https://zenodo.org/record/5156993/files/Flywing_n10.zip?download=1
 denoiseg-Flywing_n20 604b3a3a081eaa57ee25d708bc9b76b85d05235ba09d7c2b25b171e201ea966f https://zenodo.org/record/5156995/files/Flywing_n20.zip?download=1
 denoiseg-MouseNuclei_n0 5d6fd2fc23ab991a8fde4bd0ec5e9fc9299f9a9ddc2a8acb7095f9b02ff3c9d7 https://zenodo.org/record/5157001/files/Mouse_n0.zip?download=1
 denoiseg-MouseNuclei_n10 de634496e3e46a4887907b713fe6f575e410c3006046054bce67ef9398523c2c https://zenodo.org/record/5157003/files/Mouse_n10.zip?download=1
 denoiseg-MouseNuclei_n20 d3d1bf8c89bb97a673a0791874e5b75a6a516ccaaeece0244b4e1e0afe7ab3ec https://zenodo.org/record/5157008/files/Mouse_n20.zip?download=1
 
-
 # Test sample
-test-PaleBlueDot c83d5de3361a964370fc392ab213c3cf1a23d046406de377a8ac9cb5fbb087f0 https://solarsystem.nasa.gov/rails/active_storage/blobs/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBBaUZoIiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--4b5b6d8ce74a6930534a08e4d7dd002f24f1efcb/P36254.jpg
+test-PaleBlueDot 68d0f037a448dc099e893b8cbf4d303ffa4b4289903c764f737101d6ad7555dd https://download.fht.org/jug/careamics/P36254.jpg
+test-PaleBlueDotZip 90b03ec7a9e1980fd112a40c2c935015bb349cdf89fbf3db78c715dd2a49db47 https://download.fht.org/jug/careamics/pale_blue_dot.zip
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/utils/download_utils.py` & `careamics_portfolio-0.0.8/src/careamics_portfolio/utils/download_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import pooch
 from pooch import Pooch
 
 
+def get_registry_path() -> Path:
+    """Get the path to the registry.txt file.
+
+    Returns
+    -------
+    Path
+        Path to the registry.txt file.
+    """
+    return Path(__file__).parent / "../registry/registry.txt"
+
+
 def get_poochfolio(path: Optional[Union[str, Path]] = None) -> Pooch:
     """Create the pooch object for the whole portfolio.
 
     By default the files will be downloaded and cached in the user's
     cache folder and can be retrieved automatically without downloading
     the file anew (thanks pooch!).
 
@@ -29,10 +40,10 @@
 
     poochfolio = pooch.create(
         path=path,
         base_url="",
     )
 
     # Path to the registry.txt file
-    poochfolio.load_registry(Path(__file__).parent / "../datasets/registry.txt")
+    poochfolio.load_registry(get_registry_path())
 
     return poochfolio
```

### Comparing `careamics_portfolio-0.0.7/src/careamics_portfolio/utils/pale_blue_dot.py` & `careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 class PaleBlueDot(PortfolioEntry):
     """The original Pale Blue Dot image.
 
     Attributes
     ----------
         portfolio (str): Name of the portfolio to which the dataset belong.
         name (str): Name of the dataset.
-        url (str): URL to the dataset.
-        file_name (str): Name of the file.
-        hash (str): SHA256 hash of the downloaded file.
+        url (str): URL of the dataset.
         description (str): Description of the dataset.
-        citation (str): Citation of the dataset.
         license (str): License of the dataset.
-        files (dict): Dictionary of files.
-        size (float): Size of the dataset in MB.
-        tags (list): List of tags associated to the dataset.
+        citation (str): Citation to use when referring to the dataset.
+        file_name (str): Name of the downloaded file.
+        hash (str): SHA256 hash of the downloaded file.
+        files (list[str]): List of files in the dataset.
+        size (int): Size of the dataset in MB.
+        tags (list[str]): List of tags associated to the dataset.
         is_zip (bool): Whether the dataset is a zip file.
     """
 
     def __init__(self) -> None:
         super().__init__(
             portfolio="test",
             name="PaleBlueDot",
-            url="https://solarsystem.nasa.gov/rails/active_storage/blobs/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBBaUZoIiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--4b5b6d8ce74a6930534a08e4d7dd002f24f1efcb/P36254.jpg",
+            url="https://download.fht.org/jug/careamics/P36254.jpg",
             file_name="P36254.jpg",
-            sha256="c83d5de3361a964370fc392ab213c3cf1a23d046406de377a8ac9cb5fbb087f0",
+            sha256="68d0f037a448dc099e893b8cbf4d303ffa4b4289903c764f737101d6ad7555dd",
             description="Pale Blue Dot, credit NASA/JPL-Caltech."
             "Original caption: This narrow-angle color image of the"
             " Earth, dubbed 'Pale Blue Dot', is a part of the first"
             " ever 'portrait' of the solar system taken by Voyager "
             "1. The spacecraft acquired a total of 60 frames for a "
             "mosaic of the solar system from a distance of more "
             "than 4 billion miles from Earth and about 32 degrees "
@@ -43,14 +43,14 @@
             "image so close to the sun. This blown-up image of the "
             "Earth was taken through three color filters - violet, "
             "blue and green - and recombined to produce the color "
             "image. The background features in the image are "
             "artifacts resulting from the magnification.",
             citation="NASA/JPL-Caltech",
             license="Public domain",
-            files={
-                ".": ["P36254.jpg"],
-            },
+            files=[
+                "P36254.jpg",
+            ],
             size=0.4,
             tags=["pale blue dot", "voyager", "nasa", "jpl"],
             is_zip=False,
         )
```

### Comparing `careamics_portfolio-0.0.7/tests/test_denoising_datasets.py` & `careamics_portfolio-0.0.8/tests/test_denoising_datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,22 @@
     unique_hash_checker,
     unique_url_checker,
 )
 
 DATASETS = list(PortfolioManager().denoising)
 
 
+def all_datasets_getters(portfolio: PortfolioManager):
+    assert isinstance(portfolio.denoising.N2V_SEM, PortfolioEntry)
+    assert isinstance(portfolio.denoising.N2V_BSD68, PortfolioEntry)
+    assert isinstance(portfolio.denoising.N2V_RGB, PortfolioEntry)
+    assert isinstance(portfolio.denoising.flywing, PortfolioEntry)
+    assert isinstance(portfolio.denoising.Convallaria, PortfolioEntry)
+
+
 @pytest.mark.dataset
 @pytest.mark.parametrize("dataset", DATASETS)
 def test_datasets(tmp_path, dataset: PortfolioEntry):
     """Test that all denoising datasets download properly.
 
     This test also checks the files and size.
```

### Comparing `careamics_portfolio-0.0.7/tests/test_portfolio_entry.py` & `careamics_portfolio-0.0.8/tests/test_portfolio_entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from pathlib import Path
 
 import pytest
 
 from careamics_portfolio.portfolio_entry import PortfolioEntry
 
-# TODO test invalid hash
-
 
 def test_download(tmp_path, pale_blue_dot: PortfolioEntry):
     assert Path(pale_blue_dot.download(tmp_path)).exists()
 
 
+def test_download_zip(tmp_path, pale_blue_dot_zip: PortfolioEntry):
+    files = pale_blue_dot_zip.download(tmp_path)
+
+    for file in files:
+        assert Path(file).exists(), f"{file} does not exist."
+
+
 def test_download_in_invalid_path(tmp_path, pale_blue_dot: PortfolioEntry):
     """Test that downloading to an invalid path raises an error."""
     file_name = "file.txt"
     with open(tmp_path / file_name, "w") as f:
         f.write("CATS ARE NICE.")
 
     with pytest.raises((NotADirectoryError, FileNotFoundError)):
@@ -61,13 +66,35 @@
     with pytest.raises(AttributeError):
         pale_blue_dot.hash = ""
 
     with pytest.raises(AttributeError):
         pale_blue_dot.files = {}
 
 
-def test_registry_name(pale_blue_dot):
+def test_registry_name(pale_blue_dot: PortfolioEntry):
     """Test that the registry name is correct."""
     assert (
         pale_blue_dot.get_registry_name()
         == pale_blue_dot.portfolio + "-" + pale_blue_dot.name
     )
+
+
+def test_name_with_space():
+    with pytest.raises(ValueError):
+        PortfolioEntry(
+            name="name with space",
+            url="url",
+            portfolio="portfolio",
+            description="description",
+            license="license",
+            citation="citation",
+            file_name="file name",
+            sha256="34973248736ygdw3",
+            files=["dsada"],
+            size=1,
+            tags=["dsadas"],
+        )
+
+
+def test_entry_to_str(pale_blue_dot: PortfolioEntry):
+    """Test the export to str and dict."""
+    assert str(pale_blue_dot) == str(pale_blue_dot.to_dict())
```

### Comparing `careamics_portfolio-0.0.7/tests/utils.py` & `careamics_portfolio-0.0.8/tests/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 import os
 from pathlib import Path
-from typing import Dict, List
 
 import pytest
 
 from careamics_portfolio.portfolio import IterablePortfolio
 from careamics_portfolio.portfolio_entry import PortfolioEntry
 
 
-def file_checker(path: Path, root_name: str, files: Dict[str, List[str]]) -> None:
-    for folder, file_list in files.items():
-        folder_path = path / root_name / folder
-        for file in file_list:
-            assert (
-                folder_path / file
-            ).is_file(), f"{file} does not exist in {folder_path}."
-
-
 def unique_url_checker(iter_portfolio: IterablePortfolio) -> None:
+    """Check that all urls are unique."""
     urls = []
     for entry in iter_portfolio:
         # add to list of urls
         urls.append(entry.url)
 
     assert len(urls) == len(set(urls)), f"Duplicated urls in {iter_portfolio.name}."
 
 
 def unique_hash_checker(iter_portfolio: IterablePortfolio) -> None:
+    """Check that all hashes are unique."""
     hashes = []
     for entry in iter_portfolio:
         # add to list of hashes
         hashes.append(entry.hash)
 
     assert len(hashes) == len(
         set(hashes)
     ), f"Duplicated hashes in {iter_portfolio.name}."
 
 
 def portoflio_entry_checker(entry: PortfolioEntry) -> None:
+    """Check that the PortfolioEntry does not have null or empty fields,
+    as well as a non-null size and at least one file."""
     assert entry.name is not None and entry.name != "", f"Invalid name in {entry}"
     assert entry.url is not None and entry.url != "", f"Invalid url in {entry}"
     assert entry.hash is not None and entry.hash != "", f"Invalid md5 hash in {entry}"
     assert (
         entry.description is not None and entry.description != ""
     ), f"Invalid description in {entry}"
     assert (
@@ -54,26 +48,38 @@
         entry.file_name is not None and entry.file_name != ""
     ), f"Invalid file name in {entry}"
     assert entry.files is not None and len(entry.files) > 0, f"Invalid files in {entry}"
     assert entry.size is not None and entry.size > 0, f"Invalid size in {entry}"
 
 
 def download_checker(path: Path, dataset: PortfolioEntry) -> None:
+    """Test that the file can be downloaded and that all fields
+    correspond to reality."""
     # download dataset
-    dataset.download(path)
+    files = dataset.download(path)
 
     # check that the zip file exists
     path_to_zip = path / dataset.get_registry_name()
     assert (
         path_to_zip.exists()
     ), f"{dataset.get_registry_name()} does not exist after download."
 
-    # check that the files are there
+    # root folder where the downloaded files are
     if dataset.is_zip:
-        file_checker(path, dataset.get_registry_name() + ".unzip", dataset.files)
+        folder_root = path / (dataset.get_registry_name() + ".unzip")
+    else:
+        folder_root = path
+
+    # check that the files exist and are in the returned list
+    # TODO: currently some files have hidden macOS files that need to be removed in the
+    # future
+    files_portfolio = [str(Path(folder_root, s)) for s in dataset.files]
+    for file in files_portfolio:
+        assert Path(file).exists(), f"{file} does not exist."
+        assert file in files, f"{file} not in downloaded files."
 
     # check file size with a tolerance of 5% or 3MB
     file_size = os.path.getsize(path_to_zip) / 1024 / 1024  # MB
     abs_tolerance = max(0.05 * dataset.size, 3)
     assert dataset.size == pytest.approx(file_size, abs=abs_tolerance), (
         f"{dataset.name} has not the expected size "
         f"(expected {dataset.size}, got {file_size})."
```

### Comparing `careamics_portfolio-0.0.7/.gitignore` & `careamics_portfolio-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/LICENSE` & `careamics_portfolio-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.7/README.md` & `careamics_portfolio-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 
 [![License](https://img.shields.io/pypi/l/careamics-portfolio.svg?color=green)](https://github.com/CAREamics/careamics-portfolio/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/careamics-portfolio.svg?color=green)](https://pypi.org/project/careamics-portfolio)
 [![Python Version](https://img.shields.io/pypi/pyversions/careamics-portfolio.svg?color=green)](https://python.org)
 [![CI](https://github.com/CAREamics/careamics-portfolio/actions/workflows/ci.yml/badge.svg)](https://github.com/CAREamics/careamics-portfolio/actions/workflows/ci.yml)
 [![Datasets CI](https://github.com/CAREamics/careamics-portfolio/actions/workflows/datasets_ci.yml/badge.svg)](https://github.com/CAREamics/careamics-portfolio/actions/workflows/datasets_ci.yml)
 [![codecov](https://codecov.io/gh/CAREamics/careamics-portfolio/branch/main/graph/badge.svg)](https://codecov.io/gh/CAREamics/careamics-portfolio)
-[![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) 
-[![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
-[![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) 
 
-A helper package to download example datasets used in various publications by the Jug lab, including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
+A helper package based on [pooch](https://github.com/fatiando/pooch) allowing
+downloading various example datasets used in publications by the Jug lab,
+including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
 
-The portfolio relies on [pooch](https://github.com/fatiando/pooch) to download the datasets.
-
-The complete list of datasets can be found [here](https://raw.githubusercontent.com/CAREamics/careamics-portfolio/src/careamics_portfolio/datasets/datasets.json).
+The complete list of datasets can be found in 
+[datasets.json](https://raw.githubusercontent.com/CAREamics/careamics-portfolio/main/datasets/datasets.json).
 
+CAREamics-portfolio tooling was generated using [pydev-guide/pyrepo-copier](https://github.com/pydev-guide/pyrepo-copier).
 
 ## Installation
 
 To install the portfolio in your conda environment, simply use `pip`:
 ```bash
 $ pip install careamics-portfolio
 ```
@@ -50,22 +49,50 @@
 ```
 
 Finally, you can download the dataset of your choice:
 ```python
 from pathlib import Path
 
 data_path = Path('data')
+
+# to the path of your choice
 portfolio.denoising.N2V_SEM.download(data_path)
+
+# or to your system's cache
+portfolio.denoising.N2V_SEM.download()
 ```
 
 By default, if you do not pass `path` to the `download()` method, all datasets
 will be saved in your system's cache. New queries to download will not cause
-the files to be downloaded again (thanks pooch!).
+the files to be downloaded again (thanks pooch!!).
+
+**Important**: if you download all datasets of interest using the same path, 
+[pooch](https://github.com/fatiando/pooch) will maintain a regsitry of files
+and you will not have to download them again!
+
+## Add a dataset to the portfolio
+
+There are a few steps to follow in order to add a new dataset to the repository:
+
+:white_check_mark: 1 - Create a `PortfolioEntry` child class
+
+:white_check_mark: 2 - Instantiate the portfolio entry in an `IterablePortfolio`
 
-## Add a dataset to the repository
+:white_check_mark: 3 - Update `registry.txt`
+
+:white_check_mark: 4 - Make sure all tests pass
+
+
+> Note: To run the tests, you will need to have `pytest` installed. You can
+> create an environment with `careamics-portfolio` and `pytest` by running:
+> ```bash
+> pip install "careamics-portfolio[test]"
+> ```
+
+### 1 - Create a portfolio entry
 
 To add a dataset, subclass a `PortfolioEntry` and enter the following information 
 (preferably in one of the current categories, e.g. `denoising_datasets.py`):
 ```python
 class MyDataset(PortfolioEntry):
     def __init__(self) -> None:
         super().__init__(
@@ -83,30 +110,33 @@
             size=13.0, # size in MB
             tags=["tag1", "tag2"],
             is_zip=True,
         )
 ```
 
 To obtain sha256 hash of your file, you can run the following code and read out
-the sha256 from pooch prompt:
+the sha256 from the pooch prompt:
 ```python
 import pooch
 
 url = "https://url.to.myfile/MyFile.zip"
 pooch.retrieve(url, known_hash=None)
 ```
 
 Likewise, to get the size in MB of your file:
 ```python
 import os
 
 os.path.getsize(file_path) / 1024 / 1024
 ```
 
-Finally, add the file class to one of the categories (e.g. denoising) in 
+
+### 2 - Add the entry to a portfolio
+
+Add the file class to one of the categories (e.g. denoising) in 
 `portfolio.py`:
 ```python
 class Denoising(IterablePortfolio):
     def __init__(self) -> None:
         self._N2V_BSD68 = N2V_BSD68()
         self._N2V_SEM = N2V_SEM()
         self._N2V_RGB = N2V_RGB()
@@ -118,7 +148,35 @@
         [...]
 
     # and add a public getter
     @property
     def MyDataset(self) -> MyDataset:
         return self._myDataset
 ```
+
+### 3 - Update registry
+
+Finally, update the registry by running the following pythons script:
+```bash
+python script/update_registry.py
+```
+
+or run:
+```python
+from careamics_portfolio import update_registry
+update_registry()
+```
+
+The [datasets.json](https://raw.githubusercontent.com/CAREamics/careamics-portfolio/main/datasets/datasets.json)
+file is updated using:
+```bash
+python script/update_json.py
+```
+
+### 4 - Verify that all tests pass
+
+Verify that all tests pass, it can take a while:
+
+```bash
+pytest
+```
+
```

### Comparing `careamics_portfolio-0.0.7/pyproject.toml` & `careamics_portfolio-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     # "License :: OSI Approved :: BSD License",
     # "Typing :: Typed",
 ]
 # add your package dependencies here
-dependencies = ["tqdm", "pooch"]
+dependencies = ["tqdm", "pooch>=1.6.0"]
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 # "extras" (e.g. for `pip install .[test]`)
 [project.optional-dependencies]
 # add dependencies used for testing here
 test = ["pytest", "pytest-cov"]
 # add anything else you like to have in your dev environment here
```

### Comparing `careamics_portfolio-0.0.7/PKG-INFO` & `careamics_portfolio-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: careamics-portfolio
-Version: 0.0.7
+Version: 0.0.8
 Summary: A helper package to download example datasets used in various publications and deep-learning algorithms, including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
 Project-URL: homepage, https://github.com/juglab-torch/careamics-portfolio
 Project-URL: repository, https://github.com/juglab-torch/careamics-portfolio
 Author-email: Joran Deschamps <joran.deschamps@fht.org>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: pooch
+Requires-Dist: pooch>=1.6.0
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
@@ -40,24 +40,23 @@
 
 [![License](https://img.shields.io/pypi/l/careamics-portfolio.svg?color=green)](https://github.com/CAREamics/careamics-portfolio/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/careamics-portfolio.svg?color=green)](https://pypi.org/project/careamics-portfolio)
 [![Python Version](https://img.shields.io/pypi/pyversions/careamics-portfolio.svg?color=green)](https://python.org)
 [![CI](https://github.com/CAREamics/careamics-portfolio/actions/workflows/ci.yml/badge.svg)](https://github.com/CAREamics/careamics-portfolio/actions/workflows/ci.yml)
 [![Datasets CI](https://github.com/CAREamics/careamics-portfolio/actions/workflows/datasets_ci.yml/badge.svg)](https://github.com/CAREamics/careamics-portfolio/actions/workflows/datasets_ci.yml)
 [![codecov](https://codecov.io/gh/CAREamics/careamics-portfolio/branch/main/graph/badge.svg)](https://codecov.io/gh/CAREamics/careamics-portfolio)
-[![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) 
-[![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
-[![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) 
 
-A helper package to download example datasets used in various publications by the Jug lab, including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
+A helper package based on [pooch](https://github.com/fatiando/pooch) allowing
+downloading various example datasets used in publications by the Jug lab,
+including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
 
-The portfolio relies on [pooch](https://github.com/fatiando/pooch) to download the datasets.
-
-The complete list of datasets can be found [here](https://raw.githubusercontent.com/CAREamics/careamics-portfolio/src/careamics_portfolio/datasets/datasets.json).
+The complete list of datasets can be found in 
+[datasets.json](https://raw.githubusercontent.com/CAREamics/careamics-portfolio/main/datasets/datasets.json).
 
+CAREamics-portfolio tooling was generated using [pydev-guide/pyrepo-copier](https://github.com/pydev-guide/pyrepo-copier).
 
 ## Installation
 
 To install the portfolio in your conda environment, simply use `pip`:
 ```bash
 $ pip install careamics-portfolio
 ```
@@ -82,22 +81,50 @@
 ```
 
 Finally, you can download the dataset of your choice:
 ```python
 from pathlib import Path
 
 data_path = Path('data')
+
+# to the path of your choice
 portfolio.denoising.N2V_SEM.download(data_path)
+
+# or to your system's cache
+portfolio.denoising.N2V_SEM.download()
 ```
 
 By default, if you do not pass `path` to the `download()` method, all datasets
 will be saved in your system's cache. New queries to download will not cause
-the files to be downloaded again (thanks pooch!).
+the files to be downloaded again (thanks pooch!!).
+
+**Important**: if you download all datasets of interest using the same path, 
+[pooch](https://github.com/fatiando/pooch) will maintain a regsitry of files
+and you will not have to download them again!
+
+## Add a dataset to the portfolio
+
+There are a few steps to follow in order to add a new dataset to the repository:
+
+:white_check_mark: 1 - Create a `PortfolioEntry` child class
+
+:white_check_mark: 2 - Instantiate the portfolio entry in an `IterablePortfolio`
 
-## Add a dataset to the repository
+:white_check_mark: 3 - Update `registry.txt`
+
+:white_check_mark: 4 - Make sure all tests pass
+
+
+> Note: To run the tests, you will need to have `pytest` installed. You can
+> create an environment with `careamics-portfolio` and `pytest` by running:
+> ```bash
+> pip install "careamics-portfolio[test]"
+> ```
+
+### 1 - Create a portfolio entry
 
 To add a dataset, subclass a `PortfolioEntry` and enter the following information 
 (preferably in one of the current categories, e.g. `denoising_datasets.py`):
 ```python
 class MyDataset(PortfolioEntry):
     def __init__(self) -> None:
         super().__init__(
@@ -115,30 +142,33 @@
             size=13.0, # size in MB
             tags=["tag1", "tag2"],
             is_zip=True,
         )
 ```
 
 To obtain sha256 hash of your file, you can run the following code and read out
-the sha256 from pooch prompt:
+the sha256 from the pooch prompt:
 ```python
 import pooch
 
 url = "https://url.to.myfile/MyFile.zip"
 pooch.retrieve(url, known_hash=None)
 ```
 
 Likewise, to get the size in MB of your file:
 ```python
 import os
 
 os.path.getsize(file_path) / 1024 / 1024
 ```
 
-Finally, add the file class to one of the categories (e.g. denoising) in 
+
+### 2 - Add the entry to a portfolio
+
+Add the file class to one of the categories (e.g. denoising) in 
 `portfolio.py`:
 ```python
 class Denoising(IterablePortfolio):
     def __init__(self) -> None:
         self._N2V_BSD68 = N2V_BSD68()
         self._N2V_SEM = N2V_SEM()
         self._N2V_RGB = N2V_RGB()
@@ -150,7 +180,35 @@
         [...]
 
     # and add a public getter
     @property
     def MyDataset(self) -> MyDataset:
         return self._myDataset
 ```
+
+### 3 - Update registry
+
+Finally, update the registry by running the following pythons script:
+```bash
+python script/update_registry.py
+```
+
+or run:
+```python
+from careamics_portfolio import update_registry
+update_registry()
+```
+
+The [datasets.json](https://raw.githubusercontent.com/CAREamics/careamics-portfolio/main/datasets/datasets.json)
+file is updated using:
+```bash
+python script/update_json.py
+```
+
+### 4 - Verify that all tests pass
+
+Verify that all tests pass, it can take a while:
+
+```bash
+pytest
+```
+
```

