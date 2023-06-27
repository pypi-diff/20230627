# Comparing `tmp/osm-fieldwork-0.3.1rc2.tar.gz` & `tmp/osm-fieldwork-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.3.1rc2.tar", last modified: Thu Jun  1 17:30:39 2023, max compression
+gzip compressed data, was "osm-fieldwork-0.3.2.tar", last modified: Tue Jun 27 10:50:24 2023, max compression
```

## Comparing `osm-fieldwork-0.3.1rc2.tar` & `osm-fieldwork-0.3.2.tar`

### file list

```diff
@@ -1,85 +1,84 @@
--rw-r--r--   0        0        0    34625 2023-06-01 17:30:33.408398 osm-fieldwork-0.3.1rc2/LICENSE.md
--rw-r--r--   0        0        0     8656 2023-06-01 17:30:33.408398 osm-fieldwork-0.3.1rc2/README.md
--rwxr-xr-x   0        0        0    13091 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5099 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     4400 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     4205 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    27428 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/OdkCentral.py
--rw-r--r--   0        0        0        0 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0     9588 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0     9631 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2023-06-01 17:30:33.412398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      366 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      226 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      240 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      678 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      119 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      412 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      137 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      495 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0       94 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0      106 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0      104 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0      107 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0      245 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4745 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      348 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      170 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      140 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     7378 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/filter_data.py
--rwxr-xr-x   0        0        0    16479 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0    18443 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/make_data_extract.py
--rwxr-xr-x   0        0        0     5254 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0     4199 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2geojson.py
--rwxr-xr-x   0        0        0    13649 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0     8766 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0     5036 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/osm2favorities.py
--rwxr-xr-x   0        0        0    11537 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     8003 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     4474 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0     3800 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0      830 2023-06-01 17:30:33.416398 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2023-06-01 17:30:33.420399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2023-06-01 17:30:33.420399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0    69120 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    22528 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2023-06-01 17:30:33.432399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0  1537536 2023-06-01 17:30:33.436399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/slides.xls
--rw-r--r--   0        0        0   115963 2023-06-01 17:30:33.436399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   118272 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     3726 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     1694 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/pyproject.toml
--rw-r--r--   0        0        0       32 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/.flake8
--rw-r--r--   0        0        0      574 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/Test.yaml
--rw-r--r--   0        0        0     2713 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test.csv
--rwxr-xr-x   0        0        0     2324 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_convert.py
--rwxr-xr-x   0        0        0     1889 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_csv.py
--rwxr-xr-x   0        0        0     3204 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_osm.py
--rwxr-xr-x   0        0        0     1649 2023-06-01 17:30:33.440399 osm-fieldwork-0.3.1rc2/tests/test_yaml.py
--rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    34625 2023-06-27 10:50:14.222713 osm-fieldwork-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     8656 2023-06-27 10:50:14.222713 osm-fieldwork-0.3.2/README.md
+-rwxr-xr-x   0        0        0    13091 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5099 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     4400 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4205 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    27428 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/OdkCentral.py
+-rw-r--r--   0        0        0        0 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0     9592 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0     9946 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      445 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      226 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      240 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      678 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      119 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      412 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      137 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      495 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0       94 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0      106 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0      104 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0      107 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0      245 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4745 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      348 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      170 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      140 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     7378 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/filter_data.py
+-rwxr-xr-x   0        0        0    16200 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0    18873 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/make_data_extract.py
+-rwxr-xr-x   0        0        0     5254 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4199 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0    13649 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0     8766 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5336 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    11547 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     8003 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     4474 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0     3800 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0      830 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2023-06-27 10:50:14.238713 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2023-06-27 10:50:14.242714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0    69120 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    22528 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0   115963 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   118272 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     3726 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     1688 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/.flake8
+-rw-r--r--   0        0        0      574 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/Test.yaml
+-rw-r--r--   0        0        0     2713 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test.csv
+-rwxr-xr-x   0        0        0     2324 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_convert.py
+-rwxr-xr-x   0        0        0     1889 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_csv.py
+-rwxr-xr-x   0        0        0     3204 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_osm.py
+-rwxr-xr-x   0        0        0     1649 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_yaml.py
+-rw-r--r--   0        0        0     9343 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.2/PKG-INFO
```

### Comparing `osm-fieldwork-0.3.1rc2/LICENSE.md` & `osm-fieldwork-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/README.md` & `osm-fieldwork-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.3.2/osm_fieldwork/CSVDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.3.2/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.3.2/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/ODKInstance.py` & `osm-fieldwork-0.3.2/osm_fieldwork/ODKInstance.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.3.2/osm_fieldwork/OdkCentral.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.3.2/osm_fieldwork/basemapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
 
 # Get all the zoom levels we want
 zooms = list()
 if args.zooms:
     if args.zooms.find("-") > 0:
         start = int(args.zooms.split("-")[0])
