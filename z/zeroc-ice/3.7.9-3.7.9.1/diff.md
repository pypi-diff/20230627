# Comparing `tmp/zeroc-ice-3.7.9.tar.gz` & `tmp/zeroc-ice-3.7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroc-ice-3.7.9.tar", last modified: Wed Mar 22 23:07:32 2023, max compression
+gzip compressed data, was "zeroc-ice-3.7.9.1.tar", last modified: Mon Jun 26 19:30:13 2023, max compression
```

## Comparing `zeroc-ice-3.7.9.tar` & `zeroc-ice-3.7.9.1.tar`

### file list

```diff
@@ -1,778 +1,778 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.930665 zeroc-ice-3.7.9/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1901 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/BZIP2_LICENSE
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2301 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/ICE_LICENSE
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18093 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/LICENSE
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       64 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/MANIFEST.in
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1460 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/MCPP_LICENSE
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3732 2023-03-22 23:07:32.930665 zeroc-ice-3.7.9/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2409 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/README.rst
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.822664 zeroc-ice-3.7.9/lib/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.822664 zeroc-ice-3.7.9/lib/Glacier2/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2855 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/Metrics_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      933 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/PermissionsVerifierF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12788 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/PermissionsVerifier_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      588 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/RouterF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30521 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/Router_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6069 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/SSLInfo_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    46088 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/Session_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8184 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Glacier2/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.826665 zeroc-ice-3.7.9/lib/Ice/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2414 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/BuiltinSequences_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      496 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/CommunicatorF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21619 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Communicator_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      734 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ConnectionF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27713 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Connection_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6664 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Current_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1220 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/EndpointF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1665 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/EndpointTypes_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11475 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Endpoint_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      523 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/FacetMap_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4032 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Identity_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      508 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ImplicitContextF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4239 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ImplicitContext_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      913 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/InstrumentationF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25058 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Instrumentation_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    67729 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/LocalException_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      751 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/LocatorF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    32480 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Locator_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      472 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/LoggerF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2787 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Logger_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    37353 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Metrics_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      500 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ObjectAdapterF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21892 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ObjectAdapter_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2179 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ObjectFactory_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      589 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/PluginF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4554 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Plugin_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      544 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ProcessF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6118 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Process_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12052 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/PropertiesAdmin_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      695 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/PropertiesF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8047 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Properties_ice.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.826665 zeroc-ice-3.7.9/lib/Ice/Py3/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1697 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Py3/IceFuture.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       53 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Py3/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30369 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/RemoteLogger_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      538 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/RouterF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14478 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Router_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      504 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ServantLocatorF_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4727 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ServantLocator_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      643 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/SliceChecksumDict_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5287 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/ValueFactory_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6401 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/Version_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    63018 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/Ice/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.826665 zeroc-ice-3.7.9/lib/IceBox/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26667 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceBox/IceBox_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      132 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceBox/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.830664 zeroc-ice-3.7.9/lib/IceGrid/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   318048 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/Admin_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    74736 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/Descriptor_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23284 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/Exception_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6256 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/FileParser_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11953 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/PluginFacade_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    44194 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/Registry_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18488 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/Session_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7397 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/UserAccountMapper_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      346 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceGrid/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.830664 zeroc-ice-3.7.9/lib/IceMX/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      185 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceMX/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.830664 zeroc-ice-3.7.9/lib/IcePatch2/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9740 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IcePatch2/FileInfo_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27321 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IcePatch2/FileServer_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      172 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IcePatch2/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.830664 zeroc-ice-3.7.9/lib/IceStorm/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52797 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceStorm/IceStorm_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3437 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceStorm/Metrics_ice.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      138 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/IceStorm/__init__.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.818664 zeroc-ice-3.7.9/lib/slice/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.830664 zeroc-ice-3.7.9/lib/slice/Glacier2/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1328 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/Metrics.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2483 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/PermissionsVerifier.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      488 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/PermissionsVerifierF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5674 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/Router.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      441 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/RouterF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      966 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/SSLInfo.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5877 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Glacier2/Session.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.834664 zeroc-ice-3.7.9/lib/slice/Ice/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      985 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/BuiltinSequences.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21425 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Communicator.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      436 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/CommunicatorF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12592 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Connection.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      492 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ConnectionF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4077 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Current.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4687 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Endpoint.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      672 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/EndpointF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      832 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/EndpointTypes.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      523 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/FacetMap.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1220 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Identity.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3270 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ImplicitContext.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      438 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ImplicitContextF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12362 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Instrumentation.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      534 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/InstrumentationF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21122 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/LocalException.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5933 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Locator.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      452 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/LocatorF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1871 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Logger.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      430 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/LoggerF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9039 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Metrics.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22658 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ObjectAdapter.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      437 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ObjectAdapterF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1613 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ObjectFactory.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2850 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Plugin.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      498 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/PluginF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1231 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Process.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      425 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ProcessF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6926 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Properties.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2050 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/PropertiesAdmin.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      461 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/PropertiesF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5277 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/RemoteLogger.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2523 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Router.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      424 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/RouterF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4465 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ServantLocator.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      438 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ServantLocatorF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      616 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/SliceChecksumDict.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3969 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/ValueFactory.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      653 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/Ice/Version.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.834664 zeroc-ice-3.7.9/lib/slice/IceBT/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1079 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceBT/ConnectionInfo.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      821 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceBT/EndpointInfo.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      648 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceBT/Types.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceBox/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4560 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceBox/IceBox.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceDiscovery/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2326 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceDiscovery/IceDiscovery.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceGrid/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    51347 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/Admin.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18163 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/Descriptor.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5690 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/Exception.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1315 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/FileParser.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9369 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/PluginFacade.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6584 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/Registry.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3429 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/Session.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1478 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceGrid/UserAccountMapper.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceIAP/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1049 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceIAP/ConnectionInfo.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1054 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceIAP/EndpointInfo.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceLocatorDiscovery/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1872 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceLocatorDiscovery/IceLocatorDiscovery.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IcePatch2/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1347 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IcePatch2/FileInfo.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5364 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IcePatch2/FileServer.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceSSL/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1064 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceSSL/ConnectionInfo.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      479 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceSSL/ConnectionInfoF.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      663 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceSSL/EndpointInfo.ice
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/slice/IceStorm/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8330 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceStorm/IceStorm.ice
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1247 2023-02-13 11:50:27.000000 zeroc-ice-3.7.9/lib/slice/IceStorm/Metrics.ice
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      375 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/lib/slice2py.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.838664 zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3732 2023-03-22 23:07:32.000000 zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25686 2023-03-22 23:07:32.000000 zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-03-22 23:07:32.000000 zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       43 2023-03-22 23:07:32.000000 zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       74 2023-03-22 23:07:32.000000 zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-03-22 23:07:32.930665 zeroc-ice-3.7.9/setup.cfg
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8923 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/setup.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.846665 zeroc-ice-3.7.9/src/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7524 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/BatchRequestInterceptor.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      632 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/BatchRequestInterceptor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    51101 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Communicator.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      871 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Communicator.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      706 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Config.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    34918 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Connection.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      469 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Connection.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26856 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ConnectionInfo.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      395 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ConnectionInfo.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9788 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Current.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      292 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Current.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4752 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Dispatcher.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      632 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Dispatcher.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7278 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Endpoint.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      394 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Endpoint.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    28253 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/EndpointInfo.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      377 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/EndpointInfo.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9585 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ImplicitContext.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      353 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ImplicitContext.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8631 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Init.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12218 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Logger.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1073 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Logger.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48133 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ObjectAdapter.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      505 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ObjectAdapter.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   132598 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Operation.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3574 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Operation.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18488 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Properties.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      431 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Properties.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7330 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/PropertiesAdmin.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      377 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/PropertiesAdmin.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    75814 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Proxy.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1231 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Proxy.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6731 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Slice.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      249 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Slice.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2584 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Thread.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2162 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Thread.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   137373 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Types.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20790 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Types.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31417 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Util.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6664 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/Util.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11873 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ValueFactoryManager.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1983 2023-03-22 23:07:26.000000 zeroc-ice-3.7.9/src/ValueFactoryManager.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.822664 zeroc-ice-3.7.9/src/ice/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.846665 zeroc-ice-3.7.9/src/ice/bzip2/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30694 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/blocksort.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    45995 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/bzlib.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6245 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/bzlib.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13244 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/bzlib_private.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20561 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/compress.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4818 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/crctable.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20919 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/decompress.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6991 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/huffman.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3860 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/bzip2/randtable.c
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.818664 zeroc-ice-3.7.9/src/ice/cpp/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.818664 zeroc-ice-3.7.9/src/ice/cpp/include/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.854664 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12240 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Application.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5253 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/AsyncResult.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      361 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/AsyncResultF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1729 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/BatchRequestInterceptor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      366 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/BatchRequestQueueF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3296 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Buffer.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5395 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/CommunicatorAsync.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5798 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Comparable.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1318 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Config.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10608 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ConnectionAsync.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      625 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ConnectionIF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      363 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ConsoleUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      945 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DefaultValueFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1174 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DispatchInterceptor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1650 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Dispatcher.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2152 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DynamicLibrary.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      472 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DynamicLibraryF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3779 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Exception.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1690 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ExceptionHelpers.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2005 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/FactoryTable.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1592 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/FactoryTableInit.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      622 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Format.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4169 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Functional.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1264 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/GCObject.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3363 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Handle.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1530 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Ice.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9761 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/IconvStringConverter.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5300 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Incoming.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4254 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/IncomingAsync.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      662 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/IncomingAsyncF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    41173 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Initialize.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    45578 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/InputStream.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      308 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/InstanceF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1033 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/InterfaceByValue.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      646 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/LocalObject.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      330 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/LocalObjectF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4133 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/LoggerUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20895 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/MetricsAdminI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2915 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/MetricsFunctional.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17878 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/MetricsObserverI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2542 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/NativePropertiesAdmin.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18275 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Object.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      517 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ObjectF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3453 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ObserverHelper.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31190 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Optional.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22298 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/OutgoingAsync.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1172 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/OutgoingAsyncF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30822 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/OutputStream.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7049 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Protocol.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   196950 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Proxy.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      655 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ProxyF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      327 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ProxyFactoryF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6760 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ProxyHandle.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      599 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ReferenceF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4908 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/RegisterPlugins.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      673 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/RequestHandlerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      454 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ResponseHandlerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      607 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SHA1.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      334 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ServantManagerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12337 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Service.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      472 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SliceChecksums.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3833 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SlicedData.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      914 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SlicedDataF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    33174 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/StreamHelpers.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2258 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/StringConverter.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      336 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ThreadPoolF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      229 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UUID.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1178 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UniquePtr.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1402 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UniqueRef.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1454 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UserExceptionFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3602 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Value.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      274 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ValueF.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.854664 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      419 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/Config.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      546 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/IceSSL.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4138 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/OpenSSL.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21615 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/Plugin.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1845 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/SChannel.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1904 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/SecureTransport.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1614 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/UWP.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.858665 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3852 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Atomic.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6909 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Cond.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12363 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Config.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1751 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ConsoleUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      656 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/CountDownLatch.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2797 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/CtrlCHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1177 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/DisableWarnings.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8709 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Exception.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2874 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/FileUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9321 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Functional.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5191 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Handle.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1061 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/IceUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1028 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/InputUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      644 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Iterator.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2304 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Lock.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4489 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Monitor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6532 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Mutex.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      316 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/MutexProtocol.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1296 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/MutexPtrLock.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1315 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/MutexPtrTryLock.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8491 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Optional.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3960 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Options.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7392 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/OutputUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      308 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/PopDisableWarnings.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1381 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/PushDisableWarnings.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      956 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Random.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2142 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/RecMutex.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1236 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ResourceConfig.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1180 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ScannerConfig.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1442 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ScopedArray.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2019 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Shared.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      804 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/StopWatch.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5565 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/StringConverter.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2763 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/StringUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3798 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Thread.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2004 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ThreadException.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3798 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Time.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3252 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Timer.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      285 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/UUID.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      723 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/UndefSysMacros.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.818664 zeroc-ice-3.7.9/src/ice/cpp/include/generated/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.866665 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2832 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/BuiltinSequences.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    45168 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Communicator.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1665 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/CommunicatorF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    53769 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Connection.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2161 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ConnectionF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9457 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Current.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27318 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Endpoint.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3106 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/EndpointF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2227 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/EndpointTypes.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1487 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/FacetMap.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5444 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Identity.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8057 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ImplicitContext.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1695 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ImplicitContextF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    36514 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Instrumentation.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2082 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/InstrumentationF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   257285 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/LocalException.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   153507 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Locator.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2937 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/LocatorF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5056 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Logger.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1605 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/LoggerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   180120 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Metrics.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    43782 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ObjectAdapter.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1675 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ObjectAdapterF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5104 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ObjectFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7939 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Plugin.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1849 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/PluginF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    36008 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Process.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2137 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ProcessF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14925 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Properties.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    56548 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/PropertiesAdmin.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2513 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/PropertiesF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   112752 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/RemoteLogger.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    71003 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Router.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2116 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/RouterF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10187 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ServantLocator.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1685 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ServantLocatorF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1752 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/SliceChecksumDict.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9927 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ValueFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7172 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Version.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.866665 zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5655 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/ConnectionInfo.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1725 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/ConnectionInfoF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4126 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/EndpointInfo.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.822664 zeroc-ice-3.7.9/src/ice/cpp/src/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.906664 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9619 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ACM.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3244 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ACM.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      597 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ACMF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      287 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Acceptor.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      808 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Acceptor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      407 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/AcceptorF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1183 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ArgVector.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      550 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ArgVector.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2247 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/AsyncResult.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4922 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Base64.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      487 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Base64.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5980 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/BatchRequestQueue.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1382 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/BatchRequestQueue.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2978 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Buffer.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1055 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/BuiltinSequences.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11078 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CollocatedRequestHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2445 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CollocatedRequestHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1407 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Communicator.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1041 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CommunicatorF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14609 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CommunicatorI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5532 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CommunicatorI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9025 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Cond.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9233 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectRequestHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1921 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectRequestHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      495 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectRequestHandlerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2613 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Connection.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1037 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    57598 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8131 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      683 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionFactoryF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   107785 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13130 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1854 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionRequestHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      988 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionRequestHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      291 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Connector.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      565 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Connector.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      302 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectorF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3798 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CountDownLatch.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1091 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Current.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6449 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DefaultsAndOverrides.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1238 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DefaultsAndOverrides.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      364 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DefaultsAndOverridesF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      990 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DispatchInterceptor.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6780 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DynamicLibrary.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2438 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Endpoint.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1033 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4512 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3125 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      340 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactoryF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5751 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactoryManager.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      898 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactoryManager.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      376 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactoryManagerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2383 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5375 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1155 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointIF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1009 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointTypes.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      679 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EventHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1732 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EventHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      416 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EventHandlerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18698 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Exception.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1039 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/FacetMap.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3787 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/FactoryTable.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1863 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/FactoryTableInit.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9597 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/GCObject.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1113 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/HashUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16715 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/HttpParser.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2382 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/HttpParser.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18772 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IPEndpointI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4501 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IPEndpointI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      557 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IPEndpointIF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      984 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IconvStringConverter.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1077 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Identity.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1303 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContext.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1047 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContextF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13762 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContextI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1027 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContextI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22013 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Incoming.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4578 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IncomingAsync.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      508 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IncomingRequest.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16484 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Initialize.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    67914 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InputStream.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    54093 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Instance.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7800 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Instance.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3690 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Instrumentation.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1063 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InstrumentationF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26606 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InstrumentationI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8720 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InstrumentationI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    65631 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocalException.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      400 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocalObject.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    54919 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Locator.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1090 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26576 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorInfo.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5502 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorInfo.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      530 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorInfoF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1181 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Logger.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26096 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerAdminI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      792 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerAdminI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1029 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6722 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1161 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1719 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    62318 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Metrics.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18521 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/MetricsAdminI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      146 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/MetricsObserverI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    82493 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Network.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10723 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Network.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      266 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/NetworkF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7997 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/NetworkProxy.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1943 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/NetworkProxy.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      322 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/NetworkProxyF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1408 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OSLogLoggerI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      709 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OSLogLoggerI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9484 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Object.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1414 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapter.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1043 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7137 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1363 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      488 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterFactoryF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    43876 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5710 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1289 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1515 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObserverHelper.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8952 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OpaqueEndpointI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2225 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OpaqueEndpointI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30295 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OutgoingAsync.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    34888 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OutputStream.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1429 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Plugin.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1029 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PluginF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13430 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PluginManagerI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1557 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PluginManagerI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11144 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Process.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1090 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProcessF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1361 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Properties.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16688 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesAdmin.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6905 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesAdminI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1936 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesAdminI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1096 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21202 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1893 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   101096 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertyNames.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1842 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertyNames.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3275 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Protocol.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3331 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolInstance.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2202 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolInstance.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      359 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolInstanceF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1263 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolPluginFacade.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1397 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolPluginFacade.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      372 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolPluginFacadeF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    39721 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Proxy.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8556 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProxyFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1202 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProxyFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    55183 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Reference.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11621 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Reference.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    28704 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReferenceFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2142 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReferenceFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      309 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReferenceFactoryF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1251 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RegisterPluginsInit.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      233 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RegisterPluginsInit.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    32252 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RemoteLogger.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      561 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReplyStatus.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      854 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1541 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2129 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandlerFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      800 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandlerFactory.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      250 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ResponseHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      835 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ResponseHandler.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3902 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RetryQueue.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1418 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RetryQueue.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      273 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RetryQueueF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25109 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Router.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1088 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10378 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterInfo.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4067 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterInfo.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      413 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterInfoF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4118 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SHA1.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    42753 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Selector.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6994 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Selector.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1296 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantLocator.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1045 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantLocatorF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12613 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantManager.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1953 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantManager.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      653 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SharedContext.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1057 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SliceChecksumDict.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1260 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SliceChecksums.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2711 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SlicedData.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17009 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StreamSocket.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2008 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StreamSocket.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4782 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StringConverterPlugin.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      547 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StringUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3420 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SysLoggerI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      736 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SysLoggerI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1284 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SystemdJournalI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      685 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SystemdJournalI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9319 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpAcceptor.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1504 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpAcceptor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2532 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpConnector.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      962 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpConnector.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8713 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpEndpointI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2497 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpEndpointI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2761 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpTransceiver.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1409 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpTransceiver.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16449 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Thread.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    38733 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ThreadPool.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9739 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ThreadPool.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7050 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Timer.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1250 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceLevels.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      701 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceLevels.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      308 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceLevelsF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10018 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      737 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      310 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Transceiver.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1245 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Transceiver.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      679 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TransceiverF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2663 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpConnector.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      954 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpConnector.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12333 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpEndpointI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2633 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpEndpointI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    33089 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpTransceiver.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3223 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpTransceiver.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      978 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Value.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1461 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ValueFactory.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1436 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ValueFactoryManagerI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      823 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ValueFactoryManagerI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1075 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Version.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      800 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/VirtualShared.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1778 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSAcceptor.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1142 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSAcceptor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1795 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSConnector.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      844 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSConnector.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11789 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSEndpoint.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2872 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSEndpoint.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    51492 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSTransceiver.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3429 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSTransceiver.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.906664 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25879 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/IceDiscovery.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    82885 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/IceDiscovery.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7509 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LocatorI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3679 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LocatorI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16684 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LookupI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6249 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LookupI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5797 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/PluginI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      627 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/PluginI.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.906664 zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19542 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    46878 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1177 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/Plugin.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31596 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/PluginI.cpp
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.914665 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2047 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/AcceptorI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1283 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/AcceptorI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6724 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/CertificateI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1441 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/CertificateI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1317 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectionInfo.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1054 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectionInfoF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1893 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectorI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      895 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectorI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8839 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/EndpointI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2985 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/EndpointI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1303 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/EndpointInfo.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      555 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Instance.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      555 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Instance.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      666 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/InstanceF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18230 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLCertificateI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    39192 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLEngine.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1158 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLEngine.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      438 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLEngineF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2756 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLPluginI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    32160 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2444 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10220 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      886 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6919 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/PluginI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1699 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/PluginI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11933 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/RFC2253.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1427 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/RFC2253.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21416 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelCertificateI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    42771 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelEngine.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2394 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelEngine.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      408 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelEngineF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1579 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelPluginI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    36565 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelTransceiverI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3348 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelTransceiverI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8767 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SSLEngine.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2440 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SSLEngine.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      339 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SSLEngineF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    32791 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportCertificateI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52308 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportEngine.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1208 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportEngine.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      430 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportEngineF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1669 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportPluginI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22540 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2386 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    33331 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1029 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6773 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/TrustManager.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1161 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/TrustManager.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      336 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/TrustManagerF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     7857 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPCertificateI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10919 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPEngine.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      767 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPEngine.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      364 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPEngineF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1906 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPPluginI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    12350 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPTransceiverI.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1991 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPTransceiverI.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4675 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Util.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2178 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Util.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.918665 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3193 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ConsoleUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18260 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ConvertUTF.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5895 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ConvertUTF.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5168 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/CtrlCHandler.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11103 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/FileUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      664 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/InputUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      369 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/MutexProtocol.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    32067 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Options.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10693 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/OutputUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3606 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Random.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4344 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/RecMutex.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1050 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Shared.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19101 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/StringConverter.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30112 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/StringUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2997 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ThreadException.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6167 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Time.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3925 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/UUID.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5465 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Unicode.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1100 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Unicode.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19244 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/UtilException.cpp
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.926665 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    53245 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/CPlusPlusUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3318 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/CPlusPlusUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10722 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Checksum.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      316 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Checksum.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2941 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/FileTracker.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1301 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/FileTracker.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   146690 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Grammar.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3585 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Grammar.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5415 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/GrammarUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   167600 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/JavaUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13377 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/JavaUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      856 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      450 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13192 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5I.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3405 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5I.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4068 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PHPUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      718 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PHPUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   174010 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Parser.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    36241 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Parser.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19866 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Preprocessor.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1700 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Preprocessor.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26141 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Python.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    99543 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PythonUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1892 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PythonUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10266 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Ruby.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    43938 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/RubyUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1168 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/RubyUtil.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    73377 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Scanner.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10597 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/SliceUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13431 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/StringLiteralUtil.cpp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2113 2023-03-22 23:07:17.000000 zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Util.h
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-22 23:07:32.930665 zeroc-ice-3.7.9/src/ice/mcpp/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1550 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/CMakeLists.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1460 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/LICENSE
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1478 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/Makefile
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1431 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/README.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2076 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/config.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8998 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/configed.H
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52208 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/directive.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    47479 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/eval.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    93246 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/expand.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23969 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/internal.H
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31200 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/main.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9358 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/mbchar.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1893 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/mcpp.gyp
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1051 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/mcpp_lib.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      364 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/mcpp_out.h
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    68680 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/support.c
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    14700 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/system.H
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    92968 2023-03-22 23:07:18.000000 zeroc-ice-3.7.9/src/ice/mcpp/system.c
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.594753 zeroc-ice-3.7.9.1/
+-rw-r--r--   0 joe        (501) staff       (20)     1901 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/BZIP2_LICENSE
+-rw-r--r--   0 joe        (501) staff       (20)     2301 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/ICE_LICENSE
+-rw-r--r--   0 joe        (501) staff       (20)    18093 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/LICENSE
+-rw-r--r--   0 joe        (501) staff       (20)       64 2023-06-26 19:30:10.000000 zeroc-ice-3.7.9.1/MANIFEST.in
+-rw-r--r--   0 joe        (501) staff       (20)     1460 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/MCPP_LICENSE
+-rw-r--r--   0 joe        (501) staff       (20)     3734 2023-06-26 19:30:13.594609 zeroc-ice-3.7.9.1/PKG-INFO
+-rw-r--r--   0 joe        (501) staff       (20)     2409 2023-06-26 19:30:10.000000 zeroc-ice-3.7.9.1/README.rst
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.498521 zeroc-ice-3.7.9.1/lib/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.499575 zeroc-ice-3.7.9.1/lib/Glacier2/
+-rw-r--r--   0 joe        (501) staff       (20)     2855 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/Metrics_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      933 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/PermissionsVerifierF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    12788 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/PermissionsVerifier_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      588 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/RouterF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    30521 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/Router_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     6069 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/SSLInfo_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    46088 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/Session_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     8184 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Glacier2/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.504764 zeroc-ice-3.7.9.1/lib/Ice/
+-rw-r--r--   0 joe        (501) staff       (20)     2414 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/BuiltinSequences_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      496 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/CommunicatorF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    21619 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Communicator_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      734 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ConnectionF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    27713 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Connection_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     6664 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Current_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     1220 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/EndpointF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     1665 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/EndpointTypes_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    11475 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Endpoint_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      523 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/FacetMap_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     4032 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Identity_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      508 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ImplicitContextF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     4239 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ImplicitContext_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      913 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/InstrumentationF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    25058 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Instrumentation_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    67729 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/LocalException_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      751 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/LocatorF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    32480 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Locator_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      472 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/LoggerF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     2787 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Logger_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    37353 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Metrics_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      500 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ObjectAdapterF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    21892 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ObjectAdapter_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     2179 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ObjectFactory_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      589 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/PluginF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     4554 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Plugin_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      544 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ProcessF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     6118 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Process_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    12052 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/PropertiesAdmin_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      695 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/PropertiesF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     8047 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Properties_ice.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.505046 zeroc-ice-3.7.9.1/lib/Ice/Py3/
+-rw-r--r--   0 joe        (501) staff       (20)     1697 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Py3/IceFuture.py
+-rw-r--r--   0 joe        (501) staff       (20)       53 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Py3/__init__.py
+-rw-r--r--   0 joe        (501) staff       (20)    30369 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/RemoteLogger_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      538 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/RouterF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    14478 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Router_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      504 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ServantLocatorF_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     4727 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ServantLocator_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      643 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/SliceChecksumDict_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     5287 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/ValueFactory_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     6401 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/Version_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    63018 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/Ice/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.505321 zeroc-ice-3.7.9.1/lib/IceBox/
+-rw-r--r--   0 joe        (501) staff       (20)    26667 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceBox/IceBox_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      132 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceBox/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.506731 zeroc-ice-3.7.9.1/lib/IceGrid/
+-rw-r--r--   0 joe        (501) staff       (20)   318048 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/Admin_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    74736 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/Descriptor_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    23284 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/Exception_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     6256 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/FileParser_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    11953 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/PluginFacade_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    44194 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/Registry_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    18488 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/Session_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     7397 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/UserAccountMapper_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      346 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceGrid/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.506862 zeroc-ice-3.7.9.1/lib/IceMX/
+-rw-r--r--   0 joe        (501) staff       (20)      185 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceMX/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.507254 zeroc-ice-3.7.9.1/lib/IcePatch2/
+-rw-r--r--   0 joe        (501) staff       (20)     9740 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IcePatch2/FileInfo_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)    27321 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IcePatch2/FileServer_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      172 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IcePatch2/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.507622 zeroc-ice-3.7.9.1/lib/IceStorm/
+-rw-r--r--   0 joe        (501) staff       (20)    52797 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceStorm/IceStorm_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)     3437 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceStorm/Metrics_ice.py
+-rw-r--r--   0 joe        (501) staff       (20)      138 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/IceStorm/__init__.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.496310 zeroc-ice-3.7.9.1/lib/slice/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.508499 zeroc-ice-3.7.9.1/lib/slice/Glacier2/
+-rw-r--r--   0 joe        (501) staff       (20)     1328 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/Metrics.ice
+-rw-r--r--   0 joe        (501) staff       (20)     2483 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/PermissionsVerifier.ice
+-rw-r--r--   0 joe        (501) staff       (20)      488 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/PermissionsVerifierF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     5674 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/Router.ice
+-rw-r--r--   0 joe        (501) staff       (20)      441 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/RouterF.ice
+-rw-r--r--   0 joe        (501) staff       (20)      966 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/SSLInfo.ice
+-rw-r--r--   0 joe        (501) staff       (20)     5877 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Glacier2/Session.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.513840 zeroc-ice-3.7.9.1/lib/slice/Ice/
+-rw-r--r--   0 joe        (501) staff       (20)      985 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/BuiltinSequences.ice
+-rw-r--r--   0 joe        (501) staff       (20)    21425 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Communicator.ice
+-rw-r--r--   0 joe        (501) staff       (20)      436 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/CommunicatorF.ice
+-rw-r--r--   0 joe        (501) staff       (20)    12592 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Connection.ice
+-rw-r--r--   0 joe        (501) staff       (20)      492 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ConnectionF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     4077 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Current.ice
+-rw-r--r--   0 joe        (501) staff       (20)     4687 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Endpoint.ice
+-rw-r--r--   0 joe        (501) staff       (20)      672 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/EndpointF.ice
+-rw-r--r--   0 joe        (501) staff       (20)      832 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/EndpointTypes.ice
+-rw-r--r--   0 joe        (501) staff       (20)      523 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/FacetMap.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1220 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Identity.ice
+-rw-r--r--   0 joe        (501) staff       (20)     3270 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ImplicitContext.ice
+-rw-r--r--   0 joe        (501) staff       (20)      438 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ImplicitContextF.ice
+-rw-r--r--   0 joe        (501) staff       (20)    12362 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Instrumentation.ice
+-rw-r--r--   0 joe        (501) staff       (20)      534 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/InstrumentationF.ice
+-rw-r--r--   0 joe        (501) staff       (20)    21122 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/LocalException.ice
+-rw-r--r--   0 joe        (501) staff       (20)     5933 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Locator.ice
+-rw-r--r--   0 joe        (501) staff       (20)      452 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/LocatorF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1871 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Logger.ice
+-rw-r--r--   0 joe        (501) staff       (20)      430 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/LoggerF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     9039 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Metrics.ice
+-rw-r--r--   0 joe        (501) staff       (20)    22658 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ObjectAdapter.ice
+-rw-r--r--   0 joe        (501) staff       (20)      437 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ObjectAdapterF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1613 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ObjectFactory.ice
+-rw-r--r--   0 joe        (501) staff       (20)     2850 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Plugin.ice
+-rw-r--r--   0 joe        (501) staff       (20)      498 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/PluginF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1231 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Process.ice
+-rw-r--r--   0 joe        (501) staff       (20)      425 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ProcessF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     6926 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Properties.ice
+-rw-r--r--   0 joe        (501) staff       (20)     2050 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/PropertiesAdmin.ice
+-rw-r--r--   0 joe        (501) staff       (20)      461 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/PropertiesF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     5277 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/RemoteLogger.ice
+-rw-r--r--   0 joe        (501) staff       (20)     2523 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Router.ice
+-rw-r--r--   0 joe        (501) staff       (20)      424 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/RouterF.ice
+-rw-r--r--   0 joe        (501) staff       (20)     4465 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ServantLocator.ice
+-rw-r--r--   0 joe        (501) staff       (20)      438 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ServantLocatorF.ice
+-rw-r--r--   0 joe        (501) staff       (20)      616 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/SliceChecksumDict.ice
+-rw-r--r--   0 joe        (501) staff       (20)     3969 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/ValueFactory.ice
+-rw-r--r--   0 joe        (501) staff       (20)      653 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/Ice/Version.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.514235 zeroc-ice-3.7.9.1/lib/slice/IceBT/
+-rw-r--r--   0 joe        (501) staff       (20)     1079 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceBT/ConnectionInfo.ice
+-rw-r--r--   0 joe        (501) staff       (20)      821 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceBT/EndpointInfo.ice
+-rw-r--r--   0 joe        (501) staff       (20)      648 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceBT/Types.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.514359 zeroc-ice-3.7.9.1/lib/slice/IceBox/
+-rw-r--r--   0 joe        (501) staff       (20)     4560 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceBox/IceBox.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.514494 zeroc-ice-3.7.9.1/lib/slice/IceDiscovery/
+-rw-r--r--   0 joe        (501) staff       (20)     2326 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceDiscovery/IceDiscovery.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.515664 zeroc-ice-3.7.9.1/lib/slice/IceGrid/
+-rw-r--r--   0 joe        (501) staff       (20)    51347 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/Admin.ice
+-rw-r--r--   0 joe        (501) staff       (20)    18163 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/Descriptor.ice
+-rw-r--r--   0 joe        (501) staff       (20)     5690 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/Exception.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1315 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/FileParser.ice
+-rw-r--r--   0 joe        (501) staff       (20)     9369 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/PluginFacade.ice
+-rw-r--r--   0 joe        (501) staff       (20)     6584 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/Registry.ice
+-rw-r--r--   0 joe        (501) staff       (20)     3429 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/Session.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1478 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceGrid/UserAccountMapper.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.515911 zeroc-ice-3.7.9.1/lib/slice/IceIAP/
+-rw-r--r--   0 joe        (501) staff       (20)     1049 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceIAP/ConnectionInfo.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1054 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceIAP/EndpointInfo.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.516064 zeroc-ice-3.7.9.1/lib/slice/IceLocatorDiscovery/
+-rw-r--r--   0 joe        (501) staff       (20)     1872 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceLocatorDiscovery/IceLocatorDiscovery.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.516367 zeroc-ice-3.7.9.1/lib/slice/IcePatch2/
+-rw-r--r--   0 joe        (501) staff       (20)     1347 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IcePatch2/FileInfo.ice
+-rw-r--r--   0 joe        (501) staff       (20)     5364 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IcePatch2/FileServer.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.516811 zeroc-ice-3.7.9.1/lib/slice/IceSSL/
+-rw-r--r--   0 joe        (501) staff       (20)     1064 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceSSL/ConnectionInfo.ice
+-rw-r--r--   0 joe        (501) staff       (20)      479 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceSSL/ConnectionInfoF.ice
+-rw-r--r--   0 joe        (501) staff       (20)      663 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceSSL/EndpointInfo.ice
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.517108 zeroc-ice-3.7.9.1/lib/slice/IceStorm/
+-rw-r--r--   0 joe        (501) staff       (20)     8330 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceStorm/IceStorm.ice
+-rw-r--r--   0 joe        (501) staff       (20)     1247 2023-06-26 17:22:29.000000 zeroc-ice-3.7.9.1/lib/slice/IceStorm/Metrics.ice
+-rwxr-xr-x   0 joe        (501) staff       (20)      375 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/lib/slice2py.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.517873 zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/
+-rw-r--r--   0 joe        (501) staff       (20)     3734 2023-06-26 19:30:13.000000 zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/PKG-INFO
+-rw-r--r--   0 joe        (501) staff       (20)    25686 2023-06-26 19:30:13.000000 zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/SOURCES.txt
+-rw-r--r--   0 joe        (501) staff       (20)        1 2023-06-26 19:30:13.000000 zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/dependency_links.txt
+-rw-r--r--   0 joe        (501) staff       (20)       43 2023-06-26 19:30:13.000000 zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/entry_points.txt
+-rw-r--r--   0 joe        (501) staff       (20)       74 2023-06-26 19:30:13.000000 zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/top_level.txt
+-rw-r--r--   0 joe        (501) staff       (20)       38 2023-06-26 19:30:13.594794 zeroc-ice-3.7.9.1/setup.cfg
+-rw-r--r--   0 joe        (501) staff       (20)     8925 2023-06-26 19:30:10.000000 zeroc-ice-3.7.9.1/setup.py
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.523407 zeroc-ice-3.7.9.1/src/
+-rw-r--r--   0 joe        (501) staff       (20)     7524 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/BatchRequestInterceptor.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      632 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/BatchRequestInterceptor.h
+-rw-r--r--   0 joe        (501) staff       (20)    51101 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Communicator.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      871 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Communicator.h
+-rw-r--r--   0 joe        (501) staff       (20)      706 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Config.h
+-rw-r--r--   0 joe        (501) staff       (20)    34918 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Connection.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      469 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Connection.h
+-rw-r--r--   0 joe        (501) staff       (20)    26856 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ConnectionInfo.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      395 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ConnectionInfo.h
+-rw-r--r--   0 joe        (501) staff       (20)     9788 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Current.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      292 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Current.h
+-rw-r--r--   0 joe        (501) staff       (20)     4752 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Dispatcher.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      632 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Dispatcher.h
+-rw-r--r--   0 joe        (501) staff       (20)     7278 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Endpoint.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      394 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Endpoint.h
+-rw-r--r--   0 joe        (501) staff       (20)    28253 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/EndpointInfo.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      377 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/EndpointInfo.h
+-rw-r--r--   0 joe        (501) staff       (20)     9585 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ImplicitContext.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      353 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ImplicitContext.h
+-rw-r--r--   0 joe        (501) staff       (20)     8631 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Init.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    12218 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Logger.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1073 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Logger.h
+-rw-r--r--   0 joe        (501) staff       (20)    48133 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ObjectAdapter.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      505 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ObjectAdapter.h
+-rw-r--r--   0 joe        (501) staff       (20)   132598 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Operation.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3574 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Operation.h
+-rw-r--r--   0 joe        (501) staff       (20)    18488 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Properties.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      431 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Properties.h
+-rw-r--r--   0 joe        (501) staff       (20)     7330 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/PropertiesAdmin.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      377 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/PropertiesAdmin.h
+-rw-r--r--   0 joe        (501) staff       (20)    75814 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Proxy.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1231 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Proxy.h
+-rw-r--r--   0 joe        (501) staff       (20)     6731 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Slice.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      249 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Slice.h
+-rw-r--r--   0 joe        (501) staff       (20)     2584 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Thread.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2162 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Thread.h
+-rw-r--r--   0 joe        (501) staff       (20)   137373 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Types.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    20790 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Types.h
+-rw-r--r--   0 joe        (501) staff       (20)    31417 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Util.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6664 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/Util.h
+-rw-r--r--   0 joe        (501) staff       (20)    11873 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ValueFactoryManager.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1983 2023-06-26 19:30:09.000000 zeroc-ice-3.7.9.1/src/ValueFactoryManager.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.497463 zeroc-ice-3.7.9.1/src/ice/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.524576 zeroc-ice-3.7.9.1/src/ice/bzip2/
+-rw-r--r--   0 joe        (501) staff       (20)    30694 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/blocksort.c
+-rw-r--r--   0 joe        (501) staff       (20)    45995 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/bzlib.c
+-rw-r--r--   0 joe        (501) staff       (20)     6245 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/bzlib.h
+-rw-r--r--   0 joe        (501) staff       (20)    13244 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/bzlib_private.h
+-rw-r--r--   0 joe        (501) staff       (20)    20561 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/compress.c
+-rw-r--r--   0 joe        (501) staff       (20)     4818 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/crctable.c
+-rw-r--r--   0 joe        (501) staff       (20)    20919 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/decompress.c
+-rw-r--r--   0 joe        (501) staff       (20)     6991 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/huffman.c
+-rw-r--r--   0 joe        (501) staff       (20)     3860 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/bzip2/randtable.c
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.497044 zeroc-ice-3.7.9.1/src/ice/cpp/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.496861 zeroc-ice-3.7.9.1/src/ice/cpp/include/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.534374 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/
+-rw-r--r--   0 joe        (501) staff       (20)    12240 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Application.h
+-rw-r--r--   0 joe        (501) staff       (20)     5253 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/AsyncResult.h
+-rw-r--r--   0 joe        (501) staff       (20)      361 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/AsyncResultF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1729 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/BatchRequestInterceptor.h
+-rw-r--r--   0 joe        (501) staff       (20)      366 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/BatchRequestQueueF.h
+-rw-r--r--   0 joe        (501) staff       (20)     3296 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Buffer.h
+-rw-r--r--   0 joe        (501) staff       (20)     5395 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/CommunicatorAsync.h
+-rw-r--r--   0 joe        (501) staff       (20)     5798 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Comparable.h
+-rw-r--r--   0 joe        (501) staff       (20)     1318 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Config.h
+-rw-r--r--   0 joe        (501) staff       (20)    10608 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ConnectionAsync.h
+-rw-r--r--   0 joe        (501) staff       (20)      625 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ConnectionIF.h
+-rw-r--r--   0 joe        (501) staff       (20)      363 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ConsoleUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)      945 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DefaultValueFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)     1174 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DispatchInterceptor.h
+-rw-r--r--   0 joe        (501) staff       (20)     1650 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Dispatcher.h
+-rw-r--r--   0 joe        (501) staff       (20)     2152 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DynamicLibrary.h
+-rw-r--r--   0 joe        (501) staff       (20)      472 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DynamicLibraryF.h
+-rw-r--r--   0 joe        (501) staff       (20)     3779 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Exception.h
+-rw-r--r--   0 joe        (501) staff       (20)     1690 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ExceptionHelpers.h
+-rw-r--r--   0 joe        (501) staff       (20)     2005 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/FactoryTable.h
+-rw-r--r--   0 joe        (501) staff       (20)     1592 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/FactoryTableInit.h
+-rw-r--r--   0 joe        (501) staff       (20)      622 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Format.h
+-rw-r--r--   0 joe        (501) staff       (20)     4169 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Functional.h
+-rw-r--r--   0 joe        (501) staff       (20)     1264 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/GCObject.h
+-rw-r--r--   0 joe        (501) staff       (20)     3363 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Handle.h
+-rw-r--r--   0 joe        (501) staff       (20)     1530 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Ice.h
+-rw-r--r--   0 joe        (501) staff       (20)     9761 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/IconvStringConverter.h
+-rw-r--r--   0 joe        (501) staff       (20)     5300 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Incoming.h
+-rw-r--r--   0 joe        (501) staff       (20)     4254 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/IncomingAsync.h
+-rw-r--r--   0 joe        (501) staff       (20)      662 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/IncomingAsyncF.h
+-rw-r--r--   0 joe        (501) staff       (20)    41173 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Initialize.h
+-rw-r--r--   0 joe        (501) staff       (20)    45578 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/InputStream.h
+-rw-r--r--   0 joe        (501) staff       (20)      308 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/InstanceF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1033 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/InterfaceByValue.h
+-rw-r--r--   0 joe        (501) staff       (20)      646 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/LocalObject.h
+-rw-r--r--   0 joe        (501) staff       (20)      330 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/LocalObjectF.h
+-rw-r--r--   0 joe        (501) staff       (20)     4133 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/LoggerUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)    20895 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/MetricsAdminI.h
+-rw-r--r--   0 joe        (501) staff       (20)     2915 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/MetricsFunctional.h
+-rw-r--r--   0 joe        (501) staff       (20)    17878 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/MetricsObserverI.h
+-rw-r--r--   0 joe        (501) staff       (20)     2542 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/NativePropertiesAdmin.h
+-rw-r--r--   0 joe        (501) staff       (20)    18275 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Object.h
+-rw-r--r--   0 joe        (501) staff       (20)      517 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ObjectF.h
+-rw-r--r--   0 joe        (501) staff       (20)     3453 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ObserverHelper.h
+-rw-r--r--   0 joe        (501) staff       (20)    31190 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Optional.h
+-rw-r--r--   0 joe        (501) staff       (20)    22298 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/OutgoingAsync.h
+-rw-r--r--   0 joe        (501) staff       (20)     1172 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/OutgoingAsyncF.h
+-rw-r--r--   0 joe        (501) staff       (20)    30822 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/OutputStream.h
+-rw-r--r--   0 joe        (501) staff       (20)     7049 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Protocol.h
+-rw-r--r--   0 joe        (501) staff       (20)   196950 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Proxy.h
+-rw-r--r--   0 joe        (501) staff       (20)      655 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ProxyF.h
+-rw-r--r--   0 joe        (501) staff       (20)      327 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ProxyFactoryF.h
+-rw-r--r--   0 joe        (501) staff       (20)     6760 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ProxyHandle.h
+-rw-r--r--   0 joe        (501) staff       (20)      599 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ReferenceF.h
+-rw-r--r--   0 joe        (501) staff       (20)     4908 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/RegisterPlugins.h
+-rw-r--r--   0 joe        (501) staff       (20)      673 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/RequestHandlerF.h
+-rw-r--r--   0 joe        (501) staff       (20)      454 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ResponseHandlerF.h
+-rw-r--r--   0 joe        (501) staff       (20)      607 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SHA1.h
+-rw-r--r--   0 joe        (501) staff       (20)      334 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ServantManagerF.h
+-rw-r--r--   0 joe        (501) staff       (20)    12337 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Service.h
+-rw-r--r--   0 joe        (501) staff       (20)      472 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SliceChecksums.h
+-rw-r--r--   0 joe        (501) staff       (20)     3833 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SlicedData.h
+-rw-r--r--   0 joe        (501) staff       (20)      914 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SlicedDataF.h
+-rw-r--r--   0 joe        (501) staff       (20)    33174 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/StreamHelpers.h
+-rw-r--r--   0 joe        (501) staff       (20)     2258 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/StringConverter.h
+-rw-r--r--   0 joe        (501) staff       (20)      336 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ThreadPoolF.h
+-rw-r--r--   0 joe        (501) staff       (20)      229 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UUID.h
+-rw-r--r--   0 joe        (501) staff       (20)     1178 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UniquePtr.h
+-rw-r--r--   0 joe        (501) staff       (20)     1402 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UniqueRef.h
+-rw-r--r--   0 joe        (501) staff       (20)     1454 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UserExceptionFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)     3602 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Value.h
+-rw-r--r--   0 joe        (501) staff       (20)      274 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ValueF.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.535195 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/
+-rw-r--r--   0 joe        (501) staff       (20)      419 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/Config.h
+-rw-r--r--   0 joe        (501) staff       (20)      546 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/IceSSL.h
+-rw-r--r--   0 joe        (501) staff       (20)     4138 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/OpenSSL.h
+-rw-r--r--   0 joe        (501) staff       (20)    21615 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/Plugin.h
+-rw-r--r--   0 joe        (501) staff       (20)     1845 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/SChannel.h
+-rw-r--r--   0 joe        (501) staff       (20)     1904 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/SecureTransport.h
+-rw-r--r--   0 joe        (501) staff       (20)     1614 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/UWP.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.539720 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/
+-rw-r--r--   0 joe        (501) staff       (20)     3852 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Atomic.h
+-rw-r--r--   0 joe        (501) staff       (20)     6909 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Cond.h
+-rw-r--r--   0 joe        (501) staff       (20)    12363 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Config.h
+-rw-r--r--   0 joe        (501) staff       (20)     1751 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ConsoleUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)      656 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/CountDownLatch.h
+-rw-r--r--   0 joe        (501) staff       (20)     2797 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/CtrlCHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)     1177 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/DisableWarnings.h
+-rw-r--r--   0 joe        (501) staff       (20)     8709 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Exception.h
+-rw-r--r--   0 joe        (501) staff       (20)     2874 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/FileUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)     9321 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Functional.h
+-rw-r--r--   0 joe        (501) staff       (20)     5191 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Handle.h
+-rw-r--r--   0 joe        (501) staff       (20)     1061 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/IceUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)     1028 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/InputUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)      644 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Iterator.h
+-rw-r--r--   0 joe        (501) staff       (20)     2304 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Lock.h
+-rw-r--r--   0 joe        (501) staff       (20)     4489 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Monitor.h
+-rw-r--r--   0 joe        (501) staff       (20)     6532 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Mutex.h
+-rw-r--r--   0 joe        (501) staff       (20)      316 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/MutexProtocol.h
+-rw-r--r--   0 joe        (501) staff       (20)     1296 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/MutexPtrLock.h
+-rw-r--r--   0 joe        (501) staff       (20)     1315 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/MutexPtrTryLock.h
+-rw-r--r--   0 joe        (501) staff       (20)     8491 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Optional.h
+-rw-r--r--   0 joe        (501) staff       (20)     3960 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Options.h
+-rw-r--r--   0 joe        (501) staff       (20)     7392 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/OutputUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)      308 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/PopDisableWarnings.h
+-rw-r--r--   0 joe        (501) staff       (20)     1381 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/PushDisableWarnings.h
+-rw-r--r--   0 joe        (501) staff       (20)      956 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Random.h
+-rw-r--r--   0 joe        (501) staff       (20)     2142 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/RecMutex.h
+-rw-r--r--   0 joe        (501) staff       (20)     1236 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ResourceConfig.h
+-rw-r--r--   0 joe        (501) staff       (20)     1180 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ScannerConfig.h
+-rw-r--r--   0 joe        (501) staff       (20)     1442 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ScopedArray.h
+-rw-r--r--   0 joe        (501) staff       (20)     2019 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Shared.h
+-rw-r--r--   0 joe        (501) staff       (20)      804 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/StopWatch.h
+-rw-r--r--   0 joe        (501) staff       (20)     5565 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/StringConverter.h
+-rw-r--r--   0 joe        (501) staff       (20)     2763 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/StringUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)     3798 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Thread.h
+-rw-r--r--   0 joe        (501) staff       (20)     2004 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ThreadException.h
+-rw-r--r--   0 joe        (501) staff       (20)     3798 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Time.h
+-rw-r--r--   0 joe        (501) staff       (20)     3252 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Timer.h
+-rw-r--r--   0 joe        (501) staff       (20)      285 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/UUID.h
+-rw-r--r--   0 joe        (501) staff       (20)      723 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/UndefSysMacros.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.496983 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.544989 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/
+-rw-r--r--   0 joe        (501) staff       (20)     2832 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/BuiltinSequences.h
+-rw-r--r--   0 joe        (501) staff       (20)    45168 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Communicator.h
+-rw-r--r--   0 joe        (501) staff       (20)     1665 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/CommunicatorF.h
+-rw-r--r--   0 joe        (501) staff       (20)    53769 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Connection.h
+-rw-r--r--   0 joe        (501) staff       (20)     2161 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ConnectionF.h
+-rw-r--r--   0 joe        (501) staff       (20)     9457 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Current.h
+-rw-r--r--   0 joe        (501) staff       (20)    27318 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Endpoint.h
+-rw-r--r--   0 joe        (501) staff       (20)     3106 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/EndpointF.h
+-rw-r--r--   0 joe        (501) staff       (20)     2227 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/EndpointTypes.h
+-rw-r--r--   0 joe        (501) staff       (20)     1487 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/FacetMap.h
+-rw-r--r--   0 joe        (501) staff       (20)     5444 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Identity.h
+-rw-r--r--   0 joe        (501) staff       (20)     8057 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ImplicitContext.h
+-rw-r--r--   0 joe        (501) staff       (20)     1695 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ImplicitContextF.h
+-rw-r--r--   0 joe        (501) staff       (20)    36514 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Instrumentation.h
+-rw-r--r--   0 joe        (501) staff       (20)     2082 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/InstrumentationF.h
+-rw-r--r--   0 joe        (501) staff       (20)   257285 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/LocalException.h
+-rw-r--r--   0 joe        (501) staff       (20)   153507 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Locator.h
+-rw-r--r--   0 joe        (501) staff       (20)     2937 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/LocatorF.h
+-rw-r--r--   0 joe        (501) staff       (20)     5056 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Logger.h
+-rw-r--r--   0 joe        (501) staff       (20)     1605 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/LoggerF.h
+-rw-r--r--   0 joe        (501) staff       (20)   180120 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Metrics.h
+-rw-r--r--   0 joe        (501) staff       (20)    43782 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ObjectAdapter.h
+-rw-r--r--   0 joe        (501) staff       (20)     1675 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ObjectAdapterF.h
+-rw-r--r--   0 joe        (501) staff       (20)     5104 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ObjectFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)     7939 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Plugin.h
+-rw-r--r--   0 joe        (501) staff       (20)     1849 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/PluginF.h
+-rw-r--r--   0 joe        (501) staff       (20)    36008 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Process.h
+-rw-r--r--   0 joe        (501) staff       (20)     2137 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ProcessF.h
+-rw-r--r--   0 joe        (501) staff       (20)    14925 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Properties.h
+-rw-r--r--   0 joe        (501) staff       (20)    56548 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/PropertiesAdmin.h
+-rw-r--r--   0 joe        (501) staff       (20)     2513 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/PropertiesF.h
+-rw-r--r--   0 joe        (501) staff       (20)   112752 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/RemoteLogger.h
+-rw-r--r--   0 joe        (501) staff       (20)    71003 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Router.h
+-rw-r--r--   0 joe        (501) staff       (20)     2116 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/RouterF.h
+-rw-r--r--   0 joe        (501) staff       (20)    10187 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ServantLocator.h
+-rw-r--r--   0 joe        (501) staff       (20)     1685 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ServantLocatorF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1752 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/SliceChecksumDict.h
+-rw-r--r--   0 joe        (501) staff       (20)     9927 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ValueFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)     7172 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Version.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.545349 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/
+-rw-r--r--   0 joe        (501) staff       (20)     5655 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/ConnectionInfo.h
+-rw-r--r--   0 joe        (501) staff       (20)     1725 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/ConnectionInfoF.h
+-rw-r--r--   0 joe        (501) staff       (20)     4126 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/EndpointInfo.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.497398 zeroc-ice-3.7.9.1/src/ice/cpp/src/
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.575447 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/
+-rw-r--r--   0 joe        (501) staff       (20)     9619 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ACM.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3244 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ACM.h
+-rw-r--r--   0 joe        (501) staff       (20)      597 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ACMF.h
+-rw-r--r--   0 joe        (501) staff       (20)      287 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Acceptor.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      808 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Acceptor.h
+-rw-r--r--   0 joe        (501) staff       (20)      407 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/AcceptorF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1183 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ArgVector.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      550 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ArgVector.h
+-rw-r--r--   0 joe        (501) staff       (20)     2247 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/AsyncResult.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     4922 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Base64.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      487 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Base64.h
+-rw-r--r--   0 joe        (501) staff       (20)     5980 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/BatchRequestQueue.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1382 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/BatchRequestQueue.h
+-rw-r--r--   0 joe        (501) staff       (20)     2978 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Buffer.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1055 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/BuiltinSequences.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    11078 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CollocatedRequestHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2445 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CollocatedRequestHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)     1407 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Communicator.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1041 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CommunicatorF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    14609 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CommunicatorI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     5532 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CommunicatorI.h
+-rw-r--r--   0 joe        (501) staff       (20)     9025 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Cond.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     9233 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectRequestHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1921 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectRequestHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)      495 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectRequestHandlerF.h
+-rw-r--r--   0 joe        (501) staff       (20)     2613 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Connection.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1037 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    57598 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     8131 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)      683 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionFactoryF.h
+-rw-r--r--   0 joe        (501) staff       (20)   107785 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    13130 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1854 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionRequestHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      988 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionRequestHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)      291 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Connector.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      565 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Connector.h
+-rw-r--r--   0 joe        (501) staff       (20)      302 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectorF.h
+-rw-r--r--   0 joe        (501) staff       (20)     3798 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CountDownLatch.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1091 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Current.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6449 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DefaultsAndOverrides.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1238 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DefaultsAndOverrides.h
+-rw-r--r--   0 joe        (501) staff       (20)      364 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DefaultsAndOverridesF.h
+-rw-r--r--   0 joe        (501) staff       (20)      990 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DispatchInterceptor.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6780 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DynamicLibrary.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2438 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Endpoint.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1033 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     4512 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3125 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)      340 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactoryF.h
+-rw-r--r--   0 joe        (501) staff       (20)     5751 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactoryManager.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      898 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactoryManager.h
+-rw-r--r--   0 joe        (501) staff       (20)      376 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactoryManagerF.h
+-rw-r--r--   0 joe        (501) staff       (20)     2383 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     5375 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1155 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointIF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1009 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointTypes.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      679 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EventHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1732 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EventHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)      416 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EventHandlerF.h
+-rw-r--r--   0 joe        (501) staff       (20)    18698 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Exception.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1039 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/FacetMap.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3787 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/FactoryTable.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1863 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/FactoryTableInit.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     9597 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/GCObject.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1113 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/HashUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)    16715 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/HttpParser.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2382 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/HttpParser.h
+-rw-r--r--   0 joe        (501) staff       (20)    18772 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IPEndpointI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     4501 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IPEndpointI.h
+-rw-r--r--   0 joe        (501) staff       (20)      557 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IPEndpointIF.h
+-rw-r--r--   0 joe        (501) staff       (20)      984 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IconvStringConverter.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1077 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Identity.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1303 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContext.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1047 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContextF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    13762 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContextI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1027 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContextI.h
+-rw-r--r--   0 joe        (501) staff       (20)    22013 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Incoming.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     4578 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IncomingAsync.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      508 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IncomingRequest.h
+-rw-r--r--   0 joe        (501) staff       (20)    16484 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Initialize.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    67914 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InputStream.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    54093 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Instance.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     7800 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Instance.h
+-rw-r--r--   0 joe        (501) staff       (20)     3690 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Instrumentation.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1063 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InstrumentationF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    26606 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InstrumentationI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     8720 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InstrumentationI.h
+-rw-r--r--   0 joe        (501) staff       (20)    65631 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocalException.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      400 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocalObject.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    54919 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Locator.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1090 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    26576 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorInfo.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     5502 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorInfo.h
+-rw-r--r--   0 joe        (501) staff       (20)      530 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorInfoF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1181 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Logger.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    26096 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerAdminI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      792 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerAdminI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1029 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6722 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1161 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1719 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    62318 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Metrics.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    18521 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/MetricsAdminI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      146 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/MetricsObserverI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    82493 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Network.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    10723 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Network.h
+-rw-r--r--   0 joe        (501) staff       (20)      266 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/NetworkF.h
+-rw-r--r--   0 joe        (501) staff       (20)     7997 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/NetworkProxy.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1943 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/NetworkProxy.h
+-rw-r--r--   0 joe        (501) staff       (20)      322 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/NetworkProxyF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1408 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OSLogLoggerI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      709 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OSLogLoggerI.h
+-rw-r--r--   0 joe        (501) staff       (20)     9484 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Object.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1414 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapter.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1043 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     7137 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1363 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)      488 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterFactoryF.h
+-rw-r--r--   0 joe        (501) staff       (20)    43876 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     5710 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1289 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1515 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObserverHelper.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     8952 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OpaqueEndpointI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2225 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OpaqueEndpointI.h
+-rw-r--r--   0 joe        (501) staff       (20)    30295 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OutgoingAsync.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    34888 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OutputStream.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1429 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Plugin.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1029 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PluginF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    13430 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PluginManagerI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1557 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PluginManagerI.h
+-rw-r--r--   0 joe        (501) staff       (20)    11144 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Process.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1090 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProcessF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1361 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Properties.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    16688 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesAdmin.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6905 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesAdminI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1936 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesAdminI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1096 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    21202 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1893 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesI.h
+-rw-r--r--   0 joe        (501) staff       (20)   101096 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertyNames.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1842 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertyNames.h
+-rw-r--r--   0 joe        (501) staff       (20)     3275 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Protocol.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3331 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolInstance.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2202 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolInstance.h
+-rw-r--r--   0 joe        (501) staff       (20)      359 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolInstanceF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1263 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolPluginFacade.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1397 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolPluginFacade.h
+-rw-r--r--   0 joe        (501) staff       (20)      372 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolPluginFacadeF.h
+-rw-r--r--   0 joe        (501) staff       (20)    39721 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Proxy.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     8556 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProxyFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1202 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProxyFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)    55183 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Reference.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    11621 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Reference.h
+-rw-r--r--   0 joe        (501) staff       (20)    28704 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReferenceFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2142 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReferenceFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)      309 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReferenceFactoryF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1251 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RegisterPluginsInit.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      233 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RegisterPluginsInit.h
+-rw-r--r--   0 joe        (501) staff       (20)    32252 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RemoteLogger.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      561 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReplyStatus.h
+-rw-r--r--   0 joe        (501) staff       (20)      854 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1541 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)     2129 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandlerFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      800 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandlerFactory.h
+-rw-r--r--   0 joe        (501) staff       (20)      250 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ResponseHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      835 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ResponseHandler.h
+-rw-r--r--   0 joe        (501) staff       (20)     3902 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RetryQueue.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1418 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RetryQueue.h
+-rw-r--r--   0 joe        (501) staff       (20)      273 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RetryQueueF.h
+-rw-r--r--   0 joe        (501) staff       (20)    25109 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Router.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1088 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    10378 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterInfo.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     4067 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterInfo.h
+-rw-r--r--   0 joe        (501) staff       (20)      413 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterInfoF.h
+-rw-r--r--   0 joe        (501) staff       (20)     4118 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SHA1.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    42753 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Selector.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6994 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Selector.h
+-rw-r--r--   0 joe        (501) staff       (20)     1296 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantLocator.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1045 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantLocatorF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    12613 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantManager.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1953 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantManager.h
+-rw-r--r--   0 joe        (501) staff       (20)      653 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SharedContext.h
+-rw-r--r--   0 joe        (501) staff       (20)     1057 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SliceChecksumDict.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1260 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SliceChecksums.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2711 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SlicedData.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    17009 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StreamSocket.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2008 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StreamSocket.h
+-rw-r--r--   0 joe        (501) staff       (20)     4782 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StringConverterPlugin.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      547 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StringUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)     3420 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SysLoggerI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      736 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SysLoggerI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1284 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SystemdJournalI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      685 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SystemdJournalI.h
+-rw-r--r--   0 joe        (501) staff       (20)     9319 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpAcceptor.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1504 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpAcceptor.h
+-rw-r--r--   0 joe        (501) staff       (20)     2532 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpConnector.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      962 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpConnector.h
+-rw-r--r--   0 joe        (501) staff       (20)     8713 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpEndpointI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2497 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpEndpointI.h
+-rw-r--r--   0 joe        (501) staff       (20)     2761 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpTransceiver.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1409 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpTransceiver.h
+-rw-r--r--   0 joe        (501) staff       (20)    16449 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Thread.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    38733 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ThreadPool.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     9739 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ThreadPool.h
+-rw-r--r--   0 joe        (501) staff       (20)     7050 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Timer.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1250 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceLevels.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      701 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceLevels.h
+-rw-r--r--   0 joe        (501) staff       (20)      308 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceLevelsF.h
+-rw-r--r--   0 joe        (501) staff       (20)    10018 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      737 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)      310 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Transceiver.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1245 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Transceiver.h
+-rw-r--r--   0 joe        (501) staff       (20)      679 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TransceiverF.h
+-rw-r--r--   0 joe        (501) staff       (20)     2663 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpConnector.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      954 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpConnector.h
+-rw-r--r--   0 joe        (501) staff       (20)    12333 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpEndpointI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2633 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpEndpointI.h
+-rw-r--r--   0 joe        (501) staff       (20)    33089 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpTransceiver.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3223 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpTransceiver.h
+-rw-r--r--   0 joe        (501) staff       (20)      978 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Value.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1461 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ValueFactory.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1436 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ValueFactoryManagerI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      823 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ValueFactoryManagerI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1075 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Version.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      800 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/VirtualShared.h
+-rw-r--r--   0 joe        (501) staff       (20)     1778 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSAcceptor.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1142 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSAcceptor.h
+-rw-r--r--   0 joe        (501) staff       (20)     1795 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSConnector.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      844 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSConnector.h
+-rw-r--r--   0 joe        (501) staff       (20)    11789 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSEndpoint.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2872 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSEndpoint.h
+-rw-r--r--   0 joe        (501) staff       (20)    51492 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSTransceiver.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3429 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSTransceiver.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.576608 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/
+-rw-r--r--   0 joe        (501) staff       (20)    25879 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/IceDiscovery.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    82885 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/IceDiscovery.h
+-rw-r--r--   0 joe        (501) staff       (20)     7509 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LocatorI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3679 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LocatorI.h
+-rw-r--r--   0 joe        (501) staff       (20)    16684 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LookupI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6249 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LookupI.h
+-rw-r--r--   0 joe        (501) staff       (20)     5797 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/PluginI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      627 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/PluginI.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.577466 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/
+-rw-r--r--   0 joe        (501) staff       (20)    19542 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    46878 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.h
+-rw-r--r--   0 joe        (501) staff       (20)     1177 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/Plugin.h
+-rw-r--r--   0 joe        (501) staff       (20)    31596 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/PluginI.cpp
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.585307 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/
+-rw-r--r--   0 joe        (501) staff       (20)     2047 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/AcceptorI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1283 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/AcceptorI.h
+-rw-r--r--   0 joe        (501) staff       (20)     6724 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/CertificateI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1441 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/CertificateI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1317 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectionInfo.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1054 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectionInfoF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1893 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectorI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      895 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectorI.h
+-rw-r--r--   0 joe        (501) staff       (20)     8839 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/EndpointI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2985 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/EndpointI.h
+-rw-r--r--   0 joe        (501) staff       (20)     1303 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/EndpointInfo.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      555 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Instance.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      555 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Instance.h
+-rw-r--r--   0 joe        (501) staff       (20)      666 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/InstanceF.h
+-rw-r--r--   0 joe        (501) staff       (20)    18230 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLCertificateI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    39192 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLEngine.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1158 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLEngine.h
+-rw-r--r--   0 joe        (501) staff       (20)      438 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLEngineF.h
+-rw-r--r--   0 joe        (501) staff       (20)     2756 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLPluginI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    32160 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2444 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.h
+-rw-r--r--   0 joe        (501) staff       (20)    10220 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      886 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)     6919 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/PluginI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1699 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/PluginI.h
+-rw-r--r--   0 joe        (501) staff       (20)    11933 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/RFC2253.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1427 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/RFC2253.h
+-rw-r--r--   0 joe        (501) staff       (20)    21416 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelCertificateI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    42771 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelEngine.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2394 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelEngine.h
+-rw-r--r--   0 joe        (501) staff       (20)      408 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelEngineF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1579 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelPluginI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    36565 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelTransceiverI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3348 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelTransceiverI.h
+-rw-r--r--   0 joe        (501) staff       (20)     8767 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SSLEngine.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2440 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SSLEngine.h
+-rw-r--r--   0 joe        (501) staff       (20)      339 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SSLEngineF.h
+-rw-r--r--   0 joe        (501) staff       (20)    32791 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportCertificateI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    52308 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportEngine.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1208 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportEngine.h
+-rw-r--r--   0 joe        (501) staff       (20)      430 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportEngineF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1669 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportPluginI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    22540 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2386 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.h
+-rw-r--r--   0 joe        (501) staff       (20)    33331 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1029 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)     6773 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/TrustManager.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1161 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/TrustManager.h
+-rw-r--r--   0 joe        (501) staff       (20)      336 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/TrustManagerF.h
+-rw-r--r--   0 joe        (501) staff       (20)     7857 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPCertificateI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    10919 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPEngine.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      767 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPEngine.h
+-rw-r--r--   0 joe        (501) staff       (20)      364 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPEngineF.h
+-rw-r--r--   0 joe        (501) staff       (20)     1906 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPPluginI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    12350 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPTransceiverI.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1991 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPTransceiverI.h
+-rw-r--r--   0 joe        (501) staff       (20)     4675 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Util.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2178 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Util.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.587564 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/
+-rw-r--r--   0 joe        (501) staff       (20)     3193 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ConsoleUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    18260 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ConvertUTF.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     5895 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ConvertUTF.h
+-rw-r--r--   0 joe        (501) staff       (20)     5168 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/CtrlCHandler.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    11103 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/FileUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      664 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/InputUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      369 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/MutexProtocol.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    32067 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Options.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    10693 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/OutputUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3606 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Random.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     4344 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/RecMutex.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1050 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Shared.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    19101 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/StringConverter.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    30112 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/StringUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2997 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ThreadException.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     6167 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Time.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3925 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/UUID.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     5465 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Unicode.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1100 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Unicode.h
+-rw-r--r--   0 joe        (501) staff       (20)    19244 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/UtilException.cpp
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.591760 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/
+-rw-r--r--   0 joe        (501) staff       (20)    53245 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/CPlusPlusUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3318 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/CPlusPlusUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)    10722 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Checksum.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      316 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Checksum.h
+-rw-r--r--   0 joe        (501) staff       (20)     2941 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/FileTracker.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1301 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/FileTracker.h
+-rw-r--r--   0 joe        (501) staff       (20)   146690 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Grammar.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3585 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Grammar.h
+-rw-r--r--   0 joe        (501) staff       (20)     5415 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/GrammarUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)   167600 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/JavaUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    13377 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/JavaUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)      856 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      450 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5.h
+-rw-r--r--   0 joe        (501) staff       (20)    13192 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5I.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     3405 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5I.h
+-rw-r--r--   0 joe        (501) staff       (20)     4068 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PHPUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)      718 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PHPUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)   174010 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Parser.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    36241 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Parser.h
+-rw-r--r--   0 joe        (501) staff       (20)    19866 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Preprocessor.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1700 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Preprocessor.h
+-rw-r--r--   0 joe        (501) staff       (20)    26141 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Python.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    99543 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PythonUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1892 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PythonUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)    10266 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Ruby.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    43938 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/RubyUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     1168 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/RubyUtil.h
+-rw-r--r--   0 joe        (501) staff       (20)    73377 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Scanner.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    10597 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/SliceUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)    13431 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/StringLiteralUtil.cpp
+-rw-r--r--   0 joe        (501) staff       (20)     2113 2023-06-26 19:30:06.000000 zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Util.h
+drwxr-xr-x   0 joe        (501) staff       (20)        0 2023-06-26 19:30:13.594346 zeroc-ice-3.7.9.1/src/ice/mcpp/
+-rw-r--r--   0 joe        (501) staff       (20)     1550 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/CMakeLists.txt
+-rw-r--r--   0 joe        (501) staff       (20)     1460 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/LICENSE
+-rw-r--r--   0 joe        (501) staff       (20)     1478 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/Makefile
+-rw-r--r--   0 joe        (501) staff       (20)     1431 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/README.md
+-rw-r--r--   0 joe        (501) staff       (20)     2076 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/config.h
+-rw-r--r--   0 joe        (501) staff       (20)     8998 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/configed.H
+-rw-r--r--   0 joe        (501) staff       (20)    52208 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/directive.c
+-rw-r--r--   0 joe        (501) staff       (20)    47479 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/eval.c
+-rw-r--r--   0 joe        (501) staff       (20)    93246 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/expand.c
+-rw-r--r--   0 joe        (501) staff       (20)    23969 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/internal.H
+-rw-r--r--   0 joe        (501) staff       (20)    31200 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/main.c
+-rw-r--r--   0 joe        (501) staff       (20)     9358 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/mbchar.c
+-rw-r--r--   0 joe        (501) staff       (20)     1893 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/mcpp.gyp
+-rw-r--r--   0 joe        (501) staff       (20)     1051 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/mcpp_lib.h
+-rw-r--r--   0 joe        (501) staff       (20)      364 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/mcpp_out.h
+-rw-r--r--   0 joe        (501) staff       (20)    68680 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/support.c
+-rw-r--r--   0 joe        (501) staff       (20)    14700 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/system.H
+-rw-r--r--   0 joe        (501) staff       (20)    93033 2023-06-26 19:30:07.000000 zeroc-ice-3.7.9.1/src/ice/mcpp/system.c
```

### Comparing `zeroc-ice-3.7.9/BZIP2_LICENSE` & `zeroc-ice-3.7.9.1/BZIP2_LICENSE`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/ICE_LICENSE` & `zeroc-ice-3.7.9.1/ICE_LICENSE`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/LICENSE` & `zeroc-ice-3.7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/MCPP_LICENSE` & `zeroc-ice-3.7.9.1/MCPP_LICENSE`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/PKG-INFO` & `zeroc-ice-3.7.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroc-ice
-Version: 3.7.9
+Version: 3.7.9.1
 Summary: Ice is a comprehensive RPC framework with support for Python, C++, .NET, Java, JavaScript and more.
 Home-page: https://zeroc.com
 Author: ZeroC, Inc.
 Author-email: info@zeroc.com
 License: GPL v2 with exceptions
 Keywords: RPC distributed systems development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zeroc-ice-3.7.9/README.rst` & `zeroc-ice-3.7.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/Metrics_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/Metrics_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/PermissionsVerifierF_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/PermissionsVerifierF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/PermissionsVerifier_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/PermissionsVerifier_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/RouterF_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/RouterF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/Router_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/Router_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/SSLInfo_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/SSLInfo_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/Session_ice.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/Session_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Glacier2/__init__.py` & `zeroc-ice-3.7.9.1/lib/Glacier2/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/BuiltinSequences_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/BuiltinSequences_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Communicator_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Communicator_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ConnectionF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ConnectionF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Connection_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Connection_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Current_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Current_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/EndpointF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/EndpointF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/EndpointTypes_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/EndpointTypes_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Endpoint_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Endpoint_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/FacetMap_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/FacetMap_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Identity_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Identity_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ImplicitContext_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ImplicitContext_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/InstrumentationF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/InstrumentationF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Instrumentation_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Instrumentation_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/LocalException_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/LocalException_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/LocatorF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/LocatorF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Locator_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Locator_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Logger_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Logger_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Metrics_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Metrics_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ObjectAdapter_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ObjectAdapter_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ObjectFactory_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ObjectFactory_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/PluginF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/PluginF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Plugin_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Plugin_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ProcessF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ProcessF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Process_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Process_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/PropertiesAdmin_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/PropertiesAdmin_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/PropertiesF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/PropertiesF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Properties_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Properties_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Py3/IceFuture.py` & `zeroc-ice-3.7.9.1/lib/Ice/Py3/IceFuture.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/RemoteLogger_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/RemoteLogger_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/RouterF_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/RouterF_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Router_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Router_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ServantLocator_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ServantLocator_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/SliceChecksumDict_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/SliceChecksumDict_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/ValueFactory_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/ValueFactory_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/Version_ice.py` & `zeroc-ice-3.7.9.1/lib/Ice/Version_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/Ice/__init__.py` & `zeroc-ice-3.7.9.1/lib/Ice/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceBox/IceBox_ice.py` & `zeroc-ice-3.7.9.1/lib/IceBox/IceBox_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/Admin_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/Admin_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/Descriptor_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/Descriptor_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/Exception_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/Exception_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/FileParser_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/FileParser_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/PluginFacade_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/PluginFacade_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/Registry_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/Registry_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/Session_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/Session_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceGrid/UserAccountMapper_ice.py` & `zeroc-ice-3.7.9.1/lib/IceGrid/UserAccountMapper_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IcePatch2/FileInfo_ice.py` & `zeroc-ice-3.7.9.1/lib/IcePatch2/FileInfo_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IcePatch2/FileServer_ice.py` & `zeroc-ice-3.7.9.1/lib/IcePatch2/FileServer_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceStorm/IceStorm_ice.py` & `zeroc-ice-3.7.9.1/lib/IceStorm/IceStorm_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/IceStorm/Metrics_ice.py` & `zeroc-ice-3.7.9.1/lib/IceStorm/Metrics_ice.py`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Glacier2/Metrics.ice` & `zeroc-ice-3.7.9.1/lib/slice/Glacier2/Metrics.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Glacier2/PermissionsVerifier.ice` & `zeroc-ice-3.7.9.1/lib/slice/Glacier2/PermissionsVerifier.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Glacier2/Router.ice` & `zeroc-ice-3.7.9.1/lib/slice/Glacier2/Router.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Glacier2/SSLInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/Glacier2/SSLInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Glacier2/Session.ice` & `zeroc-ice-3.7.9.1/lib/slice/Glacier2/Session.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/BuiltinSequences.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/BuiltinSequences.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Communicator.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Communicator.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Connection.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Connection.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Current.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Current.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Endpoint.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Endpoint.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/EndpointF.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/EndpointF.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/EndpointTypes.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/EndpointTypes.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/FacetMap.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/FacetMap.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Identity.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Identity.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/ImplicitContext.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/ImplicitContext.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Instrumentation.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Instrumentation.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/InstrumentationF.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/InstrumentationF.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/LocalException.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/LocalException.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Locator.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Locator.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Logger.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Logger.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Metrics.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Metrics.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/ObjectAdapter.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/ObjectAdapter.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/ObjectFactory.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/ObjectFactory.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Plugin.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Plugin.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Process.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Process.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Properties.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Properties.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/PropertiesAdmin.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/PropertiesAdmin.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/RemoteLogger.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/RemoteLogger.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Router.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Router.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/ServantLocator.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/ServantLocator.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/SliceChecksumDict.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/SliceChecksumDict.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/ValueFactory.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/ValueFactory.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/Ice/Version.ice` & `zeroc-ice-3.7.9.1/lib/slice/Ice/Version.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceBT/ConnectionInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceBT/ConnectionInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceBT/EndpointInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceBT/EndpointInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceBT/Types.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceBT/Types.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceBox/IceBox.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceBox/IceBox.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceDiscovery/IceDiscovery.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceDiscovery/IceDiscovery.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/Admin.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/Admin.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/Descriptor.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/Descriptor.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/Exception.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/Exception.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/FileParser.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/FileParser.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/PluginFacade.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/PluginFacade.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/Registry.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/Registry.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/Session.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/Session.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceGrid/UserAccountMapper.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceGrid/UserAccountMapper.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceIAP/ConnectionInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceIAP/ConnectionInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceIAP/EndpointInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceIAP/EndpointInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceLocatorDiscovery/IceLocatorDiscovery.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceLocatorDiscovery/IceLocatorDiscovery.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IcePatch2/FileInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IcePatch2/FileInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IcePatch2/FileServer.ice` & `zeroc-ice-3.7.9.1/lib/slice/IcePatch2/FileServer.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceSSL/ConnectionInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceSSL/ConnectionInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceSSL/EndpointInfo.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceSSL/EndpointInfo.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceStorm/IceStorm.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceStorm/IceStorm.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/slice/IceStorm/Metrics.ice` & `zeroc-ice-3.7.9.1/lib/slice/IceStorm/Metrics.ice`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/PKG-INFO` & `zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroc-ice
-Version: 3.7.9
+Version: 3.7.9.1
 Summary: Ice is a comprehensive RPC framework with support for Python, C++, .NET, Java, JavaScript and more.
 Home-page: https://zeroc.com
 Author: ZeroC, Inc.
 Author-email: info@zeroc.com
 License: GPL v2 with exceptions
 Keywords: RPC distributed systems development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zeroc-ice-3.7.9/lib/zeroc_ice.egg-info/SOURCES.txt` & `zeroc-ice-3.7.9.1/lib/zeroc_ice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/setup.py` & `zeroc-ice-3.7.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             for e in self.extensions:
                 e.extra_link_args.append('/PDB:{0}'.format(os.path.join(self.build_temp, "IcePy.pdb")))
         build_ext.build_extensions(self)
 
 setup(
     name='zeroc-ice',
 
-    version='3.7.9',
+    version='3.7.9.1',
 
     description="Ice is a comprehensive RPC framework with support for Python, C++, .NET, Java, JavaScript and more.",
 
     long_description=long_description,
 
     # The project's main homepage.
     url='https://zeroc.com',
```

