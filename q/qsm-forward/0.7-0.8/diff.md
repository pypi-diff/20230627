# Comparing `tmp/qsm-forward-0.7.tar.gz` & `tmp/qsm-forward-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.7.tar", last modified: Fri Jun 16 01:51:07 2023, max compression
+gzip compressed data, was "qsm-forward-0.8.tar", last modified: Tue Jun 27 01:21:32 2023, max compression
```

## Comparing `qsm-forward-0.7.tar` & `qsm-forward-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.7/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-16 01:51:07.849577 qsm-forward-0.7/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)     5541 2023-06-15 07:31:12.000000 qsm-forward-0.7/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-16 01:19:51.000000 qsm-forward-0.7/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      497 2023-06-16 01:20:38.000000 qsm-forward-0.7/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    27568 2023-06-16 01:48:28.000000 qsm-forward-0.7/qsm_forward/qsm_forward.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-16 01:51:07.000000 qsm-forward-0.7/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-16 01:51:07.849577 qsm-forward-0.7/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-16 01:19:55.000000 qsm-forward-0.7/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-16 01:51:07.849577 qsm-forward-0.7/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.7/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.8/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     9000 2023-06-27 01:21:32.515067 qsm-forward-0.8/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     8229 2023-06-27 01:16:59.000000 qsm-forward-0.8/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-27 01:15:26.000000 qsm-forward-0.8/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      497 2023-06-16 01:20:38.000000 qsm-forward-0.8/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    29159 2023-06-27 00:56:58.000000 qsm-forward-0.8/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     9000 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-27 01:21:32.515067 qsm-forward-0.8/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-27 01:15:36.000000 qsm-forward-0.8/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.8/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.7/LICENSE` & `qsm-forward-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.7/PKG-INFO` & `qsm-forward-0.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: qsm-forward
-Version: 0.7
-Summary: A forward-model simulation for Quantitative Susceptibility Mapping
-Home-page: https://github.com/astewartau/qsm-forward-model
-Author: Ashley Stewart
-Author-email: Ashley Stewart <a.stewart.au@gmail.com>
-Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
-Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # QSM Forward Model
 
 Based on Marques, J. P., et al. (2021). QSM reconstruction challenge 2.0: A realistic in silico head phantom for MRI data simulation and evaluation of susceptibility mapping procedures. Magnetic Resonance in Medicine, 86(1), 526-542. https://doi.org/10.1002/mrm.28716
 
 Includes code for:
 
  - Field model (forward multiplication with dipole kernel based on chi)
@@ -31,17 +13,65 @@
 
 ## Install
 
 ```
 pip install qsm-forward
 ```
 
-## Example
+## Example using simulated sources
+
+In this example, we simulated susceptibility sources (spheres and rectangles) to generate a BIDS directory:
+
+```python
+import qsm_forward
+
+if __name__ == "__main__":
+    recon_params = qsm_forward.ReconParams()
+    recon_params.subject = "simulated-sources"
+    recon_params.peak_snr = 100
+
+    tissue_params = qsm_forward.TissueParams(chi=qsm_forward.simulate_susceptibility_sources())
+    
+    qsm_forward.generate_bids(tissue_params, recon_params, "bids")
+```
+
+```
+bids/
+└── sub-simulated-sources
+    └── ses-1
+        ├── anat
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-1_part-mag_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-1_part-mag_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-1_part-phase_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-1_part-phase_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-2_part-mag_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-2_part-mag_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-2_part-phase_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-2_part-phase_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-3_part-mag_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-3_part-mag_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-3_part-phase_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-3_part-phase_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-4_part-mag_MEGRE.json
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-4_part-mag_MEGRE.nii
+        │   ├── sub-simulated-sources_ses-1_run-1_echo-4_part-phase_MEGRE.json
+        │   └── sub-simulated-sources_ses-1_run-1_echo-4_part-phase_MEGRE.nii
+        └── extra_data
+            ├── sub-simulated-sources_ses-1_run-1_chi.nii
+            ├── sub-simulated-sources_ses-1_run-1_mask.nii
+            └── sub-simulated-sources_ses-1_run-1_segmentation.nii
+```
+
+Some repesentative images including the mask, first and last-echo phase image, and ground truth susceptibility (chi):
 