-        end = int(args.zooms.split("-")[1])
+        end = int(args.zooms.split("-")[1]) + 1
         x = range(start, end)
         for i in x:
             zooms.append(i)
     elif args.zooms.find(",") > 0:
         levels = args.zooms.split(",")
         for level in levels:
             zooms.append(int(level))
```

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/convert.py` & `osm-fieldwork-0.3.2/osm_fieldwork/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,16 @@
 class Convert(YamlFile):
     """A class to apply a YAML config file and convert ODK to OSM"""
 
     def __init__(self,
                  xform: str
                  ):
         path = xlsforms_path.replace("xlsforms", "")
-        if type(xform) == str:
-            file = f"{path}{xform}"
-            xform = file
+        if xform is not None:
+            file = xform
         else:
             file = f"{path}/xforms.yaml"
         self.yaml = YamlFile(file)
         self.filespec = file
         # Parse the file contents into a data structure to make it
         # easier to retrieve values
         self.convert = dict()
@@ -62,15 +61,18 @@
                         tag = entry
                     else:
                         tag = list(entry.keys())[0]
                         vals[tag] = entry[tag]
                 self.convert[key] = vals
         self.ignore = self.yaml.yaml["ignore"]
         self.private = self.yaml.yaml["private"]
-        self.multiple = self.yaml.yaml["multiple"]
+        if "multiple" in  self.yaml.yaml:
+            self.multiple = self.yaml.yaml["multiple"]
+        else:
+            self.multiple = list()
 
     def privateData(self,
                     keyword: str
                     ):
         """See is a keyword is in the private data category"""
         return keyword in self.private
 
@@ -118,14 +120,17 @@
                      tag: str,
                      value: str
                      ):
         """Convert a tag and value from the ODK represention to an OSM one"""
         #all = list()
 
         # If it's not in any conversion data, pass it through unchanged.
+        if tag in self.ignore:
+            # logging.debug(f"FIXME: Ignoring {tag}")
+            return None
         if (
             tag not in self.convert
             and tag not in self.ignore
             and tag not in self.private
         ):
             return {tag: value}
 
@@ -220,22 +225,26 @@
             return newtag
         else:
             return tag
 
     def dump(self):
         """Dump the contents of the yaml file"""
         print("YAML file: %s" % self.filespec)
+        print("Convert section")
         for key, val in self.convert.items():
             if type(val) is list:
-                print("Tag %s is" % key)
+                print("\tTag %s is" % key)
                 for data in val:
-                    print("\t%r" % data)
+                    print("\t\t%r" % data)
             else:
-                print("Tag %s is %s" % (key, val))
+                print("\tTag %s is %s" % (key, val))
 
+        print("Ignore Section")
+        for item in self.ignore:
+            print(f"\tIgnoring tag {item}")
 
 #
 # This script can be run standalone for debugging purposes. It's easier to debug
 # this way than using pytest,
 #
 if __name__ == "__main__":
     # Enable logging to the terminal by default
```

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.3.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.3.2/osm_fieldwork/data_models/category.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.3.2/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.3.2/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.3.2/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.3.2/osm_fieldwork/filter_data.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.3.2/osm_fieldwork/json2osm.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,32 +48,19 @@
         self.nodesets = dict()
         self.data = list()
         self.osm = None
         self.json = None
         self.features = list()
         path = xlsforms_path.replace("xlsforms", "")
         if yaml:
-            file = f"{path}{yaml}"
+            file = f"{yaml}"
         else:
             file = f"{path}/xforms.yaml"
         self.config = super().__init__(yaml)
 