### Comparing `zeroc-ice-3.7.9/src/BatchRequestInterceptor.cpp` & `zeroc-ice-3.7.9.1/src/BatchRequestInterceptor.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/BatchRequestInterceptor.h` & `zeroc-ice-3.7.9.1/src/BatchRequestInterceptor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Communicator.cpp` & `zeroc-ice-3.7.9.1/src/Communicator.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Communicator.h` & `zeroc-ice-3.7.9.1/src/Communicator.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Config.h` & `zeroc-ice-3.7.9.1/src/Config.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Connection.cpp` & `zeroc-ice-3.7.9.1/src/Connection.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ConnectionInfo.cpp` & `zeroc-ice-3.7.9.1/src/ConnectionInfo.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Current.cpp` & `zeroc-ice-3.7.9.1/src/Current.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Dispatcher.cpp` & `zeroc-ice-3.7.9.1/src/Dispatcher.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Dispatcher.h` & `zeroc-ice-3.7.9.1/src/Dispatcher.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Endpoint.cpp` & `zeroc-ice-3.7.9.1/src/Endpoint.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/EndpointInfo.cpp` & `zeroc-ice-3.7.9.1/src/EndpointInfo.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ImplicitContext.cpp` & `zeroc-ice-3.7.9.1/src/ImplicitContext.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Init.cpp` & `zeroc-ice-3.7.9.1/src/Init.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Logger.cpp` & `zeroc-ice-3.7.9.1/src/Logger.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Logger.h` & `zeroc-ice-3.7.9.1/src/Logger.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ObjectAdapter.cpp` & `zeroc-ice-3.7.9.1/src/ObjectAdapter.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Operation.cpp` & `zeroc-ice-3.7.9.1/src/Operation.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Operation.h` & `zeroc-ice-3.7.9.1/src/Operation.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Properties.cpp` & `zeroc-ice-3.7.9.1/src/Properties.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/PropertiesAdmin.cpp` & `zeroc-ice-3.7.9.1/src/PropertiesAdmin.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Proxy.cpp` & `zeroc-ice-3.7.9.1/src/Proxy.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Proxy.h` & `zeroc-ice-3.7.9.1/src/Proxy.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Slice.cpp` & `zeroc-ice-3.7.9.1/src/Slice.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Thread.cpp` & `zeroc-ice-3.7.9.1/src/Thread.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Thread.h` & `zeroc-ice-3.7.9.1/src/Thread.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Types.cpp` & `zeroc-ice-3.7.9.1/src/Types.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Types.h` & `zeroc-ice-3.7.9.1/src/Types.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Util.cpp` & `zeroc-ice-3.7.9.1/src/Util.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/Util.h` & `zeroc-ice-3.7.9.1/src/Util.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ValueFactoryManager.cpp` & `zeroc-ice-3.7.9.1/src/ValueFactoryManager.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ValueFactoryManager.h` & `zeroc-ice-3.7.9.1/src/ValueFactoryManager.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/blocksort.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/blocksort.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/bzlib.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/bzlib.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/bzlib.h` & `zeroc-ice-3.7.9.1/src/ice/bzip2/bzlib.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/bzlib_private.h` & `zeroc-ice-3.7.9.1/src/ice/bzip2/bzlib_private.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/compress.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/compress.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/crctable.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/crctable.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/decompress.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/decompress.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/huffman.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/huffman.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/bzip2/randtable.c` & `zeroc-ice-3.7.9.1/src/ice/bzip2/randtable.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Application.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Application.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/AsyncResult.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/AsyncResult.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/BatchRequestInterceptor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/BatchRequestInterceptor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Buffer.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Buffer.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/CommunicatorAsync.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/CommunicatorAsync.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Comparable.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Comparable.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Config.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Config.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ConnectionAsync.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ConnectionAsync.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ConnectionIF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ConnectionIF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DefaultValueFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DefaultValueFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DispatchInterceptor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DispatchInterceptor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Dispatcher.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Dispatcher.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/DynamicLibrary.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/DynamicLibrary.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Exception.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Exception.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ExceptionHelpers.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ExceptionHelpers.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/FactoryTable.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/FactoryTable.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/FactoryTableInit.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/FactoryTableInit.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Format.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Format.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Functional.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Functional.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/GCObject.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/GCObject.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Handle.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Handle.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Ice.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Ice.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/IconvStringConverter.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/IconvStringConverter.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Incoming.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Incoming.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/IncomingAsync.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/IncomingAsync.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/IncomingAsyncF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/IncomingAsyncF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Initialize.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Initialize.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/InputStream.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/InputStream.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/InterfaceByValue.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/InterfaceByValue.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/LocalObject.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/LocalObject.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/LoggerUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/LoggerUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/MetricsAdminI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/MetricsAdminI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/MetricsFunctional.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/MetricsFunctional.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/MetricsObserverI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/MetricsObserverI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/NativePropertiesAdmin.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/NativePropertiesAdmin.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Object.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Object.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ObjectF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ObjectF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ObserverHelper.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ObserverHelper.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Optional.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Optional.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/OutgoingAsync.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/OutgoingAsync.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/OutgoingAsyncF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/OutgoingAsyncF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/OutputStream.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/OutputStream.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Protocol.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Protocol.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Proxy.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Proxy.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ProxyF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ProxyF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ProxyHandle.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ProxyHandle.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/ReferenceF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/ReferenceF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/RegisterPlugins.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/RegisterPlugins.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/RequestHandlerF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/RequestHandlerF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SHA1.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SHA1.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Service.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Service.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SlicedData.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SlicedData.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/SlicedDataF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/SlicedDataF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/StreamHelpers.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/StreamHelpers.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/StringConverter.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/StringConverter.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UniquePtr.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UniquePtr.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UniqueRef.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UniqueRef.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/UserExceptionFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/UserExceptionFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/Ice/Value.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/Ice/Value.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/IceSSL.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/IceSSL.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/OpenSSL.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/OpenSSL.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/Plugin.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/Plugin.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/SChannel.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/SChannel.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/SecureTransport.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/SecureTransport.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceSSL/UWP.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceSSL/UWP.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Atomic.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Atomic.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Cond.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Cond.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Config.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Config.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ConsoleUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ConsoleUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/CountDownLatch.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/CountDownLatch.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/CtrlCHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/CtrlCHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/DisableWarnings.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/DisableWarnings.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Exception.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Exception.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/FileUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/FileUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Functional.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Functional.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Handle.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Handle.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/IceUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/IceUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/InputUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/InputUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Iterator.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Iterator.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Lock.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Lock.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Monitor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Monitor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Mutex.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Mutex.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/MutexPtrLock.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/MutexPtrLock.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/MutexPtrTryLock.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/MutexPtrTryLock.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Optional.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Optional.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Options.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Options.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/OutputUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/OutputUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/PushDisableWarnings.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/PushDisableWarnings.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Random.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Random.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/RecMutex.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/RecMutex.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ResourceConfig.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ResourceConfig.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ScannerConfig.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ScannerConfig.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ScopedArray.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ScopedArray.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Shared.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Shared.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/StopWatch.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/StopWatch.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/StringConverter.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/StringConverter.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/StringUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/StringUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Thread.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Thread.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/ThreadException.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/ThreadException.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Time.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Time.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/Timer.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/Timer.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/IceUtil/UndefSysMacros.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/IceUtil/UndefSysMacros.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/BuiltinSequences.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/BuiltinSequences.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Communicator.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Communicator.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/CommunicatorF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/CommunicatorF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Connection.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Connection.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ConnectionF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ConnectionF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Current.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Current.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Endpoint.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Endpoint.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/EndpointF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/EndpointF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/EndpointTypes.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/EndpointTypes.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/FacetMap.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/FacetMap.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Identity.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Identity.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ImplicitContext.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ImplicitContext.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ImplicitContextF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ImplicitContextF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Instrumentation.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Instrumentation.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/InstrumentationF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/InstrumentationF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/LocalException.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/LocalException.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Locator.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Locator.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/LocatorF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/LocatorF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Logger.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Logger.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/LoggerF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/LoggerF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Metrics.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Metrics.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ObjectAdapter.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ObjectAdapter.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ObjectAdapterF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ObjectAdapterF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ObjectFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ObjectFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Plugin.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Plugin.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/PluginF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/PluginF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Process.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Process.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ProcessF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ProcessF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Properties.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Properties.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/PropertiesAdmin.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/PropertiesAdmin.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/PropertiesF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/PropertiesF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/RemoteLogger.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/RemoteLogger.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Router.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Router.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/RouterF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/RouterF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ServantLocator.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ServantLocator.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ServantLocatorF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ServantLocatorF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/SliceChecksumDict.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/SliceChecksumDict.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/ValueFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/ValueFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/Ice/Version.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/Ice/Version.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/ConnectionInfo.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/ConnectionInfo.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/ConnectionInfoF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/ConnectionInfoF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/include/generated/IceSSL/EndpointInfo.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/include/generated/IceSSL/EndpointInfo.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ACM.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ACM.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ACM.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ACM.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ACMF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ACMF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Acceptor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Acceptor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ArgVector.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ArgVector.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ArgVector.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ArgVector.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/AsyncResult.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/AsyncResult.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Base64.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Base64.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/BatchRequestQueue.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/BatchRequestQueue.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/BatchRequestQueue.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/BatchRequestQueue.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Buffer.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Buffer.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/BuiltinSequences.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/BuiltinSequences.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CollocatedRequestHandler.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CollocatedRequestHandler.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CollocatedRequestHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CollocatedRequestHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Communicator.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Communicator.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CommunicatorF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CommunicatorF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CommunicatorI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CommunicatorI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CommunicatorI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CommunicatorI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Cond.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Cond.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectRequestHandler.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectRequestHandler.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectRequestHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectRequestHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Connection.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Connection.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionFactoryF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionFactoryF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionRequestHandler.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionRequestHandler.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ConnectionRequestHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ConnectionRequestHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Connector.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Connector.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/CountDownLatch.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/CountDownLatch.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Current.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Current.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DefaultsAndOverrides.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DefaultsAndOverrides.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DefaultsAndOverrides.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DefaultsAndOverrides.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DispatchInterceptor.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DispatchInterceptor.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/DynamicLibrary.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/DynamicLibrary.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Endpoint.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Endpoint.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactoryManager.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactoryManager.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointFactoryManager.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointFactoryManager.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointIF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointIF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EndpointTypes.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EndpointTypes.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EventHandler.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EventHandler.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/EventHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/EventHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Exception.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Exception.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/FacetMap.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/FacetMap.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/FactoryTable.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/FactoryTable.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/FactoryTableInit.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/FactoryTableInit.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/GCObject.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/GCObject.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/HashUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/HashUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/HttpParser.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/HttpParser.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/HttpParser.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/HttpParser.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IPEndpointI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IPEndpointI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IPEndpointI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IPEndpointI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IPEndpointIF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IPEndpointIF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IconvStringConverter.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IconvStringConverter.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Identity.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Identity.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContext.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContext.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContextF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContextF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContextI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContextI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ImplicitContextI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ImplicitContextI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Incoming.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Incoming.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/IncomingAsync.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/IncomingAsync.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Initialize.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Initialize.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InputStream.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InputStream.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Instance.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Instance.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Instance.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Instance.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Instrumentation.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Instrumentation.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InstrumentationF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InstrumentationF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InstrumentationI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InstrumentationI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/InstrumentationI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/InstrumentationI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocalException.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocalException.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Locator.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Locator.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorInfo.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorInfo.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorInfo.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorInfo.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LocatorInfoF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LocatorInfoF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Logger.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Logger.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerAdminI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerAdminI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerAdminI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerAdminI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/LoggerUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/LoggerUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Metrics.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Metrics.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/MetricsAdminI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/MetricsAdminI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Network.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Network.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Network.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Network.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/NetworkProxy.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/NetworkProxy.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/NetworkProxy.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/NetworkProxy.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OSLogLoggerI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OSLogLoggerI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OSLogLoggerI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OSLogLoggerI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Object.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Object.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapter.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapter.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectAdapterI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectAdapterI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObjectFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObjectFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ObserverHelper.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ObserverHelper.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OpaqueEndpointI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OpaqueEndpointI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OpaqueEndpointI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OpaqueEndpointI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OutgoingAsync.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OutgoingAsync.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/OutputStream.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/OutputStream.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Plugin.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Plugin.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PluginF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PluginF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PluginManagerI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PluginManagerI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PluginManagerI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PluginManagerI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Process.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Process.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProcessF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProcessF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Properties.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Properties.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesAdmin.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesAdmin.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesAdminI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesAdminI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesAdminI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesAdminI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertiesI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertiesI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertyNames.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertyNames.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/PropertyNames.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/PropertyNames.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Protocol.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Protocol.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolInstance.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolInstance.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolInstance.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolInstance.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolPluginFacade.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolPluginFacade.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProtocolPluginFacade.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProtocolPluginFacade.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Proxy.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Proxy.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProxyFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProxyFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ProxyFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ProxyFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Reference.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Reference.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Reference.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Reference.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReferenceFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReferenceFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReferenceFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReferenceFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RegisterPluginsInit.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RegisterPluginsInit.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RemoteLogger.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RemoteLogger.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ReplyStatus.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ReplyStatus.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandler.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandler.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandlerFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandlerFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RequestHandlerFactory.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RequestHandlerFactory.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ResponseHandler.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ResponseHandler.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RetryQueue.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RetryQueue.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RetryQueue.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RetryQueue.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Router.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Router.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterInfo.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterInfo.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/RouterInfo.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/RouterInfo.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SHA1.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SHA1.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Selector.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Selector.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Selector.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Selector.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantLocator.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantLocator.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantLocatorF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantLocatorF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantManager.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantManager.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ServantManager.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ServantManager.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SharedContext.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SharedContext.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SliceChecksumDict.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SliceChecksumDict.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SliceChecksums.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SliceChecksums.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SlicedData.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SlicedData.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StreamSocket.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StreamSocket.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StreamSocket.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StreamSocket.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StringConverterPlugin.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StringConverterPlugin.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/StringUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/StringUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SysLoggerI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SysLoggerI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SysLoggerI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SysLoggerI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SystemdJournalI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SystemdJournalI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/SystemdJournalI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/SystemdJournalI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpAcceptor.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpAcceptor.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpAcceptor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpAcceptor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpConnector.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpConnector.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpConnector.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpConnector.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpEndpointI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpEndpointI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpEndpointI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpEndpointI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpTransceiver.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpTransceiver.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TcpTransceiver.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TcpTransceiver.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Thread.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Thread.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ThreadPool.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ThreadPool.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ThreadPool.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ThreadPool.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Timer.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Timer.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceLevels.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceLevels.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceLevels.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceLevels.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TraceUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TraceUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Transceiver.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Transceiver.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/TransceiverF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/TransceiverF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpConnector.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpConnector.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpConnector.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpConnector.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpEndpointI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpEndpointI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpEndpointI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpEndpointI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpTransceiver.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpTransceiver.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/UdpTransceiver.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/UdpTransceiver.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Value.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Value.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ValueFactory.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ValueFactory.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ValueFactoryManagerI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ValueFactoryManagerI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/ValueFactoryManagerI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/ValueFactoryManagerI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/Version.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/Version.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/VirtualShared.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/VirtualShared.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSAcceptor.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSAcceptor.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSAcceptor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSAcceptor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSConnector.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSConnector.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSConnector.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSConnector.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSEndpoint.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSEndpoint.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSEndpoint.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSEndpoint.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSTransceiver.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSTransceiver.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Ice/WSTransceiver.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Ice/WSTransceiver.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/IceDiscovery.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/IceDiscovery.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/IceDiscovery.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/IceDiscovery.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LocatorI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LocatorI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LocatorI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LocatorI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LookupI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LookupI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/LookupI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/LookupI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/PluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/PluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceDiscovery/PluginI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceDiscovery/PluginI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/IceLocatorDiscovery.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/Plugin.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/Plugin.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceLocatorDiscovery/PluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceLocatorDiscovery/PluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/AcceptorI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/AcceptorI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/AcceptorI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/AcceptorI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/CertificateI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/CertificateI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/CertificateI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/CertificateI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectionInfo.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectionInfo.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectionInfoF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectionInfoF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectorI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectorI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/ConnectorI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/ConnectorI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/EndpointI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/EndpointI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/EndpointI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/EndpointI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/EndpointInfo.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/EndpointInfo.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Instance.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Instance.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Instance.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Instance.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/InstanceF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/InstanceF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLCertificateI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLCertificateI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLEngine.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLEngine.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLEngine.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLEngine.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLPluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLPluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLTransceiverI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/OpenSSLUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/OpenSSLUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/PluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/PluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/PluginI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/PluginI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/RFC2253.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/RFC2253.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/RFC2253.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/RFC2253.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelCertificateI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelCertificateI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelEngine.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelEngine.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelEngine.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelEngine.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelPluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelPluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelTransceiverI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelTransceiverI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SChannelTransceiverI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SChannelTransceiverI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SSLEngine.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SSLEngine.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SSLEngine.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SSLEngine.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportCertificateI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportCertificateI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportEngine.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportEngine.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportEngine.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportEngine.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportPluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportPluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportTransceiverI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/SecureTransportUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/SecureTransportUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/TrustManager.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/TrustManager.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/TrustManager.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/TrustManager.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPCertificateI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPCertificateI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPEngine.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPEngine.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPEngine.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPEngine.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPPluginI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPPluginI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPTransceiverI.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPTransceiverI.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/UWPTransceiverI.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/UWPTransceiverI.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Util.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Util.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceSSL/Util.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceSSL/Util.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ConsoleUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ConsoleUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ConvertUTF.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ConvertUTF.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ConvertUTF.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ConvertUTF.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/CtrlCHandler.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/CtrlCHandler.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/FileUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/FileUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/InputUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/InputUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Options.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Options.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/OutputUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/OutputUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Random.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Random.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/RecMutex.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/RecMutex.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Shared.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Shared.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/StringConverter.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/StringUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/StringUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/ThreadException.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/ThreadException.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Time.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Time.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/UUID.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/UUID.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Unicode.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Unicode.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/Unicode.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/Unicode.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/IceUtil/UtilException.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/IceUtil/UtilException.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/CPlusPlusUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/CPlusPlusUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/CPlusPlusUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/CPlusPlusUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Checksum.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Checksum.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/FileTracker.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/FileTracker.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/FileTracker.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/FileTracker.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Grammar.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Grammar.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Grammar.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Grammar.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/GrammarUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/GrammarUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/JavaUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/JavaUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/JavaUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/JavaUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5I.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5I.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/MD5I.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/MD5I.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PHPUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PHPUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PHPUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PHPUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Parser.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Parser.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Parser.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Parser.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Preprocessor.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Preprocessor.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Preprocessor.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Preprocessor.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Python.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Python.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PythonUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PythonUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/PythonUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/PythonUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Ruby.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Ruby.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/RubyUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/RubyUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/RubyUtil.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/RubyUtil.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Scanner.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Scanner.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/SliceUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/SliceUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/StringLiteralUtil.cpp` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/StringLiteralUtil.cpp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/cpp/src/Slice/Util.h` & `zeroc-ice-3.7.9.1/src/ice/cpp/src/Slice/Util.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/CMakeLists.txt` & `zeroc-ice-3.7.9.1/src/ice/mcpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/LICENSE` & `zeroc-ice-3.7.9.1/src/ice/mcpp/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/Makefile` & `zeroc-ice-3.7.9.1/src/ice/mcpp/Makefile`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/README.md` & `zeroc-ice-3.7.9.1/src/ice/mcpp/README.md`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/config.h` & `zeroc-ice-3.7.9.1/src/ice/mcpp/config.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/configed.H` & `zeroc-ice-3.7.9.1/src/ice/mcpp/configed.H`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/directive.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/directive.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/eval.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/eval.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/expand.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/expand.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/internal.H` & `zeroc-ice-3.7.9.1/src/ice/mcpp/internal.H`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/main.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/main.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/mbchar.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/mbchar.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/mcpp.gyp` & `zeroc-ice-3.7.9.1/src/ice/mcpp/mcpp.gyp`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/mcpp_lib.h` & `zeroc-ice-3.7.9.1/src/ice/mcpp/mcpp_lib.h`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/support.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/support.c`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/system.H` & `zeroc-ice-3.7.9.1/src/ice/mcpp/system.H`

 * *Files identical despite different names*

### Comparing `zeroc-ice-3.7.9/src/ice/mcpp/system.c` & `zeroc-ice-3.7.9.1/src/ice/mcpp/system.c`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,18 @@
  *
  * Routines dependent on O.S., compiler or compiler-driver.
  * To port MCPP for the systems not yet ported, you must
  *      1. specify the constants in "configed.H" or "noconfig.H",
  *      2. append the system-dependent routines in this file.
  */
 
+#ifndef _MSC_VER
+#  include <unistd.h> // For readlink()
+#endif
+
 #include    "system.H"
 #include    "internal.H"
 
 #if     HOST_SYS_FAMILY == SYS_UNIX
 #include    "unistd.h"              /* For getcwd(), readlink() */
 #elif   HOST_COMPILER == MSC || HOST_COMPILER == LCC
 #include    "direct.h"
```