-In this example, we generate a BIDS-compliant dataset based on simulated data:
+![Image](https://i.imgur.com/dtklHUh.png)
+
+## Example using head phantom data
+
+In this example, we generate a BIDS-compliant dataset based on head phantom maps. You must provide these maps yourself by gaining access to the QSM Challenge 2.0 head phantom data or generating your own realistic maps:
 
 ```python
 import qsm_forward
 import numpy as np
 
 if __name__ == "__main__":
     tissue_params = qsm_forward.TissueParams("../head-phantom-maps")
@@ -126,7 +156,12 @@
         │   └── sub-1_ses-1p2_run-1_echo-4_part-phase_MEGRE.nii
         └── extra_data
             ├── sub-1_ses-1p2_run-1_chi.nii
             ├── sub-1_ses-1p2_run-1_mask.nii
             └── sub-1_ses-1p2_run-1_segmentation.nii
 ```
 
+Some repesentative images including the ground truth chi map, first-echo magnitude image, and first and last-echo phase images:
+
+![Image](https://i.imgur.com/cE1cQ3U.png)
+
+
```

### Comparing `qsm-forward-0.7/pyproject.toml` & `qsm-forward-0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.7"
+version = "0.8"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.7/qsm_forward/qsm_forward.py` & `qsm-forward-0.8/qsm_forward/qsm_forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             self,
             root_dir = "",
             chi = "ChiModelMIX_noCalc.nii.gz",
             M0 = "M0.nii.gz",
             R1 = "R1.nii.gz",
             R2star = "R2star.nii.gz",
             mask = "BrainMask.nii.gz",
-            seg = "SegmentedModel.nii.gz"
+            seg = "SegmentedModel.nii.gz",
     ):
         if isinstance(chi, str) and not os.path.exists(os.path.join(root_dir, chi)):
             raise ValueError(f"Path to chi is invalid! ({os.path.join(root_dir, chi)})")
         self._chi = os.path.join(root_dir, chi) if isinstance(chi, str) and os.path.exists(os.path.join(root_dir, chi)) else chi if not isinstance(chi, str) else None
         self._M0 = os.path.join(root_dir, M0) if isinstance(M0, str) and os.path.exists(os.path.join(root_dir, M0)) else M0 if not isinstance(M0, str) else None
         self._R1 = os.path.join(root_dir, R1) if isinstance(R1, str) and os.path.exists(os.path.join(root_dir, R1)) else R1 if not isinstance(R1, str) else None
         self._R2star = os.path.join(root_dir, R2star) if isinstance(R2star, str) and os.path.exists(os.path.join(root_dir, R2star)) else R2star if not isinstance(R2star, str) else None
@@ -68,24 +68,66 @@
     def chi(self): return nib.load(self._chi) if isinstance(self._chi, str) else nib.Nifti1Image(self._chi, affine=self.nii_affine, header=self.nii_header)
 
     @property
     def mask(self): return nib.load(self._mask) if isinstance(self._mask, str) else nib.Nifti1Image(self._mask or np.array(self._chi != 0), affine=self.nii_affine, header=self.nii_header)
 
     @property
     def M0(self): return nib.load(self._M0) if isinstance(self._M0, str) else nib.Nifti1Image(self._M0 or np.array(self.mask.get_fdata() * 1), affine=self.nii_affine, header=self.nii_header)
+    #def M0(self): return nib.load(self._M0) if isinstance(self._M0, str) else nib.Nifti1Image(self._estimate_M0(1, self.chi.get_fdata()), affine=self.nii_affine, header=self.nii_header)
 
     @property
     def R1(self): return nib.load(self._R1) if isinstance(self._R1, str) else nib.Nifti1Image(self._R1 or np.array(self.mask.get_fdata() * 1), affine=self.nii_affine, header=self.nii_header)
     
     @property
     def R2star(self): return nib.load(self._R2star) if isinstance(self._R2star, str) else nib.Nifti1Image(self._R2star or np.array(self.mask.get_fdata() * 50), affine=self.nii_affine, header=self.nii_header)
     
     @property
     def seg(self): return nib.load(self._seg) if isinstance(self._seg, str) else nib.Nifti1Image(self._seg or self.mask.get_fdata(), affine=self.nii_affine, header=self.nii_header)
     
+    def _estimate_M0(self, B0, chi):
+        """
+        Calculate the equilibrium magnetization M0 based on B0 field strength and magnetic susceptibility (chi).
+
+        Parameters
+        ----------
+        B0 : float
+            The main magnetic field strength (in T).
+        chi : numpy.ndarray
+            The magnetic susceptibility map.
+
+        Returns
+        -------
+        M0 : numpy.ndarray
+            The calculated equilibrium magnetization.
+        """
+        
+        # Constants
+        k = 1.38064852e-23  # Boltzmann constant (m^2 kg s^-2 K^-1)
+        h = 6.62607015e-34  # Planck's constant (m^2 kg s^-1)
+        gamma = 267.522190e3  # proton gyromagnetic ratio (kHz/T to Hz/T)
+        rho = 65  # proton density (mol/L)
+        T = 298.15  # absolute temperature (K)
+        
+        # Convert gamma from Hz/T to rad/(s*T)
+        gamma = gamma * 2 * np.pi * 1e3 
+
+        # Convert rho from mol/L to mol/m^3
+        rho = rho * 1e3
+
+        # Calculate B from B0 and chi
+        B = B0 * (1 + chi)
+
+        # Calculate M0
+        M0 = gamma * rho * h * B / (2 * k * T)
+
+        nib.save(nib.Nifti1Image(M0, affine=self.nii_affine, header=self.nii_header), "M0_TEST.nii")
+        nib.save(nib.Nifti1Image(B, affine=self.nii_affine, header=self.nii_header), "B_TEST.nii")
+
+        return M0
+
 
 class ReconParams:
     """
     A class used to represent reconstruction parameters.
 
     Attributes
     ----------
@@ -232,15 +274,15 @@
         print(f"Simulating noise for echo {i+1}...")
         sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params.peak_snr)
         del sigHR_cropped
 
         # save nifti images
         mag_filename = f"{recon_name_i}_part-mag" + ("_MEGRE" if multiecho else "_T2starw")
         phs_filename = f"{recon_name_i}_part-phase" + ("_MEGRE" if multiecho else "_T2starw")
-        nib.save(nib.Nifti1Image(dataobj=np.abs(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{mag_filename}.nii"))
+        nib.save(nib.Nifti1Image(dataobj=np.abs(sigHR_cropped_noisy)*500, affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{mag_filename}.nii"))
         nib.save(nib.Nifti1Image(dataobj=np.angle(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{phs_filename}.nii"))
 
         # json header
         print(f"Creating JSON headers...")
         json_dict = { 'EchoTime': recon_params.TEs[i], 'MagneticFieldStrength': recon_params.B0, 'EchoNumber': i+1, 'ProtocolName': 'T2starw', 'ConversionSoftware': 'qsm-forward' }
 
         json_dict_phs = json_dict.copy()
@@ -252,15 +294,15 @@
             json.dump(json_dict_mag, mag_json_file)
         with open(os.path.join(session_dir, "anat", f"{phs_filename}.json"), 'w') as phs_json_file:
             json.dump(json_dict_phs, phs_json_file)
 
     print("Done!")
 
 
-def generate_field(chi):
+def generate_field(chi, voxel_size=[1, 1, 1], B0_dir=[0, 0, 1]):
     """
     Perform the forward convolution operation.
 
     This function performs the forward convolution step of the QSM simulation.
 
     Parameters
     ----------
@@ -270,15 +312,15 @@
     Returns
     -------
     numpy.ndarray
         The resulting magnetic field array after the forward convolution operation.
 
     """
     dims = np.array(chi.shape)
-    D = _generate_3d_dipole_kernel(data_shape=dims, voxel_size=[1, 1, 1], b0_dir=[0, 0, 1])
+    D = _generate_3d_dipole_kernel(data_shape=dims, voxel_size=voxel_size, B0_dir=B0_dir)
     
     chitemp = np.ones(2 * dims) * chi[-1, -1, -1]
     chitemp[:dims[0], :dims[1], :dims[2]] = chi
     field = np.real(np.fft.ifftn(np.fft.fftn(chitemp) * D))
     field = field[:dims[0], :dims[1], :dims[2]]
 
     return field
@@ -537,27 +579,27 @@
 
     if scaling:
         working_volume *= np.prod(dims) / np.prod(volume.shape)
     
     return working_volume
 
 
-def _generate_3d_dipole_kernel(data_shape, voxel_size, b0_dir):
+def _generate_3d_dipole_kernel(data_shape, voxel_size, B0_dir):
     """
     Generate a 3D dipole kernel.
 
     This function generates a 3D dipole kernel used in the forward convolution step of the QSM simulation.
 
     Parameters
     ----------
     data_shape : tuple of int
         The shape of the data array (nx, ny, nz).
     voxel_size : list of float
         The size of a voxel in each direction (dx, dy, dz).
-    b0_dir : list of float
+    B0_dir : list of float
         The direction of the B0 field (B0x, B0y, B0z).
 
     Returns
     -------
     numpy.ndarray
         A 3D array representing the dipole kernel.
 
@@ -570,15 +612,15 @@
 
     kx = kx / (2 * voxel_size[0] * np.max(np.abs(kx)))
     ky = ky / (2 * voxel_size[1] * np.max(np.abs(ky)))
     kz = kz / (2 * voxel_size[2] * np.max(np.abs(kz)))
 
     k2 = kx**2 + ky**2 + kz**2
     k2[k2 == 0] = np.finfo(float).eps
-    D = np.fft.fftshift(1 / 3 - ((kx * b0_dir[0] + ky * b0_dir[1] + kz * b0_dir[2])**2 / k2))
+    D = np.fft.fftshift(1 / 3 - ((kx * B0_dir[0] + ky * B0_dir[1] + kz * B0_dir[2])**2 / k2))
     
     return D
 
 
 def _center_of_mass(data):
     """
     Compute the center of mass of a 3D array.
```

### Comparing `qsm-forward-0.7/setup.py` & `qsm-forward-0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