-        self.ignore = ('@id',
-                       '@xmlns:ev',
-                       '@xmlns:orx',
-                       '@xmlns:odk',
-                       '@xmlns:h',
-                       '@xmlns:jr',
-                       '@xmlns:xsd',
-                       'start',
-                       'end',
-                       'today',
-                       'meta',
-                       )
-
     # def parseXLS(self, xlsfile: str):
     #     """Parse the source XLSFile if available to look for details we need"""
     #     if xlsfile is not None and len(xlsfile) > 0:
     #         entries = pd.read_excel(xlsfile, sheet_name=[0])
     #         # There will only be a single sheet
     #         names = entries[0]['name']
     #         defaults = entries[0]['default']
@@ -211,43 +198,47 @@
         total = list()
         # JSON files from Central use value as the keyword, whereas
         # GeoJSON uses features for the same thing.
         if 'value' in reader:
             data = reader['value']
         elif 'features' in reader:
             data = reader['features']
+        else:
+            data = reader
         for row in data:
             # log.info(f"ROW: {row}")
             tags = dict()
             if 'geometry' in row:
                 tags['geometry'] = row['geometry']
             if 'properties' in row:
                 indata = row['properties'] # A GeoJson formatted file
             else:
                 indata = row    # A JOSM file from ODK Central
             for keyword, value in indata.items():
                 # There's many extraneous fields in the input file which we don't need.
                 base = keyword.lower()
                 if (
                     base is None
-                    or base in self.ignore
                     or value is None
                     or len(value) == 0
                 ):
                     continue
                 if keyword is None or len(keyword) == 0:
                     continue
                 if type(value) == str:
+                    if keyword not in self.ignore:
+                        continue
                     items = self.convertEntry(keyword, value)
-                    tags.update(items)
+                    if items is not None and tags is not None:
+                        tags.update(items)
+                    else:
+                        continue
                 else:
                     alltags = self.getAllTags(value)
                     for k, v in alltags.items():
-                        # if k in self.ignore:
-                        #     continue
                         if v:
                             items = dict()
                             if type(v) == dict:
                                 v1 = alltags[k]
                                 if len(v1) > 1:
                                     log.warning("Got more than 1 result! {v1}")
                                     v2 = v1[v1.keys()]
@@ -255,15 +246,16 @@
                             else:
                                 items = self.convertEntry(k, v)
                                 #    for entry in items:
                                 #        for k, v in entry.items():
                                 #            tags[k] = v
                                 #    else:
                                 #tags[k1] = v1
-                        tags.update(items)
+                        if items is not None:
+                            tags.update(items)
             total.append(tags)
         return total
 
     def createEntry(self,
                     entry: dict
                     ):
         """Create the feature data structure"""
@@ -408,17 +400,16 @@
             continue
         if len(feature) > 0:
             if "lat" not in feature["attrs"]:
                 if 'geometry' in feature['tags']:
                     if type(feature['tags']['geometry']) == str:
                         coords = list(feature['tags']['geometry'])
                         # del feature['tags']['geometry']
-                    else:
-                        coords = feature['tags']['geometry']['coordinates']
-                        # del feature['tags']['geometry']
+                elif 'coordinates' in feature['tags']:
+                    coords = feature['tags']['coordinates']
                     feature['attrs'] = {'lat': coords[1], 'lon': coords[0]}
                 else:
                     log.warning("Bad record! %r" % feature)
                     continue
             jsonin.writeOSM(feature)
             # This GeoJson file has all the data values
             jsonin.writeGeoJson(feature)
