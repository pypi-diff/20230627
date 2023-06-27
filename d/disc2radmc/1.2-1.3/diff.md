# Comparing `tmp/disc2radmc-1.2.tar.gz` & `tmp/disc2radmc-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/disc2radmc-1.2.tar", last modified: Thu Jun 16 13:30:18 2022, max compression
+gzip compressed data, was "disc2radmc-1.3.tar", last modified: Tue Jun 27 14:42:31 2023, max compression
```

## Comparing `disc2radmc-1.2.tar` & `disc2radmc-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Sebamarino   (501) staff       (20)        0 2022-06-16 13:30:18.000000 disc2radmc-1.2/
--rw-r--r--   0 Sebamarino   (501) staff       (20)     1026 2022-06-16 13:30:18.000000 disc2radmc-1.2/PKG-INFO
--rw-r--r--   0 Sebamarino   (501) staff       (20)      804 2022-02-24 16:58:21.000000 disc2radmc-1.2/README.md
-drwxr-xr-x   0 Sebamarino   (501) staff       (20)        0 2022-06-16 13:30:18.000000 disc2radmc-1.2/disc2radmc/
--rw-r--r--   0 Sebamarino   (501) staff       (20)      304 2022-02-24 15:56:09.000000 disc2radmc-1.2/disc2radmc/__init__.py
--rw-r--r--   0 Sebamarino   (501) staff       (20)      434 2022-04-11 14:50:38.000000 disc2radmc-1.2/disc2radmc/constants.py
--rw-r--r--   0 Sebamarino   (501) staff       (20)    16112 2022-04-18 17:31:44.000000 disc2radmc-1.2/disc2radmc/functions_misc.py
--rw-r--r--   0 Sebamarino   (501) staff       (20)    36447 2022-06-16 11:00:53.000000 disc2radmc-1.2/disc2radmc/model.py
--rw-r--r--   0 Sebamarino   (501) staff       (20)    34506 2021-11-22 12:31:04.000000 disc2radmc-1.2/disc2radmc/model_old.py
-drwxr-xr-x   0 Sebamarino   (501) staff       (20)        0 2022-06-16 13:30:18.000000 disc2radmc-1.2/disc2radmc.egg-info/
--rw-r--r--   0 Sebamarino   (501) staff       (20)     1026 2022-06-16 13:30:17.000000 disc2radmc-1.2/disc2radmc.egg-info/PKG-INFO
--rw-r--r--   0 Sebamarino   (501) staff       (20)      317 2022-06-16 13:30:17.000000 disc2radmc-1.2/disc2radmc.egg-info/SOURCES.txt
--rw-r--r--   0 Sebamarino   (501) staff       (20)        1 2022-06-16 13:30:17.000000 disc2radmc-1.2/disc2radmc.egg-info/dependency_links.txt
--rw-r--r--   0 Sebamarino   (501) staff       (20)       35 2022-06-16 13:30:17.000000 disc2radmc-1.2/disc2radmc.egg-info/requires.txt
--rw-r--r--   0 Sebamarino   (501) staff       (20)       11 2022-06-16 13:30:17.000000 disc2radmc-1.2/disc2radmc.egg-info/top_level.txt
--rw-r--r--   0 Sebamarino   (501) staff       (20)       79 2022-06-16 13:30:18.000000 disc2radmc-1.2/setup.cfg
--rw-r--r--   0 Sebamarino   (501) staff       (20)     1991 2022-06-16 13:26:11.000000 disc2radmc-1.2/setup.py
+drwxr-xr-x   0 smarino  (8005548) staff       (20)        0 2023-06-27 14:42:31.563883 disc2radmc-1.3/
+-rw-r--r--   0 smarino  (8005548) staff       (20)     1069 2023-01-31 15:06:34.000000 disc2radmc-1.3/LICENSE.txt
+-rw-r--r--   0 smarino  (8005548) staff       (20)     1013 2023-06-27 14:42:31.563942 disc2radmc-1.3/PKG-INFO
+-rw-r--r--   0 smarino  (8005548) staff       (20)      736 2023-01-31 15:06:34.000000 disc2radmc-1.3/README.md
+drwxr-xr-x   0 smarino  (8005548) staff       (20)        0 2023-06-27 14:42:31.563058 disc2radmc-1.3/disc2radmc/
+-rw-r--r--   0 smarino  (8005548) staff       (20)      304 2023-01-31 15:09:11.000000 disc2radmc-1.3/disc2radmc/__init__.py
+-rw-r--r--   0 smarino  (8005548) staff       (20)      434 2023-01-31 15:09:11.000000 disc2radmc-1.3/disc2radmc/constants.py
+-rw-r--r--   0 smarino  (8005548) staff       (20)    18157 2023-01-31 15:09:11.000000 disc2radmc-1.3/disc2radmc/functions_misc.py
+-rw-r--r--   0 smarino  (8005548) staff       (20)    37762 2023-06-05 09:39:25.000000 disc2radmc-1.3/disc2radmc/model.py
+drwxr-xr-x   0 smarino  (8005548) staff       (20)        0 2023-06-27 14:42:31.563766 disc2radmc-1.3/disc2radmc.egg-info/
+-rw-r--r--   0 smarino  (8005548) staff       (20)     1013 2023-06-27 14:42:31.000000 disc2radmc-1.3/disc2radmc.egg-info/PKG-INFO
+-rw-r--r--   0 smarino  (8005548) staff       (20)      305 2023-06-27 14:42:31.000000 disc2radmc-1.3/disc2radmc.egg-info/SOURCES.txt
+-rw-r--r--   0 smarino  (8005548) staff       (20)        1 2023-06-27 14:42:31.000000 disc2radmc-1.3/disc2radmc.egg-info/dependency_links.txt
+-rw-r--r--   0 smarino  (8005548) staff       (20)       35 2023-06-27 14:42:31.000000 disc2radmc-1.3/disc2radmc.egg-info/requires.txt
+-rw-r--r--   0 smarino  (8005548) staff       (20)       11 2023-06-27 14:42:31.000000 disc2radmc-1.3/disc2radmc.egg-info/top_level.txt
+-rw-r--r--   0 smarino  (8005548) staff       (20)       79 2023-06-27 14:42:31.564191 disc2radmc-1.3/setup.cfg
+-rw-r--r--   0 smarino  (8005548) staff       (20)     1991 2023-06-27 14:40:50.000000 disc2radmc-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `disc2radmc-1.2/PKG-INFO` & `disc2radmc-1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: disc2radmc
-Version: 1.2
+Version: 1.3
 Summary: Disc2radmc is a package to create parametric models of debris discs that can be fed into RADMC3D and simulate images of dust and gas emission.
 Home-page: https://github.com/SebaMarino/disc2radmc
+Download-URL: https://github.com/SebaMarino/disc2radmc/archive/refs/tags/v1.3.tar.gz
 Author: Sebastian Marino
 Author-email: sebastian.marino.estay@gmail.com
 License: MIT
-Download-URL: https://github.com/SebaMarino/disc2radmc/archive/refs/tags/v1.2.tar.gz
-Description: UNKNOWN
 Keywords: radiative transfer,debris disc,radmc3d,circumstellar disc
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE.txt
```