```

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.3.2/osm_fieldwork/make_data_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import argparse
 import os
 import logging
 import sys
 import re
 import yaml
 import json
+from sys import argv
 from geojson import Point, Feature, FeatureCollection, dump, Polygon
 import geojson
 from osm_fieldwork.filter_data import FilterData
 from osm_fieldwork.xlsforms import xlsforms_path
 import requests
 # from requests.auth import HTTPBasicAuth
 from io import BytesIO
@@ -56,15 +57,17 @@
 # Instantiate logger
 log = logging.getLogger(__name__)
 
 
 class DatabaseAccess(object):
     def __init__(self,
                  dbhost: str = None,
-                 dbname: str = None
+                 dbname: str = None,
+                 dbuser: str = None,
+                 dbpass: str = None,
                  ):
         self.dbshell = None
         self.dbcursor = None
         self.category = None
         if dbname == "underpass":
             # Authentication data
             # self.auth = HTTPBasicAuth(self.user, self.passwd)
@@ -76,14 +79,19 @@
         else:
             logging.info("Opening database connection to: %s" % dbhost)
             connect = "PG: dbname=" + dbname
             if dbhost is None or dbhost == "localhost":
                 connect = f"dbname={dbname}"
             else:
                 connect = f"host={dbhost} dbname={dbname}"
+            if dbuser:
+                connect += f" user={dbuser}"
+            if dbpass:
+                connect += f" password={dbpass}"
+            logging.debug(connect)
             try:
                 self.dbshell = psycopg2.connect(connect)
                 self.dbshell.autocommit = True
                 self.dbcursor = self.dbshell.cursor()
                 if self.dbcursor.closed == 0:
                     logging.info(f"Opened cursor in {dbname}")
             except Exception as e:
@@ -232,28 +240,30 @@
         result = self.session.get(zip, headers=self.headers)
         fp = BytesIO(result.content)
         zfp = zipfile.ZipFile(fp, "r")
         zfp.extract("Export.geojson", "/tmp/")
         # Now take that taskid and hit /tasks/status url with get
         data = zfp.read("Export.geojson")
         os.remove("/tmp/Export.geojson")
-        return eval(data)
+        return json.loads(data)
     #   return zfp.read("Export.geojson")
 
 class PostgresClient(DatabaseAccess):
     """Class to handle SQL queries for the categories"""
     def __init__(self,
                  dbhost: str = None,
                  dbname: str = None,
-                 output: str = None
+                 dbuser: str = None,
+                 dbpass: str = None,
+                 #output: str = None
     ):
         """Initialize the postgres handler"""
         # OutputFile.__init__( self, output)
         self.boundary = None
-        super().__init__(dbhost, dbname)
+        super().__init__(dbhost, dbname, dbuser, dbpass)
 
     def getFeatures(self,
                     boundary,
                     filespec: str,
                     polygon: bool,
                     category: str,
                     xlsfile: str,
@@ -442,14 +452,18 @@
         "--category",
         default="buildings",
         choices=choices,
         help="Which category to extract",
     )
     args = parser.parse_args()
 
+    if len(argv) <= 1:
+        parser.print_help()
+        quit()
+
     # if verbose, dump to the terminal.
     if args.verbose is not None:
         root = logging.getLogger()
         log.setLevel(logging.DEBUG)
 
         ch = logging.StreamHandler(sys.stdout)
         ch.setLevel(logging.DEBUG)
@@ -482,15 +496,15 @@
         pg = PostgresClient(args.dbhost, args.dbname, outfile)
         if args.geojson:
             extract = args.geojson
         else:
             infile = FilterData(xlsfile)
             extract = infile.metadata[1]
         pg.getFeatures(args.boundary, extract, args.polygon, args.category, xlsfile)
-        log.info(f"Created /tmp/{outfile} for {args.category}")
+        log.info(f"Created {outfile} for {args.category}")
         # pg.cleanup(outfile)
     elif args.overpass:
         logging.info("Using Overpass Turbo for the data source")
         op = OverpassClient(outfile)
         clip = open(args.boundary, "r")
         geom = geojson.load(clip)
         #op.getFeatures(args.boundary, args.geojson, args.category)
```

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.3.2/osm_fieldwork/odk2csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk2geojson.py` & `osm-fieldwork-0.3.2/osm_fieldwork/odk2geojson.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.3.2/osm_fieldwork/odk_client.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/odk_merge.py` & `osm-fieldwork-0.3.2/osm_fieldwork/odk_merge.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/osm2favorities.py` & `osm-fieldwork-0.3.2/osm_fieldwork/osm2favorities.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 import geojson
 from sys import argv
 from geojson import Point, Feature, FeatureCollection, dump
 from pathlib import Path
 import gpxpy
 import gpxpy.gpx
 from lxml import etree
+from shapely.geometry import shape, Polygon
+import shapely
 
 
 # set log level for urlib
 log = logging.getLogger(__name__)
 
 def createExtension(icon):
     # camp_pitch.png, tourism_camp_site.png, topo_camp_pitch.png, topo_camp_site.png
@@ -86,16 +88,22 @@
 
         # gpxpy.gpxfield.GPXField()
         gpx = gpxpy.gpx.GPX()
         gpx.nsmap['osmand'] = "https://osmand.net"
         gpx.creator = "osm2favorites 0.1"
         for feature in indata['features']:
             coords = feature['geometry']['coordinates']
-            lat = coords[1]
-            lon = coords[0]
+            if feature['geometry']['type'] == "Polygon":
+                wkt = shape(feature['geometry'])
+                center = shapely.centroid(wkt)
+                lat = center.y
+                lon = center.x
+            else:
+                lat = coords[1]
+                lon = coords[0]
             name = ""
             if 'name' in feature['properties']:
                 name = feature['properties']['name']
                 tourism = None
                 if 'tourism' in feature['properties']:
                     tourism = feature['properties']['tourism']
                 highway = None
```

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.3.2/osm_fieldwork/osmfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             for key, value in way["tags"].items():
                 if value is None:
                     continue
                 if key == "track":
                     continue
                 if key not in attrs:
                     newkey = self.convert.escape(key)
-                    osm += "\n    <tag k='%s' v=%r/>" % (newkey, value)
+                    osm += "\n    <tag k='%s' v=%r/>" % (newkey, str(value))
             if modified:
                 osm += (
                     '\n    <tag k="fixme" v="Do not upload this without validation!"/>'
                 )
             osm += "\n"
 
         osm += "  </way>"
@@ -222,15 +222,15 @@
 
         if "tags" in node:
             osm += ">"
             for key, value in node["tags"].items():
                 if not value:
                     continue
                 if key not in attrs:
-                    osm += "\n    <tag k='%s' v=%r/>" % (key, value)
+                    osm += "\n    <tag k='%s' v=%r/>" % (key, str(value))
             if modified:
                 osm += (
                     '\n    <tag k="fixme" v="Do not upload this without validation!"/>'
                 )
             osm += "\n  </node>"
         else:
             osm += "/>"
```

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.3.2/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xforms.yaml` & `osm-fieldwork-0.3.2/osm_fieldwork/xforms.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/Makefile`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.3.2/osm_fieldwork/yamlfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/pyproject.toml` & `osm-fieldwork-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
 ]
-version = "0.3.1rc2"
+version = "0.3.2"
 
 [project.urls]
 homepage = "https://github.com/hotosm/osm-fieldwork/wiki"
 documentation = "https://github.com/hotosm/osm-fieldwork/wiki"
 repository = "https://github.com/hotosm/osm-fieldwork"
 
 [project.optional-dependencies]
@@ -68,15 +68,15 @@
 testpaths = [
     "tests",
 ]
 pythonpath = "osm_fieldwork"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.1rc2"
+version = "0.3.2"
 version_files = [
     "pyproject.toml:version",
     "osm_fieldwork/__version__.py",
     "Makefile:VERSION",
 ]
 
 [build-system]
```

### Comparing `osm-fieldwork-0.3.1rc2/tests/Test.yaml` & `osm-fieldwork-0.3.2/tests/Test.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/tests/test.csv` & `osm-fieldwork-0.3.2/tests/test.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/tests/test_convert.py` & `osm-fieldwork-0.3.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/tests/test_csv.py` & `osm-fieldwork-0.3.2/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/tests/test_osm.py` & `osm-fieldwork-0.3.2/tests/test_osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/tests/test_yaml.py` & `osm-fieldwork-0.3.2/tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.1rc2/PKG-INFO` & `osm-fieldwork-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.3.1rc2
+Version: 0.3.2
 Summary: Convert CSV files from ODK Central to OSM format.
 License: GPL-3.0-only
 Keywords: fmtm,odk,hot,openstreetmap,opendatakit
 Author-email: Rob Savoye <rob.savoye@hotosm.org>
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