### Comparing `disc2radmc-1.2/README.md` & `disc2radmc-1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 
 ## Usage
 
 See example in [docs/example_dust/Dust_model.ipynb](https://github.com/SebaMarino/disc2radmc/tree/main/docs/example_dust/Dust_model.ipynb) to know how to make images of dust and example at [docs/example_gas/Gas_model.ipynb](https://github.com/SebaMarino/disc2radmc/blob/main/docs/example_gas/Gas_model.ipynb) to make images (cubes) of gas.
 
 ## Credits
 
-If you use it for a project please cite Marino et al. 2018, MNRAS, Volume 479, Issue 4, p.5423-5439 (https://ui.adsabs.harvard.edu/abs/2018MNRAS.479.5423M/abstract) and Marino et al. in prep.
+If you use it for a project please cite Marino et al. 2022 (https://ui.adsabs.harvard.edu/abs/2022MNRAS.tmp.1702M/abstract)
```

### Comparing `disc2radmc-1.2/disc2radmc/functions_misc.py` & `disc2radmc-1.3/disc2radmc/functions_misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 import numpy as np
 import cmath as cma
 from disc2radmc.constants import *
 from astropy.io import fits
 from astropy.convolution import convolve_fft
-
+import os
 
 # function to define vertical distribution
 def rhoz_Gaussian(z, H):
     return np.exp(-(z)**2.0/(2.0*H**2.0))/(np.sqrt(2.0*np.pi)*H)
 
 #### Functions to mix optical constants following Bruggeman's mixing rule
 
@@ -61,19 +61,19 @@
     elif xi>x[Nx-1]:    #extrapol                                                                                                                                                                                                            
         alpha=np.log(y[Nx-1]/y[Nx-2])/np.log(x[Nx-1]/x[Nx-2])
         return y[Nx-1]*(xi/x[Nx-1])**alpha
 
 
 ### functions to manipulate images
 
-def convert_to_fits(path_image, path_fits, Npixf, dpc, mx=0.0, my=0.0, x0=0.0, y0=0.0, omega=0.0, fstar=-1.0, vel=False, continuum_subtraction=False, background_args=[], tag='', primary_beam=None, alpha_dust=None, new_lambda=None, verbose=False):
+def convert_to_fits(path_image, path_fits, Npixf, dpc, mx=0.0, my=0.0, x0=0.0, y0=0.0, omega=0.0, fstar=-1.0, vel=False, continuum_subtraction=False, background_args=[], tag='', primary_beam=None, alpha_dust=None, new_lambda=None, verbose=False, taumap=False):
     # alpha is defined as the spectral index in frequency space, and thus is positive for a typical disc and star at mm wavelengths
     
     ### load image
-    image_in_jypix, nx, ny, nf, lam, pixdeg_x, pixdeg_y = load_image(path_image, dpc)
+    image_in_jypix, nx, ny, nf, lam, pixdeg_x, pixdeg_y = load_image(path_image, dpc, taumap=taumap)
     istar, jstar=star_pix(nx, omega)
     
     ## if alpha is given, then disc surface brightness and stellar flux are manipulated
     if alpha_dust is not None and new_lambda is not None:
         Fstar=image_in_jypix[0,0,jstar,istar] # save stellar flux
         ### apply dust spectral index
         image_in_jypix[0,0,jstar,istar]=0.0
@@ -118,22 +118,22 @@
         inans= np.isnan(image_in_jypix_shifted)
         image_in_jypix_shifted[inans]=0.0
         
     lam0=lam[0] # um   
     reffreq=cc/(lam0*1.0e-4) # Hz
 
     ### Single image
-    if nf==1: # single image
+    if nf==1 and not taumap: # single image
         flux = np.sum(image_in_jypix_shifted[0,0,:,:])
         
         if verbose: print("flux [Jy] = ", flux)
 
 
     ### image cube
-    else: 
+    elif not taumap: 
         delta_freq= (lam[0] - lam[1])*cc*1.0e4/lam[nf//2]**2.0 # Hz
         delta_velocity = (lam[1] - lam[0])*cc*1e-5/lam0 # km/s
 
         if continuum_subtraction: # subtract continuum assuming it varies linearly with wavelength
             if verbose: print('subtracting continuum')
             m=(image_in_jypix_shifted[0,-1,:,:]- image_in_jypix_shifted[0,0,:,:])/(lam[-1]-lam[0])
             I0=image_in_jypix_shifted[0,0,:,:]*1.
@@ -160,20 +160,25 @@
     header['VELREF']=0.0
     if nf==1:
         header['CTYPE3']='FREQ'
         header['CRPIX3'] = 1.0
         header['CDELT3']  = 1.0
         header['CRVAL3']= reffreq
 
-
-    header['FLUX']=flux
-    header['BTYPE'] = 'Intensity'
-    header['BSCALE'] = 1
-    header['BZERO'] = 0
-    header['BUNIT'] = 'JY/PIXEL'#'erg/s/cm^2/Hz/ster'
+    if not taumap:
+        header['FLUX']=flux
+        header['BTYPE'] = 'Intensity'
+        header['BSCALE'] = 1
+        header['BZERO'] = 0
+        header['BUNIT'] = 'JY/PIXEL'#'erg/s/cm^2/Hz/ster'
+    else:
+        header['BTYPE'] = 'Tau'
+        header['BSCALE'] = 1
+        header['BZERO'] = 0
+        header['BUNIT'] = ''#'erg/s/cm^2/Hz/ster'
 
 
     header['CTYPE1'] = 'RA---TAN'
     header['CTYPE2'] = 'DEC--TAN'
     if Npixf%2==1: ## if odd number of pixels, central pixel coincides with center
         header['CRVAL1'] = x0
         header['CRVAL2'] = y0
@@ -362,15 +367,15 @@
 
     header1['BUNIT']='Jy/beam'
 
     path_fits=path_image[:-5]+'_beamconvolved.fits'
     fits.writeto(path_fits, Fout1, header1, output_verify='fix', overwrite=True)
 
     
-def load_image(path_image, dpc):
+def load_image(path_image, dpc, taumap=False):
 
     f=open(path_image,'r')
     iformat=int(f.readline())
 
     if (iformat < 1) or (iformat > 4):
         assert False, "ERROR: File format of image not recognized"
 
@@ -388,30 +393,34 @@
 
     for k in range(nf):
         for j in range(ny):
             for i in range(nx):
 
                 image[0,k,j,i] = float(f.readline())
 
-                if (j == ny-1) and (i == nx-1):
-                    f.readline()
+                # if (j == ny-1) and (i == nx-1):
+                #     f.readline()
+        f.readline()
 
     f.close()
 
     # Compute the flux in this image as seen at dpc (pc)    
     pixdeg_x = 180.0*(sizepix_x/(dpc*pc))/np.pi
     pixdeg_y = 180.0*(sizepix_y/(dpc*pc))/np.pi
 
     # Compute the conversion factor from erg/cm^2/s/Hz/ster to erg/cm^2/s/Hz/ster at dpc
     pixsurf_ster = pixdeg_x*pixdeg_y * (np.pi/180.)**2
     factor = 1e+23 * pixsurf_ster
     # And scale the image array accordingly:
     image_in_jypix = factor * image
 
-    return image_in_jypix, nx, ny, nf, lam, pixdeg_x, pixdeg_y
+    if taumap:
+        return image, nx, ny, nf, lam, pixdeg_x, pixdeg_y
+    else:
+        return image_in_jypix, nx, ny, nf, lam, pixdeg_x, pixdeg_y
 
 
 def star_pix(nx, omega):
 
     omega= omega%360.0
 
     if nx%2==0.0: # even number of pixels
@@ -490,7 +499,46 @@
     ys=np.linspace(-Xmax, Xmax, Ni)
 
     Xs, Ys =np.meshgrid(xs, ys)
     rs=np.sqrt( (Xs-offx)**2. + (Ys-offy)**2. )
 
     F=Gauss2d(Xs , Ys, offx, offy, Rmaj, Rmin, -(Rpa+90.)*np.pi/180.)
     return F*Flux/np.sum(F)
+
+
+def append_new_line(file_name, text_to_append): # from https://thispointer.com/how-to-append-text-or-lines-to-a-file-in-python/
+    """Append given text as a new line at the end of file"""
+    # Open the file in append & read mode ('a+')
+    with open(file_name, "a+") as file_object:
+        # Move read cursor to the start of file.
+        file_object.seek(0)
+        # If file is not empty then append '\n'
+        data = file_object.read(100)
+        if len(data) > 0:
+            file_object.write("\n")
+        # Append text at the end of file
+        file_object.write(text_to_append)
+
+def delete_last_line(file_name, encoding="utf-8"): # adapted from https://stackoverflow.com/questions/1877999/delete-final-line-in-file-with-python
+
+    with open(file_name, "r+", encoding = encoding) as file:
+
+        # Move the pointer (similar to a cursor in a text editor) to the end of the file
+        file.seek(0, os.SEEK_END)
+
+        # This code means the following code skips the very last character in the file -
+        # i.e. in the case the last line is null we delete the last line
+        # and the penultimate one
+        pos = file.tell() - 1
+
+        # Read each character in the file one at a time from the penultimate
+        # character going backwards, searching for a newline character
+        # If we find a new line, exit the search
+        while pos > 0 and file.read(1) != "\n":
+            pos -= 1
+            file.seek(pos, os.SEEK_SET)
+
+        # So long as we're not at the start of the file, delete all the characters ahead
+        # of this position
+        if pos > 0:
+            file.seek(pos, os.SEEK_SET)
+            file.truncate()
```

### Comparing `disc2radmc-1.2/disc2radmc/model.py` & `disc2radmc-1.3/disc2radmc/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import os,sys
 from disc2radmc.constants import *
 from disc2radmc.functions_misc import *
 from astropy.io.votable import parse
+home_directory = os.path.expanduser( '~' )
+
 
 class simulation:
     """
     A class to run radmc3d and convert output files 
     """
 
     def __init__(self,  nphot=1000000, nphot_scat=1000000, nphot_spec=10000, nphot_mono=10000, scattering_mode=1, modified_random_walk=0, istar_sphere=0, tgas_eq_tdust=1, incl_lines=0, setthreads=4, rto_style=3, verbose=True):
@@ -50,37 +52,62 @@
 
     def mctherm(self):
         if self.verbose:
             os.system('radmc3d mctherm')
         else:
             os.system('radmc3d mctherm > mctherm.log')
 
-    def simimage(self, dpc=1., imagename='', wavelength=880., Npix=256, dpix=0.05, inc=0., PA=0., offx=0.0, offy=0.0, X0=0., Y0=0., tag='', omega=0.0, Npixf=-1, fstar=-1.0, background_args=[], primary_beam=None):
+    def simimage(self, dpc=1., imagename='', wavelength=880., Npix=256, dpix=0.05, inc=0., PA=0., offx=0.0, offy=0.0, X0=0., Y0=0., tag='', omega=0.0, Npixf=-1, fstar=-1.0, background_args=[], primary_beam=None, taumap=False):
         # X0, Y0, stellar position (e.g. useful if using a mosaic)
         # images: array of names for images produced at wavelengths
         # wavelgnths: wavelengths at which to produce image in um
         # fields: fields where to make images (=[0] unless observations are a mosaic)
 
         if Npixf==-1:
             Npixf=Npix
 
         sau=Npix*dpix*dpc
-        image_command='radmc3d image incl %1.5f  phi  %1.5f posang %1.5f  npix %1.0f  lambda %1.5f sizeau %1.5f  secondorder'%(inc,omega, PA-90.0, Npix, wavelength, sau)
+
+        if hasattr(wavelength, "__len__"):
+            image_command='radmc3d image incl %1.5f  phi  %1.5f posang %1.5f  npix %1.0f  loadlambda sizeau %1.5f  secondorder'%(inc,omega, PA-90.0, Npix, sau)
+            # write wavelengths into camera_wavelength_micron.inp
+            Nw=len(wavelength)
+            path='camera_wavelength_micron.inp'
+            arch=open(path,'w')
+            arch.write(str(Nw)+'\n')
+            for i in range(Nw):
+                arch.write('%1.8e \n'%(wavelength[i]))
+            arch.close()
+
+        else:
+            image_command='radmc3d image incl %1.5f  phi  %1.5f posang %1.5f  npix %1.0f  lambda %1.5f sizeau %1.5f  secondorder'%(inc,omega, PA-90.0, Npix, wavelength, sau)
+
+        if taumap: # compute taumap instead of image. Need to modify radmc3d.inp
+            append_new_line("radmc3d.inp", 'camera_tracemode = -2')
+            
         if self.verbose:
             print('image size = %1.1e au'%sau)
             print(image_command)
             os.system(image_command)
         else:
             os.system(image_command+'  > simimgaes.log')
 
-        pathin ='image_'+imagename+'_'+tag+'.out'
-        pathout='images/image_'+imagename+'_'+tag+'.fits'
+        if taumap: # compute taumap instead of image. Need to remove last line in radmc3d.inp 
+            delete_last_line("radmc3d.inp")
+            
+        if taumap:
+            pathin ='image_'+imagename+'_'+tag+'_taumap.out'
+            pathout='images/image_'+imagename+'_'+tag+'_taumap.fits'
+        else:
+            pathin ='image_'+imagename+'_'+tag+'.out'
+            pathout='images/image_'+imagename+'_'+tag+'.fits'
+
         os.system('mv image.out '+pathin)
         
-        convert_to_fits(pathin, pathout, Npixf, dpc, mx=offx, my=offy, x0=X0, y0=Y0, omega=omega,  fstar=fstar, background_args=background_args, tag=tag, primary_beam=primary_beam)
+        convert_to_fits(pathin, pathout, Npixf, dpc, mx=offx, my=offy, x0=X0, y0=Y0, omega=omega,  fstar=fstar, background_args=background_args, tag=tag, primary_beam=primary_beam, taumap=taumap)
 
     
     def simcube(self, dpc=1., imagename='', mol=1, line=1, vmax=30., Nnu=20, Npix=256, dpix=0.05, inc=0., PA=0., offx=0., offy=0., X0=0., Y0=0., tag='', omega=0., Npixf=-1, fstar=-1., background_args=[], primary_beam=None, vel=False, continuum_subtraction=False):
 
         if Npixf==-1:
             Npixf=Npix
 
@@ -351,15 +378,18 @@
         self.N_species=N_species
         self.N_per_bin=N_per_bin
         self.tag=tag
 
         ### size grid
         self.Agrid_edges=np.logspace(np.log10(self.amin), np.log10(self.amax), self.N_species+1)
         self.Agrid=np.sqrt(self.Agrid_edges[1:]*self.Agrid_edges[:-1])
-        self.Mgrid=self.Agrid**(self.slope+4.)
+        if slope!=-4:
+            self.Mgrid=self.Agrid_edges[1:]**(self.slope+4.)-self.Agrid_edges[:-1]**(self.slope+4.)
+        else:
+            self.Mgrid=np.log(self.Agrid_edges[1:]/self.Agrid_edges[:-1])
         self.Mgrid=Mdust*self.Mgrid/np.sum(self.Mgrid)
         
         if isinstance(lnk_file, str): # if one optical constant given
             self.lnk_file_p=lnk_file
             self.density=density
             
         elif isinstance(self.lnk_file, list):
@@ -436,26 +466,28 @@
             file_opacity.write('3 \n')
             file_opacity.write(str(self.wavelength_grid.Nlam)+'\n')
             for i in range(self.wavelength_grid.Nlam):
                 file_opacity.write('%f \t %f \t %f \t %f\n' %(self.wavelength_grid.lams[i],opctj[i,0],opctj[i,1],opctj[i,2]))
             file_opacity.close()
 
         os.system('rm ./Tempkappa/*')
-        path='dustopac.inp'
-        file_list_opacities=open(path,'w')
+        os.system('rm '+path+'param.inp')
+
+        pathfile='dustopac.inp'
+        file_list_opacities=open(pathfile,'w')
         file_list_opacities.write("2               Format number of this file \n")
         file_list_opacities.write(str(self.N_species)+"              Nr of dust species \n")
         file_list_opacities.write("============================================================================ \n")
         for i in range(self.N_species):
             file_list_opacities.write("1               Way in which this dust species is read \n")
             file_list_opacities.write("0               0=Thermal grain \n")
             file_list_opacities.write(self.tag+"_"+str(i+1)+ " Extension of name of dustkappa_***.inp file \n")
             file_list_opacities.write("---------------------------------------------------------------------------- \n")
         file_list_opacities.close()
-        
+
     def mix_opct_bruggeman(self, pathout='opct_mix.lnk'):
 
         # Mixing rule Bruggeman for max 3 species
 
         N_opct=len(self.lnk_file)
        
 
@@ -508,15 +540,15 @@
             for ia in range(self.N_species):
                 self.functions_rhoz.append(rhoz_Gaussian)
         else:
             assert len(functions_rhoz)==self.N_species, "functions_rhoz should be an array of function with a length equal to the number of species"
             self.functions_rhoz=functions_rhoz
         
         """
-        funtion_sigma: function that defines the surface density. The first two arguments are two nd numpy arrays for rho and z
+        funtion_sigma: function that defines the surface density. The first two arguments are two nd numpy arrays for rho and phi
         """
         
         assert grid is not None, "grid object needed to define dust density distribution"
         assert function_sigma is not None, "surface density profile needed to define dust density distribution"
 
         ## strange cases ntheta=1, mirror, etc
         self.grid=grid
@@ -610,15 +642,15 @@
         
 
 class star:
     """
     A class to define the star and companions
     """
     def __init__(self, lam_grid,
-                 dir_stellar_templates='/Users/Sebamarino/Astronomy/Stellar_templates/BT-Settl/bt-settl/',
+                 dir_stellar_templates=home_directory+'/Astronomy/Stellar_templates/BT-Settl/bt-settl/',
                  Tstar=None,
                  Rstar=None,
                  Mstar=None,
                  g=4.
                  # companion=False
                  # separation=0.0,
                  # inc=0.0,
```

### Comparing `disc2radmc-1.2/disc2radmc.egg-info/PKG-INFO` & `disc2radmc-1.3/disc2radmc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: disc2radmc
-Version: 1.2
+Version: 1.3
 Summary: Disc2radmc is a package to create parametric models of debris discs that can be fed into RADMC3D and simulate images of dust and gas emission.
 Home-page: https://github.com/SebaMarino/disc2radmc
+Download-URL: https://github.com/SebaMarino/disc2radmc/archive/refs/tags/v1.3.tar.gz
 Author: Sebastian Marino
 Author-email: sebastian.marino.estay@gmail.com
 License: MIT
-Download-URL: https://github.com/SebaMarino/disc2radmc/archive/refs/tags/v1.2.tar.gz
-Description: UNKNOWN
 Keywords: radiative transfer,debris disc,radmc3d,circumstellar disc
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE.txt
```

### Comparing `disc2radmc-1.2/setup.py` & `disc2radmc-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 setup(
     name = 'disc2radmc',         # How you named your package folder (MyLib)
     packages = ['disc2radmc'],   # Chose the same as "name"
-    version = '1.2',      # Start with a small number and increase it with every change you make
+    version = '1.3',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Disc2radmc is a package to create parametric models of debris discs that can be fed into RADMC3D and simulate images of dust and gas emission.',   # Give a short description about your library
     author = 'Sebastian Marino',                   # Type in your name
     author_email = 'sebastian.marino.estay@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/SebaMarino/disc2radmc',   # Provide either the link to your github or to your website
-    download_url = 'https://github.com/SebaMarino/disc2radmc/archive/refs/tags/v1.2.tar.gz',    #
+    download_url = 'https://github.com/SebaMarino/disc2radmc/archive/refs/tags/v1.3.tar.gz',    #
     keywords = ['radiative transfer', 'debris disc', 'radmc3d', 'circumstellar disc'],   # Keywords that define your package best
     install_requires=[
         'numpy',
         'matplotlib',
         'astropy',
         'cma',
         'scipy'],
```

